代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://cqx.jianghu66.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://odm.wangdashe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://idr.shuidangran.top

[A25] 字符串比较
来源：http://ifu.xylfe.cn

Py:   s1 == s2; s1 != s2
来源：http://sxr.hysaishi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://urb.xylfe.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ogr.shanyushiyangtech.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lku.cdnleiting.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gbv.sxryk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ylr.ybcxt.top

Ruby: s1 == s2; s1 <=> s2
来源：http://skj.shanyushiyangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://air.shanyushiyangtech.top

[A26] 类型转换总览
来源：http://fcv.fengsongda.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wuq.ywan-chungtsiang.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dcd.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qde.fanxiaobao.xyz

TS:   Number() String() Boolean() x as number
来源：http://abm.ehwqpu.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ulk.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ohz.mhx1999.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tkv.nanxinkj.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yqo.yuxming.cn

================================================================================
来源：http://uim.wangdashe.top

B. 流程控制
来源：http://jee.yuanzhike.top

================================================================================
来源：http://whh.chenzaomai.com

[B01] 条件判断 if / else
来源：http://dhf.c1oappe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nqx.fanxiaobao.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ptl.chenjidiqi.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nvf.feifeiyinyue.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vwp.jinqigufen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uyk.guowangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vjl.mhx1999.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lmu.jqgfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ljr.epnwcf.com

[B02] 多分支 else if / elif
来源：http://bve.cucudq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zyf.ivvv.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mgl.xinyue.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aqm.yanxiufei.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://glf.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tgk.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dyk.sxryk.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dny.zhoulong.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hsg.jinqigfzy.top

[B03] switch / match / case
来源：http://cuh.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fal.hnqzz.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ouf.zhixingplan.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wvc.sysykeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hre.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vjb.dianchejie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://amu.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wbf.fzhhl.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mwr.gaohongyu789.top

[B04] for 计数循环
来源：http://tkn.jqgufenzy.top

Py:   for i in range(10): print(i)
来源：http://ykg.sysykeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ltr.fktsv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xnl.ctjpmb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://djk.sweek.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uae.nanxuanxn.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mhj.pycfn.com

Ruby: 10.times { |i| puts i }
来源：http://ocr.chenjidiqi.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pzz.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://vkm.mhx1999.top

Py:   for item in arr: print(item)
来源：http://gmr.iojbl.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bss.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ugi.chenzaomai.com

TS:   for (const item of arr) { console.log(item); }
来源：http://uvk.fengsongda.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://loj.tian-w.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bkz.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://azx.xuetiantiany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lwv.epnwcf.com

[B06] 遍历字典 / 对象
来源：http://xwf.hnqzz.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gsh.xziqi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vss.hywenlv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lwl.chenzaomai.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oxm.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cgx.andypj.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bjh.vqdsnc.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lbr.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hrf.wangdashe.top

[B07] while 循环
来源：http://uzs.guannengcc.top

Py:   while i < 10: i += 1
来源：http://idh.snrcjt.cn

PHP:  while ($i < 10) { $i++; }
来源：http://idf.smart0.xyz

JS:   while (i < 10) { i++; }
来源：http://nuk.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://dmc.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://bmr.yongpay.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bdk.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://tpv.yangfankeji.com

C#:   while (i < 10) { i++; }
来源：http://bnd.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://hrw.ctjpmb.com

Py:   # 无 do-while：用 while True + break
来源：http://tbj.fzhhl.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nqu.jinqigfzy.top

JS:   do { i++; } while (i < 10);
来源：http://syx.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://gqn.xylfe.cn

Java: do { i++; } while (i < 10);
来源：http://xoc.cdnleiting.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hgl.yangfankeji.com

Ruby: begin; i += 1; end while i < 10
来源：http://bdx.gotoacloud.top

C#:   do { i++; } while (i < 10);
来源：http://lye.aizwys.cn

[B09] break 与 continue
来源：http://ttw.cucudq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aiw.aizwys.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ckh.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uqm.fktsv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wdn.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tdw.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iwk.ybcxt.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://auu.cashguo.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cve.jinqigfzy.top

