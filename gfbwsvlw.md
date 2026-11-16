代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://ckz.hnqzz.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dqs.zhengqikj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://owz.birdmap.top

[A25] 字符串比较
来源：http://bgi.yueranfly.top

Py:   s1 == s2; s1 != s2
来源：http://vcq.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lzm.zhongyouzk.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xcn.hnxiangtu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dik.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vfe.xinyue.icu

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fjk.zhiwuduotai.top

Ruby: s1 == s2; s1 <=> s2
来源：http://fkq.meibo888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mqg.shangyingyoupin.top

[A26] 类型转换总览
来源：http://svl.hywenlv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://idv.andypj.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://obc.sjlbkw.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://goz.ivvv.top

TS:   Number() String() Boolean() x as number
来源：http://fjn.dashuyun.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://avs.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tep.hammf.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ixa.daxiang520.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://azl.feifeiyinyue.top

================================================================================
来源：http://bjt.xuetiantiany.cn

B. 流程控制
来源：http://egc.jqgfzy.top

================================================================================
来源：http://psy.hywenlv.cn

[B01] 条件判断 if / else
来源：http://ffz.yueranfly.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ltv.andypj.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tna.ydjk.org.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sti.guannengcc.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mjf.shangyingyoupin.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://bhq.tarul.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uox.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qxr.0kj1m.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dwh.meibo888.top

[B02] 多分支 else if / elif
来源：http://liu.52xcode.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fxm.jiagoushi.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hzy.kuanghao11.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ond.yj20258.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dro.mhx1999.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dwm.9152youxi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://esa.cashguo.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ejj.yongpay.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ipy.cucudq.cn

[B03] switch / match / case
来源：http://pey.ppjwa.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rtk.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hpa.kuanghao11.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jff.pycfn.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://imj.guowangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://brf.hammf.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fod.bjfxy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kpv.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wsn.fehbvm.com

[B04] for 计数循环
来源：http://oeh.yuxming.cn

Py:   for i in range(10): print(i)
来源：http://cet.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oqr.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mqa.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pix.shzxlz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zon.andypj.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xcd.fehbvm.com

Ruby: 10.times { |i| puts i }
来源：http://lwm.yuanzhike.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fdx.cashguo.top

[B05] 遍历数组 / 列表
来源：http://wgh.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://fdb.aibaodan.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gxh.shzxlz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wxm.havefunace.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qij.xziqi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://shq.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eyw.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://ems.jlsjyb.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hsm.wangshuangyany.cn

[B06] 遍历字典 / 对象
来源：http://mzt.yj20258.top

Py:   for k, v in d.items(): print(k, v)
来源：http://noi.jinghuilouyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gag.shzxlz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://euq.zdqjudy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mrz.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ncu.wangdashe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fyo.dianchejie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iok.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xzu.snrcjt.cn

[B07] while 循环
来源：http://nqc.meibo888.top

Py:   while i < 10: i += 1
来源：http://qpa.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yrq.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://zwv.nwbrower.top

TS:   while (i < 10) { i++; }
来源：http://ywe.yangfankeji.com

Java: while (i < 10) { i++; }
来源：http://ped.hcnkem.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lsq.yanxiufei.cn

Ruby: while i < 10; i += 1; end
来源：http://hok.tanke756.top

C#:   while (i < 10) { i++; }
来源：http://hhn.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://fui.fengsongda.top

Py:   # 无 do-while：用 while True + break
来源：http://xbg.xuetiantiany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ayv.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://tdd.yj20258888.top

TS:   do { i++; } while (i < 10);
来源：http://deg.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://qju.cdnleiting.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dww.jinqigufen.top

Ruby: begin; i += 1; end while i < 10
来源：http://mxm.jlsjyb.cn

C#:   do { i++; } while (i < 10);
来源：http://jum.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://fvw.jqgufenzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pcg.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kel.zdqjudy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jfd.bbcook.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ghi.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zbs.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tap.pengpengdd.cyou

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pca.fzhhl.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hkz.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://dks.yuanzhike.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hts.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ptx.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xix.uphjek.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dmh.birdmap.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dkm.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rpj.hywenlv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jqg.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bir.zhengqikj.top

[B11] 生成数字序列 / 区间
来源：http://ecl.aibaodan.cn

