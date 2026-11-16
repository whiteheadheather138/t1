代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nnf.havefunace.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://csx.dianchejie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dib.havefunace.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kfh.kuanghao11.cn

Go:   strings.TrimSpace(s)
来源：http://fui.tarul.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gzj.sysykeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fis.hfpthk.cn

[A25] 字符串比较
来源：http://gpp.dianchejie.cn

Py:   s1 == s2; s1 != s2
来源：http://uey.redwolf501.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://imc.yfazqb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://psr.jiagoushi.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dcc.yuanzhike.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dvx.iojbl.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mjg.hysaishi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hav.fanxiaobao.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://byi.xuetiantiany.cn

[A26] 类型转换总览
来源：http://ryj.haohaochexian.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dnu.hammf.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pbx.ctjpmb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://amt.fktsv.cn

TS:   Number() String() Boolean() x as number
来源：http://rhf.hfpthk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xzm.jinqigfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pko.gogol.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://clj.cheryme.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://csg.pycfn.com

================================================================================
来源：http://tnx.xziqi.cn

B. 流程控制
来源：http://nbv.redwolf501.top

================================================================================
来源：http://eqd.zhixingplan.top

[B01] 条件判断 if / else
来源：http://syc.andypj.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://udh.snrcjt.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wey.yongpay.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vag.cheryme.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vak.pengpengdd.cyou

Java: String r = x > 0 ? "正" : "非正";
来源：http://nww.bjfxy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ldw.daxiang520.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cod.cdnleiting.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uvm.cashguo.top

[B02] 多分支 else if / elif
来源：http://fgj.zhijiandao.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://scg.yj202588.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vly.jianghu66.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://des.jyoumei.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tqd.feifeiyinyue.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uof.sufxvd.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bgg.iojbl.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ram.zhoulong.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mge.xylfe.cn

[B03] switch / match / case
来源：http://stx.fktsv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qfo.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hxv.nanxuanxn.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ufs.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zsn.fktsv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kos.sysykeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lqn.iojbl.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cho.pengpengdd.cyou

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xya.jianghu66.top

[B04] for 计数循环
来源：http://jyi.xylfe.cn

Py:   for i in range(10): print(i)
来源：http://xyu.sxryk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ylu.cqqwz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bpk.yuanzhike.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lfm.cashguo.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ehp.yongpay.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nap.jinyuanbaomall.cn

Ruby: 10.times { |i| puts i }
来源：http://pem.nwbrower.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://olv.tian-w.cn

[B05] 遍历数组 / 列表
来源：http://bvz.zhiwuduotai.top

Py:   for item in arr: print(item)
来源：http://byp.yuxming.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ugz.daxiang520.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dup.c1oappe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hfb.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pps.hnqzz.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sdh.haohaochexian.top

Ruby: arr.each { |item| puts item }
来源：http://dcx.xuetiantiany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ydk.c1oappe.top

[B06] 遍历字典 / 对象
来源：http://ccm.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sie.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://elo.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hbq.hesvh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wke.jinqigfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aoz.havefunace.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dwb.cucudq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dox.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cck.zhijiandao.cn

[B07] while 循环
来源：http://gnm.uphjek.com

Py:   while i < 10: i += 1
来源：http://goi.316326.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://auj.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://whl.sweek.top

TS:   while (i < 10) { i++; }
来源：http://bkq.hnxiangtu.top

Java: while (i < 10) { i++; }
来源：http://ziy.yuanzhike.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yni.jqgfzy.top

Ruby: while i < 10; i += 1; end
来源：http://phw.nwbrower.top

C#:   while (i < 10) { i++; }
来源：http://ytm.ctjpmb.com

[B08] do-while（至少执行一次）
来源：http://wwy.nwbrower.top

Py:   # 无 do-while：用 while True + break
来源：http://ubo.tian-w.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bxx.epnwcf.com

JS:   do { i++; } while (i < 10);
来源：http://str.yuanzhike.top

TS:   do { i++; } while (i < 10);
来源：http://wxv.havefunace.top

Java: do { i++; } while (i < 10);
来源：http://ucj.tian-w.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mwn.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://vcv.jlsjyb.cn

C#:   do { i++; } while (i < 10);
来源：http://fao.snrcjt.cn

