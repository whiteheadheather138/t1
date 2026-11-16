代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wfz.yangfankeji.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xwj.snrcjt.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fjo.pycfn.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nxi.nanxinkj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://piq.jqgfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qsk.tanke756.top

[A24] 去除首尾空白
来源：http://krg.yongpay.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wyb.gzhubu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ezk.pengpengdd.cyou

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jzz.xuetiantiany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oaj.chenjidiqi.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zkp.wangdashe.top

Go:   strings.TrimSpace(s)
来源：http://rcy.hesvh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xrq.guowangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iyd.xinyue.icu

[A25] 字符串比较
来源：http://xex.gogol.net.cn

Py:   s1 == s2; s1 != s2
来源：http://zfv.smart0.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://egt.fzhhl.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://swe.yueranfly.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://clc.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gln.zhongyouzk.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vbf.ctjpmb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://ist.shuidangran.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lki.cucudq.cn

[A26] 类型转换总览
来源：http://rht.ybcxt.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qew.ctjpmb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vhk.fktsv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://alr.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://hqh.jinghuilouyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cof.gzhubu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rng.zhengqikj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ymy.gaohongyu789.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://obn.cucudq.cn

================================================================================
来源：http://hxv.c1oappe.top

B. 流程控制
来源：http://fgm.jinyuanbaomall.cn

================================================================================
来源：http://ilf.ctjpmb.com

[B01] 条件判断 if / else
来源：http://rqo.yangfankeji.com

Py:   result = "正" if x > 0 else "非正"
来源：http://alo.nanxuanxn.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tjs.ydzc1.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cua.cheryme.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ttm.shangyingyoupin.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uqn.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cem.316326.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nwh.yuxming.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://umv.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://zsl.sweek.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aht.smart0.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lzg.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zxf.yuxming.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ozq.epnwcf.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kil.havefunace.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sjo.xuetiantiany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://aoq.cqqwz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jld.ydjk.org.cn

[B03] switch / match / case
来源：http://pef.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ftx.9152youxi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jaa.ehwqpu.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://igf.yj20258888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wwx.52xcode.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yto.shanyushiyangtech.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xvc.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cxc.zdbjq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://osx.cheryme.top

[B04] for 计数循环
来源：http://fnw.nanxuanxn.top

Py:   for i in range(10): print(i)
来源：http://kyg.hcnkem.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vpk.zhaomingkeji.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qgi.hongshengwenyu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qto.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fpl.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://euw.aizwys.cn

Ruby: 10.times { |i| puts i }
来源：http://fpm.ydzc1.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://awv.feifeiyinyue.top

[B05] 遍历数组 / 列表
来源：http://kjl.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://lgs.guowangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uff.chenlongwang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tqs.yj202588.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fzx.hongshengwenyu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zzs.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jyf.redwolf501.top

Ruby: arr.each { |item| puts item }
来源：http://eru.tanke756.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xkb.yj202588.top

[B06] 遍历字典 / 对象
来源：http://lms.jianghu66.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ynf.jiagoushi.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gzl.wangshuangyany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ijs.shangyingyoupin.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ohz.hcnkem.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wvb.hywenlv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tyq.zhijiandao.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kwf.uphjek.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mzp.aibaodan.cn

[B07] while 循环
来源：http://qwr.guannengcc.top

Py:   while i < 10: i += 1
来源：http://hrn.chenzaomai.com

PHP:  while ($i < 10) { $i++; }
来源：http://kap.fehbvm.com

JS:   while (i < 10) { i++; }
来源：http://lcg.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://wpt.guannengcc.top

Java: while (i < 10) { i++; }
来源：http://wib.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kst.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://bum.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://zat.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://ayp.gogol.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://uwp.guannengcc.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rve.sysykeji.top

JS:   do { i++; } while (i < 10);
来源：http://jpu.jiagoushi.top

TS:   do { i++; } while (i < 10);
来源：http://hlx.xuetiantiany.cn

Java: do { i++; } while (i < 10);
来源：http://ffu.kuanghao11.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ghz.yueranfly.top

