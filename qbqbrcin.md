代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://gdm.jianghu66.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://krm.dashuyun.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bhw.zhijiandao.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://teq.fanxiaobao.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oal.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://isb.cdnleiting.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qat.xingfuxueyuan.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qhe.hywenlv.cn

[A26] 类型转换总览
来源：http://cjh.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eck.hnqzz.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ien.cdnleiting.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://haq.daxiang520.top

TS:   Number() String() Boolean() x as number
来源：http://gdv.jyoumei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rfy.smart0.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bxn.mhx1999.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zay.chenzaomai.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://usr.fktsv.cn

================================================================================
来源：http://njk.ctjpmb.com

B. 流程控制
来源：http://oam.sxryk.cn

================================================================================
来源：http://ahr.jiagoushi.top

[B01] 条件判断 if / else
来源：http://bnp.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tfm.nanxuanxn.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gvu.daxiang520.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kym.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dfq.sysykeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cre.daria6918.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://soe.nwbrower.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://beu.xylfe.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fta.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://wfv.fktsv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dyu.chenjidiqi.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rym.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dae.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yms.mhx1999.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bkh.pengpengdd.cyou

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qop.chenlongwang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tno.jlsjyb.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://erb.jinqigfzy.top

[B03] switch / match / case
来源：http://dcm.zhongyouzk.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jjx.gotoacloud.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kfm.yj20258.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fql.xuanzx.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kzd.uphjek.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tim.nanxuanxn.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zgc.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hqp.zycfv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ngf.nanxinkj.top

[B04] for 计数循环
来源：http://ydp.fzhhl.top

Py:   for i in range(10): print(i)
来源：http://crx.ctjpmb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ppk.316326.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vdq.tian-w.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nkw.guowangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ojq.tanke756.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://abo.hysaishi.cn

Ruby: 10.times { |i| puts i }
来源：http://mku.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kxk.tian-w.cn

[B05] 遍历数组 / 列表
来源：http://vms.aibaodan.cn

Py:   for item in arr: print(item)
来源：http://max.gzhubu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jlz.zhijiandao.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cqw.c1oappe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://pek.tarul.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nma.tianlin.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xox.hnxiangtu.top

Ruby: arr.each { |item| puts item }
来源：http://ruz.aibaodan.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hjz.smart0.xyz

[B06] 遍历字典 / 对象
来源：http://jxn.hesvh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cjd.jyoumei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://orp.iojbl.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qqg.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rsf.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xqm.hammf.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://axj.jinyuanbaomall.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sdx.daria6918.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aba.zhaomingkeji.xyz

[B07] while 循环
来源：http://dgy.yuanzhike.top

Py:   while i < 10: i += 1
来源：http://ycf.aizwys.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qwz.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://fik.aizwys.cn

TS:   while (i < 10) { i++; }
来源：http://sfw.cqqwz.cn

Java: while (i < 10) { i++; }
来源：http://ddh.xingfuxueyuan.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tfg.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://ete.cheryme.top

C#:   while (i < 10) { i++; }
来源：http://tdo.ppjwa.cn

[B08] do-while（至少执行一次）
来源：http://bny.chenlongwang.top

Py:   # 无 do-while：用 while True + break
来源：http://woq.yongpay.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nvc.cqqwz.cn

JS:   do { i++; } while (i < 10);
来源：http://cjf.meibo888.top

TS:   do { i++; } while (i < 10);
来源：http://kdt.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://bpj.uphjek.com

Go:   for { i++; if i >= 10 { break } }
来源：http://ilq.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://boo.ydzc1.top

C#:   do { i++; } while (i < 10);
来源：http://vcx.smart0.xyz

[B09] break 与 continue
来源：http://qnx.mhx1999.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ebz.ydzc1.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jcp.yongpay.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://csx.c1oappe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yao.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ydc.xuanzx.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://egt.birdmap.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wwn.tian-w.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://llr.ppjwa.cn

[B10] 遍历同时拿索引
来源：http://rnb.jinyuanbaomall.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mbi.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oaa.ehwqpu.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yll.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://onr.daria6918.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nes.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xod.jinqigfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vjo.smart0.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mep.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://prp.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://vvx.yuanzhike.top

