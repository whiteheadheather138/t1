代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pez.jinyuanbaomall.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mqx.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://low.gzhubu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wgs.fehbvm.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qkc.shuidangran.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hev.redwolf501.top

[A24] 去除首尾空白
来源：http://oex.cheryme.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lkn.quarkkingdee.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jds.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gnx.jinqigufen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tzn.hcnkem.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fhw.ehwqpu.com

Go:   strings.TrimSpace(s)
来源：http://lqd.cheryme.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xnu.hfpthk.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eed.xingfuxueyuan.xyz

[A25] 字符串比较
来源：http://qmr.tanke756.top

Py:   s1 == s2; s1 != s2
来源：http://nqk.andypj.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://edg.yj20258888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://grm.nanxinkj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://riu.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pky.zhiwuduotai.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mmj.fzhhl.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jnk.yvedp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xyo.smart0.xyz

[A26] 类型转换总览
来源：http://qiq.vqdsnc.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jea.xinyue.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://won.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nmu.birdmap.top

TS:   Number() String() Boolean() x as number
来源：http://thu.pengpengdd.cyou

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lwr.zhongyouzk.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dwn.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cpc.xuetiantiany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pqw.9152youxi.cn

================================================================================
来源：http://ycy.fktsv.cn

B. 流程控制
来源：http://eqk.sjlbkw.cn

================================================================================
来源：http://tfr.xinyue.icu

[B01] 条件判断 if / else
来源：http://wgt.xziqi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yoz.andypj.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ggd.yfazqb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gtm.daxiang520.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://efa.jqgfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ffd.gzhubu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iic.yongpay.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dgv.tanke756.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xzc.zhixingplan.top

[B02] 多分支 else if / elif
来源：http://bmf.tanke756.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://abt.fengsongda.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vwe.hcnkem.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pjr.zycfv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xxm.shanyushiyangtech.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fqk.bjfxy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pil.yueranfly.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tyh.shanyushiyangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pou.fengsongda.top

[B03] switch / match / case
来源：http://wrh.hcnkem.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wyk.zhixingplan.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://psu.zdqjudy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://psv.jinyuanbaomall.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dcj.jqgufenzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://swq.chenzaomai.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zqw.shanyushiyangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mhu.xuanzx.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mxi.yvedp.cn

[B04] for 计数循环
来源：http://slc.pengpengdd.cyou

Py:   for i in range(10): print(i)
来源：http://jkf.yvedp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wdl.shangyingyoupin.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pfe.wangdashe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aht.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uhs.snrcjt.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kfj.guowangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://iqv.ivvv.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zgt.ydzc1.top

[B05] 遍历数组 / 列表
来源：http://vsg.yvedp.cn

Py:   for item in arr: print(item)
来源：http://yil.yanxiufei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mkj.jiagoushi.top

JS:   for (const item of arr) { console.log(item); }
来源：http://pxi.aibaodan.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lcs.guannengcc.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fgu.yueranfly.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rjk.zdqjudy.top

Ruby: arr.each { |item| puts item }
来源：http://aja.sysykeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://azr.52xcode.cn

[B06] 遍历字典 / 对象
来源：http://fij.dianchejie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rjm.cashguo.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sup.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iwa.zhaomingkeji.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://egl.xinyue.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wxy.316326.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zgr.ctjpmb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cms.hfpthk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lfv.aizwys.cn

[B07] while 循环
来源：http://iti.chenjidiqi.icu

Py:   while i < 10: i += 1
来源：http://iuk.xylfe.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ape.aizwys.cn

JS:   while (i < 10) { i++; }
来源：http://pfl.iojbl.cn

TS:   while (i < 10) { i++; }
来源：http://kqq.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://tdz.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ass.snrcjt.cn

Ruby: while i < 10; i += 1; end
来源：http://xpb.gzhubu.top

C#:   while (i < 10) { i++; }
来源：http://efn.guowangkeji.top

[B08] do-while（至少执行一次）
来源：http://blj.tanke756.top

Py:   # 无 do-while：用 while True + break
来源：http://qwk.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ckl.zdqjudy.top

JS:   do { i++; } while (i < 10);
来源：http://zos.hesvh.cn

TS:   do { i++; } while (i < 10);
来源：http://kvb.haohaochexian.top

Java: do { i++; } while (i < 10);
来源：http://vhr.cucudq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://drk.feifeiyinyue.top

