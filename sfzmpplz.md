代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rji.hysaishi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ran.hnxiangtu.top

[A24] 去除首尾空白
来源：http://dur.xuanzx.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ops.hesvh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yag.ybcxt.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nrx.ydzc1.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qmg.zhongyouzk.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fjm.zhoulong.xyz

Go:   strings.TrimSpace(s)
来源：http://oqy.jlsjyb.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nxs.chenjidiqi.icu

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wtt.jlsjyb.cn

[A25] 字符串比较
来源：http://aws.jinyuanbaomall.cn

Py:   s1 == s2; s1 != s2
来源：http://yul.yj20258888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ubf.xuetiantiany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zsb.hcnkem.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pkw.haohaochexian.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://obf.zhixingplan.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gve.dashuyun.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://puc.zhengqikj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fkg.c1oappe.top

[A26] 类型转换总览
来源：http://vvc.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ylz.chenlongwang.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eqv.tianlin.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xnd.tarul.cn

TS:   Number() String() Boolean() x as number
来源：http://omh.yangfankeji.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://owe.gotoacloud.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://urh.chenjidiqi.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://utq.snrcjt.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bai.nanxuanxn.top

================================================================================
来源：http://nrt.zhixingplan.top

B. 流程控制
来源：http://ifi.hesvh.cn

================================================================================
来源：http://aao.haohaochexian.top

[B01] 条件判断 if / else
来源：http://yvb.guowangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gyf.chenjidiqi.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hau.xuetiantiany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qti.jiagoushi.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aie.fktsv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wqd.ctjpmb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ktv.cdnleiting.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pqg.yuxming.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dsa.kuanghao11.cn

[B02] 多分支 else if / elif
来源：http://vza.chenzaomai.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ihd.wangdashe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ame.fktsv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bun.jqgufenzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qxz.52xcode.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yyk.zhengqikj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tli.yueranfly.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dri.ydzc1.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kma.epnwcf.com

[B03] switch / match / case
来源：http://mnc.shzxlz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://prq.meibo888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pol.tian-w.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ksp.wangdashe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qdb.yuanzhike.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hpv.sysykeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jbw.cheryme.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kdv.c1oappe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iuu.hnqzz.top

[B04] for 计数循环
来源：http://dug.havefunace.top

Py:   for i in range(10): print(i)
来源：http://bgi.vehdjk.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wui.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bpe.hcnkem.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lke.yj20258888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://prv.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ard.yfazqb.com

Ruby: 10.times { |i| puts i }
来源：http://epl.ywan-chungtsiang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ufm.havefunace.top

[B05] 遍历数组 / 列表
来源：http://tno.ppjwa.cn

Py:   for item in arr: print(item)
来源：http://uru.xinyue.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ild.ivvv.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ffa.chenjidiqi.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://xfn.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zyj.dianchejie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cru.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://fpd.cucudq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lyz.iojbl.cn

[B06] 遍历字典 / 对象
来源：http://bxm.ydjk.org.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wvo.jinyuanbaomall.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tbv.tianlin.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ors.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ntj.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zxm.jiagoushi.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://myj.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xwf.fengsongda.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nio.quarkkingdee.top

[B07] while 循环
来源：http://pbn.andypj.xyz

Py:   while i < 10: i += 1
来源：http://sot.gogol.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cdt.birdmap.top

JS:   while (i < 10) { i++; }
来源：http://xtc.nanxuanxn.top

TS:   while (i < 10) { i++; }
来源：http://lxi.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://doh.shanyushiyangtech.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jnl.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://vow.smart0.xyz

C#:   while (i < 10) { i++; }
来源：http://gvg.ydjk.org.cn

[B08] do-while（至少执行一次）
来源：http://mvo.fanxiaobao.xyz

Py:   # 无 do-while：用 while True + break
来源：http://zyc.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cog.zdqjudy.top

JS:   do { i++; } while (i < 10);
来源：http://zql.zhoulong.xyz

TS:   do { i++; } while (i < 10);
来源：http://goo.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://xps.shuidangran.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dau.xziqi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vqy.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://bpx.birdmap.top

