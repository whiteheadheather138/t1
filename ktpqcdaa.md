代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://eac.andypj.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uuh.pengpengdd.cyou

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mgk.vqdsnc.cn

[A25] 字符串比较
来源：http://ldd.316326.xyz

Py:   s1 == s2; s1 != s2
来源：http://trn.hfpthk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uxc.yuanzhike.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gcs.sweek.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zsv.smart0.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uyo.zhengqikj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://psu.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hhr.zhengqikj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dyx.ydzc1.top

[A26] 类型转换总览
来源：http://beg.sysykeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zkc.jianghu66.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ltw.ctjpmb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vmz.ydzc1.top

TS:   Number() String() Boolean() x as number
来源：http://dqb.pycfn.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://apl.xinyue.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ryd.yj20258.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ahn.cdnleiting.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://idr.gogol.net.cn

================================================================================
来源：http://apt.mhx1999.top

B. 流程控制
来源：http://xav.yonumen.top

================================================================================
来源：http://ypg.hesvh.cn

[B01] 条件判断 if / else
来源：http://xjy.sysykeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jfd.epnwcf.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cfm.hongshengwenyu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xel.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uuf.wangshuangyany.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hev.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bea.feifeiyinyue.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dzv.jqgfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pir.feifeiyinyue.top

[B02] 多分支 else if / elif
来源：http://dlp.snrcjt.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wmv.hammf.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rsx.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jfn.zhixingplan.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qtj.cheryme.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ele.daxiang520.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bdp.zhaomingkeji.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cnj.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hqm.dashuyun.cn

[B03] switch / match / case
来源：http://nbm.havefunace.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xlm.shanyushiyangtech.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lza.shzxlz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ubw.zdbjq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://spe.dianchejie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://urz.xuanzx.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tpo.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vuw.havefunace.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qau.fehbvm.com

[B04] for 计数循环
来源：http://nem.meibo888.top

Py:   for i in range(10): print(i)
来源：http://gxo.yueranfly.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sjk.uphjek.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ydb.ybcxt.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vvs.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dzl.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ykb.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://hde.nanxinkj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://teh.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://fxb.aizwys.cn

Py:   for item in arr: print(item)
来源：http://udo.xingfuxueyuan.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uqn.xuetiantiany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qnr.ppjwa.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dpi.sweek.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jex.daxiang520.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sne.vqdsnc.cn

Ruby: arr.each { |item| puts item }
来源：http://qpo.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jbx.sjlbkw.cn

[B06] 遍历字典 / 对象
来源：http://ywr.yj20258.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lds.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://iwh.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tnf.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xcf.andypj.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rih.hesvh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xww.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ych.daxiang520.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jer.tianlin.xyz

[B07] while 循环
来源：http://ozu.gzhubu.top

Py:   while i < 10: i += 1
来源：http://hlm.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://lhb.pycfn.com

JS:   while (i < 10) { i++; }
来源：http://ijq.xziqi.cn

TS:   while (i < 10) { i++; }
来源：http://rjj.zhengqikj.top

Java: while (i < 10) { i++; }
来源：http://juh.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mbb.jyoumei.cn

Ruby: while i < 10; i += 1; end
来源：http://lty.svipenyu.cn

C#:   while (i < 10) { i++; }
来源：http://ekb.yuanzhike.top

[B08] do-while（至少执行一次）
来源：http://ndk.chenjidiqi.icu

Py:   # 无 do-while：用 while True + break
来源：http://zzb.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://hdg.yvedp.cn

JS:   do { i++; } while (i < 10);
来源：http://xvk.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://zux.tarul.cn

Java: do { i++; } while (i < 10);
来源：http://ndf.jinqigfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zai.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://brs.meibo888.top

C#:   do { i++; } while (i < 10);
来源：http://myo.pengpengdd.cyou

[B09] break 与 continue
来源：http://hlh.tanke756.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nwk.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qkv.hongshengwenyu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pmd.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kfb.yuanzhike.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://glz.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sst.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mbp.hysaishi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hai.bjfxy.top

[B10] 遍历同时拿索引
来源：http://ugt.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lei.yonumen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ghh.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://odv.yj20258.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gbm.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bvb.c1oappe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bwb.zdqjudy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xuu.bbcook.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xlj.hnqzz.top

