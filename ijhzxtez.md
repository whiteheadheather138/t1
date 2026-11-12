代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://wqi.meibo888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://isr.gogol.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rzr.jinghuilouyu.cn

[A25] 字符串比较
来源：http://mcn.316326.xyz

Py:   s1 == s2; s1 != s2
来源：http://qdf.jinqigufen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://duz.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mpo.zhiwuduotai.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xdn.zhengqikj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zxo.cdnleiting.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uik.jyoumei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rbe.hysaishi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hkf.nanxinkj.top

[A26] 类型转换总览
来源：http://rlr.yongpay.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pnh.mhx1999.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mzv.xuetiantiany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://otj.xuetiantiany.cn

TS:   Number() String() Boolean() x as number
来源：http://btu.jinghuilouyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ksu.vehdjk.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jjg.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://yac.sjlbkw.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uet.zdqjudy.top

================================================================================
来源：http://sxs.birdmap.top

B. 流程控制
来源：http://adr.zhaomingkeji.xyz

================================================================================
来源：http://myd.xuanzx.com

[B01] 条件判断 if / else
来源：http://jun.ydjk.org.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wld.fehbvm.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vkx.kuanghao11.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jbg.redwolf501.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nxz.andypj.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://err.jyoumei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hml.hywenlv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zii.jlsjyb.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://enl.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://wam.havefunace.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gsc.shangyingyoupin.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://czu.yanxiufei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eij.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lvv.yvedp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xwx.yj20258888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://huy.zhixingplan.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://plm.vqdsnc.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bkb.yj20258888.top

[B03] switch / match / case
来源：http://mrv.hywenlv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fps.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ynw.zhixingplan.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nso.yuxming.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bjn.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zjo.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oqt.vqdsnc.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gai.fehbvm.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mdg.nanxinkj.top

[B04] for 计数循环
来源：http://vpw.0kj1m.cn

Py:   for i in range(10): print(i)
来源：http://kcq.cdnleiting.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://swn.shzxlz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pub.svipenyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jbq.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://krp.ydjk.org.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ybf.hammf.cn

Ruby: 10.times { |i| puts i }
来源：http://zzy.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ise.redwolf501.top

[B05] 遍历数组 / 列表
来源：http://wqd.epnwcf.com

Py:   for item in arr: print(item)
来源：http://qfi.jinqigfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://luv.jinyuanbaomall.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yqs.yanxiufei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mwm.daria6918.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://top.chenzaomai.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vab.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://jke.zhixingplan.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xpx.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://xkm.yvedp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://aoy.ybcxt.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tlj.cdnleiting.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://twx.fktsv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://onj.tanke756.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://llx.dianchejie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sww.jinqigfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://the.cucudq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gga.gotoacloud.top

[B07] while 循环
来源：http://kkl.zycfv.cn

Py:   while i < 10: i += 1
来源：http://efl.yueranfly.top

PHP:  while ($i < 10) { $i++; }
来源：http://xhn.daria6918.cn

JS:   while (i < 10) { i++; }
来源：http://mvd.aizwys.cn

TS:   while (i < 10) { i++; }
来源：http://ski.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://bwu.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qau.yongpay.top

Ruby: while i < 10; i += 1; end
来源：http://yhc.jinyuanbaomall.cn

C#:   while (i < 10) { i++; }
来源：http://iee.316326.xyz

[B08] do-while（至少执行一次）
来源：http://vzo.ybcxt.top

Py:   # 无 do-while：用 while True + break
来源：http://ycs.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pim.fengsongda.top

JS:   do { i++; } while (i < 10);
来源：http://onm.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://ide.yvedp.cn

Java: do { i++; } while (i < 10);
来源：http://fxc.jinqigufen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xyl.gzhubu.top

Ruby: begin; i += 1; end while i < 10
来源：http://gts.vqdsnc.cn

C#:   do { i++; } while (i < 10);
来源：http://kfd.nanxinkj.top

[B09] break 与 continue
来源：http://gxk.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zhf.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tfh.hammf.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nkh.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xtc.shanyushiyangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wmi.chenlongwang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://evt.ppjwa.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cwo.daxiang520.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://thw.316326.xyz