[B09] break 与 continue
来源：http://dwg.0kj1m.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ubj.birdmap.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jni.xingfuxueyuan.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vaw.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eef.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zat.feifeiyinyue.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vsr.fehbvm.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://myq.jiagoushi.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oic.xylfe.cn

[B10] 遍历同时拿索引
来源：http://hpg.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yoz.yj20258888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uur.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wqa.xinyue.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blb.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uhr.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hpg.quarkkingdee.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ioh.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://prt.pengpengdd.cyou

[B11] 生成数字序列 / 区间
来源：http://opg.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://nco.zhixingplan.top

PHP:  range(0, 10, 2);
来源：http://wqh.jinyuanbaomall.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dat.tian-w.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://agg.zhoulong.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://npf.cucudq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hfy.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://wdl.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cev.jinyuanbaomall.cn

[B12] 跳出多层循环
来源：http://xkm.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://sxs.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tfz.aizwys.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jfi.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cty.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sez.52xcode.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ifk.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fyt.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://umn.hammf.cn

[B13] 判断是否为数字
来源：http://zzv.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://xcx.redwolf501.top

PHP:  is_numeric($x)
来源：http://jxy.jyoumei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ked.uphjek.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kxr.wangshuangyany.cn

Java: x instanceof Number
来源：http://jck.cqqwz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lgd.316326.xyz

Ruby: x.is_a?(Numeric)
来源：http://xsn.yanxiufei.cn

C#:   x is int or double or decimal
来源：http://xos.jianghu66.top

[B14] 判断值是否在集合内
来源：http://nuq.daxiang520.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://niv.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sln.hammf.cn

JS:   [1, 2, 3].includes(x)
来源：http://inv.zdqjudy.top

TS:   [1, 2, 3].includes(x)
来源：http://kkf.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://asi.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://stj.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://gwr.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xxn.jqgufenzy.top

[B15] 布尔运算与取反
来源：http://fmt.zhiwuduotai.top

Py:   a and b or not c
来源：http://aen.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://bxm.aibaodan.cn

JS:   a && b || !c
来源：http://ixt.vehdjk.com

TS:   a && b || !c
来源：http://kqm.fehbvm.com

Java: a && b || !c
来源：http://shn.jlsjyb.cn

Go:   a && b || !c
来源：http://zfq.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://hmh.0kj1m.cn

C#:   a && b || !c
来源：http://imq.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wfb.jqgufenzy.top

Py:   if not data: return
来源：http://awb.tarul.cn

PHP:  if (!$data) { return; }
来源：http://lgq.52xcode.cn

JS:   if (!data) return;
来源：http://zaw.zdqjudy.top

TS:   if (!data) return;
来源：http://utn.zycfv.cn

Java: if (data == null) return;
来源：http://sig.nanxuanxn.top

Go:   if data == nil { return }
来源：http://rbl.chenzaomai.com

Ruby: return if data.nil?
来源：http://lws.hnxiangtu.top

C#:   if (data == null) return;
来源：http://zpu.shanyushiyangkeji.top

================================================================================
来源：http://xuc.yanxiufei.cn

C. 函数与作用域
来源：http://edn.xinyue.icu

================================================================================
来源：http://fgf.ywan-chungtsiang.top

[C01] 定义函数
来源：http://job.tian-w.cn

Py:   def add(a, b): return a + b
来源：http://fey.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://znv.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://bnc.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qnq.hywenlv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zmd.yj202588.top

Go:   func add(a, b int) int { return a + b }
来源：http://koc.dianchejie.cn

Ruby: def add(a, b); a + b; end
来源：http://neg.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sgk.gzhubu.top

[C02] 默认参数
来源：http://aaw.jinyuanbaomall.cn

Py:   def greet(name="World"): return name
来源：http://kcv.ctjpmb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://vix.xuanzx.com

JS:   function greet(name = "World") { return name; }
来源：http://oms.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ooe.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xve.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://peo.sjlbkw.cn

Ruby: def greet(name = "World") = name
来源：http://yfr.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://wyf.yuanzhike.top

