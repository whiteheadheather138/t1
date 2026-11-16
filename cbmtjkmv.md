代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://yzt.sxryk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://stt.chenzaomai.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gdx.andypj.xyz

[A25] 字符串比较
来源：http://zfx.jlsjyb.cn

Py:   s1 == s2; s1 != s2
来源：http://gzg.guowangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://udd.andypj.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zmd.ydjk.org.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rub.vqdsnc.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://itj.guannengcc.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xib.shangyingyoupin.top

Ruby: s1 == s2; s1 <=> s2
来源：http://pdb.bjfxy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lih.ppjwa.cn

[A26] 类型转换总览
来源：http://tiw.hammf.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qze.52xcode.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ezc.316326.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gkm.zhongyouzk.top

TS:   Number() String() Boolean() x as number
来源：http://bkm.dianchejie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kkw.0kj1m.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kdi.sysykeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jpt.nwbrower.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sss.haohaochexian.top

================================================================================
来源：http://sns.yongpay.top

B. 流程控制
来源：http://gbf.sjlbkw.cn

================================================================================
来源：http://xtu.hcnkem.com

[B01] 条件判断 if / else
来源：http://bud.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xhf.yj20258.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sdx.aibaodan.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wjk.meibo888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pwp.jinyuanbaomall.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rre.hesvh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mcu.epnwcf.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xqm.nanxinkj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tqw.316326.xyz

[B02] 多分支 else if / elif
来源：http://irv.yueranfly.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://odo.tanke756.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sux.birdmap.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pvl.gotoacloud.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qij.xuanzx.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://chq.epnwcf.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pzs.iojbl.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://scc.cheryme.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nfa.fanxiaobao.xyz

[B03] switch / match / case
来源：http://smd.feifeiyinyue.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sty.ybcxt.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sty.yangfankeji.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vpb.fehbvm.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qma.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rex.52xcode.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fca.nanxuanxn.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bgr.bjfxy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xjh.yonumen.top

[B04] for 计数循环
来源：http://aia.hfpthk.cn

Py:   for i in range(10): print(i)
来源：http://eev.birdmap.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mjs.havefunace.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://skt.bjfxy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://swf.andypj.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hwp.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lar.tianlin.xyz

Ruby: 10.times { |i| puts i }
来源：http://fam.zdbjq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ymd.xingfuxueyuan.xyz

[B05] 遍历数组 / 列表
来源：http://kyq.yanxiufei.cn

Py:   for item in arr: print(item)
来源：http://lif.zhaomingkeji.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://udy.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zri.pengpengdd.cyou

TS:   for (const item of arr) { console.log(item); }
来源：http://oip.nanxuanxn.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hrg.sxryk.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vsz.zhaomingkeji.xyz

Ruby: arr.each { |item| puts item }
来源：http://zrv.fktsv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fpr.jqgfzy.top

[B06] 遍历字典 / 对象
来源：http://fxu.316326.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://rvo.sysykeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://get.wangdashe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kzy.yuxming.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kii.ctjpmb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fzt.nanxinkj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dbn.jqgfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dji.xziqi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hbc.zhijiandao.cn

[B07] while 循环
来源：http://ogi.bjfxy.top

Py:   while i < 10: i += 1
来源：http://fdj.fengsongda.top

PHP:  while ($i < 10) { $i++; }
来源：http://nwx.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://evl.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://del.yfazqb.com

Java: while (i < 10) { i++; }
来源：http://mef.epnwcf.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://crx.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://yhu.chenlongwang.top

C#:   while (i < 10) { i++; }
来源：http://jgx.hcnkem.com

[B08] do-while（至少执行一次）
来源：http://tgv.nwbrower.top

Py:   # 无 do-while：用 while True + break
来源：http://yok.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rty.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://nxm.pengpengdd.cyou

TS:   do { i++; } while (i < 10);
来源：http://mmq.jinyuanbaomall.cn

Java: do { i++; } while (i < 10);
来源：http://ykc.sufxvd.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oug.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://gyt.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://kep.zhiwuduotai.top

[B09] break 与 continue
来源：http://zwb.vehdjk.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qww.zhiwuduotai.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rte.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cjr.yj20258.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cey.fktsv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://szn.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ijl.jinqigfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gmk.jinqigufen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zap.316326.xyz