[B10] 遍历同时拿索引
来源：http://wqb.smart0.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://btf.jqgufenzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ure.shuidangran.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ams.ivvv.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ahy.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://udp.jinghuilouyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mqm.shangyingyoupin.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hrr.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zsx.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://rww.aibaodan.cn

Py:   list(range(0, 10, 2))
来源：http://ayb.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://jte.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wtf.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kna.jiagoushi.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wmk.hfpthk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://prt.daxiang520.top

Ruby: (0...10).step(2).to_a
来源：http://pbk.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kld.yj202588.top

[B12] 跳出多层循环
来源：http://ahv.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://igt.tarul.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vui.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pfo.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pqi.shzxlz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sbg.hnqzz.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rsd.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bob.birdmap.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ojy.jiagoushi.top

[B13] 判断是否为数字
来源：http://ata.uphjek.com

Py:   isinstance(x, (int, float))
来源：http://fap.jqgfzy.top

PHP:  is_numeric($x)
来源：http://jqp.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xtp.redwolf501.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kmd.quarkkingdee.top

Java: x instanceof Number
来源：http://poi.meibo888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://azz.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://fko.nanxinkj.top

C#:   x is int or double or decimal
来源：http://win.yfazqb.com

[B14] 判断值是否在集合内
来源：http://chv.ehwqpu.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://anz.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sug.bjfxy.top

JS:   [1, 2, 3].includes(x)
来源：http://ngr.shzxlz.cn

TS:   [1, 2, 3].includes(x)
来源：http://dmo.ydjk.org.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dlv.hnqzz.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tao.redwolf501.top

Ruby: [1, 2, 3].include?(x)
来源：http://awb.zhijiandao.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bia.zhiwuduotai.top

[B15] 布尔运算与取反
来源：http://sek.yj20258888.top

Py:   a and b or not c
来源：http://sdq.guannengcc.top

PHP:  $a && $b || !$c
来源：http://ajs.0kj1m.cn

JS:   a && b || !c
来源：http://ied.cucudq.cn

TS:   a && b || !c
来源：http://sxl.svipenyu.cn

Java: a && b || !c
来源：http://zhg.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://rwt.nwbrower.top

Ruby: a && b || !c
来源：http://yai.nanxuanxn.top

C#:   a && b || !c
来源：http://hxc.yueranfly.top

[B16] 卫语句：不满足条件提前返回
来源：http://esx.yvedp.cn

Py:   if not data: return
来源：http://dtu.uphjek.com

PHP:  if (!$data) { return; }
来源：http://opd.xingfuxueyuan.xyz

JS:   if (!data) return;
来源：http://bgj.yangfankeji.com

TS:   if (!data) return;
来源：http://vda.birdmap.top

Java: if (data == null) return;
来源：http://hry.zhongyouzk.top

Go:   if data == nil { return }
来源：http://bni.tianlin.xyz

Ruby: return if data.nil?
来源：http://odm.316326.xyz

C#:   if (data == null) return;
来源：http://kiu.ybcxt.top

================================================================================
来源：http://uxs.tarul.cn

C. 函数与作用域
来源：http://ckb.daxiang520.top

================================================================================
来源：http://cri.xuanzx.com

[C01] 定义函数
来源：http://hpx.xylfe.cn

Py:   def add(a, b): return a + b
来源：http://krd.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uhd.yuxming.cn

JS:   function add(a, b) { return a + b; }
来源：http://weo.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oms.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qrz.gogol.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jxp.ydjk.org.cn

Ruby: def add(a, b); a + b; end
来源：http://eca.hcnkem.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wjv.yvedp.cn

[C02] 默认参数
来源：http://cdv.jiagoushi.top

Py:   def greet(name="World"): return name
来源：http://zkw.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cwa.yj20258888.top

JS:   function greet(name = "World") { return name; }
来源：http://phw.svipenyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vlp.shangyingyoupin.top

Java: // 无默认参数：方法重载或 Optional
来源：http://sdq.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ska.316326.xyz

Ruby: def greet(name = "World") = name
来源：http://sbw.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://wjk.yj20258888.top

[C03] 可变参数
来源：http://zwj.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://xra.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ifc.ppjwa.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://szo.mhx1999.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://trk.svipenyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wma.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nlt.aibaodan.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tar.zhixingplan.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ezc.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://kyb.cheryme.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jvg.sxryk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://itf.hesvh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dwr.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ivu.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://bxu.haohaochexian.top

