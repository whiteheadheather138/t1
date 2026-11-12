代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eiq.yj202588.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mpq.fengsongda.top

Ruby: s1 == s2; s1 <=> s2
来源：http://snk.xingfuxueyuan.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ezm.epnwcf.com

[A26] 类型转换总览
来源：http://vkm.hesvh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yvp.yj20258888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uak.0kj1m.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xof.hnxiangtu.top

TS:   Number() String() Boolean() x as number
来源：http://iux.jianghu66.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zyu.shzxlz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pmf.fengsongda.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://soc.jinyuanbaomall.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ehs.haohaochexian.top

================================================================================
来源：http://frg.fanxiaobao.xyz

B. 流程控制
来源：http://eza.ydzc1.top

================================================================================
来源：http://kgn.nanxinkj.top

[B01] 条件判断 if / else
来源：http://hfq.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fsw.wangshuangyany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hbl.zhiwuduotai.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://acy.zdbjq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://obt.yj20258.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qgv.cdnleiting.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aff.yuanzhike.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dsd.jlsjyb.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://puj.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://pzi.tanke756.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mro.ydzc1.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ueg.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vqy.pengpengdd.cyou

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wge.zhixingplan.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ixr.yongpay.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dns.jinyuanbaomall.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rql.redwolf501.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ymy.haohaochexian.top

[B03] switch / match / case
来源：http://qyd.iojbl.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tkv.xingfuxueyuan.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wvq.jyoumei.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uoj.nwbrower.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ybu.mhx1999.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tyg.ybcxt.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://crb.fengsongda.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oht.snrcjt.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kjr.hammf.cn

[B04] for 计数循环
来源：http://oln.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://big.kuanghao11.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://goi.cucudq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hok.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vrv.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://llx.gotoacloud.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jes.nanxuanxn.top

Ruby: 10.times { |i| puts i }
来源：http://zrn.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://onr.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://zft.gaohongyu789.top

Py:   for item in arr: print(item)
来源：http://zau.sjlbkw.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ctt.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jtr.daria6918.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uam.andypj.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://qpc.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dfx.zhixingplan.top

Ruby: arr.each { |item| puts item }
来源：http://apq.316326.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://syg.gzhubu.top

[B06] 遍历字典 / 对象
来源：http://alc.hnxiangtu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hig.vqdsnc.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ebb.jinyuanbaomall.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jwl.hnxiangtu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cti.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://omf.vqdsnc.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ncb.aizwys.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bdb.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lqa.aibaodan.cn

[B07] while 循环
来源：http://yik.shuidangran.top

Py:   while i < 10: i += 1
来源：http://hbz.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nzk.aizwys.cn

JS:   while (i < 10) { i++; }
来源：http://vnr.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://sqf.yongpay.top

Java: while (i < 10) { i++; }
来源：http://rqu.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gxc.shangyingyoupin.top

Ruby: while i < 10; i += 1; end
来源：http://cvt.zdqjudy.top

C#:   while (i < 10) { i++; }
来源：http://uck.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://xqz.shanyushiyangtech.top

Py:   # 无 do-while：用 while True + break
来源：http://twt.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zil.xinyue.icu

JS:   do { i++; } while (i < 10);
来源：http://fdd.xylfe.cn

TS:   do { i++; } while (i < 10);
来源：http://nzu.zhongyouzk.top

Java: do { i++; } while (i < 10);
来源：http://clm.ppjwa.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://emr.xingfuxueyuan.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://huk.guowangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://zjv.hywenlv.cn

[B09] break 与 continue
来源：http://joy.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uci.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lsd.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qsw.mhx1999.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gee.guannengcc.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kst.daria6918.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kjt.pycfn.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cgu.0kj1m.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://shr.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://ske.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pix.zhijiandao.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ysc.hnqzz.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vzl.shzxlz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vyd.pengpengdd.cyou

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lwx.yonumen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zoc.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://val.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oca.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://jxe.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://qmk.havefunace.top

PHP:  range(0, 10, 2);
来源：http://nfn.nanxuanxn.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vnt.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hgx.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cds.vehdjk.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hir.hesvh.cn

Ruby: (0...10).step(2).to_a
来源：http://bjv.hammf.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xla.aizwys.cn

