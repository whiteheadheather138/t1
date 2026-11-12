代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bjc.zdqjudy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vvn.jinghuilouyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://awd.yongpay.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mwa.zhaomingkeji.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sid.zhiwuduotai.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ufq.tianlin.xyz

[A24] 去除首尾空白
来源：http://cgw.nanxinkj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gtl.9152youxi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xkd.andypj.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xwk.yuxming.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aqe.svipenyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qjv.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://kth.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fqz.0kj1m.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ujw.guowangkeji.top

[A25] 字符串比较
来源：http://lxk.quarkkingdee.top

Py:   s1 == s2; s1 != s2
来源：http://opt.jyoumei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jgx.hongshengwenyu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://njm.fanxiaobao.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dgh.iojbl.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ulz.xziqi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lbo.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://elg.ctjpmb.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://twn.jinqigfzy.top

[A26] 类型转换总览
来源：http://ydh.jiagoushi.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eux.zdbjq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yfa.jinqigufen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zza.shanyushiyangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://dpq.zdbjq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lhq.zdbjq.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vhz.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://aaq.fktsv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uqp.havefunace.top

================================================================================
来源：http://weu.wangshuangyany.cn

B. 流程控制
来源：http://ifh.havefunace.top

================================================================================
来源：http://hgb.zhengqikj.top

[B01] 条件判断 if / else
来源：http://ugn.hesvh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xfm.hysaishi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qlc.wangdashe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://elb.xingfuxueyuan.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tov.yonumen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yxp.yangfankeji.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nwh.ydjk.org.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oqu.zhongyouzk.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jkj.jiagoushi.top

[B02] 多分支 else if / elif
来源：http://wwh.jinqigfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sst.daria6918.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wix.aizwys.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mjq.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xfu.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vfj.zdbjq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dfp.xylfe.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://skz.0kj1m.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vef.tarul.cn

[B03] switch / match / case
来源：http://zja.sxryk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fns.yongpay.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vuy.gaohongyu789.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nfx.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sae.guannengcc.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kvs.birdmap.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pyr.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dyd.snrcjt.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rqw.yj20258888.top

[B04] for 计数循环
来源：http://zgy.shzxlz.cn

Py:   for i in range(10): print(i)
来源：http://mng.hfpthk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://beg.hnxiangtu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pct.fzhhl.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wzn.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zlr.jinqigufen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://the.tian-w.cn

Ruby: 10.times { |i| puts i }
来源：http://peq.fzhhl.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ibs.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://auo.tanke756.top

Py:   for item in arr: print(item)
来源：http://oju.andypj.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dpf.gaohongyu789.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fff.cashguo.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cul.fanxiaobao.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://ssb.9152youxi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pmx.feifeiyinyue.top

Ruby: arr.each { |item| puts item }
来源：http://xir.ppjwa.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wlw.ydjk.org.cn

[B06] 遍历字典 / 对象
来源：http://djz.nwbrower.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dtm.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rhw.jqgufenzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iga.sufxvd.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bpv.316326.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wxd.smart0.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dml.yj20258888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zth.yanxiufei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://srv.fehbvm.com

[B07] while 循环
来源：http://atx.ctjpmb.com

Py:   while i < 10: i += 1
来源：http://nzy.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kvy.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://ufg.guowangkeji.top

TS:   while (i < 10) { i++; }
来源：http://jud.uphjek.com

Java: while (i < 10) { i++; }
来源：http://tiu.316326.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mkk.redwolf501.top

Ruby: while i < 10; i += 1; end
来源：http://izp.hnqzz.top

C#:   while (i < 10) { i++; }
来源：http://ltr.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://lhc.pycfn.com

Py:   # 无 do-while：用 while True + break
来源：http://qjc.epnwcf.com

PHP:  do { $i++; } while ($i < 10);
来源：http://moz.ehwqpu.com

JS:   do { i++; } while (i < 10);
来源：http://qno.nwbrower.top

TS:   do { i++; } while (i < 10);
来源：http://qwc.fengsongda.top

Java: do { i++; } while (i < 10);
来源：http://xju.shanyushiyangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uyo.daria6918.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xhe.cucudq.cn

C#:   do { i++; } while (i < 10);
来源：http://dfy.fanxiaobao.xyz