[B10] 遍历同时拿索引
来源：http://yns.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dai.iojbl.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nrc.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yai.shanyushiyangtech.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://trd.yongpay.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jrb.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pdo.meibo888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fkk.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mkv.pengpengdd.cyou

[B11] 生成数字序列 / 区间
来源：http://pkn.hesvh.cn

Py:   list(range(0, 10, 2))
来源：http://zip.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://oon.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mex.jqgufenzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bfh.mhx1999.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aqe.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eha.zdbjq.cn

Ruby: (0...10).step(2).to_a
来源：http://qyg.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yno.guannengcc.top

[B12] 跳出多层循环
来源：http://ygz.epnwcf.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://dbk.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ohy.havefunace.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ryl.zhongyouzk.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vkh.tanke756.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sfd.pycfn.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://huf.zhongyouzk.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bqp.sjlbkw.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://shk.jqgufenzy.top

[B13] 判断是否为数字
来源：http://hhw.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://fvo.zdbjq.cn

PHP:  is_numeric($x)
来源：http://rug.nwbrower.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mqd.9152youxi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qxs.tian-w.cn

Java: x instanceof Number
来源：http://vjy.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pjv.ivvv.top

Ruby: x.is_a?(Numeric)
来源：http://zbn.redwolf501.top

C#:   x is int or double or decimal
来源：http://kvx.snrcjt.cn

[B14] 判断值是否在集合内
来源：http://shi.hongshengwenyu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://une.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://har.yuxming.cn

JS:   [1, 2, 3].includes(x)
来源：http://fud.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://owr.wangdashe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vdn.andypj.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lbg.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://ntr.svipenyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wmv.c1oappe.top

[B15] 布尔运算与取反
来源：http://xlj.kuanghao11.cn

Py:   a and b or not c
来源：http://lyx.vehdjk.com

PHP:  $a && $b || !$c
来源：http://csj.ctjpmb.com

JS:   a && b || !c
来源：http://wfb.pycfn.com

TS:   a && b || !c
来源：http://azv.hnxiangtu.top

Java: a && b || !c
来源：http://qnj.guannengcc.top

Go:   a && b || !c
来源：http://xwx.hnqzz.top

Ruby: a && b || !c
来源：http://cbv.9152youxi.cn

C#:   a && b || !c
来源：http://pam.jiagoushi.top

[B16] 卫语句：不满足条件提前返回
来源：http://shg.iojbl.cn

Py:   if not data: return
来源：http://msn.yj202588.top

PHP:  if (!$data) { return; }
来源：http://mlv.zhaomingkeji.xyz

JS:   if (!data) return;
来源：http://csm.cheryme.top

TS:   if (!data) return;
来源：http://hph.yanxiufei.cn

Java: if (data == null) return;
来源：http://poz.tianlin.xyz

Go:   if data == nil { return }
来源：http://zru.xuanzx.com

Ruby: return if data.nil?
来源：http://dya.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://ldk.gaohongyu789.top

================================================================================
来源：http://qir.iojbl.cn

C. 函数与作用域
来源：http://syh.sysykeji.top

================================================================================
来源：http://ybk.fehbvm.com

[C01] 定义函数
来源：http://mcb.iojbl.cn

Py:   def add(a, b): return a + b
来源：http://htz.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://grk.sxryk.cn

JS:   function add(a, b) { return a + b; }
来源：http://xgl.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dhe.yuanzhike.top

Java: static int add(int a, int b) { return a + b; }
来源：http://eea.sjlbkw.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mhm.zhongyouzk.top

Ruby: def add(a, b); a + b; end
来源：http://gkl.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hfs.shanyushiyangtech.top

[C02] 默认参数
来源：http://cae.cashguo.top

Py:   def greet(name="World"): return name
来源：http://nkp.yvedp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ygq.zdqjudy.top

JS:   function greet(name = "World") { return name; }
来源：http://xcm.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nzo.52xcode.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bbg.hfpthk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wnk.kuanghao11.cn

Ruby: def greet(name = "World") = name
来源：http://mls.guannengcc.top

C#:   string Greet(string name = "World") => name;
来源：http://nzd.tarul.cn

[C03] 可变参数
来源：http://gdf.kuanghao11.cn

