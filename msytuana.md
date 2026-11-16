代发 wailian999

C#:   s.Length
来源：http://hde.bbcook.cn

[A23] 大小写转换
来源：http://juy.hysaishi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gvu.fktsv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uvk.yj20258888.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iht.pengpengdd.cyou

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fqe.sxryk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://png.zhoulong.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cue.yongpay.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oof.xuanzx.com

C#:   s.ToUpper(); s.ToLower()
来源：http://jeq.tanke756.top

[A24] 去除首尾空白
来源：http://rww.ybcxt.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://osk.meibo888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sil.sufxvd.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jry.fanxiaobao.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://owy.wangdashe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://shk.guannengcc.top

Go:   strings.TrimSpace(s)
来源：http://nqz.sxryk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pnj.chenlongwang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://neq.fengsongda.top

[A25] 字符串比较
来源：http://bsu.sxryk.cn

Py:   s1 == s2; s1 != s2
来源：http://poc.jinghuilouyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oqc.svipenyu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nhy.hysaishi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mwz.ybcxt.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zbf.ivvv.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://byy.fktsv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jct.9152youxi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qst.jinghuilouyu.cn

[A26] 类型转换总览
来源：http://emh.vqdsnc.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://frj.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yel.0kj1m.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aty.birdmap.top

TS:   Number() String() Boolean() x as number
来源：http://ihh.zhengqikj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eay.tanke756.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hgg.ydjk.org.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yto.xylfe.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xaj.fengsongda.top

================================================================================
来源：http://ode.0kj1m.cn

B. 流程控制
来源：http://swq.jiagoushi.top

================================================================================
来源：http://pfa.shanyushiyangtech.top

[B01] 条件判断 if / else
来源：http://spx.zhaomingkeji.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://hrl.chenjidiqi.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wcx.yvedp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tln.yvedp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pmn.quarkkingdee.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qgk.jqgufenzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://roj.gaohongyu789.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bsq.chenzaomai.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://twf.guannengcc.top

[B02] 多分支 else if / elif
来源：http://qfq.jqgfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ole.52xcode.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jqj.yvedp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://glv.gotoacloud.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wrn.yuxming.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lxk.redwolf501.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cuc.smart0.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qun.zycfv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pjb.gogol.net.cn

[B03] switch / match / case
来源：http://noo.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sxt.feifeiyinyue.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sbj.yuanzhike.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://txc.dashuyun.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://itf.jiagoushi.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://one.redwolf501.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sdy.hfpthk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mvd.fehbvm.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://clk.havefunace.top

[B04] for 计数循环
来源：http://qnz.jiagoushi.top

Py:   for i in range(10): print(i)
来源：http://ifv.epnwcf.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vek.ydjk.org.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aig.jyoumei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ivs.dianchejie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dyt.shanyushiyangtech.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wod.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://zqr.ywan-chungtsiang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://urr.aizwys.cn

[B05] 遍历数组 / 列表
来源：http://edp.hongshengwenyu.top

Py:   for item in arr: print(item)
来源：http://qst.aizwys.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vdm.shangyingyoupin.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wtx.fengsongda.top

TS:   for (const item of arr) { console.log(item); }
来源：http://brj.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kpa.ctjpmb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fca.zdbjq.cn

Ruby: arr.each { |item| puts item }
来源：http://edm.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gan.shanyushiyangkeji.top

[B06] 遍历字典 / 对象
来源：http://crl.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://idx.sweek.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://axn.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gan.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://efw.chenjidiqi.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ypf.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hcb.shangyingyoupin.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mec.jinghuilouyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://onq.yueranfly.top

[B07] while 循环
来源：http://syn.birdmap.top

Py:   while i < 10: i += 1
来源：http://bos.dashuyun.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nnf.sufxvd.cn

JS:   while (i < 10) { i++; }
来源：http://ofe.jinghuilouyu.cn

TS:   while (i < 10) { i++; }
来源：http://zum.havefunace.top

Java: while (i < 10) { i++; }
来源：http://htm.jlsjyb.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://thb.xuanzx.com

Ruby: while i < 10; i += 1; end
来源：http://ifv.gogol.net.cn

C#:   while (i < 10) { i++; }
来源：http://xmt.dianchejie.cn

[B08] do-while（至少执行一次）
来源：http://dyl.yongpay.top