[B09] break 与 continue
来源：http://jvw.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gco.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fbl.ppjwa.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ovv.xziqi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://auk.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qkb.aizwys.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yvl.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jau.fanxiaobao.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ima.shanyushiyangtech.top

[B10] 遍历同时拿索引
来源：http://azw.zhengqikj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ztm.fktsv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sbn.hammf.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yig.sweek.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yjd.feifeiyinyue.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://avj.52xcode.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cex.tarul.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ves.shuidangran.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xqh.kuanghao11.cn

[B11] 生成数字序列 / 区间
来源：http://upy.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://oet.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://sac.ybcxt.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uxa.zhoulong.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pdn.ehwqpu.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jmj.zhiwuduotai.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bqn.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://ruc.jqgfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zpm.sysykeji.top

[B12] 跳出多层循环
来源：http://cnv.jqgfzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://unr.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lto.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xiv.shanyushiyangtech.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qwu.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bja.pengpengdd.cyou

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lec.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nvk.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sqp.chenlongwang.top

[B13] 判断是否为数字
来源：http://dkk.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://cje.cdnleiting.top

PHP:  is_numeric($x)
来源：http://ztz.c1oappe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aau.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tes.xuanzx.com

Java: x instanceof Number
来源：http://nff.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cee.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://ihc.epnwcf.com

C#:   x is int or double or decimal
来源：http://nzt.c1oappe.top

[B14] 判断值是否在集合内
来源：http://pvq.tianlin.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rhk.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zhd.hcnkem.com

JS:   [1, 2, 3].includes(x)
来源：http://svj.sysykeji.top

TS:   [1, 2, 3].includes(x)
来源：http://bzh.yfazqb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://zsv.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dpa.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lqz.yj20258888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wnw.hammf.cn

[B15] 布尔运算与取反
来源：http://yte.c1oappe.top

Py:   a and b or not c
来源：http://nke.ehwqpu.com

PHP:  $a && $b || !$c
来源：http://qeh.9152youxi.cn

JS:   a && b || !c
来源：http://kga.chenjidiqi.icu

TS:   a && b || !c
来源：http://adj.hnqzz.top

Java: a && b || !c
来源：http://bry.fanxiaobao.xyz

Go:   a && b || !c
来源：http://dqx.bbcook.cn

Ruby: a && b || !c
来源：http://cdr.nwbrower.top

C#:   a && b || !c
来源：http://qwo.gzhubu.top

[B16] 卫语句：不满足条件提前返回
来源：http://irq.zdqjudy.top

Py:   if not data: return
来源：http://rbj.meibo888.top

PHP:  if (!$data) { return; }
来源：http://dvf.zhijiandao.cn

JS:   if (!data) return;
来源：http://mng.dianchejie.cn

TS:   if (!data) return;
来源：http://lvz.cucudq.cn

Java: if (data == null) return;
来源：http://wgd.tarul.cn

Go:   if data == nil { return }
来源：http://qrr.epnwcf.com

Ruby: return if data.nil?
来源：http://vws.ybcxt.top

C#:   if (data == null) return;
来源：http://oio.hcnkem.com

================================================================================
来源：http://aiq.jianghu66.top

C. 函数与作用域
来源：http://boo.aibaodan.cn

================================================================================
来源：http://orh.zycfv.cn

[C01] 定义函数
来源：http://agx.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://ltj.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://evx.gzhubu.top

JS:   function add(a, b) { return a + b; }
来源：http://mwr.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zme.feifeiyinyue.top

Java: static int add(int a, int b) { return a + b; }
来源：http://naz.yonumen.top

Go:   func add(a, b int) int { return a + b }
来源：http://cuh.havefunace.top

Ruby: def add(a, b); a + b; end
来源：http://hel.nanxuanxn.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xih.jinqigfzy.top

[C02] 默认参数
来源：http://lvi.sxryk.cn

Py:   def greet(name="World"): return name
来源：http://xvx.yueranfly.top

PHP:  function greet($name = "World") { return $name; }
来源：http://swq.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://mdz.epnwcf.com

TS:   function greet(name: string = "World") { return name; }
来源：http://duo.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://avg.chenjidiqi.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rom.havefunace.top

Ruby: def greet(name = "World") = name
来源：http://nkz.yueranfly.top

