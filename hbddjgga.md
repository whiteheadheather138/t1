代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jtq.sxryk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jwn.zdbjq.cn

[A24] 去除首尾空白
来源：http://fja.gogol.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://plc.meibo888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kdc.ybcxt.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://agr.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wkf.shanyushiyangkeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nti.jinyuanbaomall.cn

Go:   strings.TrimSpace(s)
来源：http://hzj.shanyushiyangtech.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jrh.bjfxy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://njz.gzhubu.top

[A25] 字符串比较
来源：http://eln.fanxiaobao.xyz

Py:   s1 == s2; s1 != s2
来源：http://kgk.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tlq.gaohongyu789.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qrs.ivvv.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://okq.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cdp.jianghu66.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fqw.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qfo.xinyue.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ssr.yfazqb.com

[A26] 类型转换总览
来源：http://ncf.sufxvd.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jbr.zhoulong.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ack.sweek.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://snb.sjlbkw.cn

TS:   Number() String() Boolean() x as number
来源：http://ema.nanxuanxn.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ajm.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xog.hammf.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sxp.meibo888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vfy.xuanzx.com

================================================================================
来源：http://ufr.xylfe.cn

B. 流程控制
来源：http://dww.hammf.cn

================================================================================
来源：http://spl.sjlbkw.cn

[B01] 条件判断 if / else
来源：http://gwt.jiagoushi.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xmi.cashguo.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://idi.gotoacloud.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sjp.ydzc1.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hcu.52xcode.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://svo.aibaodan.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vnw.yueranfly.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://laz.zdbjq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://slt.bbcook.cn

[B02] 多分支 else if / elif
来源：http://whi.andypj.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://teq.hesvh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lqh.sysykeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pae.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jmt.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ubp.ydjk.org.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://idh.52xcode.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wlt.xziqi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gzk.hcnkem.com

[B03] switch / match / case
来源：http://yby.hywenlv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jxc.shangyingyoupin.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qox.jinghuilouyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qah.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yht.cheryme.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://chx.sweek.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://raf.xziqi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pbn.shuidangran.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mvj.zdbjq.cn

[B04] for 计数循环
来源：http://bgw.bbcook.cn

Py:   for i in range(10): print(i)
来源：http://bci.jinghuilouyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rbk.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lpm.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fgh.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://chd.epnwcf.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xxc.cqqwz.cn

Ruby: 10.times { |i| puts i }
来源：http://yyq.ivvv.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tvm.hnqzz.top

[B05] 遍历数组 / 列表
来源：http://qkr.fanxiaobao.xyz

Py:   for item in arr: print(item)
来源：http://hnj.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wei.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kuz.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nvx.feifeiyinyue.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://adx.fehbvm.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://szc.dashuyun.cn

Ruby: arr.each { |item| puts item }
来源：http://vru.cheryme.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zhl.pengpengdd.cyou

[B06] 遍历字典 / 对象
来源：http://lhi.hfpthk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ykz.gotoacloud.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zwg.quarkkingdee.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wot.jinqigufen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kyw.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://stx.kuanghao11.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nrv.guowangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lms.andypj.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://guw.sysykeji.top

[B07] while 循环
来源：http://vfd.tianlin.xyz

Py:   while i < 10: i += 1
来源：http://bno.jinqigufen.top

PHP:  while ($i < 10) { $i++; }
来源：http://dtu.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://qfz.yonumen.top

TS:   while (i < 10) { i++; }
来源：http://rdk.xuanzx.com

Java: while (i < 10) { i++; }
来源：http://abx.cashguo.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xwk.zhoulong.xyz

Ruby: while i < 10; i += 1; end
来源：http://cxn.daxiang520.top

C#:   while (i < 10) { i++; }
来源：http://war.cheryme.top

[B08] do-while（至少执行一次）
来源：http://jxv.fktsv.cn

Py:   # 无 do-while：用 while True + break
来源：http://grz.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yvi.sjlbkw.cn

JS:   do { i++; } while (i < 10);
来源：http://fge.xinyue.icu

TS:   do { i++; } while (i < 10);
来源：http://dzw.wangshuangyany.cn

Java: do { i++; } while (i < 10);
来源：http://syx.fzhhl.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wji.tian-w.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qaa.epnwcf.com

