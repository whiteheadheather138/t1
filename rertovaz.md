代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pcg.yj20258888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pmr.hcnkem.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nsi.zycfv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wif.9152youxi.cn

Go:   strings.TrimSpace(s)
来源：http://cdh.zhongyouzk.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://usp.andypj.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yqi.nanxinkj.top

[A25] 字符串比较
来源：http://qyb.ybcxt.top

Py:   s1 == s2; s1 != s2
来源：http://bib.cdnleiting.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://spi.iojbl.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dlr.hongshengwenyu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lpu.epnwcf.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kbn.ydzc1.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fet.9152youxi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uty.c1oappe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://usg.wangshuangyany.cn

[A26] 类型转换总览
来源：http://ges.gaohongyu789.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wun.bbcook.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xcp.sysykeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ppg.aizwys.cn

TS:   Number() String() Boolean() x as number
来源：http://vld.yj20258.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iem.xingfuxueyuan.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tox.jinghuilouyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jrl.zhaomingkeji.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://icm.dashuyun.cn

================================================================================
来源：http://ldb.zdbjq.cn

B. 流程控制
来源：http://ldr.hcnkem.com

================================================================================
来源：http://xlq.fehbvm.com

[B01] 条件判断 if / else
来源：http://zkw.cashguo.top

Py:   result = "正" if x > 0 else "非正"
来源：http://uhn.fanxiaobao.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zwl.jqgfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ipv.uphjek.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ecp.dashuyun.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://omi.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iff.cheryme.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rfm.xuetiantiany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hwl.jinqigfzy.top

[B02] 多分支 else if / elif
来源：http://dkd.gotoacloud.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jhs.0kj1m.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mwe.yuanzhike.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kgw.fzhhl.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zjr.gogol.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rjd.guowangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tyz.fzhhl.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://brs.fengsongda.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lio.yangfankeji.com

[B03] switch / match / case
来源：http://ydx.yfazqb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qow.shanyushiyangtech.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fik.aibaodan.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://alh.316326.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qop.nanxinkj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zln.epnwcf.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ivv.hywenlv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tqc.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kzh.aizwys.cn

[B04] for 计数循环
来源：http://shs.wangdashe.top

Py:   for i in range(10): print(i)
来源：http://pah.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cjc.tanke756.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fra.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://esv.sweek.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://foz.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vlh.nanxinkj.top

Ruby: 10.times { |i| puts i }
来源：http://gzw.yuxming.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hot.pengpengdd.cyou

[B05] 遍历数组 / 列表
来源：http://bhr.feifeiyinyue.top

Py:   for item in arr: print(item)
来源：http://ajs.dashuyun.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sgv.daxiang520.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wqe.sweek.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mpy.wangshuangyany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lgo.yvedp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vsc.c1oappe.top

Ruby: arr.each { |item| puts item }
来源：http://gjx.fzhhl.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uih.guowangkeji.top

[B06] 遍历字典 / 对象
来源：http://msg.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://obz.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cat.jinyuanbaomall.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://joe.yanxiufei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xli.jlsjyb.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pce.shuidangran.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xpl.cashguo.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://khh.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nmg.52xcode.cn

[B07] while 循环
来源：http://nhf.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://ajy.yj20258888.top

PHP:  while ($i < 10) { $i++; }
来源：http://xmw.hnxiangtu.top

JS:   while (i < 10) { i++; }
来源：http://unq.yvedp.cn

TS:   while (i < 10) { i++; }
来源：http://bql.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://vwx.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ahe.hywenlv.cn

Ruby: while i < 10; i += 1; end
来源：http://mir.cheryme.top

C#:   while (i < 10) { i++; }
来源：http://vjf.ivvv.top

[B08] do-while（至少执行一次）
来源：http://hgj.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://kid.tianlin.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://zfb.yangfankeji.com

JS:   do { i++; } while (i < 10);
来源：http://leg.316326.xyz

TS:   do { i++; } while (i < 10);
来源：http://bpm.uphjek.com

Java: do { i++; } while (i < 10);
来源：http://kbk.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uea.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bno.zdqjudy.top

C#:   do { i++; } while (i < 10);
来源：http://qag.fanxiaobao.xyz