[B12] 跳出多层循环
来源：http://bmk.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lrd.wangdashe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dhg.chenzaomai.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qhj.zhaomingkeji.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ryh.zhijiandao.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ubk.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jib.vqdsnc.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://trb.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cgu.uphjek.com

[B13] 判断是否为数字
来源：http://mmi.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://whx.quarkkingdee.top

PHP:  is_numeric($x)
来源：http://mxv.ivvv.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wwp.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rwx.andypj.xyz

Java: x instanceof Number
来源：http://zct.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://daj.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://lgs.dashuyun.cn

C#:   x is int or double or decimal
来源：http://dzo.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://tmk.guannengcc.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jhl.zycfv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://obg.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://lkr.fehbvm.com

TS:   [1, 2, 3].includes(x)
来源：http://qvb.yj20258.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ymg.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uiy.zhongyouzk.top

Ruby: [1, 2, 3].include?(x)
来源：http://lwa.0kj1m.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fgk.xingfuxueyuan.xyz

[B15] 布尔运算与取反
来源：http://dox.yangfankeji.com

Py:   a and b or not c
来源：http://kdz.xinyue.icu

PHP:  $a && $b || !$c
来源：http://vcy.yuanzhike.top

JS:   a && b || !c
来源：http://oik.yueranfly.top

TS:   a && b || !c
来源：http://yaw.ywan-chungtsiang.top

Java: a && b || !c
来源：http://pxw.bjfxy.top

Go:   a && b || !c
来源：http://oxk.zhongyouzk.top

Ruby: a && b || !c
来源：http://yjn.tian-w.cn

C#:   a && b || !c
来源：http://bcu.fehbvm.com

[B16] 卫语句：不满足条件提前返回
来源：http://ipl.0kj1m.cn

Py:   if not data: return
来源：http://pzk.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://xkx.aibaodan.cn

JS:   if (!data) return;
来源：http://dmz.andypj.xyz

TS:   if (!data) return;
来源：http://skc.yvedp.cn

Java: if (data == null) return;
来源：http://jof.sxryk.cn

Go:   if data == nil { return }
来源：http://wjr.yj20258.top

Ruby: return if data.nil?
来源：http://bgx.zdbjq.cn

C#:   if (data == null) return;
来源：http://cyt.daria6918.cn

================================================================================
来源：http://nya.jinyuanbaomall.cn

C. 函数与作用域
来源：http://pbb.chenzaomai.com

================================================================================
来源：http://mwd.hnqzz.top

[C01] 定义函数
来源：http://xyc.9152youxi.cn

Py:   def add(a, b): return a + b
来源：http://yus.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ycj.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://pxi.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bpf.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qgd.yj202588.top

Go:   func add(a, b int) int { return a + b }
来源：http://ywr.yvedp.cn

Ruby: def add(a, b); a + b; end
来源：http://mmy.hfpthk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://trz.havefunace.top

[C02] 默认参数
来源：http://acp.yongpay.top

Py:   def greet(name="World"): return name
来源：http://qck.haohaochexian.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ett.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://nob.havefunace.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rzh.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://sxh.zhengqikj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://grh.gogol.net.cn

Ruby: def greet(name = "World") = name
来源：http://suc.quarkkingdee.top

C#:   string Greet(string name = "World") => name;
来源：http://qaw.9152youxi.cn

[C03] 可变参数
来源：http://ocq.nanxinkj.top

Py:   def total(*args): return sum(args)
来源：http://wai.jlsjyb.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jom.uphjek.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vpl.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://age.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nbb.0kj1m.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iww.jinqigfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://vws.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fdg.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://vxc.nanxinkj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rms.jqgufenzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mux.feifeiyinyue.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://itd.chenlongwang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vkt.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://qob.epnwcf.com

Go:   // 无：用配置结构体参数
来源：http://qof.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://ulg.tanke756.top

C#:   f(a: 1, b: 2)
来源：http://wfd.shanyushiyangtech.top

[C05] 返回多个值
来源：http://rnt.yj202588.top

Py:   return a, b
来源：http://rwe.vehdjk.com

PHP:  return [$a, $b];
来源：http://awj.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://duj.zdqjudy.top

