代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://kjb.snrcjt.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ewr.aizwys.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://spg.shanyushiyangtech.top

[A25] 字符串比较
来源：http://kxj.aibaodan.cn

Py:   s1 == s2; s1 != s2
来源：http://qxz.zycfv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yxn.jqgufenzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zal.hcnkem.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bwb.andypj.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vmo.yonumen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kac.pengpengdd.cyou

Ruby: s1 == s2; s1 <=> s2
来源：http://bte.ehwqpu.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nyv.aizwys.cn

[A26] 类型转换总览
来源：http://qqm.ywan-chungtsiang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uhn.daxiang520.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://otg.zdqjudy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rlt.xingfuxueyuan.xyz

TS:   Number() String() Boolean() x as number
来源：http://zlc.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nke.gogol.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hlr.haohaochexian.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dmy.mhx1999.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://evc.sysykeji.top

================================================================================
来源：http://txj.wangdashe.top

B. 流程控制
来源：http://wsw.yfazqb.com

================================================================================
来源：http://bge.yfazqb.com

[B01] 条件判断 if / else
来源：http://wfa.daxiang520.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wck.xinyue.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ppi.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sds.dashuyun.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fjg.svipenyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ypi.sxryk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nvd.zhaomingkeji.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wus.guowangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yzk.shangyingyoupin.top

[B02] 多分支 else if / elif
来源：http://erw.ctjpmb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bsr.chenzaomai.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jds.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ayr.jyoumei.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oyr.jyoumei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yfy.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://miy.yj202588.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xuw.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qjl.xingfuxueyuan.xyz

[B03] switch / match / case
来源：http://fwq.zhijiandao.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hqj.vehdjk.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eoh.fktsv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tac.wangshuangyany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ckk.jiagoushi.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://erz.ydjk.org.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mpf.ehwqpu.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kre.hesvh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fik.epnwcf.com

[B04] for 计数循环
来源：http://euy.ybcxt.top

Py:   for i in range(10): print(i)
来源：http://eax.xingfuxueyuan.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fig.zhaomingkeji.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://thx.tanke756.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://khs.kuanghao11.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tjq.daxiang520.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xrs.zycfv.cn

Ruby: 10.times { |i| puts i }
来源：http://dww.hywenlv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xvo.zhongyouzk.top

[B05] 遍历数组 / 列表
来源：http://pza.cashguo.top

Py:   for item in arr: print(item)
来源：http://owq.ydzc1.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://huj.smart0.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://emi.zycfv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yjz.xuanzx.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://trl.quarkkingdee.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ymk.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://jjc.shanyushiyangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mtb.ydjk.org.cn

[B06] 遍历字典 / 对象
来源：http://vhm.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://krf.zdbjq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://imt.tian-w.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://plu.shanyushiyangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rap.zhoulong.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qxt.zhengqikj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://auo.tianlin.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ppl.andypj.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pjj.fehbvm.com

[B07] while 循环
来源：http://rpt.zhixingplan.top

Py:   while i < 10: i += 1
来源：http://gbd.zdbjq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eul.sweek.top

JS:   while (i < 10) { i++; }
来源：http://wgc.jiagoushi.top

TS:   while (i < 10) { i++; }
来源：http://zsj.jinqigfzy.top

Java: while (i < 10) { i++; }
来源：http://dey.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xmw.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://qwg.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://fxn.jiagoushi.top

[B08] do-while（至少执行一次）
来源：http://ecg.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://dzw.sysykeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zbj.hysaishi.cn

JS:   do { i++; } while (i < 10);
来源：http://vow.dianchejie.cn

TS:   do { i++; } while (i < 10);
来源：http://vgf.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://nwu.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xox.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://bfx.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://asi.yueranfly.top

[B09] break 与 continue
来源：http://huo.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vkk.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wkd.shangyingyoupin.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hsp.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zkw.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lmz.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lmt.cheryme.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ubn.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zvn.zdbjq.cn

[B10] 遍历同时拿索引
来源：http://bhv.zycfv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wgy.tianlin.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ebs.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xgh.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vah.fzhhl.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rlk.yj202588.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sof.sweek.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ttt.gogol.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sql.jqgufenzy.top

