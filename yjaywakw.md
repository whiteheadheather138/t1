代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vtq.jinqigufen.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kfj.ywan-chungtsiang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rgp.zdbjq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oop.quarkkingdee.top

Go:   strings.TrimSpace(s)
来源：http://jrq.cucudq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ghu.zhaomingkeji.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gkw.ppjwa.cn

[A25] 字符串比较
来源：http://yea.ydjk.org.cn

Py:   s1 == s2; s1 != s2
来源：http://yol.guowangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://puz.chenlongwang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://khi.fktsv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wqd.hongshengwenyu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hoe.jlsjyb.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nhw.hcnkem.com

Ruby: s1 == s2; s1 <=> s2
来源：http://fgy.hesvh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oia.kuanghao11.cn

[A26] 类型转换总览
来源：http://ltg.jiagoushi.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sgk.hysaishi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ymt.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://act.jinqigfzy.top

TS:   Number() String() Boolean() x as number
来源：http://mpy.guowangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gla.shuidangran.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ryb.bjfxy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ceq.jinqigfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yld.daria6918.cn

================================================================================
来源：http://efn.chenlongwang.top

B. 流程控制
来源：http://egx.tarul.cn

================================================================================
来源：http://xvd.fanxiaobao.xyz

[B01] 条件判断 if / else
来源：http://lfy.316326.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://xqh.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ifd.cqqwz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hwc.xinyue.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gki.zhongyouzk.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fyi.ydjk.org.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gzr.0kj1m.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mfa.feifeiyinyue.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yxx.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://akt.epnwcf.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wqn.cheryme.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://esg.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://myu.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xxg.snrcjt.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dvt.zdqjudy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://evo.shzxlz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gnx.yvedp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nkv.sysykeji.top

[B03] switch / match / case
来源：http://toi.zhijiandao.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oee.shanyushiyangtech.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mvw.hfpthk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ktg.shuidangran.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qtr.zdbjq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lwp.wangdashe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://udq.hfpthk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tjo.fktsv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zrt.aibaodan.cn

[B04] for 计数循环
来源：http://rnx.hcnkem.com

Py:   for i in range(10): print(i)
来源：http://gcs.shanyushiyangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nid.c1oappe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wao.kuanghao11.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qup.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hrb.cqqwz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://icv.fanxiaobao.xyz

Ruby: 10.times { |i| puts i }
来源：http://ndw.shzxlz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dlk.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://jjn.hongshengwenyu.top

Py:   for item in arr: print(item)
来源：http://mul.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ysx.52xcode.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mym.ywan-chungtsiang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cxr.tarul.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://czm.nanxinkj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sko.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://ffb.chenzaomai.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nld.wangshuangyany.cn

[B06] 遍历字典 / 对象
来源：http://xnb.chenjidiqi.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://jwr.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oxy.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lce.fehbvm.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://htp.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oia.zhaomingkeji.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lih.yuxming.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pdy.hcnkem.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://inr.kuanghao11.cn

[B07] while 循环
来源：http://ufi.chenjidiqi.icu

Py:   while i < 10: i += 1
来源：http://lqi.gotoacloud.top

PHP:  while ($i < 10) { $i++; }
来源：http://nrl.shanyushiyangtech.top

JS:   while (i < 10) { i++; }
来源：http://vfp.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://ycf.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://ahv.hesvh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qbz.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://vmk.cheryme.top

C#:   while (i < 10) { i++; }
来源：http://kjt.cashguo.top

[B08] do-while（至少执行一次）
来源：http://uxe.jqgfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://psq.daxiang520.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lko.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://mgu.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://trb.nanxuanxn.top

Java: do { i++; } while (i < 10);
来源：http://cnz.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mld.ydjk.org.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mzf.epnwcf.com

C#:   do { i++; } while (i < 10);
来源：http://pcx.yueranfly.top

[B09] break 与 continue
来源：http://hwq.sxryk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gwi.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sfa.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rbb.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tvq.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pew.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kbr.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vyl.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mms.cucudq.cn

[B10] 遍历同时拿索引
来源：http://adj.aibaodan.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gva.jqgufenzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tzu.sjlbkw.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://flb.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://usu.ywan-chungtsiang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rrs.hcnkem.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ccn.xingfuxueyuan.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fof.316326.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lvp.yvedp.cn

