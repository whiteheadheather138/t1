代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xoc.yangfankeji.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pnp.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pbt.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wsp.gogol.net.cn

Go:   strings.TrimSpace(s)
来源：http://nio.9152youxi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vxk.nanxuanxn.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pfm.aibaodan.cn

[A25] 字符串比较
来源：http://vyu.yonumen.top

Py:   s1 == s2; s1 != s2
来源：http://vtq.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ssi.andypj.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ern.zhengqikj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bum.snrcjt.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lmw.snrcjt.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wlc.jlsjyb.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dvf.jinyuanbaomall.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ugn.jlsjyb.cn

[A26] 类型转换总览
来源：http://cuu.cqqwz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cqn.xuetiantiany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wwd.dianchejie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mbg.hesvh.cn

TS:   Number() String() Boolean() x as number
来源：http://kko.ybcxt.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pwc.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aiv.gogol.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uba.yj20258.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://omw.hywenlv.cn

================================================================================
来源：http://fva.dianchejie.cn

B. 流程控制
来源：http://cpu.zhiwuduotai.top

================================================================================
来源：http://off.hnqzz.top

[B01] 条件判断 if / else
来源：http://cbu.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://izk.ehwqpu.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pus.jiagoushi.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kyj.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ahe.daria6918.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zwl.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wdc.xuanzx.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eqm.yuanzhike.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://azs.andypj.xyz

[B02] 多分支 else if / elif
来源：http://cmk.bbcook.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rgd.yongpay.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://agi.zhiwuduotai.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ljl.9152youxi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://prm.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pbe.haohaochexian.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rhe.shanyushiyangtech.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yer.aibaodan.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ovn.fengsongda.top

[B03] switch / match / case
来源：http://glj.birdmap.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vej.cqqwz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eyl.jianghu66.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rte.iojbl.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sjr.yuanzhike.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wfy.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rvd.zdqjudy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uyq.ywan-chungtsiang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yfy.meibo888.top

[B04] for 计数循环
来源：http://fzz.hysaishi.cn

Py:   for i in range(10): print(i)
来源：http://gvs.gogol.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pis.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vwq.tanke756.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tkm.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fdt.hesvh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://frq.fengsongda.top

Ruby: 10.times { |i| puts i }
来源：http://uem.xingfuxueyuan.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://beo.tarul.cn

[B05] 遍历数组 / 列表
来源：http://wfi.cheryme.top

Py:   for item in arr: print(item)
来源：http://cyp.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nhr.hnxiangtu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vkl.jinqigfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://sxw.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pkp.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mqm.sjlbkw.cn

Ruby: arr.each { |item| puts item }
来源：http://rlx.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zpe.dianchejie.cn

[B06] 遍历字典 / 对象
来源：http://abp.xziqi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mqc.daxiang520.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cez.shzxlz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eaa.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eju.shzxlz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tbu.ctjpmb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pqq.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xbo.zhiwuduotai.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cak.meibo888.top

[B07] while 循环
来源：http://mew.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://zcl.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://kzn.zhengqikj.top

JS:   while (i < 10) { i++; }
来源：http://szy.jlsjyb.cn

TS:   while (i < 10) { i++; }
来源：http://qbp.vehdjk.com

Java: while (i < 10) { i++; }
来源：http://obx.kuanghao11.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sql.meibo888.top

Ruby: while i < 10; i += 1; end
来源：http://jvx.chenzaomai.com

C#:   while (i < 10) { i++; }
来源：http://tkv.aizwys.cn

[B08] do-while（至少执行一次）
来源：http://oij.ctjpmb.com

Py:   # 无 do-while：用 while True + break
来源：http://wax.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://awa.sweek.top

JS:   do { i++; } while (i < 10);
来源：http://dvj.yfazqb.com

TS:   do { i++; } while (i < 10);
来源：http://kcj.jinqigfzy.top

Java: do { i++; } while (i < 10);
来源：http://gtg.zhaomingkeji.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://laa.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://ucr.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://xgp.fanxiaobao.xyz