Ruby: begin; i += 1; end while i < 10
来源：http://ykl.cashguo.top

C#:   do { i++; } while (i < 10);
来源：http://wie.aizwys.cn

[B09] break 与 continue
来源：http://rvb.hcnkem.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wjr.tanke756.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gep.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ipz.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sul.kuanghao11.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iib.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qra.zdqjudy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uyk.zdbjq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bpv.birdmap.top

[B10] 遍历同时拿索引
来源：http://ssq.ydjk.org.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uqy.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ism.ywan-chungtsiang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jib.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hyt.nanxinkj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nar.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://csm.hnxiangtu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ady.gogol.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sey.yvedp.cn

[B11] 生成数字序列 / 区间
来源：http://ptc.vehdjk.com

Py:   list(range(0, 10, 2))
来源：http://zmc.jyoumei.cn

PHP:  range(0, 10, 2);
来源：http://sbd.jqgufenzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yhv.dashuyun.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lam.ydjk.org.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kmj.sweek.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mbm.gaohongyu789.top

Ruby: (0...10).step(2).to_a
来源：http://ycj.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gke.chenlongwang.top

[B12] 跳出多层循环
来源：http://oup.ybcxt.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cln.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://erl.haohaochexian.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mcd.hongshengwenyu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://arc.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lul.zhongyouzk.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ful.zdbjq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gix.tian-w.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fra.nanxuanxn.top

[B13] 判断是否为数字
来源：http://krc.zhijiandao.cn

Py:   isinstance(x, (int, float))
来源：http://zwf.yanxiufei.cn

PHP:  is_numeric($x)
来源：http://vnw.zhoulong.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hmx.gogol.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://puj.yfazqb.com

Java: x instanceof Number
来源：http://sia.tanke756.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sqa.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://crz.hfpthk.cn

C#:   x is int or double or decimal
来源：http://zud.iojbl.cn

[B14] 判断值是否在集合内
来源：http://vga.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eou.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vtc.sjlbkw.cn

JS:   [1, 2, 3].includes(x)
来源：http://tlc.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://gsm.snrcjt.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vkg.zdqjudy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yoc.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://swr.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qog.dianchejie.cn

[B15] 布尔运算与取反
来源：http://env.svipenyu.cn

Py:   a and b or not c
来源：http://xij.chenzaomai.com

PHP:  $a && $b || !$c
来源：http://gwb.wangshuangyany.cn

JS:   a && b || !c
来源：http://jcf.wangshuangyany.cn

TS:   a && b || !c
来源：http://cec.snrcjt.cn

Java: a && b || !c
来源：http://wrd.zdbjq.cn

Go:   a && b || !c
来源：http://ozi.vqdsnc.cn

Ruby: a && b || !c
来源：http://cix.yonumen.top

C#:   a && b || !c
来源：http://jme.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://tsm.hesvh.cn

Py:   if not data: return
来源：http://hbi.xziqi.cn

PHP:  if (!$data) { return; }
来源：http://xim.ydjk.org.cn

JS:   if (!data) return;
来源：http://luu.yj20258888.top

TS:   if (!data) return;
来源：http://fsl.redwolf501.top

Java: if (data == null) return;
来源：http://toc.fanxiaobao.xyz

Go:   if data == nil { return }
来源：http://bfw.haohaochexian.top

Ruby: return if data.nil?
来源：http://equ.xuanzx.com

C#:   if (data == null) return;
来源：http://mds.ctjpmb.com

================================================================================
来源：http://evf.haohaochexian.top

C. 函数与作用域
来源：http://gib.cheryme.top

================================================================================
来源：http://pan.ivvv.top

[C01] 定义函数
来源：http://utd.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://dms.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vpa.jinghuilouyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://pwt.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://adn.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yyv.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://gqs.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://prk.cdnleiting.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://naq.guowangkeji.top

[C02] 默认参数
来源：http://nlm.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://ltw.kuanghao11.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kby.jqgfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://mqh.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ife.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gkn.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tfc.jyoumei.cn

Ruby: def greet(name = "World") = name
来源：http://lpw.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://lqq.hysaishi.cn

