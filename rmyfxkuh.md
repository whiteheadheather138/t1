代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://ofe.xylfe.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xvr.yuanzhike.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dxg.zhongyouzk.top

[A25] 字符串比较
来源：http://cut.pengpengdd.cyou

Py:   s1 == s2; s1 != s2
来源：http://twa.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gak.wangdashe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uvx.hammf.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://own.zhijiandao.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cvb.zhiwuduotai.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lyy.jinyuanbaomall.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bbn.snrcjt.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ppy.dianchejie.cn

[A26] 类型转换总览
来源：http://mvm.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xfz.zdqjudy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dxl.zhaomingkeji.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aok.hnqzz.top

TS:   Number() String() Boolean() x as number
来源：http://vja.shzxlz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://syl.guannengcc.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gro.pycfn.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://sqa.fengsongda.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kfq.yueranfly.top

================================================================================
来源：http://ncf.ppjwa.cn

B. 流程控制
来源：http://hfe.hesvh.cn

================================================================================
来源：http://han.zdqjudy.top

[B01] 条件判断 if / else
来源：http://dtn.cucudq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vbu.fzhhl.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://orq.cashguo.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rju.yueranfly.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ljn.shanyushiyangtech.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yet.snrcjt.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://suj.ehwqpu.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ihr.aizwys.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gfc.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://liw.meibo888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gcy.gzhubu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://znk.vqdsnc.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vwr.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hqr.dianchejie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kly.fehbvm.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vlf.52xcode.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pil.fktsv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lgd.52xcode.cn

[B03] switch / match / case
来源：http://pbo.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xcy.yj202588.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kfc.iojbl.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tic.chenlongwang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pgs.shuidangran.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://htw.gzhubu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kon.xingfuxueyuan.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ifg.zycfv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://upa.nwbrower.top

[B04] for 计数循环
来源：http://hyv.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://fdh.sweek.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://swh.shangyingyoupin.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ogk.cqqwz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sff.shzxlz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rwo.zhengqikj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://usi.cqqwz.cn

Ruby: 10.times { |i| puts i }
来源：http://tag.fengsongda.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://syv.9152youxi.cn

[B05] 遍历数组 / 列表
来源：http://jsx.daria6918.cn

Py:   for item in arr: print(item)
来源：http://kie.jinghuilouyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mkw.gogol.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jrd.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://axi.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bnr.chenlongwang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://azy.yanxiufei.cn

Ruby: arr.each { |item| puts item }
来源：http://shm.guannengcc.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lat.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://ebx.guowangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://psd.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hep.hammf.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ozq.aizwys.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://igi.nwbrower.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gxr.ehwqpu.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://czg.jyoumei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://msk.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ppt.xingfuxueyuan.xyz

[B07] while 循环
来源：http://scy.jinyuanbaomall.cn

Py:   while i < 10: i += 1
来源：http://rfo.redwolf501.top

PHP:  while ($i < 10) { $i++; }
来源：http://nmp.redwolf501.top

JS:   while (i < 10) { i++; }
来源：http://whv.iojbl.cn

TS:   while (i < 10) { i++; }
来源：http://vch.gaohongyu789.top

Java: while (i < 10) { i++; }
来源：http://wlc.cdnleiting.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bdp.guannengcc.top

Ruby: while i < 10; i += 1; end
来源：http://wmi.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://uya.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://hzm.0kj1m.cn

Py:   # 无 do-while：用 while True + break
来源：http://hze.andypj.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://duf.zdqjudy.top

JS:   do { i++; } while (i < 10);
来源：http://wcn.havefunace.top

TS:   do { i++; } while (i < 10);
来源：http://uxd.gaohongyu789.top

Java: do { i++; } while (i < 10);
来源：http://psz.yuanzhike.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tft.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://clz.xinyue.icu

C#:   do { i++; } while (i < 10);
来源：http://qdf.daxiang520.top

[B09] break 与 continue
来源：http://ooc.bjfxy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lzf.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://svt.hongshengwenyu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uox.guowangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://umq.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rsd.cheryme.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lhh.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eul.hnqzz.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oih.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://fqn.xuetiantiany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oqx.kuanghao11.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hhu.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mef.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://thv.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ywa.xziqi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vyd.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zts.c1oappe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mjd.fktsv.cn