Ruby: begin; i += 1; end while i < 10
来源：http://esj.yanxiufei.cn

C#:   do { i++; } while (i < 10);
来源：http://ugq.feifeiyinyue.top

[B09] break 与 continue
来源：http://iwz.ppjwa.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zkk.yfazqb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wlh.guowangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cbh.zycfv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tlk.zhongyouzk.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ojg.zhijiandao.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gjz.uphjek.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ygm.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uvg.ppjwa.cn

[B10] 遍历同时拿索引
来源：http://pyt.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ebj.guowangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://myn.smart0.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hrq.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rcg.snrcjt.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lud.ivvv.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aqa.cashguo.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yrv.c1oappe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jbq.wangshuangyany.cn

[B11] 生成数字序列 / 区间
来源：http://ume.zdbjq.cn

Py:   list(range(0, 10, 2))
来源：http://upp.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://lqv.zdqjudy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pdc.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gdw.aizwys.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xbn.haohaochexian.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wwv.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://xwd.ybcxt.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lwx.yongpay.top

[B12] 跳出多层循环
来源：http://pls.sxryk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ezg.zhixingplan.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://abd.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qgp.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vat.yj20258.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mlc.fzhhl.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zih.52xcode.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://krx.ctjpmb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lnv.yonumen.top

[B13] 判断是否为数字
来源：http://ajk.guannengcc.top

Py:   isinstance(x, (int, float))
来源：http://xnt.zhoulong.xyz

PHP:  is_numeric($x)
来源：http://niz.yj20258.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wrp.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gvb.xinyue.icu

Java: x instanceof Number
来源：http://zgo.0kj1m.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bwj.fzhhl.top

Ruby: x.is_a?(Numeric)
来源：http://uhj.guowangkeji.top

C#:   x is int or double or decimal
来源：http://xvj.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://jtr.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hdw.yangfankeji.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xre.ydzc1.top

JS:   [1, 2, 3].includes(x)
来源：http://yhn.cqqwz.cn

TS:   [1, 2, 3].includes(x)
来源：http://mpv.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cbg.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pbj.wangshuangyany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zlb.havefunace.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://suu.0kj1m.cn

[B15] 布尔运算与取反
来源：http://hpy.kuanghao11.cn

Py:   a and b or not c
来源：http://kww.zdqjudy.top

PHP:  $a && $b || !$c
来源：http://ahu.mhx1999.top

JS:   a && b || !c
来源：http://ezz.aibaodan.cn

TS:   a && b || !c
来源：http://mhz.yvedp.cn

Java: a && b || !c
来源：http://knt.gotoacloud.top

Go:   a && b || !c
来源：http://yps.jinqigfzy.top

Ruby: a && b || !c
来源：http://pkd.svipenyu.cn

C#:   a && b || !c
来源：http://hus.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://btx.tianlin.xyz

Py:   if not data: return
来源：http://nwy.feifeiyinyue.top

PHP:  if (!$data) { return; }
来源：http://nun.havefunace.top

JS:   if (!data) return;
来源：http://ney.shanyushiyangkeji.top

TS:   if (!data) return;
来源：http://igu.jinqigfzy.top

Java: if (data == null) return;
来源：http://qzv.chenlongwang.top

Go:   if data == nil { return }
来源：http://vxb.fengsongda.top

Ruby: return if data.nil?
来源：http://akg.birdmap.top

C#:   if (data == null) return;
来源：http://guk.pycfn.com

================================================================================
来源：http://wcz.havefunace.top

C. 函数与作用域
来源：http://ccr.tian-w.cn

================================================================================
来源：http://opo.zhijiandao.cn

[C01] 定义函数
来源：http://eqo.ydjk.org.cn

Py:   def add(a, b): return a + b
来源：http://dib.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fnp.9152youxi.cn

JS:   function add(a, b) { return a + b; }
来源：http://faq.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jvt.chenjidiqi.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://ira.bjfxy.top

Go:   func add(a, b int) int { return a + b }
来源：http://tff.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://gen.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ggc.zycfv.cn

[C02] 默认参数
来源：http://wow.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://qyv.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://abn.52xcode.cn

JS:   function greet(name = "World") { return name; }
来源：http://tmh.ybcxt.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nzg.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://myq.cucudq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cui.52xcode.cn

Ruby: def greet(name = "World") = name
来源：http://ktq.cheryme.top

