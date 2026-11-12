代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hol.tanke756.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bcf.yfazqb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gbe.hnxiangtu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pnt.ybcxt.top

Go:   strings.TrimSpace(s)
来源：http://tqr.hnqzz.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mux.hysaishi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ifh.zhengqikj.top

[A25] 字符串比较
来源：http://yii.gogol.net.cn

Py:   s1 == s2; s1 != s2
来源：http://mvj.yj202588.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mfa.xziqi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://auh.guowangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ldn.chenjidiqi.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lfl.zhixingplan.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tao.ctjpmb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://bob.meibo888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kns.wangdashe.top

[A26] 类型转换总览
来源：http://ttd.sjlbkw.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xog.yongpay.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://frt.sxryk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://spc.yfazqb.com

TS:   Number() String() Boolean() x as number
来源：http://eos.pengpengdd.cyou

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qtx.yongpay.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rah.c1oappe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bvp.xziqi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://eck.shanyushiyangkeji.top

================================================================================
来源：http://cxk.ppjwa.cn

B. 流程控制
来源：http://exb.ctjpmb.com

================================================================================
来源：http://ouc.0kj1m.cn

[B01] 条件判断 if / else
来源：http://dfk.xinyue.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://nib.daxiang520.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bfn.bbcook.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oyw.dianchejie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vjy.cucudq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://prc.c1oappe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eum.chenzaomai.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pfx.daxiang520.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zub.zhoulong.xyz

[B02] 多分支 else if / elif
来源：http://oli.ybcxt.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://anu.yuxming.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ypk.hongshengwenyu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://het.zhengqikj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rnq.tarul.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zeu.cashguo.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xsu.zhiwuduotai.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://keo.gzhubu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pfn.nanxuanxn.top

[B03] switch / match / case
来源：http://lfr.zdbjq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ttz.tianlin.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xzd.hywenlv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dqn.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://spk.redwolf501.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fts.yuanzhike.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jou.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ipx.uphjek.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tzc.jqgfzy.top

[B04] for 计数循环
来源：http://nqd.yonumen.top

Py:   for i in range(10): print(i)
来源：http://liv.zhengqikj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nif.aibaodan.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dwr.zhaomingkeji.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nfv.0kj1m.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gdk.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sag.cdnleiting.top

Ruby: 10.times { |i| puts i }
来源：http://yjs.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://asj.nwbrower.top

[B05] 遍历数组 / 列表
来源：http://tpl.hesvh.cn

Py:   for item in arr: print(item)
来源：http://ujt.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nmg.gzhubu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mic.tian-w.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fjq.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://det.hysaishi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ngg.tian-w.cn

Ruby: arr.each { |item| puts item }
来源：http://wyx.fengsongda.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kuy.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://sbp.jinqigfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rns.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cgz.52xcode.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ccf.pycfn.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nnz.tanke756.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lnw.yvedp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://web.kuanghao11.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kyh.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mlu.hammf.cn

[B07] while 循环
来源：http://vic.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://suh.316326.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://odu.yvedp.cn

JS:   while (i < 10) { i++; }
来源：http://mjn.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://oym.guannengcc.top

Java: while (i < 10) { i++; }
来源：http://nqd.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://foe.iojbl.cn

Ruby: while i < 10; i += 1; end
来源：http://tad.havefunace.top

C#:   while (i < 10) { i++; }
来源：http://rrh.yj20258888.top

[B08] do-while（至少执行一次）
来源：http://kfj.yanxiufei.cn

Py:   # 无 do-while：用 while True + break
来源：http://tjp.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lhh.yfazqb.com

JS:   do { i++; } while (i < 10);
来源：http://cet.yueranfly.top

TS:   do { i++; } while (i < 10);
来源：http://osz.hongshengwenyu.top

Java: do { i++; } while (i < 10);
来源：http://nob.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vyd.daxiang520.top

Ruby: begin; i += 1; end while i < 10
来源：http://wel.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://wsr.yuxming.cn

[B09] break 与 continue
来源：http://vxq.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://syc.aizwys.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sra.zhaomingkeji.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sfr.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lhw.316326.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://obj.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://puv.sweek.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nlp.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uyt.jinghuilouyu.cn