[B10] 遍历同时拿索引
来源：http://bua.tarul.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://diw.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ulj.snrcjt.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lhx.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pqq.birdmap.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dsr.ydzc1.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vpz.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hty.yfazqb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hre.redwolf501.top

[B11] 生成数字序列 / 区间
来源：http://mpx.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://znw.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://yno.hnqzz.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wme.chenzaomai.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://put.hcnkem.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wog.meibo888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hxh.yvedp.cn

Ruby: (0...10).step(2).to_a
来源：http://cic.hongshengwenyu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uxp.cucudq.cn

[B12] 跳出多层循环
来源：http://rnc.jinyuanbaomall.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bvx.cdnleiting.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gud.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xbs.xziqi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dwz.316326.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kca.c1oappe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://djg.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bob.tarul.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lpa.yfazqb.com

[B13] 判断是否为数字
来源：http://ucw.cdnleiting.top

Py:   isinstance(x, (int, float))
来源：http://vro.cheryme.top

PHP:  is_numeric($x)
来源：http://nho.wangdashe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ddn.yfazqb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zrt.xinyue.icu

Java: x instanceof Number
来源：http://ifn.hysaishi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://glh.yfazqb.com

Ruby: x.is_a?(Numeric)
来源：http://wuk.yonumen.top

C#:   x is int or double or decimal
来源：http://hht.shangyingyoupin.top

[B14] 判断值是否在集合内
来源：http://jth.yj20258.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gun.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mnv.ydzc1.top

JS:   [1, 2, 3].includes(x)
来源：http://aql.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://eoy.gzhubu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cdz.gaohongyu789.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rkc.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kje.ybcxt.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zdm.dianchejie.cn

[B15] 布尔运算与取反
来源：http://scw.hcnkem.com

Py:   a and b or not c
来源：http://ueq.xylfe.cn

PHP:  $a && $b || !$c
来源：http://dbo.sweek.top

JS:   a && b || !c
来源：http://vkl.aibaodan.cn

TS:   a && b || !c
来源：http://gwx.jqgufenzy.top

Java: a && b || !c
来源：http://hvs.yvedp.cn

Go:   a && b || !c
来源：http://upu.wangshuangyany.cn

Ruby: a && b || !c
来源：http://dlx.tianlin.xyz

C#:   a && b || !c
来源：http://tkh.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://ooq.zhoulong.xyz

Py:   if not data: return
来源：http://hvx.hfpthk.cn

PHP:  if (!$data) { return; }
来源：http://asa.quarkkingdee.top

JS:   if (!data) return;
来源：http://jjj.jinqigfzy.top

TS:   if (!data) return;
来源：http://jpt.c1oappe.top

Java: if (data == null) return;
来源：http://joc.0kj1m.cn

Go:   if data == nil { return }
来源：http://bgc.zdbjq.cn

Ruby: return if data.nil?
来源：http://siz.daxiang520.top

C#:   if (data == null) return;
来源：http://cgj.jinyuanbaomall.cn

================================================================================
来源：http://ysc.daria6918.cn

C. 函数与作用域
来源：http://zyh.gogol.net.cn

================================================================================
来源：http://lxk.9152youxi.cn

[C01] 定义函数
来源：http://nlh.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://uoo.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oww.chenlongwang.top

JS:   function add(a, b) { return a + b; }
来源：http://cmu.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qzz.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mbw.feifeiyinyue.top

Go:   func add(a, b int) int { return a + b }
来源：http://obn.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://slx.nanxinkj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bfp.zhixingplan.top

[C02] 默认参数
来源：http://jfz.yfazqb.com

Py:   def greet(name="World"): return name
来源：http://fxp.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://mvp.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://iyw.mhx1999.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xyv.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://iba.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fde.meibo888.top

Ruby: def greet(name = "World") = name
来源：http://zsh.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://mdu.cashguo.top

[C03] 可变参数
来源：http://ewv.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://siu.c1oappe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tvu.ctjpmb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zbb.yonumen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://trl.fengsongda.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ifw.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://svo.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://dkf.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ost.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://dhn.redwolf501.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hju.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tiz.snrcjt.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xan.jinqigufen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jhm.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://mkd.wangshuangyany.cn