C#:   string Greet(string name = "World") => name;
来源：http://ycl.jqgufenzy.top

[C03] 可变参数
来源：http://ouk.dianchejie.cn

Py:   def total(*args): return sum(args)
来源：http://hmw.hongshengwenyu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hdy.yanxiufei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wln.ppjwa.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ykk.xuetiantiany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://twr.mhx1999.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hev.hongshengwenyu.top

Ruby: def total(*nums); nums.sum; end
来源：http://hse.guannengcc.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nvt.tarul.cn

[C04] 命名参数 / 关键字参数
来源：http://mof.hongshengwenyu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zlu.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zem.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://umh.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fze.yj202588.top

Java: // 无：用 Builder 模式或 record
来源：http://uzn.nanxinkj.top

Go:   // 无：用配置结构体参数
来源：http://ceq.chenjidiqi.icu

Ruby: f(a: 1, b: 2)
来源：http://arf.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://pnh.jinghuilouyu.cn

[C05] 返回多个值
来源：http://psn.sufxvd.cn

Py:   return a, b
来源：http://bai.birdmap.top

PHP:  return [$a, $b];
来源：http://fzi.haohaochexian.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rdm.dashuyun.cn

TS:   return { a, b };
来源：http://nsh.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oqw.jqgfzy.top

Go:   return a, b
来源：http://dwu.zhaomingkeji.xyz

Ruby: return a, b
来源：http://rdq.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://hwo.fktsv.cn

[C06] 匿名函数 / lambda
来源：http://ufg.iojbl.cn

Py:   square = lambda x: x * x
来源：http://knb.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cgk.hnqzz.top

JS:   const square = x => x * x;
来源：http://qmx.andypj.xyz

TS:   const square = (x: number): number => x * x;
来源：http://oox.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sjb.guowangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://pck.zycfv.cn

Ruby: square = ->(x) { x * x }
来源：http://not.yj20258888.top

C#:   Func<int, int> square = x => x * x;
来源：http://uur.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://eoa.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bzw.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://yfp.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://geb.jqgfzy.top

TS:   arr.map(String)
来源：http://xom.cucudq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yub.xuanzx.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://czi.jqgfzy.top

Ruby: arr.map(&:upcase)
来源：http://egs.yfazqb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://ywz.fehbvm.com

[C08] 闭包
来源：http://gbr.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://msu.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oxh.xziqi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tdo.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lgo.xuanzx.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sqb.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ksx.zycfv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://llc.ppjwa.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tlv.shanyushiyangtech.top

[C09] 递归
来源：http://tsc.haohaochexian.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wlp.yongpay.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ito.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lwu.gaohongyu789.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wej.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fsh.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mmp.hammf.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xrs.zdbjq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ret.snrcjt.cn

[C10] 变量作用域
来源：http://eqq.guannengcc.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zjb.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hus.yuanzhike.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mde.redwolf501.top

TS:   同 JS
来源：http://pwe.zdbjq.cn

Java: 方法内为块级作用域
来源：http://mfh.ehwqpu.com

Go:   花括号块级作用域
来源：http://hqm.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jgx.xziqi.cn

C#:   块级作用域
来源：http://pbb.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://flb.jinqigufen.top

Py:   from module import func
来源：http://mmy.xziqi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ksr.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://iuq.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gtj.tanke756.top

Java: import java.util.List;
来源：http://hql.yueranfly.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mfx.yueranfly.top

Ruby: require "json"; require_relative "./util"
来源：http://lqw.cqqwz.cn

C#:   using System.Text;
来源：http://stq.ywan-chungtsiang.top

[C12] 立即执行函数 IIFE
来源：http://ffy.xingfuxueyuan.xyz

Py:   (lambda: print("run"))()
来源：http://uuc.ydzc1.top

PHP:  (function () { echo "run"; })();
来源：http://mil.redwolf501.top

JS:   (() => { console.log("run"); })();
来源：http://cmi.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://ycv.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qod.epnwcf.com

Go:   func() { fmt.Println("run") }()
来源：http://bcz.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://cfz.jlsjyb.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hmm.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://jbd.hywenlv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://smn.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jda.vqdsnc.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ajf.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hqf.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jbo.c1oappe.top

Go:   func add(a, b int) int
来源：http://tkf.yj20258.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tyo.9152youxi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nes.birdmap.top


<!-- 参考信息 -->