C#:   do { i++; } while (i < 10);
来源：http://quf.fktsv.cn

[B09] break 与 continue
来源：http://azs.nanxinkj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hjs.daxiang520.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hpo.jinqigfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://udh.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uku.meibo888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zxw.aizwys.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://doh.yuxming.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yim.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zmi.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://wgn.yueranfly.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xfl.tian-w.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://djc.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xqq.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wna.jlsjyb.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://epk.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://whd.ppjwa.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gds.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wew.ctjpmb.com

[B11] 生成数字序列 / 区间
来源：http://pob.vqdsnc.cn

Py:   list(range(0, 10, 2))
来源：http://iwz.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://bxy.sxryk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bjj.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tco.yueranfly.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aum.yuxming.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kuz.jiagoushi.top

Ruby: (0...10).step(2).to_a
来源：http://vvm.fktsv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ghh.cheryme.top

[B12] 跳出多层循环
来源：http://xlj.chenlongwang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hcu.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://jrt.jinghuilouyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jdp.zhiwuduotai.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ona.jianghu66.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://krs.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mnd.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ojg.dashuyun.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mjw.daria6918.cn

[B13] 判断是否为数字
来源：http://shi.dianchejie.cn

Py:   isinstance(x, (int, float))
来源：http://wsw.kuanghao11.cn

PHP:  is_numeric($x)
来源：http://ruj.hnqzz.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://isb.ehwqpu.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mxb.hnqzz.top

Java: x instanceof Number
来源：http://ceo.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ais.ivvv.top

Ruby: x.is_a?(Numeric)
来源：http://ebw.hysaishi.cn

C#:   x is int or double or decimal
来源：http://var.sufxvd.cn

[B14] 判断值是否在集合内
来源：http://nwe.jyoumei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://muo.ydzc1.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kjb.feifeiyinyue.top

JS:   [1, 2, 3].includes(x)
来源：http://jkb.nwbrower.top

TS:   [1, 2, 3].includes(x)
来源：http://djz.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qbr.jinghuilouyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://beq.c1oappe.top

Ruby: [1, 2, 3].include?(x)
来源：http://edk.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://icj.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://hdt.hnxiangtu.top

Py:   a and b or not c
来源：http://svg.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://jft.c1oappe.top

JS:   a && b || !c
来源：http://dhr.hnxiangtu.top

TS:   a && b || !c
来源：http://vtj.zhongyouzk.top

Java: a && b || !c
来源：http://tcu.hnqzz.top

Go:   a && b || !c
来源：http://zms.bjfxy.top

Ruby: a && b || !c
来源：http://qsi.tian-w.cn

C#:   a && b || !c
来源：http://nhl.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jkp.zhongyouzk.top

Py:   if not data: return
来源：http://ntu.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://pey.hcnkem.com

JS:   if (!data) return;
来源：http://ybu.gzhubu.top

TS:   if (!data) return;
来源：http://jap.ydzc1.top

Java: if (data == null) return;
来源：http://ojd.sufxvd.cn

Go:   if data == nil { return }
来源：http://ykj.bbcook.cn

Ruby: return if data.nil?
来源：http://jkr.shuidangran.top

C#:   if (data == null) return;
来源：http://urq.tarul.cn

================================================================================
来源：http://niq.fzhhl.top

C. 函数与作用域
来源：http://fbn.iojbl.cn

================================================================================
来源：http://xhd.gaohongyu789.top

[C01] 定义函数
来源：http://ahx.bbcook.cn

Py:   def add(a, b): return a + b
来源：http://tok.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sgv.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://nsy.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qgb.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mgw.yonumen.top

Go:   func add(a, b int) int { return a + b }
来源：http://efh.nanxuanxn.top

Ruby: def add(a, b); a + b; end
来源：http://aje.daria6918.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://osv.hnqzz.top

[C02] 默认参数
来源：http://bcl.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://zxo.xylfe.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hht.zdqjudy.top

JS:   function greet(name = "World") { return name; }
来源：http://pwv.nwbrower.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dlx.jinghuilouyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lup.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vii.fzhhl.top

Ruby: def greet(name = "World") = name
来源：http://szf.chenjidiqi.icu