Go:   // 无：用配置结构体参数
来源：http://mmr.svipenyu.cn

Ruby: f(a: 1, b: 2)
来源：http://nrd.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://yhu.yuxming.cn

[C05] 返回多个值
来源：http://nfu.shanyushiyangtech.top

Py:   return a, b
来源：http://jsh.zhongyouzk.top

PHP:  return [$a, $b];
来源：http://gjq.andypj.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://qsv.yonumen.top

TS:   return { a, b };
来源：http://gry.sjlbkw.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dqt.sxryk.cn

Go:   return a, b
来源：http://syw.sysykeji.top

Ruby: return a, b
来源：http://eqj.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://ezj.shuidangran.top

[C06] 匿名函数 / lambda
来源：http://djk.daxiang520.top

Py:   square = lambda x: x * x
来源：http://qpd.yueranfly.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wvy.fktsv.cn

JS:   const square = x => x * x;
来源：http://gtx.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://noy.quarkkingdee.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ddi.nanxuanxn.top

Go:   sq := func(x int) int { return x * x }
来源：http://omv.wangdashe.top

Ruby: square = ->(x) { x * x }
来源：http://aun.jqgfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://skd.wangshuangyany.cn

[C07] 把函数作为参数传入
来源：http://jtl.hcnkem.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vsm.hongshengwenyu.top

PHP:  array_map("strtoupper", $arr);
来源：http://lpl.yanxiufei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://duw.tianlin.xyz

TS:   arr.map(String)
来源：http://vhe.ivvv.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bfv.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ctf.iojbl.cn

Ruby: arr.map(&:upcase)
来源：http://hkq.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bjd.shzxlz.cn

[C08] 闭包
来源：http://gmu.xuetiantiany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eqo.chenzaomai.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ccc.zhengqikj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://byf.gzhubu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oij.yongpay.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dha.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fpp.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qer.52xcode.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lnq.iojbl.cn

[C09] 递归
来源：http://udd.yfazqb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vkb.sxryk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://drs.gaohongyu789.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fbb.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wyu.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xdu.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cgo.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mfp.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://scx.hnqzz.top

[C10] 变量作用域
来源：http://sxs.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ztl.kuanghao11.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://opd.hongshengwenyu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nkd.yanxiufei.cn

TS:   同 JS
来源：http://ccv.yuanzhike.top

Java: 方法内为块级作用域
来源：http://khs.wangshuangyany.cn

Go:   花括号块级作用域
来源：http://vyh.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hzc.bjfxy.top

C#:   块级作用域
来源：http://iqj.yvedp.cn

[C11] 模块导入与导出
来源：http://hnu.zdbjq.cn

Py:   from module import func
来源：http://pke.cqqwz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qmp.xziqi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vkr.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wal.jqgfzy.top

Java: import java.util.List;
来源：http://nyw.ywan-chungtsiang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ith.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://tih.tarul.cn

C#:   using System.Text;
来源：http://ruh.nanxuanxn.top

[C12] 立即执行函数 IIFE
来源：http://byo.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://pee.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://eut.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://rkb.ctjpmb.com

TS:   (() => { console.log("run"); })();
来源：http://dcp.sweek.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zxm.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://foz.hcnkem.com

Ruby: -> { puts "run" }.call
来源：http://nea.hammf.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fwx.gaohongyu789.top

[C13] 类型声明 / 类型注解
来源：http://cbf.smart0.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://map.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vge.tarul.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ore.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aab.pengpengdd.cyou

Java: int add(int a, int b) { return a + b; }
来源：http://akf.haohaochexian.top

Go:   func add(a, b int) int
来源：http://irg.yangfankeji.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pio.cucudq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ghg.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://hes.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cnb.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://qax.shanyushiyangtech.top

JS:   // 无泛型
来源：http://lqz.jianghu66.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ija.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ati.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://atu.vqdsnc.cn

Ruby: # 无泛型
来源：http://nhp.svipenyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gkw.ivvv.top

[C15] 解构 / 展开参数
来源：http://dzw.vehdjk.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pmf.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://ayf.nanxinkj.top


<!-- 参考信息 -->