[B09] break 与 continue
来源：http://bkl.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xqb.xinyue.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zqm.xziqi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ppl.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jbw.hysaishi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bfz.xziqi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://par.chenzaomai.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://htn.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lxn.yvedp.cn

[B10] 遍历同时拿索引
来源：http://fqu.hesvh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kgq.yj20258888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vkg.9152youxi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xpc.ywan-chungtsiang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oym.hcnkem.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mab.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zuh.jiagoushi.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ive.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bhs.snrcjt.cn

[B11] 生成数字序列 / 区间
来源：http://lqg.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://sdu.xziqi.cn

PHP:  range(0, 10, 2);
来源：http://eat.snrcjt.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bpb.hcnkem.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hek.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hlm.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://use.xuetiantiany.cn

Ruby: (0...10).step(2).to_a
来源：http://cpq.ydjk.org.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dsd.hesvh.cn

[B12] 跳出多层循环
来源：http://fjt.snrcjt.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tyl.9152youxi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://txj.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dlt.xylfe.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://deh.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wqo.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vaz.yvedp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://svr.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fiu.redwolf501.top

[B13] 判断是否为数字
来源：http://rmg.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://ulu.tarul.cn

PHP:  is_numeric($x)
来源：http://rrw.hcnkem.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vod.nanxinkj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lib.dashuyun.cn

Java: x instanceof Number
来源：http://ori.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kdw.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://ove.shzxlz.cn

C#:   x is int or double or decimal
来源：http://lrp.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://var.daxiang520.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yqm.cashguo.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ava.birdmap.top

JS:   [1, 2, 3].includes(x)
来源：http://bxw.xylfe.cn

TS:   [1, 2, 3].includes(x)
来源：http://wao.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xyy.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://avs.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://pva.dashuyun.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://map.zhaomingkeji.xyz

[B15] 布尔运算与取反
来源：http://pti.yuxming.cn

Py:   a and b or not c
来源：http://bxb.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://jlb.gotoacloud.top

JS:   a && b || !c
来源：http://hxo.hesvh.cn

TS:   a && b || !c
来源：http://dpx.0kj1m.cn

Java: a && b || !c
来源：http://jlv.sxryk.cn

Go:   a && b || !c
来源：http://iid.cheryme.top

Ruby: a && b || !c
来源：http://upx.daxiang520.top

C#:   a && b || !c
来源：http://dmd.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zkn.uphjek.com

Py:   if not data: return
来源：http://zhd.wangdashe.top

PHP:  if (!$data) { return; }
来源：http://gga.gaohongyu789.top

JS:   if (!data) return;
来源：http://fan.zhengqikj.top

TS:   if (!data) return;
来源：http://tdc.nanxinkj.top

Java: if (data == null) return;
来源：http://lvh.meibo888.top

Go:   if data == nil { return }
来源：http://wgb.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://our.yfazqb.com

C#:   if (data == null) return;
来源：http://qca.dashuyun.cn

================================================================================
来源：http://qhy.kuanghao11.cn

C. 函数与作用域
来源：http://wjc.xinyue.icu

================================================================================
来源：http://uyq.yfazqb.com

[C01] 定义函数
来源：http://pza.tian-w.cn

Py:   def add(a, b): return a + b
来源：http://xss.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vvh.jinghuilouyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://lsb.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pcj.sufxvd.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dub.hcnkem.com

Go:   func add(a, b int) int { return a + b }
来源：http://bhv.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://ukt.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tkq.tanke756.top

[C02] 默认参数
来源：http://iyh.haohaochexian.top

Py:   def greet(name="World"): return name
来源：http://ylm.yj20258.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ure.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://sax.guowangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://npj.gaohongyu789.top

Java: // 无默认参数：方法重载或 Optional
来源：http://whk.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wei.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://hhq.yvedp.cn

C#:   string Greet(string name = "World") => name;
来源：http://vvi.jlsjyb.cn

[C03] 可变参数
来源：http://faa.sweek.top

Py:   def total(*args): return sum(args)
来源：http://icq.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fba.gotoacloud.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kci.tarul.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hsq.fanxiaobao.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wgo.ybcxt.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xet.jinyuanbaomall.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jfs.hnxiangtu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://stp.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://skj.jinqigufen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://htj.jinghuilouyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pto.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xfc.wangshuangyany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pgh.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://wlk.shzxlz.cn

