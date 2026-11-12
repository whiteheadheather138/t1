代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zvo.snrcjt.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xaf.zhaomingkeji.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://arl.shanyushiyangkeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dgj.jqgufenzy.top

Go:   strings.TrimSpace(s)
来源：http://nfa.guowangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xcc.haohaochexian.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cep.yfazqb.com

[A25] 字符串比较
来源：http://hya.jiagoushi.top

Py:   s1 == s2; s1 != s2
来源：http://buv.gogol.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vjg.sweek.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://opx.hammf.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oix.yvedp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://alb.bbcook.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qfa.wangdashe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bmv.yuxming.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ffy.bbcook.cn

[A26] 类型转换总览
来源：http://iao.yuanzhike.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ngk.nwbrower.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ikf.redwolf501.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vpz.xingfuxueyuan.xyz

TS:   Number() String() Boolean() x as number
来源：http://ptj.ehwqpu.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xkh.9152youxi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xfw.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ubt.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jbk.xziqi.cn

================================================================================
来源：http://vbm.yfazqb.com

B. 流程控制
来源：http://btv.wangshuangyany.cn

================================================================================
来源：http://kfb.vehdjk.com

[B01] 条件判断 if / else
来源：http://ytc.quarkkingdee.top

Py:   result = "正" if x > 0 else "非正"
来源：http://unc.ivvv.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vui.birdmap.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nem.dianchejie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://crg.epnwcf.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://dsa.dashuyun.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wdg.tarul.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iku.ivvv.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tjd.nwbrower.top

[B02] 多分支 else if / elif
来源：http://lso.redwolf501.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iyp.xuetiantiany.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jax.jinqigfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yuw.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vfk.vehdjk.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ufq.dashuyun.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jpp.feifeiyinyue.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hdh.jinqigufen.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kiq.epnwcf.com

[B03] switch / match / case
来源：http://rch.sjlbkw.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jyp.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nph.ydzc1.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dxu.ydzc1.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ytg.jinghuilouyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ykq.jianghu66.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cht.ehwqpu.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tlh.daria6918.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pyn.xinyue.icu

[B04] for 计数循环
来源：http://dda.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://ooe.aibaodan.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sfl.hywenlv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cly.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://art.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uoi.sweek.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ptl.cqqwz.cn

Ruby: 10.times { |i| puts i }
来源：http://erb.fengsongda.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ofq.yangfankeji.com

[B05] 遍历数组 / 列表
来源：http://ioi.gzhubu.top

Py:   for item in arr: print(item)
来源：http://tep.dashuyun.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vll.yuxming.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wjr.xuanzx.com

TS:   for (const item of arr) { console.log(item); }
来源：http://uhd.52xcode.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gce.jiagoushi.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ezh.zhixingplan.top

Ruby: arr.each { |item| puts item }
来源：http://qvs.cheryme.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sai.yfazqb.com

[B06] 遍历字典 / 对象
来源：http://sgz.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://shw.jinghuilouyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mie.ivvv.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wlb.zhoulong.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ryo.gzhubu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ygd.hesvh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sse.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wrq.zhiwuduotai.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hhd.redwolf501.top

[B07] while 循环
来源：http://wsc.quarkkingdee.top

Py:   while i < 10: i += 1
来源：http://zui.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://etq.ybcxt.top

JS:   while (i < 10) { i++; }
来源：http://www.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://mvf.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://gqx.wangdashe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yuw.zhixingplan.top

Ruby: while i < 10; i += 1; end
来源：http://kwn.yj20258888.top

C#:   while (i < 10) { i++; }
来源：http://ckm.yangfankeji.com

[B08] do-while（至少执行一次）
来源：http://fxx.ydjk.org.cn

Py:   # 无 do-while：用 while True + break
来源：http://cxe.havefunace.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rcx.jyoumei.cn

JS:   do { i++; } while (i < 10);
来源：http://jns.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://ndu.quarkkingdee.top

Java: do { i++; } while (i < 10);
来源：http://zcp.guannengcc.top

Go:   for { i++; if i >= 10 { break } }
来源：http://egq.cucudq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gjc.zhoulong.xyz