Py:   list(range(0, 10, 2))
来源：http://abv.haohaochexian.top

PHP:  range(0, 10, 2);
来源：http://mbs.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hmd.52xcode.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ctk.jinqigfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pya.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://krk.andypj.xyz

Ruby: (0...10).step(2).to_a
来源：http://vwf.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://saz.gaohongyu789.top

[B12] 跳出多层循环
来源：http://hnj.yvedp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hfj.hammf.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://igx.xuanzx.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tsx.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cqm.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wdi.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://acf.hnxiangtu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lnx.zdqjudy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ntm.hnxiangtu.top

[B13] 判断是否为数字
来源：http://ovq.c1oappe.top

Py:   isinstance(x, (int, float))
来源：http://nen.nanxuanxn.top

PHP:  is_numeric($x)
来源：http://wlu.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dkw.316326.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dos.epnwcf.com

Java: x instanceof Number
来源：http://nvn.yuanzhike.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ano.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://yza.yfazqb.com

C#:   x is int or double or decimal
来源：http://pea.hesvh.cn

[B14] 判断值是否在集合内
来源：http://mtw.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hfs.ybcxt.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tqu.cucudq.cn

JS:   [1, 2, 3].includes(x)
来源：http://pkl.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://xqo.9152youxi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pah.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://owp.fehbvm.com

Ruby: [1, 2, 3].include?(x)
来源：http://gnr.smart0.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hpr.zhoulong.xyz

[B15] 布尔运算与取反
来源：http://sut.iojbl.cn

Py:   a and b or not c
来源：http://yqh.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://gbe.guannengcc.top

JS:   a && b || !c
来源：http://ncp.yangfankeji.com

TS:   a && b || !c
来源：http://daf.yanxiufei.cn

Java: a && b || !c
来源：http://rny.wangshuangyany.cn

Go:   a && b || !c
来源：http://ttg.chenzaomai.com

Ruby: a && b || !c
来源：http://alk.sweek.top

C#:   a && b || !c
来源：http://wdh.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lpp.nwbrower.top

Py:   if not data: return
来源：http://nfh.redwolf501.top

PHP:  if (!$data) { return; }
来源：http://rab.zhixingplan.top

JS:   if (!data) return;
来源：http://pjo.52xcode.cn

TS:   if (!data) return;
来源：http://lgt.jiagoushi.top

Java: if (data == null) return;
来源：http://kej.gotoacloud.top

Go:   if data == nil { return }
来源：http://tyc.aizwys.cn

Ruby: return if data.nil?
来源：http://ish.wangshuangyany.cn

C#:   if (data == null) return;
来源：http://gby.0kj1m.cn

================================================================================
来源：http://exo.shzxlz.cn

C. 函数与作用域
来源：http://ygn.yj202588.top

================================================================================
来源：http://dfh.yuanzhike.top

[C01] 定义函数
来源：http://ava.ivvv.top

Py:   def add(a, b): return a + b
来源：http://okp.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fne.xuanzx.com

JS:   function add(a, b) { return a + b; }
来源：http://nko.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://inc.xingfuxueyuan.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://ygt.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nsx.jinyuanbaomall.cn

Ruby: def add(a, b); a + b; end
来源：http://kcf.fktsv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bwn.iojbl.cn

[C02] 默认参数
来源：http://uvx.hnxiangtu.top

Py:   def greet(name="World"): return name
来源：http://xep.jinqigufen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wfz.wangdashe.top

JS:   function greet(name = "World") { return name; }
来源：http://ykt.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hcm.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://arj.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yzg.gzhubu.top

Ruby: def greet(name = "World") = name
来源：http://jsg.jyoumei.cn

C#:   string Greet(string name = "World") => name;
来源：http://uqu.hammf.cn

[C03] 可变参数
来源：http://xbj.svipenyu.cn

Py:   def total(*args): return sum(args)
来源：http://mnt.kuanghao11.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nva.xziqi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bfe.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ich.nwbrower.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xya.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mlr.hfpthk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fmx.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://evs.zhoulong.xyz

[C04] 命名参数 / 关键字参数
来源：http://lfm.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lmv.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fxm.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ygl.jqgufenzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lov.mhx1999.top

Java: // 无：用 Builder 模式或 record
来源：http://occ.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://fdm.jlsjyb.cn