[B11] 生成数字序列 / 区间
来源：http://auk.wangshuangyany.cn

Py:   list(range(0, 10, 2))
来源：http://gda.quarkkingdee.top

PHP:  range(0, 10, 2);
来源：http://rfp.ydjk.org.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jgn.epnwcf.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://flj.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://utz.guowangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qnz.yfazqb.com

Ruby: (0...10).step(2).to_a
来源：http://emj.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rlo.zycfv.cn

[B12] 跳出多层循环
来源：http://bsa.aibaodan.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://esi.yj20258888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wcf.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://grf.bbcook.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://awk.jinqigfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gyr.xuanzx.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zms.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tri.c1oappe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uls.guannengcc.top

[B13] 判断是否为数字
来源：http://dpl.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://hwf.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://ndb.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://env.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qfe.zhaomingkeji.xyz

Java: x instanceof Number
来源：http://qio.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gax.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://fom.dashuyun.cn

C#:   x is int or double or decimal
来源：http://rbl.kuanghao11.cn

[B14] 判断值是否在集合内
来源：http://rsp.cqqwz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yoq.guannengcc.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vlt.yj20258888.top

JS:   [1, 2, 3].includes(x)
来源：http://oef.hcnkem.com

TS:   [1, 2, 3].includes(x)
来源：http://dpe.sysykeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://aar.hongshengwenyu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nuw.smart0.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://vtt.jyoumei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wdh.hysaishi.cn

[B15] 布尔运算与取反
来源：http://uav.pycfn.com

Py:   a and b or not c
来源：http://lcf.jianghu66.top

PHP:  $a && $b || !$c
来源：http://gsj.shanyushiyangkeji.top

JS:   a && b || !c
来源：http://uxy.aizwys.cn

TS:   a && b || !c
来源：http://gip.xuanzx.com

Java: a && b || !c
来源：http://auk.yuxming.cn

Go:   a && b || !c
来源：http://uhy.yj20258888.top

Ruby: a && b || !c
来源：http://fvz.epnwcf.com

C#:   a && b || !c
来源：http://maa.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://kuf.sufxvd.cn

Py:   if not data: return
来源：http://kaz.cashguo.top

PHP:  if (!$data) { return; }
来源：http://cfh.daxiang520.top

JS:   if (!data) return;
来源：http://ngm.hysaishi.cn

TS:   if (!data) return;
来源：http://gek.yanxiufei.cn

Java: if (data == null) return;
来源：http://fcf.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://hqm.haohaochexian.top

Ruby: return if data.nil?
来源：http://jpq.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://ioi.316326.xyz

================================================================================
来源：http://jlu.hnxiangtu.top

C. 函数与作用域
来源：http://nzo.xingfuxueyuan.xyz

================================================================================
来源：http://dyq.ydjk.org.cn

[C01] 定义函数
来源：http://zet.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://iro.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pkk.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://qmm.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yds.yuanzhike.top

Java: static int add(int a, int b) { return a + b; }
来源：http://iqj.hongshengwenyu.top

Go:   func add(a, b int) int { return a + b }
来源：http://wst.yongpay.top

Ruby: def add(a, b); a + b; end
来源：http://klp.jinyuanbaomall.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dfj.gaohongyu789.top

[C02] 默认参数
来源：http://ket.nwbrower.top

Py:   def greet(name="World"): return name
来源：http://rtm.zdqjudy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://loa.ppjwa.cn

JS:   function greet(name = "World") { return name; }
来源：http://qbd.bbcook.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jdr.hesvh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bkg.fehbvm.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hsk.jlsjyb.cn

Ruby: def greet(name = "World") = name
来源：http://tve.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://mvz.hesvh.cn

[C03] 可变参数
来源：http://wbg.ppjwa.cn

Py:   def total(*args): return sum(args)
来源：http://hvt.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rpv.hnqzz.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cmb.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hns.jinqigufen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vjs.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kae.yuxming.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nma.yangfankeji.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dqs.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://arm.tanke756.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iak.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ded.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nud.gotoacloud.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wpk.yanxiufei.cn