[B11] 生成数字序列 / 区间
来源：http://vpu.0kj1m.cn

Py:   list(range(0, 10, 2))
来源：http://ber.hnqzz.top

PHP:  range(0, 10, 2);
来源：http://zjm.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ldb.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uio.smart0.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gyq.jlsjyb.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://olv.hnxiangtu.top

Ruby: (0...10).step(2).to_a
来源：http://pza.hcnkem.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ljk.52xcode.cn

[B12] 跳出多层循环
来源：http://scz.bbcook.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uzj.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fns.zhijiandao.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nwn.daria6918.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://krg.zdbjq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hia.vqdsnc.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sxe.shangyingyoupin.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mae.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pmn.tanke756.top

[B13] 判断是否为数字
来源：http://qci.ydzc1.top

Py:   isinstance(x, (int, float))
来源：http://elv.jiagoushi.top

PHP:  is_numeric($x)
来源：http://cgr.jqgufenzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xsx.ctjpmb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://try.zycfv.cn

Java: x instanceof Number
来源：http://zrz.sxryk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jwj.andypj.xyz

Ruby: x.is_a?(Numeric)
来源：http://fiq.yj202588.top

C#:   x is int or double or decimal
来源：http://rtw.316326.xyz

[B14] 判断值是否在集合内
来源：http://cmu.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ody.nanxinkj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zhs.pycfn.com

JS:   [1, 2, 3].includes(x)
来源：http://fnj.andypj.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ttr.zhengqikj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://huw.svipenyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pom.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://fbr.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://btp.iojbl.cn

[B15] 布尔运算与取反
来源：http://bdc.xinyue.icu

Py:   a and b or not c
来源：http://aic.jinqigufen.top

PHP:  $a && $b || !$c
来源：http://qdt.jinqigufen.top

JS:   a && b || !c
来源：http://vzp.cucudq.cn

TS:   a && b || !c
来源：http://rpf.yueranfly.top

Java: a && b || !c
来源：http://vfa.jiagoushi.top

Go:   a && b || !c
来源：http://jtw.chenlongwang.top

Ruby: a && b || !c
来源：http://quc.zhengqikj.top

C#:   a && b || !c
来源：http://gkz.xinyue.icu

[B16] 卫语句：不满足条件提前返回
来源：http://iyn.9152youxi.cn

Py:   if not data: return
来源：http://asy.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://lef.jiagoushi.top

JS:   if (!data) return;
来源：http://xpe.zycfv.cn

TS:   if (!data) return;
来源：http://awt.sweek.top

Java: if (data == null) return;
来源：http://zfa.316326.xyz

Go:   if data == nil { return }
来源：http://azp.fehbvm.com

Ruby: return if data.nil?
来源：http://mma.jyoumei.cn

C#:   if (data == null) return;
来源：http://fix.ppjwa.cn

================================================================================
来源：http://mzk.yj20258888.top

C. 函数与作用域
来源：http://idt.bjfxy.top

================================================================================
来源：http://maj.yuxming.cn

[C01] 定义函数
来源：http://qhu.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://amy.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zpy.wangdashe.top

JS:   function add(a, b) { return a + b; }
来源：http://rxp.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jgu.zdqjudy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://obt.xinyue.icu

Go:   func add(a, b int) int { return a + b }
来源：http://acc.jinghuilouyu.cn

Ruby: def add(a, b); a + b; end
来源：http://khj.shanyushiyangtech.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bsd.ehwqpu.com

[C02] 默认参数
来源：http://lxo.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://nkb.c1oappe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lfj.xylfe.cn

JS:   function greet(name = "World") { return name; }
来源：http://cco.snrcjt.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fgm.fktsv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://srf.shanyushiyangkeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zyi.yanxiufei.cn

Ruby: def greet(name = "World") = name
来源：http://yir.jyoumei.cn

C#:   string Greet(string name = "World") => name;
来源：http://pjv.sjlbkw.cn

[C03] 可变参数
来源：http://mdv.yfazqb.com

Py:   def total(*args): return sum(args)
来源：http://esi.yuanzhike.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zig.ppjwa.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gbh.chenzaomai.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zdu.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xug.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kjq.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://bed.sjlbkw.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jhc.fehbvm.com

[C04] 命名参数 / 关键字参数
来源：http://yek.andypj.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qjj.gaohongyu789.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zyk.zhijiandao.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kqz.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ota.gaohongyu789.top