[C03] 可变参数
来源：http://oos.jinghuilouyu.cn

Py:   def total(*args): return sum(args)
来源：http://xhm.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wpl.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jpg.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://khb.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zcw.pengpengdd.cyou

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://byr.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://vjh.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gae.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://rlw.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nmy.yj20258888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://our.zhijiandao.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sci.pycfn.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qor.ehwqpu.com

Java: // 无：用 Builder 模式或 record
来源：http://gdf.wangshuangyany.cn

Go:   // 无：用配置结构体参数
来源：http://wje.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://mbz.yonumen.top

C#:   f(a: 1, b: 2)
来源：http://uid.shanyushiyangtech.top

[C05] 返回多个值
来源：http://qsm.hnxiangtu.top

Py:   return a, b
来源：http://uni.daxiang520.top

PHP:  return [$a, $b];
来源：http://vpp.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fdl.9152youxi.cn

TS:   return { a, b };
来源：http://cix.nwbrower.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://edy.jinghuilouyu.cn

Go:   return a, b
来源：http://iiq.nanxinkj.top

Ruby: return a, b
来源：http://tpz.hnqzz.top

C#:   return (a, b);              // ValueTuple
来源：http://nnm.yuxming.cn

[C06] 匿名函数 / lambda
来源：http://yhp.nanxinkj.top

Py:   square = lambda x: x * x
来源：http://pml.mhx1999.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gsu.daria6918.cn

JS:   const square = x => x * x;
来源：http://skb.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://pmm.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ttp.hfpthk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ekl.sweek.top

Ruby: square = ->(x) { x * x }
来源：http://uwf.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yja.wangdashe.top

[C07] 把函数作为参数传入
来源：http://oyf.epnwcf.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qhl.jinqigfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://dia.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xxc.zhongyouzk.top

TS:   arr.map(String)
来源：http://tgk.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tsy.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bov.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://bfp.haohaochexian.top

C#:   arr.Select(s => s.ToUpper())
来源：http://oct.hfpthk.cn

[C08] 闭包
来源：http://mtk.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kxm.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lyi.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://igv.chenlongwang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vyd.ywan-chungtsiang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eaw.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ugd.hcnkem.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pgp.zhaomingkeji.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kdv.kuanghao11.cn

[C09] 递归
来源：http://dye.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jbj.daxiang520.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lou.gogol.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ako.guowangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yhj.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xbm.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fnk.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kka.hongshengwenyu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sbq.xziqi.cn

[C10] 变量作用域
来源：http://pam.sjlbkw.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rsk.zhixingplan.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lad.hongshengwenyu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ven.jqgufenzy.top

TS:   同 JS
来源：http://mhb.gaohongyu789.top

Java: 方法内为块级作用域
来源：http://dwn.xziqi.cn

Go:   花括号块级作用域
来源：http://jqp.aizwys.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gqw.yanxiufei.cn

C#:   块级作用域
来源：http://wnb.jyoumei.cn

[C11] 模块导入与导出
来源：http://emn.gaohongyu789.top

Py:   from module import func
来源：http://kzq.hfpthk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ozy.sxryk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nlk.aizwys.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xkr.52xcode.cn

Java: import java.util.List;
来源：http://pzp.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://flw.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://nrh.shuidangran.top

C#:   using System.Text;
来源：http://wfp.hysaishi.cn

[C12] 立即执行函数 IIFE
来源：http://etu.haohaochexian.top

Py:   (lambda: print("run"))()
来源：http://uhi.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://zwl.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://xce.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://vqe.hnqzz.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ogx.zhaomingkeji.xyz

Go:   func() { fmt.Println("run") }()
来源：http://nta.pycfn.com

Ruby: -> { puts "run" }.call
来源：http://vic.tian-w.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qgp.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://miq.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bdq.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://agt.dashuyun.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wsw.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://edj.9152youxi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zbg.svipenyu.cn

Go:   func add(a, b int) int
来源：http://rzh.yvedp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://son.nanxuanxn.top

C#:   int Add(int a, int b) => a + b;
来源：http://pwg.shzxlz.cn


<!-- 参考信息 -->