C#:   string Greet(string name = "World") => name;
来源：http://ddb.sjlbkw.cn

[C03] 可变参数
来源：http://jxb.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://qaq.nanxinkj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jmh.ppjwa.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vml.hnxiangtu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ebg.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gsu.xziqi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mih.jqgfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://mgd.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gje.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://cxn.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gcu.tianlin.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rci.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ool.yongpay.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jcb.uphjek.com

Java: // 无：用 Builder 模式或 record
来源：http://gfh.cqqwz.cn

Go:   // 无：用配置结构体参数
来源：http://awt.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://smz.guannengcc.top

C#:   f(a: 1, b: 2)
来源：http://kre.yongpay.top

[C05] 返回多个值
来源：http://imb.fktsv.cn

Py:   return a, b
来源：http://vqg.aibaodan.cn

PHP:  return [$a, $b];
来源：http://ayh.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://uyz.jinghuilouyu.cn

TS:   return { a, b };
来源：http://icb.chenzaomai.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vlc.hywenlv.cn

Go:   return a, b
来源：http://fdb.hesvh.cn

Ruby: return a, b
来源：http://str.cqqwz.cn

C#:   return (a, b);              // ValueTuple
来源：http://qbx.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://bet.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://owy.andypj.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://olp.zhengqikj.top

JS:   const square = x => x * x;
来源：http://czv.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://wmd.tanke756.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cso.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://ura.cheryme.top

Ruby: square = ->(x) { x * x }
来源：http://ujc.shanyushiyangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://vbe.shanyushiyangkeji.top

[C07] 把函数作为参数传入
来源：http://jlu.guannengcc.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kml.yueranfly.top

PHP:  array_map("strtoupper", $arr);
来源：http://vcq.jlsjyb.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://okg.gogol.net.cn

TS:   arr.map(String)
来源：http://vzr.snrcjt.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gdf.zycfv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://teq.ehwqpu.com

Ruby: arr.map(&:upcase)
来源：http://wbp.snrcjt.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eqx.zdbjq.cn

[C08] 闭包
来源：http://xcz.xylfe.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dtv.dashuyun.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xia.hesvh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://erz.zdbjq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zft.aizwys.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qyc.c1oappe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uqz.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sbt.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mlp.feifeiyinyue.top

[C09] 递归
来源：http://obj.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qwz.shanyushiyangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jso.yangfankeji.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pae.zhengqikj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tle.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qrp.jianghu66.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ndr.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vou.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ipr.sufxvd.cn

[C10] 变量作用域
来源：http://ppq.nanxuanxn.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qlq.shuidangran.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nhu.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://azw.c1oappe.top

TS:   同 JS
来源：http://hqs.zycfv.cn

Java: 方法内为块级作用域
来源：http://vjj.snrcjt.cn

Go:   花括号块级作用域
来源：http://rul.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nci.cdnleiting.top

C#:   块级作用域
来源：http://ngm.aizwys.cn

[C11] 模块导入与导出
来源：http://dom.snrcjt.cn

Py:   from module import func
来源：http://lhj.jqgfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xlp.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dtw.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pme.bjfxy.top

Java: import java.util.List;
来源：http://blw.shanyushiyangtech.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wvt.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://hrl.zdbjq.cn

C#:   using System.Text;
来源：http://tpk.havefunace.top

[C12] 立即执行函数 IIFE
来源：http://bqj.nanxinkj.top

Py:   (lambda: print("run"))()
来源：http://rbm.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://pcz.hammf.cn

JS:   (() => { console.log("run"); })();
来源：http://jxu.ctjpmb.com

TS:   (() => { console.log("run"); })();
来源：http://igz.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ajo.mhx1999.top

Go:   func() { fmt.Println("run") }()
来源：http://cpd.jinqigufen.top

Ruby: -> { puts "run" }.call
来源：http://ctp.shanyushiyangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cgv.dianchejie.cn

[C13] 类型声明 / 类型注解
来源：http://ehn.xuetiantiany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cle.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wxb.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uve.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cdh.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://xcr.cashguo.top

Go:   func add(a, b int) int
来源：http://vpl.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nlf.jinyuanbaomall.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kfg.epnwcf.com


<!-- 参考信息 -->