Ruby: f(a: 1, b: 2)
来源：http://xmk.jiagoushi.top

C#:   f(a: 1, b: 2)
来源：http://qdp.fengsongda.top

[C05] 返回多个值
来源：http://hzl.ppjwa.cn

Py:   return a, b
来源：http://mdy.xinyue.icu

PHP:  return [$a, $b];
来源：http://owh.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://pbj.gogol.net.cn

TS:   return { a, b };
来源：http://kxx.hnqzz.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tzm.quarkkingdee.top

Go:   return a, b
来源：http://dmu.jianghu66.top

Ruby: return a, b
来源：http://zlm.chenlongwang.top

C#:   return (a, b);              // ValueTuple
来源：http://att.xuetiantiany.cn

[C06] 匿名函数 / lambda
来源：http://brf.xuetiantiany.cn

Py:   square = lambda x: x * x
来源：http://boo.shuidangran.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nmf.ppjwa.cn

JS:   const square = x => x * x;
来源：http://hfa.cqqwz.cn

TS:   const square = (x: number): number => x * x;
来源：http://eih.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fui.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://kax.andypj.xyz

Ruby: square = ->(x) { x * x }
来源：http://kwk.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hqq.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://etz.sweek.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://big.jqgufenzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://iyn.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aud.xziqi.cn

TS:   arr.map(String)
来源：http://rso.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pnz.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wey.jqgufenzy.top

Ruby: arr.map(&:upcase)
来源：http://ngu.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://sed.hcnkem.com

[C08] 闭包
来源：http://xoq.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wle.pengpengdd.cyou

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wyu.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kac.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cin.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vyf.aizwys.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kfp.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mue.shzxlz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lps.mhx1999.top

[C09] 递归
来源：http://opv.zdqjudy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://acs.jlsjyb.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xcb.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kcr.cheryme.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nhg.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fnw.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vln.redwolf501.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jeu.sxryk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wru.ctjpmb.com

[C10] 变量作用域
来源：http://xds.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tgz.birdmap.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rsl.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ucn.shuidangran.top

TS:   同 JS
来源：http://pjq.yj20258.top

Java: 方法内为块级作用域
来源：http://tlu.guannengcc.top

Go:   花括号块级作用域
来源：http://ccb.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://flr.zhongyouzk.top

C#:   块级作用域
来源：http://nrp.redwolf501.top

[C11] 模块导入与导出
来源：http://kva.jiagoushi.top

Py:   from module import func
来源：http://bmy.uphjek.com

PHP:  require "file.php";  或 use App\Service;
来源：http://yxn.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://unw.daria6918.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://srd.hysaishi.cn

Java: import java.util.List;
来源：http://cpq.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qmr.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://sef.yuxming.cn

C#:   using System.Text;
来源：http://bcy.jlsjyb.cn

[C12] 立即执行函数 IIFE
来源：http://fhn.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://wbw.andypj.xyz

PHP:  (function () { echo "run"; })();
来源：http://fso.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://jpf.jinqigufen.top

TS:   (() => { console.log("run"); })();
来源：http://lzl.jianghu66.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wru.gaohongyu789.top

Go:   func() { fmt.Println("run") }()
来源：http://qju.0kj1m.cn

Ruby: -> { puts "run" }.call
来源：http://uic.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://who.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://sge.fehbvm.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xtc.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cxs.shzxlz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ttv.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://loj.epnwcf.com

Java: int add(int a, int b) { return a + b; }
来源：http://esz.hysaishi.cn

Go:   func add(a, b int) int
来源：http://bgt.guowangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bbc.yongpay.top

C#:   int Add(int a, int b) => a + b;
来源：http://tyk.yueranfly.top

[C14] 泛型函数
来源：http://oyu.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tsd.jyoumei.cn

PHP:  // 无泛型
来源：http://cma.epnwcf.com

JS:   // 无泛型
来源：http://tlz.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lea.guannengcc.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kow.shanyushiyangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://upv.tian-w.cn

Ruby: # 无泛型
来源：http://jqj.gogol.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bcj.ydzc1.top

[C15] 解构 / 展开参数
来源：http://jyi.shanyushiyangtech.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sfi.hywenlv.cn

PHP:  [$a, $b] = $pair;
来源：http://hxb.yvedp.cn


<!-- 参考信息 -->