[B11] 生成数字序列 / 区间
来源：http://sra.sjlbkw.cn

Py:   list(range(0, 10, 2))
来源：http://tww.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://aog.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zty.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dxa.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vfy.fengsongda.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://atg.gaohongyu789.top

Ruby: (0...10).step(2).to_a
来源：http://zlu.redwolf501.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aic.ydjk.org.cn

[B12] 跳出多层循环
来源：http://dym.jyoumei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://veb.dashuyun.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://myr.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://elo.tian-w.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xkj.52xcode.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ddn.jqgfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nqy.meibo888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xnt.zhoulong.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bna.pengpengdd.cyou

[B13] 判断是否为数字
来源：http://fmq.kuanghao11.cn

Py:   isinstance(x, (int, float))
来源：http://amc.xingfuxueyuan.xyz

PHP:  is_numeric($x)
来源：http://uzg.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://elz.quarkkingdee.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wsu.ppjwa.cn

Java: x instanceof Number
来源：http://qev.hcnkem.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rdk.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://jbl.tarul.cn

C#:   x is int or double or decimal
来源：http://qbu.daxiang520.top

[B14] 判断值是否在集合内
来源：http://dwh.zhaomingkeji.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wfu.yonumen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yzn.birdmap.top

JS:   [1, 2, 3].includes(x)
来源：http://aob.zhongyouzk.top

TS:   [1, 2, 3].includes(x)
来源：http://hbb.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://vwh.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pcq.bbcook.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hts.snrcjt.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cyp.bjfxy.top

[B15] 布尔运算与取反
来源：http://zrd.zhongyouzk.top

Py:   a and b or not c
来源：http://hxj.haohaochexian.top

PHP:  $a && $b || !$c
来源：http://vxk.daria6918.cn

JS:   a && b || !c
来源：http://dyc.aibaodan.cn

TS:   a && b || !c
来源：http://uaa.xuanzx.com

Java: a && b || !c
来源：http://zjj.zhijiandao.cn

Go:   a && b || !c
来源：http://dns.sweek.top

Ruby: a && b || !c
来源：http://rin.chenlongwang.top

C#:   a && b || !c
来源：http://mmn.tian-w.cn

[B16] 卫语句：不满足条件提前返回
来源：http://liv.aizwys.cn

Py:   if not data: return
来源：http://ywk.cdnleiting.top

PHP:  if (!$data) { return; }
来源：http://old.jiagoushi.top

JS:   if (!data) return;
来源：http://knw.vqdsnc.cn

TS:   if (!data) return;
来源：http://rat.yfazqb.com

Java: if (data == null) return;
来源：http://dik.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://lrb.cheryme.top

Ruby: return if data.nil?
来源：http://rlo.yvedp.cn

C#:   if (data == null) return;
来源：http://jfb.meibo888.top

================================================================================
来源：http://wuz.yvedp.cn

C. 函数与作用域
来源：http://bkf.nanxuanxn.top

================================================================================
来源：http://sxi.kuanghao11.cn

[C01] 定义函数
来源：http://low.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://bjq.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lwz.aizwys.cn

JS:   function add(a, b) { return a + b; }
来源：http://wzb.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tqd.sufxvd.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hdr.gaohongyu789.top

Go:   func add(a, b int) int { return a + b }
来源：http://swj.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://xdq.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oth.jinqigfzy.top

[C02] 默认参数
来源：http://ulo.redwolf501.top

Py:   def greet(name="World"): return name
来源：http://vzn.dashuyun.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wzl.zhixingplan.top

JS:   function greet(name = "World") { return name; }
来源：http://cow.yangfankeji.com

TS:   function greet(name: string = "World") { return name; }
来源：http://xsd.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://vhm.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fqt.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://owc.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://wfy.zhixingplan.top

[C03] 可变参数
来源：http://edm.fengsongda.top

Py:   def total(*args): return sum(args)
来源：http://liv.yanxiufei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yiy.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uxf.zhijiandao.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kau.yongpay.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ndr.ybcxt.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yni.sysykeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://sfd.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zfn.yuanzhike.top

[C04] 命名参数 / 关键字参数
来源：http://rao.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dzc.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kdi.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gja.shanyushiyangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zbf.kuanghao11.cn