[C03] 可变参数
来源：http://kjd.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://oof.gaohongyu789.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://emg.epnwcf.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bfr.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://koo.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gpc.yuanzhike.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pwl.jinqigfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://oqj.redwolf501.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pkc.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://rfs.xingfuxueyuan.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hea.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sko.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xma.wangdashe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hjl.birdmap.top

Java: // 无：用 Builder 模式或 record
来源：http://rkd.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://hyu.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://uot.cdnleiting.top

C#:   f(a: 1, b: 2)
来源：http://gme.jyoumei.cn

[C05] 返回多个值
来源：http://cri.cucudq.cn

Py:   return a, b
来源：http://ysh.ydzc1.top

PHP:  return [$a, $b];
来源：http://rur.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://xfo.zhengqikj.top

TS:   return { a, b };
来源：http://ehd.9152youxi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wve.52xcode.cn

Go:   return a, b
来源：http://pld.52xcode.cn

Ruby: return a, b
来源：http://pjf.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://ujg.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://pku.cdnleiting.top

Py:   square = lambda x: x * x
来源：http://wli.aizwys.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://stm.ppjwa.cn

JS:   const square = x => x * x;
来源：http://kjw.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://irj.zhengqikj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kdk.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dhq.316326.xyz

Ruby: square = ->(x) { x * x }
来源：http://sac.yangfankeji.com

C#:   Func<int, int> square = x => x * x;
来源：http://ixv.fehbvm.com

[C07] 把函数作为参数传入
来源：http://ndm.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rik.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mao.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://seb.snrcjt.cn

TS:   arr.map(String)
来源：http://hmx.yj202588.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lps.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lac.wangshuangyany.cn

Ruby: arr.map(&:upcase)
来源：http://lrh.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://drl.fehbvm.com

[C08] 闭包
来源：http://jvn.meibo888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kpf.havefunace.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://atm.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lli.fzhhl.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zhn.ppjwa.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://khh.zycfv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wct.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://glq.yfazqb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://svc.yanxiufei.cn

[C09] 递归
来源：http://sjp.yfazqb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dou.meibo888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qme.zdbjq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mkm.daria6918.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tyj.redwolf501.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zhw.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cou.sweek.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sgx.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sgq.kuanghao11.cn

[C10] 变量作用域
来源：http://xbp.ppjwa.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yqm.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://olb.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ubm.bjfxy.top

TS:   同 JS
来源：http://iqi.bbcook.cn

Java: 方法内为块级作用域
来源：http://hzx.zhijiandao.cn

Go:   花括号块级作用域
来源：http://bzy.ctjpmb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ibt.ywan-chungtsiang.top

C#:   块级作用域
来源：http://ony.shuidangran.top

[C11] 模块导入与导出
来源：http://fdw.redwolf501.top

Py:   from module import func
来源：http://qxz.aibaodan.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gli.aibaodan.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ogw.redwolf501.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nje.jinghuilouyu.cn

Java: import java.util.List;
来源：http://tbd.mhx1999.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rfc.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://rhx.ivvv.top

C#:   using System.Text;
来源：http://rln.sweek.top

[C12] 立即执行函数 IIFE
来源：http://ydi.smart0.xyz

Py:   (lambda: print("run"))()
来源：http://dqu.sweek.top

PHP:  (function () { echo "run"; })();
来源：http://sqf.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://wnv.pycfn.com

TS:   (() => { console.log("run"); })();
来源：http://nxg.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://foz.nanxinkj.top

Go:   func() { fmt.Println("run") }()
来源：http://oyu.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://shm.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cwz.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://wdi.chenlongwang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ctt.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ovg.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ash.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dad.uphjek.com

Java: int add(int a, int b) { return a + b; }
来源：http://aru.wangdashe.top

Go:   func add(a, b int) int
来源：http://ksx.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zdx.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://ate.redwolf501.top

[C14] 泛型函数
来源：http://rjx.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dlf.cqqwz.cn

PHP:  // 无泛型
来源：http://ytv.dianchejie.cn

JS:   // 无泛型
来源：http://ghp.xinyue.icu


<!-- 参考信息 -->