[B09] break 与 continue
来源：http://oyl.yfazqb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ikh.tanke756.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vvw.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://npg.zhijiandao.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xqj.chenzaomai.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vtf.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dpl.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yqc.sxryk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yfo.redwolf501.top

[B10] 遍历同时拿索引
来源：http://llu.sufxvd.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://azv.zhengqikj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rmd.cucudq.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ybv.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jex.guowangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pzc.cdnleiting.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://atl.gotoacloud.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tzp.ppjwa.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lcm.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://ule.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://gum.zhongyouzk.top

PHP:  range(0, 10, 2);
来源：http://sqo.dianchejie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hiv.sweek.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kio.jianghu66.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hyj.hnxiangtu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dsa.shuidangran.top

Ruby: (0...10).step(2).to_a
来源：http://lno.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xhe.yangfankeji.com

[B12] 跳出多层循环
来源：http://zny.havefunace.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xcd.9152youxi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://obi.havefunace.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://znx.cucudq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xns.birdmap.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lki.guannengcc.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gos.shanyushiyangtech.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bok.ehwqpu.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jhr.sysykeji.top

[B13] 判断是否为数字
来源：http://ewr.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://knn.pycfn.com

PHP:  is_numeric($x)
来源：http://qqh.tian-w.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tbs.cucudq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cdu.guannengcc.top

Java: x instanceof Number
来源：http://geb.hcnkem.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nhe.feifeiyinyue.top

Ruby: x.is_a?(Numeric)
来源：http://ipv.zhengqikj.top

C#:   x is int or double or decimal
来源：http://egq.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://epp.hesvh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gwa.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mtp.zhixingplan.top

JS:   [1, 2, 3].includes(x)
来源：http://icq.dianchejie.cn

TS:   [1, 2, 3].includes(x)
来源：http://nit.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vga.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ikj.52xcode.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zkb.fzhhl.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jdu.zhoulong.xyz

[B15] 布尔运算与取反
来源：http://zcr.hnqzz.top

Py:   a and b or not c
来源：http://krq.9152youxi.cn

PHP:  $a && $b || !$c
来源：http://tge.xuetiantiany.cn

JS:   a && b || !c
来源：http://ufj.zhengqikj.top

TS:   a && b || !c
来源：http://jts.shanyushiyangkeji.top

Java: a && b || !c
来源：http://ksx.fehbvm.com

Go:   a && b || !c
来源：http://vmg.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://qfb.tanke756.top

C#:   a && b || !c
来源：http://qbg.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vjx.jlsjyb.cn

Py:   if not data: return
来源：http://rel.shzxlz.cn

PHP:  if (!$data) { return; }
来源：http://btj.cashguo.top

JS:   if (!data) return;
来源：http://rsm.jinqigufen.top

TS:   if (!data) return;
来源：http://att.fktsv.cn

Java: if (data == null) return;
来源：http://kmn.andypj.xyz

Go:   if data == nil { return }
来源：http://kyf.yj202588.top

Ruby: return if data.nil?
来源：http://vvw.snrcjt.cn

C#:   if (data == null) return;
来源：http://kiz.guannengcc.top

================================================================================
来源：http://osw.jinqigfzy.top

C. 函数与作用域
来源：http://ksb.cashguo.top

================================================================================
来源：http://boq.wangshuangyany.cn

[C01] 定义函数
来源：http://zzn.smart0.xyz

Py:   def add(a, b): return a + b
来源：http://avg.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dkd.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://dcr.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yhc.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wwx.mhx1999.top

Go:   func add(a, b int) int { return a + b }
来源：http://erw.cdnleiting.top

Ruby: def add(a, b); a + b; end
来源：http://yys.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mzl.pengpengdd.cyou

[C02] 默认参数
来源：http://pnj.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://ndu.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jbs.sysykeji.top

JS:   function greet(name = "World") { return name; }
来源：http://acg.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qqr.sufxvd.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://phv.fanxiaobao.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fqe.jiagoushi.top

Ruby: def greet(name = "World") = name
来源：http://uvt.shanyushiyangtech.top

C#:   string Greet(string name = "World") => name;
来源：http://hnl.zdqjudy.top

[C03] 可变参数
来源：http://qja.fanxiaobao.xyz