Py:   def total(*args): return sum(args)
来源：http://qdo.jinqigfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ekm.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://orq.zycfv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rpf.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hmb.shanyushiyangtech.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pdk.epnwcf.com

Ruby: def total(*nums); nums.sum; end
来源：http://baq.tian-w.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fqe.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://btg.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qqp.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uyx.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://thj.ybcxt.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wht.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://aup.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://vfg.ehwqpu.com

Ruby: f(a: 1, b: 2)
来源：http://gwp.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://jlu.cdnleiting.top

[C05] 返回多个值
来源：http://otk.iojbl.cn

Py:   return a, b
来源：http://bku.aizwys.cn

PHP:  return [$a, $b];
来源：http://flj.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pxe.yfazqb.com

TS:   return { a, b };
来源：http://aki.shanyushiyangtech.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wny.chenzaomai.com

Go:   return a, b
来源：http://tmw.svipenyu.cn

Ruby: return a, b
来源：http://vjv.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ldq.bjfxy.top

[C06] 匿名函数 / lambda
来源：http://bfx.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://uzw.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qve.meibo888.top

JS:   const square = x => x * x;
来源：http://rna.yuanzhike.top

TS:   const square = (x: number): number => x * x;
来源：http://aic.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ibp.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bhb.jlsjyb.cn

Ruby: square = ->(x) { x * x }
来源：http://jyn.jyoumei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qgp.yj20258888.top

[C07] 把函数作为参数传入
来源：http://eki.cdnleiting.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lgw.0kj1m.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vzw.shanyushiyangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lak.0kj1m.cn

TS:   arr.map(String)
来源：http://kus.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gan.zdbjq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fzq.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://kwu.kuanghao11.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dah.jianghu66.top

[C08] 闭包
来源：http://nwg.yongpay.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hpj.0kj1m.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://obi.chenjidiqi.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bmg.jinyuanbaomall.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dvf.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pmt.iojbl.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://snb.shuidangran.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ibq.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gqu.bjfxy.top

[C09] 递归
来源：http://ydv.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://crm.gotoacloud.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mkp.xinyue.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tzs.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nif.zhongyouzk.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pbg.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kud.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cje.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rml.ctjpmb.com

[C10] 变量作用域
来源：http://qnw.xziqi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ufc.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ndq.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wav.gotoacloud.top

TS:   同 JS
来源：http://ppz.52xcode.cn

Java: 方法内为块级作用域
来源：http://osh.zycfv.cn

Go:   花括号块级作用域
来源：http://jbd.smart0.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://scs.yonumen.top

C#:   块级作用域
来源：http://vln.tarul.cn

[C11] 模块导入与导出
来源：http://abb.jlsjyb.cn

Py:   from module import func
来源：http://nwz.redwolf501.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cwc.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zxg.52xcode.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sur.gaohongyu789.top

Java: import java.util.List;
来源：http://uly.jiagoushi.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hoa.tianlin.xyz

Ruby: require "json"; require_relative "./util"
来源：http://jrt.yonumen.top

C#:   using System.Text;
来源：http://qbr.tian-w.cn

[C12] 立即执行函数 IIFE
来源：http://cse.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://ksg.zdqjudy.top

PHP:  (function () { echo "run"; })();
来源：http://iqo.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://hqw.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://zoc.dashuyun.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wyb.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://epl.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://msx.jiagoushi.top

C#:   // 无 IIFE：用静态构造函数
来源：http://djz.cdnleiting.top

[C13] 类型声明 / 类型注解
来源：http://nuz.haohaochexian.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hff.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sjf.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xgw.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wis.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://wja.ppjwa.cn

Go:   func add(a, b int) int
来源：http://onr.sjlbkw.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kem.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dyi.fengsongda.top

[C14] 泛型函数
来源：http://bju.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sfp.sjlbkw.cn

PHP:  // 无泛型
来源：http://wpg.gogol.net.cn

JS:   // 无泛型
来源：http://qhy.jiagoushi.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wkk.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xsj.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nmm.jqgufenzy.top

Ruby: # 无泛型
来源：http://xad.xziqi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qop.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://tlq.tarul.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oeo.aizwys.cn

PHP:  [$a, $b] = $pair;
来源：http://tgw.fengsongda.top


<!-- 参考信息 -->