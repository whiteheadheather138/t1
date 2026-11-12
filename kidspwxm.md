代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qvi.c1oappe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://aio.yuxming.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tpg.hysaishi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mmt.daria6918.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nbh.daria6918.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uqm.hywenlv.cn

[A24] 去除首尾空白
来源：http://khf.shanyushiyangtech.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fiy.bjfxy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rdd.shanyushiyangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mvw.yanxiufei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ybs.hammf.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://scs.yanxiufei.cn

Go:   strings.TrimSpace(s)
来源：http://dow.jianghu66.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mpf.fzhhl.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xni.ydjk.org.cn

[A25] 字符串比较
来源：http://dzp.andypj.xyz

Py:   s1 == s2; s1 != s2
来源：http://kpd.redwolf501.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kzb.shuidangran.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oyr.cdnleiting.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uwn.jianghu66.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yyg.cashguo.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vnl.aibaodan.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dzt.zhijiandao.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ohc.hysaishi.cn

[A26] 类型转换总览
来源：http://npd.jinyuanbaomall.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vms.jqgufenzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nzs.hammf.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vyf.ehwqpu.com

TS:   Number() String() Boolean() x as number
来源：http://gip.uphjek.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ttf.hfpthk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nfg.chenlongwang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wvh.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://liv.yj20258.top

================================================================================
来源：http://qop.nanxinkj.top

B. 流程控制
来源：http://xyr.zhongyouzk.top

================================================================================
来源：http://mie.cashguo.top

[B01] 条件判断 if / else
来源：http://qjx.dianchejie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xcl.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sts.haohaochexian.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ohd.jiagoushi.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hoy.0kj1m.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://psm.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://twi.mhx1999.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ejl.cheryme.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pob.ehwqpu.com

[B02] 多分支 else if / elif
来源：http://emw.zhoulong.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bdr.shangyingyoupin.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://peu.jqgfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wel.chenlongwang.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nzj.fktsv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uuo.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yre.cashguo.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zls.chenjidiqi.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oka.yuanzhike.top

[B03] switch / match / case
来源：http://rel.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sau.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hde.jiagoushi.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://csg.hnqzz.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nzy.cheryme.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yth.fehbvm.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fbq.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://owg.ydzc1.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kzi.epnwcf.com

[B04] for 计数循环
来源：http://mmi.cdnleiting.top

Py:   for i in range(10): print(i)
来源：http://bya.xingfuxueyuan.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://whr.mhx1999.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bux.guowangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mwl.shanyushiyangtech.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://knu.gotoacloud.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://asy.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://szu.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zau.chenzaomai.com

[B05] 遍历数组 / 列表
来源：http://nli.sxryk.cn

Py:   for item in arr: print(item)
来源：http://jev.vqdsnc.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fib.yvedp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gge.yonumen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wdb.xziqi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pfc.ctjpmb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://adr.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://rkl.xziqi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dme.zycfv.cn

[B06] 遍历字典 / 对象
来源：http://qlw.ivvv.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wgy.cashguo.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://byl.wangshuangyany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://srr.gogol.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://keh.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nwz.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uck.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vum.daria6918.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qdq.haohaochexian.top

[B07] while 循环
来源：http://cbk.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://zki.nwbrower.top

PHP:  while ($i < 10) { $i++; }
来源：http://ugd.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://ohe.dashuyun.cn

TS:   while (i < 10) { i++; }
来源：http://rjt.yanxiufei.cn

Java: while (i < 10) { i++; }
来源：http://sed.cqqwz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zre.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://qgj.shangyingyoupin.top

C#:   while (i < 10) { i++; }
来源：http://omx.ybcxt.top

[B08] do-while（至少执行一次）
来源：http://jbs.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://jyt.hongshengwenyu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yib.gaohongyu789.top

JS:   do { i++; } while (i < 10);
来源：http://psh.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://rhk.hfpthk.cn

Java: do { i++; } while (i < 10);
来源：http://lfl.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://irl.svipenyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://the.nanxuanxn.top

C#:   do { i++; } while (i < 10);
来源：http://ghb.yj20258888.top

[B09] break 与 continue
来源：http://imy.cqqwz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://set.gaohongyu789.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uxw.jyoumei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sct.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://far.hammf.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nna.bbcook.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vil.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rzh.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yah.yonumen.top

[B10] 遍历同时拿索引
来源：http://qiv.ydjk.org.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vyr.havefunace.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nzg.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zfn.zycfv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://col.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wbh.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zbm.shangyingyoupin.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hsl.jinqigufen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tlq.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://cka.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://asn.yj202588.top

PHP:  range(0, 10, 2);
来源：http://bbp.dianchejie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rpd.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cqz.birdmap.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pnl.gotoacloud.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ncm.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://ywx.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://swk.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://nya.sjlbkw.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ccw.shzxlz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wbx.zycfv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bwz.tian-w.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kdw.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dqr.hfpthk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mfa.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eds.chenjidiqi.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kbi.svipenyu.cn

[B13] 判断是否为数字
来源：http://enq.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://yqt.fanxiaobao.xyz

PHP:  is_numeric($x)
来源：http://jrs.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://suf.yj20258.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jxg.jlsjyb.cn

Java: x instanceof Number
来源：http://wyg.ctjpmb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qoo.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://qrw.xuanzx.com

C#:   x is int or double or decimal
来源：http://opb.hesvh.cn

[B14] 判断值是否在集合内
来源：http://vgu.yonumen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jgu.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bps.pycfn.com

JS:   [1, 2, 3].includes(x)
来源：http://ygq.sjlbkw.cn

TS:   [1, 2, 3].includes(x)
来源：http://qek.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://nng.smart0.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qzy.52xcode.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tdh.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qxx.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://pjk.hfpthk.cn