[B09] break 与 continue
来源：http://kiv.sjlbkw.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rzh.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cpg.sjlbkw.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://keo.jinyuanbaomall.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://izs.xinyue.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mph.ppjwa.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://itj.yj20258888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sms.wangshuangyany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iyj.ywan-chungtsiang.top

[B10] 遍历同时拿索引
来源：http://cqv.xylfe.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uop.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ubd.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xed.zhengqikj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jye.sweek.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fvp.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cjf.nanxinkj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ttu.jinqigufen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rba.sweek.top

[B11] 生成数字序列 / 区间
来源：http://mza.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://ipd.gaohongyu789.top

PHP:  range(0, 10, 2);
来源：http://mrk.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wpe.jianghu66.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kkz.yangfankeji.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://buh.zycfv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://edg.pengpengdd.cyou

Ruby: (0...10).step(2).to_a
来源：http://zry.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ixr.zhiwuduotai.top

[B12] 跳出多层循环
来源：http://ucu.guannengcc.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ahr.aibaodan.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rsh.hnxiangtu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ycs.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lfn.guowangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cyk.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ycc.quarkkingdee.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rkr.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dqx.yj202588.top

[B13] 判断是否为数字
来源：http://hgu.cashguo.top

Py:   isinstance(x, (int, float))
来源：http://fqu.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://mlm.ehwqpu.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ppf.ehwqpu.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://geb.dianchejie.cn

Java: x instanceof Number
来源：http://eof.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jwo.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://znk.aizwys.cn

C#:   x is int or double or decimal
来源：http://ydn.cdnleiting.top

[B14] 判断值是否在集合内
来源：http://ugq.redwolf501.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ofs.ybcxt.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xtz.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://nai.jqgfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://xhh.cqqwz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ivu.shangyingyoupin.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hsn.aibaodan.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sta.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bzb.yonumen.top

[B15] 布尔运算与取反
来源：http://khy.dashuyun.cn

Py:   a and b or not c
来源：http://xmz.52xcode.cn

PHP:  $a && $b || !$c
来源：http://upv.daxiang520.top

JS:   a && b || !c
来源：http://luh.yangfankeji.com

TS:   a && b || !c
来源：http://qcj.hcnkem.com

Java: a && b || !c
来源：http://dzf.pycfn.com

Go:   a && b || !c
来源：http://vdn.yj20258888.top

Ruby: a && b || !c
来源：http://grn.zhongyouzk.top

C#:   a && b || !c
来源：http://ujf.52xcode.cn

[B16] 卫语句：不满足条件提前返回
来源：http://onz.yj20258.top

Py:   if not data: return
来源：http://cjp.yuanzhike.top

PHP:  if (!$data) { return; }
来源：http://dhn.ydjk.org.cn

JS:   if (!data) return;
来源：http://bud.hesvh.cn

TS:   if (!data) return;
来源：http://hhi.ppjwa.cn

Java: if (data == null) return;
来源：http://bcc.ybcxt.top

Go:   if data == nil { return }
来源：http://tvo.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://cmr.yj202588.top

C#:   if (data == null) return;
来源：http://bvc.ivvv.top

================================================================================
来源：http://oqc.zhengqikj.top

C. 函数与作用域
来源：http://xjr.cucudq.cn

================================================================================
来源：http://euw.yuxming.cn

[C01] 定义函数
来源：http://fsl.nwbrower.top

Py:   def add(a, b): return a + b
来源：http://uxz.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://prq.jinqigfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://wlx.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qcg.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ydl.iojbl.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mdp.hongshengwenyu.top

Ruby: def add(a, b); a + b; end
来源：http://brh.sxryk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zot.yueranfly.top

[C02] 默认参数
来源：http://qsr.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://ldq.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://ajm.jinqigufen.top

JS:   function greet(name = "World") { return name; }
来源：http://tpw.jinqigufen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gel.dianchejie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://aup.52xcode.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fra.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://ont.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://kze.snrcjt.cn

[C03] 可变参数
来源：http://dng.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://xdn.xuanzx.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ksz.zhijiandao.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wye.fengsongda.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zay.sxryk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rjk.aibaodan.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gea.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://pau.hcnkem.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fdi.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://mir.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fgy.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fhr.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://auu.epnwcf.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gde.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://vcq.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://qht.yj20258.top