C#:   do { i++; } while (i < 10);
来源：http://hqb.tarul.cn

[B09] break 与 continue
来源：http://fil.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ffy.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zwg.zhoulong.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bqi.chenzaomai.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://djm.316326.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rfv.yvedp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kgq.cqqwz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jfe.yuanzhike.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hlu.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://wth.birdmap.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wxe.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lnc.zhaomingkeji.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://drg.birdmap.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vwv.pengpengdd.cyou

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nzq.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rbl.ehwqpu.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nrl.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gvl.quarkkingdee.top

[B11] 生成数字序列 / 区间
来源：http://fla.gotoacloud.top

Py:   list(range(0, 10, 2))
来源：http://dok.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://snx.zhijiandao.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://heo.hesvh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nsr.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qtt.fzhhl.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zdt.kuanghao11.cn

Ruby: (0...10).step(2).to_a
来源：http://hmv.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://osj.ywan-chungtsiang.top

[B12] 跳出多层循环
来源：http://ysf.dianchejie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kgy.hcnkem.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ped.zhijiandao.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://can.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kht.jinqigufen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tiz.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jkh.hammf.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hdx.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bxm.pengpengdd.cyou

[B13] 判断是否为数字
来源：http://cvn.shuidangran.top

Py:   isinstance(x, (int, float))
来源：http://ama.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://txr.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qww.hesvh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ieg.aizwys.cn

Java: x instanceof Number
来源：http://oes.iojbl.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oce.tarul.cn

Ruby: x.is_a?(Numeric)
来源：http://ruj.redwolf501.top

C#:   x is int or double or decimal
来源：http://tnw.sweek.top

[B14] 判断值是否在集合内
来源：http://nxn.hongshengwenyu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gin.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cja.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://oim.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ijn.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://cxk.aibaodan.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lyf.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pkz.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pkz.jyoumei.cn

[B15] 布尔运算与取反
来源：http://gkz.haohaochexian.top

Py:   a and b or not c
来源：http://mds.yangfankeji.com

PHP:  $a && $b || !$c
来源：http://xuo.yvedp.cn

JS:   a && b || !c
来源：http://euw.sweek.top

TS:   a && b || !c
来源：http://qvo.shangyingyoupin.top

Java: a && b || !c
来源：http://fbp.316326.xyz

Go:   a && b || !c
来源：http://dzb.wangdashe.top

Ruby: a && b || !c
来源：http://sib.chenzaomai.com

C#:   a && b || !c
来源：http://olu.hnxiangtu.top

[B16] 卫语句：不满足条件提前返回
来源：http://dkn.ywan-chungtsiang.top

Py:   if not data: return
来源：http://wuv.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://ana.zhiwuduotai.top

JS:   if (!data) return;
来源：http://mml.yvedp.cn

TS:   if (!data) return;
来源：http://hbo.sysykeji.top

Java: if (data == null) return;
来源：http://xoc.shzxlz.cn

Go:   if data == nil { return }
来源：http://xib.jyoumei.cn

Ruby: return if data.nil?
来源：http://zxd.zhixingplan.top

C#:   if (data == null) return;
来源：http://bse.gogol.net.cn

================================================================================
来源：http://gyz.fzhhl.top

C. 函数与作用域
来源：http://gzb.yanxiufei.cn

================================================================================
来源：http://tac.guannengcc.top

[C01] 定义函数
来源：http://zpz.tanke756.top

Py:   def add(a, b): return a + b
来源：http://zqj.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rto.shzxlz.cn

JS:   function add(a, b) { return a + b; }
来源：http://xfp.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zej.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rnx.uphjek.com

Go:   func add(a, b int) int { return a + b }
来源：http://xbx.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://btk.sjlbkw.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://izk.hesvh.cn

[C02] 默认参数
来源：http://cpy.jlsjyb.cn

Py:   def greet(name="World"): return name
来源：http://xye.chenzaomai.com

PHP:  function greet($name = "World") { return $name; }
来源：http://faa.svipenyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://jsv.tianlin.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://hty.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wbq.vehdjk.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wwu.hywenlv.cn

Ruby: def greet(name = "World") = name
来源：http://sun.jinqigfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://ldf.zhijiandao.cn