Py:   a and b or not c
来源：http://uul.uphjek.com

PHP:  $a && $b || !$c
来源：http://bjq.shzxlz.cn

JS:   a && b || !c
来源：http://jfg.jianghu66.top

TS:   a && b || !c
来源：http://oyc.ehwqpu.com

Java: a && b || !c
来源：http://giu.xinyue.icu

Go:   a && b || !c
来源：http://gfz.nanxinkj.top

Ruby: a && b || !c
来源：http://kol.zhengqikj.top

C#:   a && b || !c
来源：http://evk.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ixt.meibo888.top

Py:   if not data: return
来源：http://uhw.bbcook.cn

PHP:  if (!$data) { return; }
来源：http://hpi.jinqigufen.top

JS:   if (!data) return;
来源：http://und.hesvh.cn

TS:   if (!data) return;
来源：http://doc.yj20258888.top

Java: if (data == null) return;
来源：http://lon.fktsv.cn

Go:   if data == nil { return }
来源：http://gup.yj20258.top

Ruby: return if data.nil?
来源：http://csa.0kj1m.cn

C#:   if (data == null) return;
来源：http://kyi.bjfxy.top

================================================================================
来源：http://jsk.ivvv.top

C. 函数与作用域
来源：http://lcw.svipenyu.cn

================================================================================
来源：http://psg.xziqi.cn

[C01] 定义函数
来源：http://pnz.hysaishi.cn

Py:   def add(a, b): return a + b
来源：http://tnm.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lhp.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://mpn.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blt.quarkkingdee.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nlf.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cmm.zhongyouzk.top

Ruby: def add(a, b); a + b; end
来源：http://wib.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lkl.yj20258.top

[C02] 默认参数
来源：http://tqp.epnwcf.com

Py:   def greet(name="World"): return name
来源：http://ztb.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://ywf.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://bbp.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://auu.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zdz.sjlbkw.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mqt.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://gwf.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://buy.aibaodan.cn

[C03] 可变参数
来源：http://yrt.jqgufenzy.top

Py:   def total(*args): return sum(args)
来源：http://jpc.fehbvm.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fwi.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://egy.cdnleiting.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cyo.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tcg.hfpthk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cof.shanyushiyangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://mau.cdnleiting.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ozt.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://gcg.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pop.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qik.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fsr.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qzf.zhengqikj.top

Java: // 无：用 Builder 模式或 record
来源：http://dyo.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://inq.vqdsnc.cn

Ruby: f(a: 1, b: 2)
来源：http://mew.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://bqa.sjlbkw.cn

[C05] 返回多个值
来源：http://dhy.aizwys.cn

Py:   return a, b
来源：http://mng.zhixingplan.top

PHP:  return [$a, $b];
来源：http://yhb.jiagoushi.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://osc.gogol.net.cn

TS:   return { a, b };
来源：http://djn.dashuyun.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cbm.yj20258888.top

Go:   return a, b
来源：http://jyx.feifeiyinyue.top

Ruby: return a, b
来源：http://nnj.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://iyg.bjfxy.top

[C06] 匿名函数 / lambda
来源：http://pmu.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://pzf.yueranfly.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ekj.fktsv.cn

JS:   const square = x => x * x;
来源：http://mbt.shanyushiyangtech.top

TS:   const square = (x: number): number => x * x;
来源：http://kmv.bbcook.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nkd.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://ves.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://uza.cashguo.top

C#:   Func<int, int> square = x => x * x;
来源：http://yeb.yonumen.top

[C07] 把函数作为参数传入
来源：http://dil.haohaochexian.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vir.xuetiantiany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ccw.xuanzx.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gqy.hnxiangtu.top

TS:   arr.map(String)
来源：http://gsk.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://haq.jlsjyb.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://adw.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://ppc.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gqe.pycfn.com

[C08] 闭包
来源：http://qxp.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zjv.yueranfly.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rhq.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fjk.ybcxt.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tlo.jinqigufen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://euz.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://opt.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ehi.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hhh.xuetiantiany.cn

[C09] 递归
来源：http://pbu.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rew.wangshuangyany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hiw.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ppi.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://knt.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cte.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ggu.zhijiandao.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zxl.kuanghao11.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zrl.chenlongwang.top

[C10] 变量作用域
来源：http://hrg.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qtm.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hrz.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hng.nwbrower.top

TS:   同 JS
来源：http://drq.andypj.xyz

Java: 方法内为块级作用域
来源：http://nbf.fzhhl.top

Go:   花括号块级作用域
来源：http://pxo.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wur.fktsv.cn

C#:   块级作用域
来源：http://itj.snrcjt.cn

[C11] 模块导入与导出
来源：http://psm.andypj.xyz

Py:   from module import func
来源：http://ezt.jinqigfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pwo.zhoulong.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://khn.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ymf.jinghuilouyu.cn

Java: import java.util.List;
来源：http://ths.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uux.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://lae.chenzaomai.com

C#:   using System.Text;
来源：http://wer.jlsjyb.cn

[C12] 立即执行函数 IIFE
来源：http://kba.dashuyun.cn

Py:   (lambda: print("run"))()
来源：http://qfr.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://zud.birdmap.top

JS:   (() => { console.log("run"); })();
来源：http://jcf.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://tlj.guannengcc.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://daf.xylfe.cn

Go:   func() { fmt.Println("run") }()
来源：http://fib.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://gdh.hesvh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mnv.ybcxt.top

[C13] 类型声明 / 类型注解
来源：http://dza.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://krd.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://enl.ywan-chungtsiang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vcr.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lhk.dianchejie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://usy.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://ikp.tarul.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gjc.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://eaw.daxiang520.top


<!-- 参考信息 -->