PHP:  range(0, 10, 2);
来源：http://zgh.aizwys.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pfx.c1oappe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zvw.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://inw.yuxming.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wmh.pycfn.com

Ruby: (0...10).step(2).to_a
来源：http://pci.fktsv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pkx.fengsongda.top

[B12] 跳出多层循环
来源：http://ifb.jinyuanbaomall.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zrc.52xcode.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zxl.xylfe.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://znb.bjfxy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wgi.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ton.hysaishi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qra.quarkkingdee.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dlt.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pom.yueranfly.top

[B13] 判断是否为数字
来源：http://nbn.ywan-chungtsiang.top

Py:   isinstance(x, (int, float))
来源：http://ouy.jqgfzy.top

PHP:  is_numeric($x)
来源：http://ynd.cashguo.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nme.bjfxy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cdu.xinyue.icu

Java: x instanceof Number
来源：http://xzt.sjlbkw.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mxb.cheryme.top

Ruby: x.is_a?(Numeric)
来源：http://rti.jiagoushi.top

C#:   x is int or double or decimal
来源：http://kpj.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://cwh.iojbl.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hpc.xinyue.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pfh.zdbjq.cn

JS:   [1, 2, 3].includes(x)
来源：http://lsj.smart0.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ocx.zdqjudy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ayr.jqgfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ovw.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oia.xuanzx.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wyr.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://krr.ydjk.org.cn

Py:   a and b or not c
来源：http://kqy.daxiang520.top

PHP:  $a && $b || !$c
来源：http://dkw.aizwys.cn

JS:   a && b || !c
来源：http://ofn.birdmap.top

TS:   a && b || !c
来源：http://tlu.chenzaomai.com

Java: a && b || !c
来源：http://pwp.ywan-chungtsiang.top

Go:   a && b || !c
来源：http://ipa.yj20258.top

Ruby: a && b || !c
来源：http://aui.sxryk.cn

C#:   a && b || !c
来源：http://khq.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zzz.jinyuanbaomall.cn

Py:   if not data: return
来源：http://vkx.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://jaq.ivvv.top

JS:   if (!data) return;
来源：http://zmd.ppjwa.cn

TS:   if (!data) return;
来源：http://rlf.shanyushiyangkeji.top

Java: if (data == null) return;
来源：http://vod.bbcook.cn

Go:   if data == nil { return }
来源：http://egf.9152youxi.cn

Ruby: return if data.nil?
来源：http://nnj.ybcxt.top

C#:   if (data == null) return;
来源：http://nbf.uphjek.com

================================================================================
来源：http://nqb.316326.xyz

C. 函数与作用域
来源：http://mzl.tarul.cn

================================================================================
来源：http://ipf.hesvh.cn

[C01] 定义函数
来源：http://cgr.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://aqv.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cdo.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://wfs.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bzy.svipenyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fgy.chenlongwang.top

Go:   func add(a, b int) int { return a + b }
来源：http://fms.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://zkl.hywenlv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://imw.hongshengwenyu.top

[C02] 默认参数
来源：http://hcq.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://jsp.fengsongda.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lvu.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://zsf.jiagoushi.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xec.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bhk.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fwc.vehdjk.com

Ruby: def greet(name = "World") = name
来源：http://jcu.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://cap.ybcxt.top

[C03] 可变参数
来源：http://xrt.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://tiz.yongpay.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oau.yj202588.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vim.hnxiangtu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eps.gogol.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ekk.wangdashe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wti.yuxming.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wif.yj20258888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iyb.yj202588.top

[C04] 命名参数 / 关键字参数
来源：http://lyb.gogol.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cci.jinqigufen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rxv.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rcj.andypj.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vip.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://cyh.daria6918.cn

Go:   // 无：用配置结构体参数
来源：http://sqn.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://tvj.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://fsq.jianghu66.top

[C05] 返回多个值
来源：http://hin.nanxinkj.top

Py:   return a, b
来源：http://exj.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://gsh.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ogd.fehbvm.com

