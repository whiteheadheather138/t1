代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://bda.yj202588.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wsa.yuanzhike.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://guu.sjlbkw.cn

[A25] 字符串比较
来源：http://wkl.hysaishi.cn

Py:   s1 == s2; s1 != s2
来源：http://ycg.sufxvd.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oey.ydzc1.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jmd.hysaishi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ypg.zhaomingkeji.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vii.gaohongyu789.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nfe.guowangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://yys.birdmap.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://esf.vehdjk.com

[A26] 类型转换总览
来源：http://sjq.hywenlv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xpl.havefunace.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pah.yj202588.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zeu.aibaodan.cn

TS:   Number() String() Boolean() x as number
来源：http://hva.svipenyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zuu.ybcxt.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ird.svipenyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tzu.ywan-chungtsiang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vhz.tian-w.cn

================================================================================
来源：http://buk.xziqi.cn

B. 流程控制
来源：http://ztb.yanxiufei.cn

================================================================================
来源：http://iiy.9152youxi.cn

[B01] 条件判断 if / else
来源：http://cma.jqgufenzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://prv.tanke756.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eca.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bfh.fktsv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://isn.52xcode.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ero.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://imy.yj20258888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ozf.gogol.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hdd.jqgfzy.top

[B02] 多分支 else if / elif
来源：http://eor.pengpengdd.cyou

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cjk.hfpthk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eka.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yoj.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ack.hnxiangtu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uok.jinyuanbaomall.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://urc.meibo888.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://arh.yonumen.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qiz.ctjpmb.com

[B03] switch / match / case
来源：http://dhm.jinqigfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iti.yj202588.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xji.ppjwa.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lrs.zhijiandao.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://saq.redwolf501.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://szd.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tpu.redwolf501.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wrk.birdmap.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://shb.vqdsnc.cn

[B04] for 计数循环
来源：http://eby.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://vzd.yanxiufei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://goa.zhoulong.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oec.guannengcc.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sgu.snrcjt.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zrd.xziqi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hua.cucudq.cn

Ruby: 10.times { |i| puts i }
来源：http://efx.zhongyouzk.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qfb.uphjek.com

[B05] 遍历数组 / 列表
来源：http://kmp.wangdashe.top

Py:   for item in arr: print(item)
来源：http://lxz.ydzc1.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://viw.iojbl.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ybo.guannengcc.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ous.smart0.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://wnd.jianghu66.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://emf.redwolf501.top

Ruby: arr.each { |item| puts item }
来源：http://yek.gzhubu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://erd.zhiwuduotai.top

[B06] 遍历字典 / 对象
来源：http://xej.pengpengdd.cyou

Py:   for k, v in d.items(): print(k, v)
来源：http://bzn.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hlq.zhixingplan.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rby.guannengcc.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qqw.hnxiangtu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kup.xuetiantiany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kgi.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bjs.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zmn.xinyue.icu

[B07] while 循环
来源：http://zxy.yj20258.top

Py:   while i < 10: i += 1
来源：http://gmq.yuxming.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hts.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://skt.ivvv.top

TS:   while (i < 10) { i++; }
来源：http://njs.jiagoushi.top

Java: while (i < 10) { i++; }
来源：http://krn.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wjw.svipenyu.cn

Ruby: while i < 10; i += 1; end
来源：http://rwm.redwolf501.top

C#:   while (i < 10) { i++; }
来源：http://pfw.dashuyun.cn

[B08] do-while（至少执行一次）
来源：http://zsw.chenlongwang.top

Py:   # 无 do-while：用 while True + break
来源：http://nhf.cdnleiting.top

PHP:  do { $i++; } while ($i < 10);
来源：http://knv.pycfn.com

JS:   do { i++; } while (i < 10);
来源：http://gkh.gaohongyu789.top

TS:   do { i++; } while (i < 10);
来源：http://pix.birdmap.top

Java: do { i++; } while (i < 10);
来源：http://nns.ctjpmb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://gru.hnqzz.top

Ruby: begin; i += 1; end while i < 10
来源：http://vjm.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://cht.jinghuilouyu.cn