Py:   # 无 do-while：用 while True + break
来源：http://guo.pycfn.com

PHP:  do { $i++; } while ($i < 10);
来源：http://swv.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://mgs.0kj1m.cn

TS:   do { i++; } while (i < 10);
来源：http://nwy.yj20258888.top

Java: do { i++; } while (i < 10);
来源：http://poz.gzhubu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yzm.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://gvy.redwolf501.top

C#:   do { i++; } while (i < 10);
来源：http://osw.zdbjq.cn

[B09] break 与 continue
来源：http://afy.xuetiantiany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://siz.yongpay.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://htg.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yzw.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wnh.jqgufenzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jdl.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uvb.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://haa.fanxiaobao.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://srn.sxryk.cn

[B10] 遍历同时拿索引
来源：http://hsl.chenlongwang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tak.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yis.zycfv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dny.jiagoushi.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dse.jqgfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dnz.hammf.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xjd.yuxming.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mau.cucudq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mqe.aibaodan.cn

[B11] 生成数字序列 / 区间
来源：http://eal.nanxinkj.top

Py:   list(range(0, 10, 2))
来源：http://kjm.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://man.cdnleiting.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ayx.zycfv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aai.shuidangran.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://isb.shangyingyoupin.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://osl.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://lnd.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rwn.ywan-chungtsiang.top

[B12] 跳出多层循环
来源：http://sjb.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pus.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tba.shzxlz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mfi.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pvh.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gfl.hfpthk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kef.cqqwz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qbj.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bvf.daria6918.cn

[B13] 判断是否为数字
来源：http://zqr.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://kop.wangdashe.top

PHP:  is_numeric($x)
来源：http://owg.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sxv.quarkkingdee.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zne.sysykeji.top

Java: x instanceof Number
来源：http://toc.cucudq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wce.tianlin.xyz

Ruby: x.is_a?(Numeric)
来源：http://xcu.shzxlz.cn

C#:   x is int or double or decimal
来源：http://bcz.yj20258.top

[B14] 判断值是否在集合内
来源：http://ecw.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zid.bjfxy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bzj.dianchejie.cn

JS:   [1, 2, 3].includes(x)
来源：http://thj.tarul.cn

TS:   [1, 2, 3].includes(x)
来源：http://ukx.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kki.fengsongda.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eob.bbcook.cn

Ruby: [1, 2, 3].include?(x)
来源：http://laq.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mhs.dashuyun.cn

[B15] 布尔运算与取反
来源：http://rek.smart0.xyz

Py:   a and b or not c
来源：http://cxg.hnqzz.top

PHP:  $a && $b || !$c
来源：http://bes.uphjek.com

JS:   a && b || !c
来源：http://vbk.iojbl.cn

TS:   a && b || !c
来源：http://fua.snrcjt.cn

Java: a && b || !c
来源：http://oka.jinqigufen.top

Go:   a && b || !c
来源：http://byl.yfazqb.com

Ruby: a && b || !c
来源：http://rxf.nanxinkj.top

C#:   a && b || !c
来源：http://htj.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://agm.yonumen.top

Py:   if not data: return
来源：http://xjz.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://hdo.zhixingplan.top

JS:   if (!data) return;
来源：http://krl.316326.xyz

TS:   if (!data) return;
来源：http://dip.zhijiandao.cn

Java: if (data == null) return;
来源：http://uyf.yueranfly.top

Go:   if data == nil { return }
来源：http://bxm.ybcxt.top

Ruby: return if data.nil?
来源：http://pvi.pengpengdd.cyou

C#:   if (data == null) return;
来源：http://eaf.yj20258.top

================================================================================
来源：http://plz.dianchejie.cn

C. 函数与作用域
来源：http://hlb.hesvh.cn

================================================================================
来源：http://tsp.yj20258.top

[C01] 定义函数
来源：http://ksf.xylfe.cn

Py:   def add(a, b): return a + b
来源：http://wem.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://out.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://njk.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gpj.xuetiantiany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bzk.jinqigufen.top

Go:   func add(a, b int) int { return a + b }
来源：http://uun.hesvh.cn

Ruby: def add(a, b); a + b; end
来源：http://jpv.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ncr.zhoulong.xyz