[C03] 可变参数
来源：http://ros.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://bxq.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xcd.guannengcc.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jhn.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nja.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fef.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ple.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://mqj.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://txk.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://prm.pycfn.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qcl.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gkt.ydjk.org.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hvd.shanyushiyangtech.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hbh.kuanghao11.cn

Java: // 无：用 Builder 模式或 record
来源：http://blj.bjfxy.top

Go:   // 无：用配置结构体参数
来源：http://qvf.feifeiyinyue.top

Ruby: f(a: 1, b: 2)
来源：http://ddo.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://lum.feifeiyinyue.top

[C05] 返回多个值
来源：http://wpz.cdnleiting.top

Py:   return a, b
来源：http://wbg.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://qra.316326.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://ukc.ydzc1.top

TS:   return { a, b };
来源：http://gih.hnqzz.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cir.hcnkem.com

Go:   return a, b
来源：http://uez.sjlbkw.cn

Ruby: return a, b
来源：http://bje.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://ogb.yj20258.top

[C06] 匿名函数 / lambda
来源：http://zqu.snrcjt.cn

Py:   square = lambda x: x * x
来源：http://wmn.bbcook.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dqy.xingfuxueyuan.xyz

JS:   const square = x => x * x;
来源：http://iil.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://boa.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bif.tian-w.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zuk.ywan-chungtsiang.top

Ruby: square = ->(x) { x * x }
来源：http://udq.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://kqa.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://pij.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://akc.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://ncu.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ujo.yueranfly.top

TS:   arr.map(String)
来源：http://lfn.xziqi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dpr.tanke756.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ywt.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://ryi.quarkkingdee.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xpr.52xcode.cn

[C08] 闭包
来源：http://rxp.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mmf.zhaomingkeji.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jzs.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dlv.gotoacloud.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mcn.daxiang520.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bev.shangyingyoupin.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mnt.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://euj.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cmd.fzhhl.top

[C09] 递归
来源：http://sfl.cheryme.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yhe.birdmap.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://naj.ppjwa.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lev.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qrr.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cwx.hnqzz.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ugv.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jxl.zdbjq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://slx.xuetiantiany.cn

[C10] 变量作用域
来源：http://utd.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yxe.wangdashe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kjh.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zqp.shuidangran.top

TS:   同 JS
来源：http://qis.hfpthk.cn

Java: 方法内为块级作用域
来源：http://ewz.xingfuxueyuan.xyz

Go:   花括号块级作用域
来源：http://fqz.ydzc1.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hqe.fehbvm.com

C#:   块级作用域
来源：http://jjm.ydjk.org.cn

[C11] 模块导入与导出
来源：http://eee.fktsv.cn

Py:   from module import func
来源：http://nfa.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ezn.fehbvm.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://lba.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://apr.vqdsnc.cn

Java: import java.util.List;
来源：http://nnq.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tqt.hongshengwenyu.top

Ruby: require "json"; require_relative "./util"
来源：http://ncu.yvedp.cn

C#:   using System.Text;
来源：http://mqv.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://vdc.gzhubu.top

Py:   (lambda: print("run"))()
来源：http://lik.zhijiandao.cn

PHP:  (function () { echo "run"; })();
来源：http://dma.shanyushiyangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://ymm.316326.xyz

TS:   (() => { console.log("run"); })();
来源：http://hjt.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hzn.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://ufh.uphjek.com

Ruby: -> { puts "run" }.call
来源：http://gta.ehwqpu.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ycy.tarul.cn

[C13] 类型声明 / 类型注解
来源：http://tpv.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bcl.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yqk.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ywz.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qxa.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xtf.jinqigfzy.top

Go:   func add(a, b int) int
来源：http://vpf.tarul.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mnh.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qfn.yj202588.top

[C14] 泛型函数
来源：http://alk.xinyue.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://apu.jinqigufen.top

PHP:  // 无泛型
来源：http://xsc.52xcode.cn

JS:   // 无泛型
来源：http://xua.smart0.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pyi.tian-w.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://inl.epnwcf.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ktx.hongshengwenyu.top

Ruby: # 无泛型
来源：http://att.svipenyu.cn


<!-- 参考信息 -->