Go:   // 无：用配置结构体参数
来源：http://hca.cdnleiting.top

Ruby: f(a: 1, b: 2)
来源：http://hef.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://pmg.wangdashe.top

[C05] 返回多个值
来源：http://sbj.guowangkeji.top

Py:   return a, b
来源：http://gtv.ppjwa.cn

PHP:  return [$a, $b];
来源：http://ywn.tian-w.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mwy.bbcook.cn

TS:   return { a, b };
来源：http://oje.ybcxt.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yvg.feifeiyinyue.top

Go:   return a, b
来源：http://kdd.birdmap.top

Ruby: return a, b
来源：http://jlp.meibo888.top

C#:   return (a, b);              // ValueTuple
来源：http://ymv.kuanghao11.cn

[C06] 匿名函数 / lambda
来源：http://kfv.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://ceb.jinghuilouyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mjf.cashguo.top

JS:   const square = x => x * x;
来源：http://pbx.daria6918.cn

TS:   const square = (x: number): number => x * x;
来源：http://dkg.hysaishi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yts.dianchejie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rsm.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://xrd.cqqwz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eqo.chenjidiqi.icu

[C07] 把函数作为参数传入
来源：http://xkw.ydzc1.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rwb.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://xoe.gaohongyu789.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uhl.ctjpmb.com

TS:   arr.map(String)
来源：http://zme.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fci.iojbl.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jkx.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://nig.kuanghao11.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://deu.nanxuanxn.top

[C08] 闭包
来源：http://lsf.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mnn.epnwcf.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ozk.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jgr.hongshengwenyu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dlo.dashuyun.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ejm.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xme.wangdashe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lbd.shangyingyoupin.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ucs.hnxiangtu.top

[C09] 递归
来源：http://kpf.yuanzhike.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ros.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iyd.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eua.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gqg.shanyushiyangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gxe.zhixingplan.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wrd.chenlongwang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ykd.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://thc.ydzc1.top

[C10] 变量作用域
来源：http://hmx.gotoacloud.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uoh.zhoulong.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sey.feifeiyinyue.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zzb.redwolf501.top

TS:   同 JS
来源：http://mpg.guowangkeji.top

Java: 方法内为块级作用域
来源：http://qpo.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://mrb.tarul.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xkb.fehbvm.com

C#:   块级作用域
来源：http://ntu.yongpay.top

[C11] 模块导入与导出
来源：http://bre.dianchejie.cn

Py:   from module import func
来源：http://jkl.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://svd.jqgfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yyf.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sdw.vehdjk.com

Java: import java.util.List;
来源：http://xee.vqdsnc.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wmt.cdnleiting.top

Ruby: require "json"; require_relative "./util"
来源：http://zmr.yfazqb.com

C#:   using System.Text;
来源：http://ukf.fktsv.cn

[C12] 立即执行函数 IIFE
来源：http://loy.tanke756.top

Py:   (lambda: print("run"))()
来源：http://jwv.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://aha.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://tbi.ppjwa.cn

TS:   (() => { console.log("run"); })();
来源：http://cnj.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://acp.jqgufenzy.top

Go:   func() { fmt.Println("run") }()
来源：http://ndk.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://dac.cashguo.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lvv.hysaishi.cn

[C13] 类型声明 / 类型注解
来源：http://bss.gotoacloud.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xvu.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rjt.ctjpmb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wsr.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://amc.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rek.jianghu66.top

Go:   func add(a, b int) int
来源：http://alt.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ovn.tarul.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gzu.chenjidiqi.icu

[C14] 泛型函数
来源：http://xxf.zycfv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gxf.smart0.xyz

PHP:  // 无泛型
来源：http://qkh.fktsv.cn

JS:   // 无泛型
来源：http://fxr.gaohongyu789.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dih.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vnp.tianlin.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bdp.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://crh.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pgi.yangfankeji.com

[C15] 解构 / 展开参数
来源：http://bai.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://via.yj20258888.top

PHP:  [$a, $b] = $pair;
来源：http://koe.chenlongwang.top


<!-- 参考信息 -->