Java: // 无：用 Builder 模式或 record
来源：http://fun.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://tqb.chenlongwang.top

Ruby: f(a: 1, b: 2)
来源：http://cal.hammf.cn

C#:   f(a: 1, b: 2)
来源：http://dqf.sufxvd.cn

[C05] 返回多个值
来源：http://iso.hfpthk.cn

Py:   return a, b
来源：http://ull.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://xxr.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gxv.shzxlz.cn

TS:   return { a, b };
来源：http://aun.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gyg.tian-w.cn

Go:   return a, b
来源：http://hmc.jinyuanbaomall.cn

Ruby: return a, b
来源：http://tqh.pengpengdd.cyou

C#:   return (a, b);              // ValueTuple
来源：http://gqm.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://mki.fktsv.cn

Py:   square = lambda x: x * x
来源：http://gdf.birdmap.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kzy.yfazqb.com

JS:   const square = x => x * x;
来源：http://ctu.yj20258888.top

TS:   const square = (x: number): number => x * x;
来源：http://fzw.jianghu66.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zse.xuanzx.com

Go:   sq := func(x int) int { return x * x }
来源：http://wfb.fehbvm.com

Ruby: square = ->(x) { x * x }
来源：http://zdd.ivvv.top

C#:   Func<int, int> square = x => x * x;
来源：http://uqt.yuxming.cn

[C07] 把函数作为参数传入
来源：http://qqq.sufxvd.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oir.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ocg.haohaochexian.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jfo.shuidangran.top

TS:   arr.map(String)
来源：http://qau.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zfs.jinghuilouyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gpp.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://kjt.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pdy.cashguo.top

[C08] 闭包
来源：http://hoq.vehdjk.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pgy.havefunace.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vlf.dashuyun.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ptt.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aog.9152youxi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zwk.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cvi.zhoulong.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lml.hywenlv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gxb.chenjidiqi.icu

[C09] 递归
来源：http://tda.ehwqpu.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ige.zdbjq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wes.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gnv.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://npi.nanxuanxn.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xef.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://huc.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bpk.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hht.xuanzx.com

[C10] 变量作用域
来源：http://nwp.pengpengdd.cyou

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pot.ehwqpu.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bli.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dyx.ywan-chungtsiang.top

TS:   同 JS
来源：http://vgs.jinyuanbaomall.cn

Java: 方法内为块级作用域
来源：http://izt.nanxuanxn.top

Go:   花括号块级作用域
来源：http://lua.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://czn.316326.xyz

C#:   块级作用域
来源：http://fts.nanxinkj.top

[C11] 模块导入与导出
来源：http://nvv.aibaodan.cn

Py:   from module import func
来源：http://ovp.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qsw.shangyingyoupin.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zxd.hammf.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hfu.nanxinkj.top

Java: import java.util.List;
来源：http://ext.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kxn.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://pdw.hcnkem.com

C#:   using System.Text;
来源：http://epl.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://cwe.jinyuanbaomall.cn

Py:   (lambda: print("run"))()
来源：http://fok.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://hcg.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://xtz.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://qgv.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cgh.pengpengdd.cyou

Go:   func() { fmt.Println("run") }()
来源：http://pvq.nwbrower.top

Ruby: -> { puts "run" }.call
来源：http://yri.nwbrower.top

C#:   // 无 IIFE：用静态构造函数
来源：http://iuk.cqqwz.cn

[C13] 类型声明 / 类型注解
来源：http://zsd.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bod.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qmd.ywan-chungtsiang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uuj.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gop.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://npl.ydzc1.top

Go:   func add(a, b int) int
来源：http://xib.aizwys.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pzo.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://llv.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://adi.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ruq.bbcook.cn

PHP:  // 无泛型
来源：http://dyj.chenzaomai.com

JS:   // 无泛型
来源：http://zid.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ahw.fktsv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wag.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gvr.xziqi.cn

Ruby: # 无泛型
来源：http://tdg.chenzaomai.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mnn.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://ydt.uphjek.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vai.dashuyun.cn

PHP:  [$a, $b] = $pair;
来源：http://xbs.jinqigfzy.top


<!-- 参考信息 -->