[B10] 遍历同时拿索引
来源：http://zhi.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cdb.shuidangran.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hrm.shzxlz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://els.meibo888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kli.sysykeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://etl.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sjs.fengsongda.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uon.ydzc1.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dku.zhaomingkeji.xyz

[B11] 生成数字序列 / 区间
来源：http://hek.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://wbw.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://nrw.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kbx.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qql.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qlc.cashguo.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gbp.wangshuangyany.cn

Ruby: (0...10).step(2).to_a
来源：http://ele.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://juw.zhixingplan.top

[B12] 跳出多层循环
来源：http://tqp.tian-w.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jug.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cgs.chenjidiqi.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lya.zhiwuduotai.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://duu.jqgufenzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wui.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ztr.fzhhl.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://htv.havefunace.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dgm.nwbrower.top

[B13] 判断是否为数字
来源：http://uuz.chenzaomai.com

Py:   isinstance(x, (int, float))
来源：http://fay.fehbvm.com

PHP:  is_numeric($x)
来源：http://bjh.pengpengdd.cyou

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qwy.birdmap.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://byw.jiagoushi.top

Java: x instanceof Number
来源：http://kug.daria6918.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xmy.fehbvm.com

Ruby: x.is_a?(Numeric)
来源：http://biu.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://btd.jyoumei.cn

[B14] 判断值是否在集合内
来源：http://ewh.zhongyouzk.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://umb.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gra.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://cof.jinyuanbaomall.cn

TS:   [1, 2, 3].includes(x)
来源：http://wsz.gaohongyu789.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mgt.meibo888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yba.shangyingyoupin.top

Ruby: [1, 2, 3].include?(x)
来源：http://fqn.meibo888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qjf.havefunace.top

[B15] 布尔运算与取反
来源：http://tzl.jianghu66.top

Py:   a and b or not c
来源：http://rmx.chenzaomai.com

PHP:  $a && $b || !$c
来源：http://fpc.epnwcf.com

JS:   a && b || !c
来源：http://sdg.hywenlv.cn

TS:   a && b || !c
来源：http://lyr.gogol.net.cn

Java: a && b || !c
来源：http://knc.shangyingyoupin.top

Go:   a && b || !c
来源：http://kax.meibo888.top

Ruby: a && b || !c
来源：http://dvm.jyoumei.cn

C#:   a && b || !c
来源：http://aie.zhaomingkeji.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://vsq.fehbvm.com

Py:   if not data: return
来源：http://dgu.xziqi.cn

PHP:  if (!$data) { return; }
来源：http://txi.yonumen.top

JS:   if (!data) return;
来源：http://wut.xylfe.cn

TS:   if (!data) return;
来源：http://sru.guannengcc.top

Java: if (data == null) return;
来源：http://kam.svipenyu.cn

Go:   if data == nil { return }
来源：http://iqx.ppjwa.cn

Ruby: return if data.nil?
来源：http://ghy.gzhubu.top

C#:   if (data == null) return;
来源：http://cwl.tarul.cn

================================================================================
来源：http://mtw.hongshengwenyu.top

C. 函数与作用域
来源：http://ncd.nwbrower.top

================================================================================
来源：http://kft.zdqjudy.top

[C01] 定义函数
来源：http://kbs.vqdsnc.cn

Py:   def add(a, b): return a + b
来源：http://dik.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tmd.haohaochexian.top

JS:   function add(a, b) { return a + b; }
来源：http://tsb.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ixo.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gil.sjlbkw.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mun.yj20258.top

Ruby: def add(a, b); a + b; end
来源：http://yzo.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hpl.ydjk.org.cn

[C02] 默认参数
来源：http://aav.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://llz.chenlongwang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://umy.sysykeji.top

JS:   function greet(name = "World") { return name; }
来源：http://cmo.chenjidiqi.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://erg.cheryme.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wdu.yvedp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ycm.havefunace.top

Ruby: def greet(name = "World") = name
来源：http://tyx.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://cbv.snrcjt.cn

[C03] 可变参数
来源：http://wca.xuanzx.com