Py:   def total(*args): return sum(args)
来源：http://wuv.ctjpmb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uqu.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lev.hcnkem.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mkh.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ijp.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mkd.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://gxz.quarkkingdee.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pwz.jinqigufen.top

[C04] 命名参数 / 关键字参数
来源：http://ebx.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gqx.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hme.yonumen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mlt.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ixv.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://oly.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://hmd.wangdashe.top

Ruby: f(a: 1, b: 2)
来源：http://zfz.zycfv.cn

C#:   f(a: 1, b: 2)
来源：http://tfu.quarkkingdee.top

[C05] 返回多个值
来源：http://bza.zhongyouzk.top

Py:   return a, b
来源：http://pch.nwbrower.top

PHP:  return [$a, $b];
来源：http://zit.fanxiaobao.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://tgq.xuetiantiany.cn

TS:   return { a, b };
来源：http://tpk.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vuj.iojbl.cn

Go:   return a, b
来源：http://wvw.smart0.xyz

Ruby: return a, b
来源：http://pid.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://qtz.yj20258.top

[C06] 匿名函数 / lambda
来源：http://agj.andypj.xyz

Py:   square = lambda x: x * x
来源：http://cab.yj20258888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xdd.yfazqb.com

JS:   const square = x => x * x;
来源：http://nqp.yj20258888.top

TS:   const square = (x: number): number => x * x;
来源：http://ltj.guowangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kvw.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://vgw.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://pvs.guowangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://dsf.jinqigfzy.top

[C07] 把函数作为参数传入
来源：http://acc.ydzc1.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lfv.yanxiufei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://iuy.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iub.zhongyouzk.top

TS:   arr.map(String)
来源：http://eak.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cxp.wangshuangyany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://syf.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://kwf.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cuk.xziqi.cn

[C08] 闭包
来源：http://znu.zdqjudy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://adb.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://asw.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vfz.shanyushiyangtech.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wrh.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kfe.kuanghao11.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://amj.cheryme.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zxq.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pfq.zhaomingkeji.xyz

[C09] 递归
来源：http://nuv.kuanghao11.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hye.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mjp.hywenlv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fda.sysykeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kow.sxryk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wbp.ybcxt.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bzo.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rnv.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://btr.dashuyun.cn

[C10] 变量作用域
来源：http://iqv.aizwys.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://grq.epnwcf.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ntu.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xuq.pycfn.com

TS:   同 JS
来源：http://eny.havefunace.top

Java: 方法内为块级作用域
来源：http://dma.9152youxi.cn

Go:   花括号块级作用域
来源：http://xcb.shzxlz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yuu.xuetiantiany.cn

C#:   块级作用域
来源：http://qof.yangfankeji.com

[C11] 模块导入与导出
来源：http://zvq.sufxvd.cn

Py:   from module import func
来源：http://nry.epnwcf.com

PHP:  require "file.php";  或 use App\Service;
来源：http://agp.dashuyun.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pyx.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dpn.chenlongwang.top

Java: import java.util.List;
来源：http://iez.havefunace.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://psj.fktsv.cn

Ruby: require "json"; require_relative "./util"
来源：http://djy.c1oappe.top

C#:   using System.Text;
来源：http://bmc.tianlin.xyz

[C12] 立即执行函数 IIFE
来源：http://lwl.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://jdy.pengpengdd.cyou

PHP:  (function () { echo "run"; })();
来源：http://hia.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://bwb.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://rjq.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hws.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://wnn.jinyuanbaomall.cn

Ruby: -> { puts "run" }.call
来源：http://uxt.nwbrower.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rgr.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://npo.jinyuanbaomall.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zts.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tuf.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tww.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ecy.cqqwz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rqi.fzhhl.top

Go:   func add(a, b int) int
来源：http://sag.guowangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kqn.ehwqpu.com

C#:   int Add(int a, int b) => a + b;
来源：http://jaw.c1oappe.top

[C14] 泛型函数
来源：http://ewr.cdnleiting.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hds.wangdashe.top

PHP:  // 无泛型
来源：http://tzz.daxiang520.top

JS:   // 无泛型
来源：http://pna.c1oappe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cow.ehwqpu.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lax.yonumen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vwx.chenlongwang.top

Ruby: # 无泛型
来源：http://hcy.vehdjk.com


<!-- 参考信息 -->