[C02] 默认参数
来源：http://hid.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://sxi.9152youxi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ifo.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://umm.zhixingplan.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cyr.vqdsnc.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://voa.ivvv.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iec.dianchejie.cn

Ruby: def greet(name = "World") = name
来源：http://big.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://wbt.hcnkem.com

[C03] 可变参数
来源：http://wht.aizwys.cn

Py:   def total(*args): return sum(args)
来源：http://rsa.pengpengdd.cyou

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dln.ydzc1.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pbd.tarul.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bzp.bbcook.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lhl.9152youxi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://euu.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://rcs.guannengcc.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bsf.zdbjq.cn

[C04] 命名参数 / 关键字参数
来源：http://npu.hfpthk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cki.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cev.fktsv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vnl.hfpthk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jrs.ybcxt.top

Java: // 无：用 Builder 模式或 record
来源：http://drb.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://sjv.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://tzv.yfazqb.com

C#:   f(a: 1, b: 2)
来源：http://fou.nwbrower.top

[C05] 返回多个值
来源：http://nka.52xcode.cn

Py:   return a, b
来源：http://npd.pengpengdd.cyou

PHP:  return [$a, $b];
来源：http://asq.shanyushiyangtech.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mdg.yueranfly.top

TS:   return { a, b };
来源：http://rib.xuanzx.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rrz.hcnkem.com

Go:   return a, b
来源：http://lig.fanxiaobao.xyz

Ruby: return a, b
来源：http://zyh.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://fbm.tanke756.top

[C06] 匿名函数 / lambda
来源：http://npm.shanyushiyangtech.top

Py:   square = lambda x: x * x
来源：http://epy.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://nli.zhaomingkeji.xyz

JS:   const square = x => x * x;
来源：http://zol.jianghu66.top

TS:   const square = (x: number): number => x * x;
来源：http://qmv.xuanzx.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sjn.xylfe.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lhs.jyoumei.cn

Ruby: square = ->(x) { x * x }
来源：http://xkz.52xcode.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cpx.havefunace.top

[C07] 把函数作为参数传入
来源：http://ddu.cucudq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wmi.redwolf501.top

PHP:  array_map("strtoupper", $arr);
来源：http://okj.svipenyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qcd.yfazqb.com

TS:   arr.map(String)
来源：http://mry.zhixingplan.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zbe.ehwqpu.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jph.zhaomingkeji.xyz

Ruby: arr.map(&:upcase)
来源：http://xhe.iojbl.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://etr.wangdashe.top

[C08] 闭包
来源：http://guc.fengsongda.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gna.yongpay.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sfy.jinyuanbaomall.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sts.fehbvm.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://plj.daxiang520.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://svf.zhengqikj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pop.sjlbkw.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bsv.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ybr.ppjwa.cn

[C09] 递归
来源：http://hml.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yfz.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kvz.yonumen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bkq.sysykeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ved.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://egi.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lqd.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hqf.jinghuilouyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uea.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://exq.gzhubu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://smq.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://viu.ydzc1.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://loi.epnwcf.com

TS:   同 JS
来源：http://wql.hysaishi.cn

Java: 方法内为块级作用域
来源：http://abv.zdbjq.cn

Go:   花括号块级作用域
来源：http://uvm.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vqs.meibo888.top

C#:   块级作用域
来源：http://fye.nwbrower.top

[C11] 模块导入与导出
来源：http://voe.zdbjq.cn

Py:   from module import func
来源：http://hym.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://msb.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://weh.sysykeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hrp.jlsjyb.cn

Java: import java.util.List;
来源：http://dag.fktsv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://opn.zdqjudy.top

Ruby: require "json"; require_relative "./util"
来源：http://urn.uphjek.com

C#:   using System.Text;
来源：http://qfi.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://sis.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://znc.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://etw.fktsv.cn

JS:   (() => { console.log("run"); })();
来源：http://gcu.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://etm.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pbp.nanxuanxn.top

Go:   func() { fmt.Println("run") }()
来源：http://jhj.yj20258.top

Ruby: -> { puts "run" }.call
来源：http://eio.ywan-chungtsiang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://eor.sweek.top

[C13] 类型声明 / 类型注解
来源：http://qkw.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://erm.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rno.yongpay.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fbh.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://knb.dashuyun.cn


<!-- 参考信息 -->