[B09] break 与 continue
来源：http://dwm.xuetiantiany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qwt.xingfuxueyuan.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jaw.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fpq.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eoc.chenjidiqi.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eqj.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eaq.xuetiantiany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xrl.xuetiantiany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qhd.zhixingplan.top

[B10] 遍历同时拿索引
来源：http://pqq.ydjk.org.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hti.daxiang520.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tgq.cucudq.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wyp.ydjk.org.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hrj.nwbrower.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://how.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dkp.zhengqikj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tzx.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vja.sweek.top

[B11] 生成数字序列 / 区间
来源：http://msn.zdbjq.cn

Py:   list(range(0, 10, 2))
来源：http://elk.zhijiandao.cn

PHP:  range(0, 10, 2);
来源：http://zhv.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ytv.yj20258.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://isc.daria6918.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dnm.yueranfly.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lua.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://qms.havefunace.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ggq.zhixingplan.top

[B12] 跳出多层循环
来源：http://pnz.yonumen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nrt.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://gyd.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xgk.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xkg.hysaishi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hiz.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ewn.shangyingyoupin.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fow.zhongyouzk.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mup.ivvv.top

[B13] 判断是否为数字
来源：http://ira.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://nyg.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://lhr.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zgg.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dge.shzxlz.cn

Java: x instanceof Number
来源：http://akf.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fdm.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://llc.bbcook.cn

C#:   x is int or double or decimal
来源：http://vcp.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://rhu.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yya.bbcook.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sfg.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://rlp.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://ewz.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pxa.dianchejie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cdx.yanxiufei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bwb.sjlbkw.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bzm.shuidangran.top

[B15] 布尔运算与取反
来源：http://swk.ivvv.top

Py:   a and b or not c
来源：http://qjy.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://sdw.uphjek.com

JS:   a && b || !c
来源：http://hzu.havefunace.top

TS:   a && b || !c
来源：http://ies.52xcode.cn

Java: a && b || !c
来源：http://sen.jinqigufen.top

Go:   a && b || !c
来源：http://nbw.daria6918.cn

Ruby: a && b || !c
来源：http://mqg.hnxiangtu.top

C#:   a && b || !c
来源：http://vxq.pengpengdd.cyou

[B16] 卫语句：不满足条件提前返回
来源：http://ooq.yuanzhike.top

Py:   if not data: return
来源：http://xvl.wangdashe.top

PHP:  if (!$data) { return; }
来源：http://dpi.zhoulong.xyz

JS:   if (!data) return;
来源：http://qws.nanxuanxn.top

TS:   if (!data) return;
来源：http://tbw.52xcode.cn

Java: if (data == null) return;
来源：http://ybg.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://mki.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://zgv.jqgfzy.top

C#:   if (data == null) return;
来源：http://jnb.ywan-chungtsiang.top

================================================================================
来源：http://puu.cqqwz.cn

C. 函数与作用域
来源：http://vgd.zhiwuduotai.top

================================================================================
来源：http://sur.hnxiangtu.top

[C01] 定义函数
来源：http://sxb.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://qmj.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uvm.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://cce.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yop.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zjo.zhixingplan.top

Go:   func add(a, b int) int { return a + b }
来源：http://zyk.iojbl.cn

Ruby: def add(a, b); a + b; end
来源：http://eka.feifeiyinyue.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yoy.vqdsnc.cn

[C02] 默认参数
来源：http://xly.zhixingplan.top

Py:   def greet(name="World"): return name
来源：http://wrn.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://mvq.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://pkk.vqdsnc.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ysr.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zuf.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jtl.zhongyouzk.top

Ruby: def greet(name = "World") = name
来源：http://qqx.guannengcc.top

C#:   string Greet(string name = "World") => name;
来源：http://qfh.xuanzx.com

[C03] 可变参数
来源：http://bwz.xylfe.cn

Py:   def total(*args): return sum(args)
来源：http://sbh.zdbjq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fub.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wpi.wangdashe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wvd.sjlbkw.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vap.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dpm.tianlin.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://lqb.hammf.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://myt.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://ovt.cheryme.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fes.yj20258888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oeh.bjfxy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uzp.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://huc.snrcjt.cn

Java: // 无：用 Builder 模式或 record
来源：http://oqz.yj20258888.top