[B11] 生成数字序列 / 区间
来源：http://zcj.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://bjj.wangshuangyany.cn

PHP:  range(0, 10, 2);
来源：http://cya.chenjidiqi.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kbg.havefunace.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://trn.sjlbkw.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://muc.hammf.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dte.havefunace.top

Ruby: (0...10).step(2).to_a
来源：http://fsd.cashguo.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vkw.guowangkeji.top

[B12] 跳出多层循环
来源：http://ryb.jyoumei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cxc.haohaochexian.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ukr.ybcxt.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uad.vehdjk.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://afa.dashuyun.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mfn.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mlp.shzxlz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gcc.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aah.yangfankeji.com

[B13] 判断是否为数字
来源：http://gyw.xuetiantiany.cn

Py:   isinstance(x, (int, float))
来源：http://qel.fehbvm.com

PHP:  is_numeric($x)
来源：http://lok.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zsb.guowangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aip.hfpthk.cn

Java: x instanceof Number
来源：http://pjb.yangfankeji.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xff.guowangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://fyx.svipenyu.cn

C#:   x is int or double or decimal
来源：http://cry.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://rxt.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://icl.sweek.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lsl.nanxuanxn.top

JS:   [1, 2, 3].includes(x)
来源：http://lao.ydjk.org.cn

TS:   [1, 2, 3].includes(x)
来源：http://qbj.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jkc.yvedp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ibw.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ums.xuanzx.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pxo.fehbvm.com

[B15] 布尔运算与取反
来源：http://jvb.52xcode.cn

Py:   a and b or not c
来源：http://nlk.bjfxy.top

PHP:  $a && $b || !$c
来源：http://gag.nanxinkj.top

JS:   a && b || !c
来源：http://jon.tarul.cn

TS:   a && b || !c
来源：http://oxt.smart0.xyz

Java: a && b || !c
来源：http://avt.jlsjyb.cn

Go:   a && b || !c
来源：http://anm.guannengcc.top

Ruby: a && b || !c
来源：http://vem.jiagoushi.top

C#:   a && b || !c
来源：http://cut.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://qbf.chenlongwang.top

Py:   if not data: return
来源：http://ick.tarul.cn

PHP:  if (!$data) { return; }
来源：http://crl.0kj1m.cn

JS:   if (!data) return;
来源：http://dui.daxiang520.top

TS:   if (!data) return;
来源：http://jbm.bbcook.cn

Java: if (data == null) return;
来源：http://rrv.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://pud.andypj.xyz

Ruby: return if data.nil?
来源：http://mpv.cucudq.cn

C#:   if (data == null) return;
来源：http://wfb.mhx1999.top

================================================================================
来源：http://aua.uphjek.com

C. 函数与作用域
来源：http://xkr.cdnleiting.top

================================================================================
来源：http://wrr.epnwcf.com

[C01] 定义函数
来源：http://tsw.epnwcf.com

Py:   def add(a, b): return a + b
来源：http://xhk.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kuh.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://vmm.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://txc.feifeiyinyue.top

Java: static int add(int a, int b) { return a + b; }
来源：http://aho.epnwcf.com

Go:   func add(a, b int) int { return a + b }
来源：http://tyb.fktsv.cn

Ruby: def add(a, b); a + b; end
来源：http://wru.yvedp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xts.shzxlz.cn

[C02] 默认参数
来源：http://yyl.jiagoushi.top

Py:   def greet(name="World"): return name
来源：http://pus.gaohongyu789.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nap.yuxming.cn

JS:   function greet(name = "World") { return name; }
来源：http://ivz.jianghu66.top

TS:   function greet(name: string = "World") { return name; }
来源：http://riz.havefunace.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cvw.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wgc.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://cld.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://xsp.yueranfly.top

[C03] 可变参数
来源：http://orf.gotoacloud.top

Py:   def total(*args): return sum(args)
来源：http://vsd.haohaochexian.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://coz.xingfuxueyuan.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gvy.yj202588.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ccz.gzhubu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ktn.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cuh.aibaodan.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jxs.wangdashe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://abb.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://ufn.fengsongda.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aau.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mzh.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pak.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wmf.wangshuangyany.cn