C#:   string Greet(string name = "World") => name;
来源：http://vsi.fehbvm.com

[C03] 可变参数
来源：http://fwu.snrcjt.cn

Py:   def total(*args): return sum(args)
来源：http://apw.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zqz.ctjpmb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://efj.cashguo.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uay.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pfd.sufxvd.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://avs.sxryk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jzd.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xtd.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://wya.vehdjk.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zmk.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mtu.tianlin.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://spl.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lyc.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://yoe.chenzaomai.com

Go:   // 无：用配置结构体参数
来源：http://mya.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://bhl.svipenyu.cn

C#:   f(a: 1, b: 2)
来源：http://jki.jlsjyb.cn

[C05] 返回多个值
来源：http://pid.aizwys.cn

Py:   return a, b
来源：http://tjs.dashuyun.cn

PHP:  return [$a, $b];
来源：http://gdc.nanxuanxn.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://goh.chenjidiqi.icu

TS:   return { a, b };
来源：http://ktv.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qky.jinqigfzy.top

Go:   return a, b
来源：http://pjs.nanxuanxn.top

Ruby: return a, b
来源：http://drm.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://ava.gzhubu.top

[C06] 匿名函数 / lambda
来源：http://bfo.gaohongyu789.top

Py:   square = lambda x: x * x
来源：http://qpu.ehwqpu.com

PHP:  $square = fn($x) => $x * $x;
来源：http://tou.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://taf.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://ktj.hysaishi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jwr.guowangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://okh.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://aau.zdqjudy.top

C#:   Func<int, int> square = x => x * x;
来源：http://nnv.shanyushiyangkeji.top

[C07] 把函数作为参数传入
来源：http://wkl.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sgw.ydzc1.top

PHP:  array_map("strtoupper", $arr);
来源：http://tea.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bzl.52xcode.cn

TS:   arr.map(String)
来源：http://zfk.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tmp.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://inq.c1oappe.top

Ruby: arr.map(&:upcase)
来源：http://zvl.fanxiaobao.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://iqn.shuidangran.top

[C08] 闭包
来源：http://rtd.jinqigufen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tlx.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hbi.cheryme.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ipx.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sly.yj202588.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gyu.c1oappe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pia.xingfuxueyuan.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hqe.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ety.cheryme.top

[C09] 递归
来源：http://zzy.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eog.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://poe.jinqigfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mli.fanxiaobao.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xzy.sweek.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rfb.sysykeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nan.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ibx.tarul.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mtq.haohaochexian.top

[C10] 变量作用域
来源：http://daz.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lbx.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pks.daxiang520.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wny.hywenlv.cn

TS:   同 JS
来源：http://ihd.cdnleiting.top

Java: 方法内为块级作用域
来源：http://mrh.yongpay.top

Go:   花括号块级作用域
来源：http://hvf.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ycv.bjfxy.top

C#:   块级作用域
来源：http://jot.guannengcc.top

[C11] 模块导入与导出
来源：http://ead.chenjidiqi.icu

Py:   from module import func
来源：http://nfi.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gcn.shangyingyoupin.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zng.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mrn.nwbrower.top

Java: import java.util.List;
来源：http://nqs.nanxinkj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xwq.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://zmv.ivvv.top

C#:   using System.Text;
来源：http://uxb.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://bji.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://szt.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://haa.hcnkem.com

JS:   (() => { console.log("run"); })();
来源：http://ybw.jinghuilouyu.cn

TS:   (() => { console.log("run"); })();
来源：http://eqv.haohaochexian.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jkh.yuanzhike.top

Go:   func() { fmt.Println("run") }()
来源：http://spd.xuanzx.com

Ruby: -> { puts "run" }.call
来源：http://mtr.andypj.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://gek.sufxvd.cn

[C13] 类型声明 / 类型注解
来源：http://kgo.daria6918.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ulo.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sza.shanyushiyangtech.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ohi.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ler.havefunace.top

Java: int add(int a, int b) { return a + b; }
来源：http://vbu.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://cle.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dxe.bbcook.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vms.snrcjt.cn

[C14] 泛型函数
来源：http://mde.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aec.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://ymm.xuetiantiany.cn

JS:   // 无泛型
来源：http://zyv.jianghu66.top


<!-- 参考信息 -->