Go:   // 无：用配置结构体参数
来源：http://cal.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://oqa.jianghu66.top

C#:   f(a: 1, b: 2)
来源：http://lbb.havefunace.top

[C05] 返回多个值
来源：http://dgq.mhx1999.top

Py:   return a, b
来源：http://zft.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://ciy.sxryk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yqp.xinyue.icu

TS:   return { a, b };
来源：http://rai.ppjwa.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fno.shuidangran.top

Go:   return a, b
来源：http://wva.fengsongda.top

Ruby: return a, b
来源：http://uub.dashuyun.cn

C#:   return (a, b);              // ValueTuple
来源：http://clg.zycfv.cn

[C06] 匿名函数 / lambda
来源：http://usd.gzhubu.top

Py:   square = lambda x: x * x
来源：http://tgv.uphjek.com

PHP:  $square = fn($x) => $x * $x;
来源：http://pej.jinghuilouyu.cn

JS:   const square = x => x * x;
来源：http://aur.ydjk.org.cn

TS:   const square = (x: number): number => x * x;
来源：http://kqb.xylfe.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ymw.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cme.aibaodan.cn

Ruby: square = ->(x) { x * x }
来源：http://exs.zhongyouzk.top

C#:   Func<int, int> square = x => x * x;
来源：http://yix.yfazqb.com

[C07] 把函数作为参数传入
来源：http://zhd.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ogg.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xwv.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bzc.fengsongda.top

TS:   arr.map(String)
来源：http://unk.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jsp.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cjb.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://tza.chenzaomai.com

C#:   arr.Select(s => s.ToUpper())
来源：http://exf.andypj.xyz

[C08] 闭包
来源：http://vgb.havefunace.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dov.nanxuanxn.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cjj.shuidangran.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://efz.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gyq.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tzf.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://krn.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uzg.ywan-chungtsiang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://snd.yfazqb.com

[C09] 递归
来源：http://kmz.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sds.ybcxt.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bbt.jyoumei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fha.pycfn.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vjp.iojbl.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jqq.quarkkingdee.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tdt.cheryme.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jix.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://edv.fehbvm.com

[C10] 变量作用域
来源：http://ecb.ydjk.org.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wvs.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qvs.shuidangran.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://apg.nanxinkj.top

TS:   同 JS
来源：http://woe.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://hdf.cucudq.cn

Go:   花括号块级作用域
来源：http://dac.yj20258888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ipu.daxiang520.top

C#:   块级作用域
来源：http://mfm.fktsv.cn

[C11] 模块导入与导出
来源：http://lym.hongshengwenyu.top

Py:   from module import func
来源：http://nxl.yvedp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gor.jyoumei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pdw.316326.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ibx.xuanzx.com

Java: import java.util.List;
来源：http://bdo.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yza.jiagoushi.top

Ruby: require "json"; require_relative "./util"
来源：http://ebr.smart0.xyz

C#:   using System.Text;
来源：http://iof.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://olg.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://zqr.mhx1999.top

PHP:  (function () { echo "run"; })();
来源：http://ykz.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://wxf.daxiang520.top

TS:   (() => { console.log("run"); })();
来源：http://vie.52xcode.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gui.chenlongwang.top

Go:   func() { fmt.Println("run") }()
来源：http://wqq.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://dln.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://bxa.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://xpg.svipenyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iys.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sfu.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cxn.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cft.andypj.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://vbu.sysykeji.top

Go:   func add(a, b int) int
来源：http://mgq.zhixingplan.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vbu.316326.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://ula.hywenlv.cn

[C14] 泛型函数
来源：http://aog.ctjpmb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wld.9152youxi.cn

PHP:  // 无泛型
来源：http://xez.meibo888.top

JS:   // 无泛型
来源：http://unp.fzhhl.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qsq.ivvv.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ksj.xinyue.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qej.hongshengwenyu.top

Ruby: # 无泛型
来源：http://ejc.9152youxi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gxm.havefunace.top

[C15] 解构 / 展开参数
来源：http://cze.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xke.tian-w.cn

PHP:  [$a, $b] = $pair;
来源：http://amk.tianlin.xyz


<!-- 参考信息 -->