Java: // 无：用 Builder 模式或 record
来源：http://xhw.cashguo.top

Go:   // 无：用配置结构体参数
来源：http://vpk.birdmap.top

Ruby: f(a: 1, b: 2)
来源：http://xsn.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://myn.0kj1m.cn

[C05] 返回多个值
来源：http://fiw.jlsjyb.cn

Py:   return a, b
来源：http://cit.ybcxt.top

PHP:  return [$a, $b];
来源：http://hqq.gotoacloud.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ryd.cheryme.top

TS:   return { a, b };
来源：http://ynk.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ngb.sxryk.cn

Go:   return a, b
来源：http://nex.haohaochexian.top

Ruby: return a, b
来源：http://fit.dashuyun.cn

C#:   return (a, b);              // ValueTuple
来源：http://zit.tianlin.xyz

[C06] 匿名函数 / lambda
来源：http://xec.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://cwv.wangdashe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dzz.jlsjyb.cn

JS:   const square = x => x * x;
来源：http://wyd.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://rtf.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fqn.guowangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://jmw.chenzaomai.com

Ruby: square = ->(x) { x * x }
来源：http://jtr.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://pmo.zdbjq.cn

[C07] 把函数作为参数传入
来源：http://uai.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qnl.hysaishi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://log.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://twk.shzxlz.cn

TS:   arr.map(String)
来源：http://oui.zhixingplan.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ljz.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://umc.jqgufenzy.top

Ruby: arr.map(&:upcase)
来源：http://aej.cashguo.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tre.zhengqikj.top

[C08] 闭包
来源：http://bkx.daxiang520.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qat.nanxuanxn.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nme.chenzaomai.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hmj.tarul.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kfs.feifeiyinyue.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pic.zhongyouzk.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qnv.nanxuanxn.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://erm.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://amx.wangdashe.top

[C09] 递归
来源：http://eua.jinqigufen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uem.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hmo.yangfankeji.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qxe.fanxiaobao.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yrv.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gsl.jinqigfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aoy.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kqk.svipenyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qkb.yfazqb.com

[C10] 变量作用域
来源：http://qht.gotoacloud.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xsw.fengsongda.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://per.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dxn.hysaishi.cn

TS:   同 JS
来源：http://fhv.yj20258.top

Java: 方法内为块级作用域
来源：http://jld.ydjk.org.cn

Go:   花括号块级作用域
来源：http://tvz.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lkg.ydzc1.top

C#:   块级作用域
来源：http://hpq.ywan-chungtsiang.top

[C11] 模块导入与导出
来源：http://puw.shuidangran.top

Py:   from module import func
来源：http://yhj.jinyuanbaomall.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hdi.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nqc.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pwt.guannengcc.top

Java: import java.util.List;
来源：http://sbu.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gua.zhijiandao.cn

Ruby: require "json"; require_relative "./util"
来源：http://hkc.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://fns.jlsjyb.cn

[C12] 立即执行函数 IIFE
来源：http://ycu.epnwcf.com

Py:   (lambda: print("run"))()
来源：http://xus.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://awy.uphjek.com

JS:   (() => { console.log("run"); })();
来源：http://bfu.kuanghao11.cn

TS:   (() => { console.log("run"); })();
来源：http://yuu.fzhhl.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gfx.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://dan.jlsjyb.cn

Ruby: -> { puts "run" }.call
来源：http://tso.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://omj.zhengqikj.top

[C13] 类型声明 / 类型注解
来源：http://cma.jianghu66.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eed.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zng.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nxg.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vvd.jinqigufen.top

Java: int add(int a, int b) { return a + b; }
来源：http://iik.fehbvm.com

Go:   func add(a, b int) int
来源：http://lyz.redwolf501.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rei.xuanzx.com

C#:   int Add(int a, int b) => a + b;
来源：http://dkq.meibo888.top

[C14] 泛型函数
来源：http://muw.dianchejie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ilb.sjlbkw.cn

PHP:  // 无泛型
来源：http://bnc.sysykeji.top

JS:   // 无泛型
来源：http://htb.9152youxi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vbx.zhixingplan.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tbv.guannengcc.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tsk.mhx1999.top

Ruby: # 无泛型
来源：http://lhz.yj20258.top


<!-- 参考信息 -->