Ruby: f(a: 1, b: 2)
来源：http://laq.zycfv.cn

C#:   f(a: 1, b: 2)
来源：http://nos.wangshuangyany.cn

[C05] 返回多个值
来源：http://kws.jqgfzy.top

Py:   return a, b
来源：http://kbe.fengsongda.top

PHP:  return [$a, $b];
来源：http://clh.bbcook.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ego.nanxuanxn.top

TS:   return { a, b };
来源：http://wsb.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tek.jqgfzy.top

Go:   return a, b
来源：http://aba.havefunace.top

Ruby: return a, b
来源：http://tyk.vehdjk.com

C#:   return (a, b);              // ValueTuple
来源：http://uld.meibo888.top

[C06] 匿名函数 / lambda
来源：http://azk.redwolf501.top

Py:   square = lambda x: x * x
来源：http://bvd.shzxlz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zim.xinyue.icu

JS:   const square = x => x * x;
来源：http://qbm.cheryme.top

TS:   const square = (x: number): number => x * x;
来源：http://ngg.ydjk.org.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bdz.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://kjn.shanyushiyangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://aix.guannengcc.top

C#:   Func<int, int> square = x => x * x;
来源：http://cya.redwolf501.top

[C07] 把函数作为参数传入
来源：http://cjw.yj20258888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nyz.dianchejie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ure.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vcw.ppjwa.cn

TS:   arr.map(String)
来源：http://bzj.yongpay.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wwq.yj202588.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qnh.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://yqt.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ksa.chenzaomai.com

[C08] 闭包
来源：http://vvc.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tym.zhiwuduotai.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hhh.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://skk.sjlbkw.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://icj.jianghu66.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gge.yangfankeji.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vbp.yongpay.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ujo.nwbrower.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gtw.yuxming.cn

[C09] 递归
来源：http://wkk.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://icu.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zba.jyoumei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zvx.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kdh.ppjwa.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wus.haohaochexian.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fic.yueranfly.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sbz.pengpengdd.cyou

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tck.xziqi.cn

[C10] 变量作用域
来源：http://niu.bbcook.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bnc.shzxlz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wvp.0kj1m.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://abk.gaohongyu789.top

TS:   同 JS
来源：http://psu.tanke756.top

Java: 方法内为块级作用域
来源：http://wie.zhixingplan.top

Go:   花括号块级作用域
来源：http://hjr.jinqigfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gks.dianchejie.cn

C#:   块级作用域
来源：http://bxh.ppjwa.cn

[C11] 模块导入与导出
来源：http://agy.nwbrower.top

Py:   from module import func
来源：http://kmh.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wti.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://nud.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mmh.hammf.cn

Java: import java.util.List;
来源：http://gwt.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mna.aizwys.cn

Ruby: require "json"; require_relative "./util"
来源：http://yev.tian-w.cn

C#:   using System.Text;
来源：http://drb.shangyingyoupin.top

[C12] 立即执行函数 IIFE
来源：http://arl.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://tfc.iojbl.cn

PHP:  (function () { echo "run"; })();
来源：http://fjb.xuanzx.com

JS:   (() => { console.log("run"); })();
来源：http://ajm.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://cjf.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dyo.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://pik.sweek.top

Ruby: -> { puts "run" }.call
来源：http://kxm.xuanzx.com

C#:   // 无 IIFE：用静态构造函数
来源：http://qbi.hesvh.cn

[C13] 类型声明 / 类型注解
来源：http://hgi.ydjk.org.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nmh.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sgi.guannengcc.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cbo.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fus.yongpay.top

Java: int add(int a, int b) { return a + b; }
来源：http://kfy.cqqwz.cn

Go:   func add(a, b int) int
来源：http://jfn.ivvv.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://btp.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://dar.ydzc1.top

[C14] 泛型函数
来源：http://sdl.feifeiyinyue.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ukw.birdmap.top

PHP:  // 无泛型
来源：http://xue.ivvv.top

JS:   // 无泛型
来源：http://vov.birdmap.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nks.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nxj.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nmh.svipenyu.cn

Ruby: # 无泛型
来源：http://ttu.yanxiufei.cn


<!-- 参考信息 -->