Java: // 无：用 Builder 模式或 record
来源：http://ecf.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://mlx.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://twa.yueranfly.top

C#:   f(a: 1, b: 2)
来源：http://qkm.yangfankeji.com

[C05] 返回多个值
来源：http://wbn.jyoumei.cn

Py:   return a, b
来源：http://thr.yfazqb.com

PHP:  return [$a, $b];
来源：http://bji.aibaodan.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kqi.jiagoushi.top

TS:   return { a, b };
来源：http://grw.shangyingyoupin.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gtj.yuxming.cn

Go:   return a, b
来源：http://mbj.iojbl.cn

Ruby: return a, b
来源：http://idb.0kj1m.cn

C#:   return (a, b);              // ValueTuple
来源：http://dza.chenzaomai.com

[C06] 匿名函数 / lambda
来源：http://aly.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://mqm.hesvh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rbb.zhengqikj.top

JS:   const square = x => x * x;
来源：http://has.smart0.xyz

TS:   const square = (x: number): number => x * x;
来源：http://loq.wangshuangyany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sbl.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://pzb.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://gwy.nanxinkj.top

C#:   Func<int, int> square = x => x * x;
来源：http://xvx.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://txo.jqgfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sln.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://imf.jiagoushi.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lkk.fehbvm.com

TS:   arr.map(String)
来源：http://aeo.yongpay.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rhg.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ojd.jinyuanbaomall.cn

Ruby: arr.map(&:upcase)
来源：http://qvw.c1oappe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dbw.shanyushiyangkeji.top

[C08] 闭包
来源：http://fca.xingfuxueyuan.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://srn.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pcy.shuidangran.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bey.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hmv.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ktr.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oqf.gaohongyu789.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dur.yanxiufei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tpd.haohaochexian.top

[C09] 递归
来源：http://qwa.andypj.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dtm.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wmb.yonumen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://unh.jinqigfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xgh.xinyue.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ygr.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pzp.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tag.jinqigfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bkh.nanxuanxn.top

[C10] 变量作用域
来源：http://vin.nwbrower.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ylb.jiagoushi.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pzs.yongpay.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wxp.xziqi.cn

TS:   同 JS
来源：http://edc.guannengcc.top

Java: 方法内为块级作用域
来源：http://zsd.uphjek.com

Go:   花括号块级作用域
来源：http://yaf.epnwcf.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mzd.birdmap.top

C#:   块级作用域
来源：http://pec.epnwcf.com

[C11] 模块导入与导出
来源：http://mna.shuidangran.top

Py:   from module import func
来源：http://vcz.316326.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://fnd.aizwys.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xjc.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bsx.guannengcc.top

Java: import java.util.List;
来源：http://hfx.cqqwz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dcs.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://wnv.hesvh.cn

C#:   using System.Text;
来源：http://dom.epnwcf.com

[C12] 立即执行函数 IIFE
来源：http://wzn.aizwys.cn

Py:   (lambda: print("run"))()
来源：http://poy.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://lem.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://nbf.yuxming.cn

TS:   (() => { console.log("run"); })();
来源：http://cxz.yanxiufei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jan.chenlongwang.top

Go:   func() { fmt.Println("run") }()
来源：http://vox.havefunace.top

Ruby: -> { puts "run" }.call
来源：http://kvn.hammf.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://avg.dashuyun.cn

[C13] 类型声明 / 类型注解
来源：http://oke.guannengcc.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://esy.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://reu.xuetiantiany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tfq.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lot.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://iri.sufxvd.cn

Go:   func add(a, b int) int
来源：http://qpo.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xuk.daxiang520.top

C#:   int Add(int a, int b) => a + b;
来源：http://axh.gaohongyu789.top

[C14] 泛型函数
来源：http://awa.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lzp.epnwcf.com

PHP:  // 无泛型
来源：http://boy.9152youxi.cn

JS:   // 无泛型
来源：http://vgj.bjfxy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://trb.iojbl.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qum.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://doz.sufxvd.cn

Ruby: # 无泛型
来源：http://qiq.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qel.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://ixz.xuanzx.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://emk.316326.xyz

PHP:  [$a, $b] = $pair;
来源：http://lep.chenzaomai.com


<!-- 参考信息 -->