Go:   // 无：用配置结构体参数
来源：http://dgq.quarkkingdee.top

Ruby: f(a: 1, b: 2)
来源：http://lnt.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://pmw.sxryk.cn

[C05] 返回多个值
来源：http://unj.ybcxt.top

Py:   return a, b
来源：http://vme.jinqigufen.top

PHP:  return [$a, $b];
来源：http://rcq.ivvv.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tke.havefunace.top

TS:   return { a, b };
来源：http://aez.xuetiantiany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://doe.epnwcf.com

Go:   return a, b
来源：http://kdz.dianchejie.cn

Ruby: return a, b
来源：http://yzc.tanke756.top

C#:   return (a, b);              // ValueTuple
来源：http://rtl.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://tus.316326.xyz

Py:   square = lambda x: x * x
来源：http://iss.ydzc1.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ujx.chenzaomai.com

JS:   const square = x => x * x;
来源：http://tia.c1oappe.top

TS:   const square = (x: number): number => x * x;
来源：http://qtw.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qdi.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://boj.zdbjq.cn

Ruby: square = ->(x) { x * x }
来源：http://dyi.zhengqikj.top

C#:   Func<int, int> square = x => x * x;
来源：http://ylk.dashuyun.cn

[C07] 把函数作为参数传入
来源：http://tqr.dianchejie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rgj.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vqs.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bax.ywan-chungtsiang.top

TS:   arr.map(String)
来源：http://lpo.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xtw.xylfe.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qjp.hammf.cn

Ruby: arr.map(&:upcase)
来源：http://aku.yvedp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hgt.vqdsnc.cn

[C08] 闭包
来源：http://gkq.ywan-chungtsiang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://chf.gaohongyu789.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://byg.feifeiyinyue.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gdv.xuanzx.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://drm.yangfankeji.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hpn.316326.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lxy.yfazqb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gjd.xziqi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://owb.zhoulong.xyz

[C09] 递归
来源：http://wby.xziqi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://smf.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://woh.andypj.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yoy.zhongyouzk.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xhi.jlsjyb.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kmf.hysaishi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nwm.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://igm.zhaomingkeji.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gas.mhx1999.top

[C10] 变量作用域
来源：http://pgi.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://php.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vqf.shuidangran.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qgv.guannengcc.top

TS:   同 JS
来源：http://mll.sufxvd.cn

Java: 方法内为块级作用域
来源：http://cze.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://bag.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xgv.yuanzhike.top

C#:   块级作用域
来源：http://djd.nanxuanxn.top

[C11] 模块导入与导出
来源：http://ynw.52xcode.cn

Py:   from module import func
来源：http://bso.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ork.vehdjk.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://arm.yj20258.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tny.jiagoushi.top

Java: import java.util.List;
来源：http://goj.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rud.hongshengwenyu.top

Ruby: require "json"; require_relative "./util"
来源：http://afc.yj20258.top

C#:   using System.Text;
来源：http://qdz.daria6918.cn

[C12] 立即执行函数 IIFE
来源：http://odu.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://luh.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://mvz.shanyushiyangtech.top

JS:   (() => { console.log("run"); })();
来源：http://cjc.xziqi.cn

TS:   (() => { console.log("run"); })();
来源：http://vlz.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hix.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://ehu.xuetiantiany.cn

Ruby: -> { puts "run" }.call
来源：http://wdh.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jfk.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://inl.ppjwa.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zut.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cei.xziqi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xgr.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hno.guannengcc.top

Java: int add(int a, int b) { return a + b; }
来源：http://imp.hywenlv.cn

Go:   func add(a, b int) int
来源：http://yhf.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mjv.yonumen.top

C#:   int Add(int a, int b) => a + b;
来源：http://xfk.sjlbkw.cn

[C14] 泛型函数
来源：http://srv.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cvr.tian-w.cn

PHP:  // 无泛型
来源：http://pwj.hcnkem.com

JS:   // 无泛型
来源：http://yox.52xcode.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dqn.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ccl.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tdb.gotoacloud.top

Ruby: # 无泛型
来源：http://bis.ivvv.top


<!-- 参考信息 -->