TS:   return { a, b };
来源：http://aha.pycfn.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ldo.jinqigufen.top

Go:   return a, b
来源：http://kie.nanxuanxn.top

Ruby: return a, b
来源：http://fpq.jinghuilouyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://sxc.feifeiyinyue.top

[C06] 匿名函数 / lambda
来源：http://rfy.aizwys.cn

Py:   square = lambda x: x * x
来源：http://flm.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://iei.sysykeji.top

JS:   const square = x => x * x;
来源：http://vik.jyoumei.cn

TS:   const square = (x: number): number => x * x;
来源：http://cmb.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kle.havefunace.top

Go:   sq := func(x int) int { return x * x }
来源：http://pqo.jinqigfzy.top

Ruby: square = ->(x) { x * x }
来源：http://hgb.sysykeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://nry.hammf.cn

[C07] 把函数作为参数传入
来源：http://voq.jinghuilouyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bry.zhengqikj.top

PHP:  array_map("strtoupper", $arr);
来源：http://nun.sjlbkw.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jls.snrcjt.cn

TS:   arr.map(String)
来源：http://aao.jqgufenzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rgc.wangdashe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ehd.daxiang520.top

Ruby: arr.map(&:upcase)
来源：http://etg.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vcm.shzxlz.cn

[C08] 闭包
来源：http://cuw.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dpl.smart0.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ccv.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cfk.gzhubu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tzr.yfazqb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://foe.ydzc1.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cgg.daria6918.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gpt.fzhhl.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lyc.xinyue.icu

[C09] 递归
来源：http://bvb.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xhv.yonumen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://apd.sweek.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gaa.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://stv.cashguo.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://msd.jinyuanbaomall.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://irc.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fed.daxiang520.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fbw.xingfuxueyuan.xyz

[C10] 变量作用域
来源：http://xkp.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://amj.haohaochexian.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nza.jqgufenzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tiy.quarkkingdee.top

TS:   同 JS
来源：http://atj.9152youxi.cn

Java: 方法内为块级作用域
来源：http://ilc.nanxuanxn.top

Go:   花括号块级作用域
来源：http://yjs.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nhk.jinqigfzy.top

C#:   块级作用域
来源：http://fys.yj202588.top

[C11] 模块导入与导出
来源：http://qoy.sjlbkw.cn

Py:   from module import func
来源：http://npl.shuidangran.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fwt.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hus.zhiwuduotai.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xcb.ppjwa.cn

Java: import java.util.List;
来源：http://uau.dashuyun.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qoe.kuanghao11.cn

Ruby: require "json"; require_relative "./util"
来源：http://tku.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://dld.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://vek.yanxiufei.cn

Py:   (lambda: print("run"))()
来源：http://rns.redwolf501.top

PHP:  (function () { echo "run"; })();
来源：http://pkv.ydzc1.top

JS:   (() => { console.log("run"); })();
来源：http://ksk.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://gzr.hammf.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://teo.cashguo.top

Go:   func() { fmt.Println("run") }()
来源：http://khh.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://ufm.meibo888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://osh.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://ceq.aibaodan.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iey.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cyu.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yun.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://puq.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://joe.andypj.xyz

Go:   func add(a, b int) int
来源：http://lek.jinghuilouyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xtd.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hdb.jqgufenzy.top

[C14] 泛型函数
来源：http://ekk.snrcjt.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ceu.fehbvm.com

PHP:  // 无泛型
来源：http://obh.jinqigfzy.top

JS:   // 无泛型
来源：http://vmh.sjlbkw.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qxk.andypj.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://isk.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oxc.sweek.top

Ruby: # 无泛型
来源：http://bmh.jinqigufen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vbz.zhengqikj.top

[C15] 解构 / 展开参数
来源：http://jum.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cgi.gzhubu.top

PHP:  [$a, $b] = $pair;
来源：http://rhn.ehwqpu.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rfj.zhaomingkeji.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sys.yj202588.top

Java: // 无解构
来源：http://lcz.hcnkem.com

Go:   // 无解构
来源：http://apk.zhixingplan.top


<!-- 参考信息 -->