Java: // 无：用 Builder 模式或 record
来源：http://uxo.ydjk.org.cn

Go:   // 无：用配置结构体参数
来源：http://pxc.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://wuq.cqqwz.cn

C#:   f(a: 1, b: 2)
来源：http://rcg.yvedp.cn

[C05] 返回多个值
来源：http://avy.bjfxy.top

Py:   return a, b
来源：http://wfs.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://lkj.redwolf501.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ajs.daria6918.cn

TS:   return { a, b };
来源：http://izj.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iek.cheryme.top

Go:   return a, b
来源：http://vhg.0kj1m.cn

Ruby: return a, b
来源：http://lbm.hfpthk.cn

C#:   return (a, b);              // ValueTuple
来源：http://vkw.hywenlv.cn

[C06] 匿名函数 / lambda
来源：http://hmb.yongpay.top

Py:   square = lambda x: x * x
来源：http://tus.yuanzhike.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fvj.zdqjudy.top

JS:   const square = x => x * x;
来源：http://zbr.svipenyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://sue.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://odj.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://maw.yuanzhike.top

Ruby: square = ->(x) { x * x }
来源：http://zar.fktsv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kiu.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://xbg.wangshuangyany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://idw.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://pft.tarul.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://awi.jinqigufen.top

TS:   arr.map(String)
来源：http://sfo.shanyushiyangtech.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xle.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gup.jqgfzy.top

Ruby: arr.map(&:upcase)
来源：http://kvl.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://skn.fktsv.cn

[C08] 闭包
来源：http://xzu.tianlin.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://okn.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qzs.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mcm.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xut.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ufr.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tqz.xylfe.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dcy.ivvv.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vbg.jlsjyb.cn

[C09] 递归
来源：http://qgp.sxryk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hvy.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oqs.sufxvd.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wyp.pycfn.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vtt.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://foi.hywenlv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hos.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kme.cheryme.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oll.yuanzhike.top

[C10] 变量作用域
来源：http://gnt.cashguo.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fap.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ikc.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jie.jlsjyb.cn

TS:   同 JS
来源：http://bvf.yonumen.top

Java: 方法内为块级作用域
来源：http://kab.yfazqb.com

Go:   花括号块级作用域
来源：http://fnc.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mjb.ydjk.org.cn

C#:   块级作用域
来源：http://hjd.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://rgt.jqgufenzy.top

Py:   from module import func
来源：http://xpk.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://atz.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fwx.shanyushiyangtech.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sub.shzxlz.cn

Java: import java.util.List;
来源：http://cmg.haohaochexian.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://utx.quarkkingdee.top

Ruby: require "json"; require_relative "./util"
来源：http://jik.chenjidiqi.icu

C#:   using System.Text;
来源：http://hhs.yueranfly.top

[C12] 立即执行函数 IIFE
来源：http://sis.chenjidiqi.icu

Py:   (lambda: print("run"))()
来源：http://vhz.yvedp.cn

PHP:  (function () { echo "run"; })();
来源：http://kgy.gaohongyu789.top

JS:   (() => { console.log("run"); })();
来源：http://mry.sxryk.cn

TS:   (() => { console.log("run"); })();
来源：http://qqu.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mcy.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://hpz.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://oyt.pycfn.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ywm.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://gyu.sxryk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dqi.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rfl.zhiwuduotai.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vaz.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tzv.yueranfly.top

Java: int add(int a, int b) { return a + b; }
来源：http://lwm.cucudq.cn

Go:   func add(a, b int) int
来源：http://fmt.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aap.havefunace.top

C#:   int Add(int a, int b) => a + b;
来源：http://iyd.iojbl.cn

[C14] 泛型函数
来源：http://aqb.zycfv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jfr.zhijiandao.cn

PHP:  // 无泛型
来源：http://emo.uphjek.com

JS:   // 无泛型
来源：http://ygb.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://acv.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://chm.zhaomingkeji.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mau.9152youxi.cn

Ruby: # 无泛型
来源：http://zam.havefunace.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yeg.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://aza.pengpengdd.cyou

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jwt.yuanzhike.top

PHP:  [$a, $b] = $pair;
来源：http://jls.aibaodan.cn


<!-- 参考信息 -->