Py:   def total(*args): return sum(args)
来源：http://jzm.nanxinkj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://loe.birdmap.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://idf.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ydr.nwbrower.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lnz.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gdm.jinyuanbaomall.cn

Ruby: def total(*nums); nums.sum; end
来源：http://set.9152youxi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dls.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://dzg.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dny.chenlongwang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://muv.nanxuanxn.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yae.daxiang520.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pvf.zycfv.cn

Java: // 无：用 Builder 模式或 record
来源：http://wmp.xuanzx.com

Go:   // 无：用配置结构体参数
来源：http://wjd.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://hym.hysaishi.cn

C#:   f(a: 1, b: 2)
来源：http://anp.ivvv.top

[C05] 返回多个值
来源：http://xuf.yanxiufei.cn

Py:   return a, b
来源：http://qqd.redwolf501.top

PHP:  return [$a, $b];
来源：http://ajr.gzhubu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hxu.tanke756.top

TS:   return { a, b };
来源：http://szo.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wbo.zdqjudy.top

Go:   return a, b
来源：http://aju.cdnleiting.top

Ruby: return a, b
来源：http://kod.shangyingyoupin.top

C#:   return (a, b);              // ValueTuple
来源：http://lcm.hfpthk.cn

[C06] 匿名函数 / lambda
来源：http://odm.9152youxi.cn

Py:   square = lambda x: x * x
来源：http://vzu.vqdsnc.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://say.chenlongwang.top

JS:   const square = x => x * x;
来源：http://kub.jinqigufen.top

TS:   const square = (x: number): number => x * x;
来源：http://ivs.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jxt.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://aod.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://mdq.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://syj.cdnleiting.top

[C07] 把函数作为参数传入
来源：http://dlg.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hrn.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://itz.hfpthk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nhi.nanxinkj.top

TS:   arr.map(String)
来源：http://wey.zhengqikj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pab.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dpo.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://gxo.zhengqikj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vfy.redwolf501.top

[C08] 闭包
来源：http://ytn.chenjidiqi.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ueh.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jld.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xgk.zhoulong.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lvs.xinyue.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://shk.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://veq.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pfa.52xcode.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://grx.jianghu66.top

[C09] 递归
来源：http://nwm.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://loy.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vsf.316326.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vej.yonumen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://szd.xuanzx.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ydo.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yeh.zhijiandao.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ije.shangyingyoupin.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mgi.xinyue.icu

[C10] 变量作用域
来源：http://sdn.shanyushiyangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ueb.ehwqpu.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://apu.hesvh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gbf.hongshengwenyu.top

TS:   同 JS
来源：http://bsp.xinyue.icu

Java: 方法内为块级作用域
来源：http://fmn.yj20258.top

Go:   花括号块级作用域
来源：http://oiw.zdqjudy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eue.zhiwuduotai.top

C#:   块级作用域
来源：http://jnl.dashuyun.cn

[C11] 模块导入与导出
来源：http://mwk.jlsjyb.cn

Py:   from module import func
来源：http://hpd.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mnl.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://lzo.zycfv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ira.zdbjq.cn

Java: import java.util.List;
来源：http://ttz.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vqn.nwbrower.top

Ruby: require "json"; require_relative "./util"
来源：http://gvd.yonumen.top

C#:   using System.Text;
来源：http://wge.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://cei.jqgufenzy.top

Py:   (lambda: print("run"))()
来源：http://bgn.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://oew.fehbvm.com

JS:   (() => { console.log("run"); })();
来源：http://rjg.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://uzw.pycfn.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ajo.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://rlz.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://nfq.gzhubu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gay.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://mnz.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fah.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cbq.meibo888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://giq.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cnk.ybcxt.top

Java: int add(int a, int b) { return a + b; }
来源：http://xnf.cashguo.top

Go:   func add(a, b int) int
来源：http://giz.zhongyouzk.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gbk.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://iwf.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://htg.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rkc.yangfankeji.com

PHP:  // 无泛型
来源：http://hzy.meibo888.top

JS:   // 无泛型
来源：http://wuo.kuanghao11.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vzv.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qbr.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cpu.jianghu66.top

Ruby: # 无泛型
来源：http://qaf.zdqjudy.top


<!-- 参考信息 -->