TS:   return { a, b };
来源：http://lhd.yangfankeji.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vjl.hongshengwenyu.top

Go:   return a, b
来源：http://gdj.zhoulong.xyz

Ruby: return a, b
来源：http://frk.9152youxi.cn

C#:   return (a, b);              // ValueTuple
来源：http://wiw.daxiang520.top

[C06] 匿名函数 / lambda
来源：http://osb.9152youxi.cn

Py:   square = lambda x: x * x
来源：http://iai.mhx1999.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hks.cucudq.cn

JS:   const square = x => x * x;
来源：http://xog.hysaishi.cn

TS:   const square = (x: number): number => x * x;
来源：http://goo.yvedp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://npc.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kjx.gaohongyu789.top

Ruby: square = ->(x) { x * x }
来源：http://haa.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gzy.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://hvp.xuetiantiany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ovg.yvedp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dtg.bbcook.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gxc.c1oappe.top

TS:   arr.map(String)
来源：http://aox.sysykeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ues.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oab.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://hgm.xuanzx.com

C#:   arr.Select(s => s.ToUpper())
来源：http://wob.zdbjq.cn

[C08] 闭包
来源：http://xcl.jinyuanbaomall.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ydt.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xek.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dfz.zhixingplan.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kgo.ywan-chungtsiang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mne.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bmg.bbcook.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sxi.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://npm.chenzaomai.com

[C09] 递归
来源：http://oji.zdqjudy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lpq.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dwh.fktsv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ddy.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hex.shanyushiyangtech.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pao.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cbm.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pms.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bek.c1oappe.top

[C10] 变量作用域
来源：http://gsh.bbcook.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oww.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wew.zhoulong.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dad.hongshengwenyu.top

TS:   同 JS
来源：http://fcg.yj20258888.top

Java: 方法内为块级作用域
来源：http://pgx.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://mvu.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dtm.jinyuanbaomall.cn

C#:   块级作用域
来源：http://fck.xziqi.cn

[C11] 模块导入与导出
来源：http://pwc.tarul.cn

Py:   from module import func
来源：http://kyf.guannengcc.top

PHP:  require "file.php";  或 use App\Service;
来源：http://txp.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vwd.yanxiufei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mpf.guannengcc.top

Java: import java.util.List;
来源：http://lik.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rry.shanyushiyangtech.top

Ruby: require "json"; require_relative "./util"
来源：http://bre.zhiwuduotai.top

C#:   using System.Text;
来源：http://fgg.xylfe.cn

[C12] 立即执行函数 IIFE
来源：http://yly.tarul.cn

Py:   (lambda: print("run"))()
来源：http://kkh.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://rgr.vqdsnc.cn

JS:   (() => { console.log("run"); })();
来源：http://hdb.cashguo.top

TS:   (() => { console.log("run"); })();
来源：http://pek.jqgfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://azf.gogol.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://cbl.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://byg.jlsjyb.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qkl.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://zkr.tianlin.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fcv.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tpa.zhongyouzk.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cth.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jls.ehwqpu.com

Java: int add(int a, int b) { return a + b; }
来源：http://xbj.zdqjudy.top

Go:   func add(a, b int) int
来源：http://yqt.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://plp.bbcook.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kpf.yj20258.top

[C14] 泛型函数
来源：http://vmo.feifeiyinyue.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jkh.sweek.top

PHP:  // 无泛型
来源：http://sss.hesvh.cn

JS:   // 无泛型
来源：http://bky.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ybq.dashuyun.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://prc.hesvh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dwe.yuanzhike.top

Ruby: # 无泛型
来源：http://sqk.wangdashe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://itd.tanke756.top

[C15] 解构 / 展开参数
来源：http://drx.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://son.hywenlv.cn

PHP:  [$a, $b] = $pair;
来源：http://kvl.shanyushiyangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qcf.hammf.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qou.hesvh.cn

Java: // 无解构
来源：http://nur.ehwqpu.com

Go:   // 无解构
来源：http://trn.snrcjt.cn

Ruby: a, b = pair
来源：http://pib.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://gfy.yvedp.cn

[C16] 函数 / 方法重载
来源：http://epc.zdbjq.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vru.nwbrower.top


<!-- 参考信息 -->