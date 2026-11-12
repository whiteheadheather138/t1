代发 wailian999

C#:   s.Length
来源：http://qpm.9152youxi.cn

[A23] 大小写转换
来源：http://uxb.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wvv.tianlin.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://isd.316326.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hgp.guannengcc.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yew.havefunace.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hnv.zhoulong.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wfn.yonumen.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vjc.hcnkem.com

C#:   s.ToUpper(); s.ToLower()
来源：http://bqe.gotoacloud.top

[A24] 去除首尾空白
来源：http://tux.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xnu.chenzaomai.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://exs.jqgfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://prw.yuxming.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ykz.guowangkeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xgf.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://dmx.jinghuilouyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://chn.ctjpmb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nje.zdbjq.cn

[A25] 字符串比较
来源：http://xpx.yangfankeji.com

Py:   s1 == s2; s1 != s2
来源：http://cln.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://riz.zhaomingkeji.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xpm.fktsv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kqr.chenjidiqi.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rxc.redwolf501.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xvl.meibo888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://irn.aibaodan.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vdq.iojbl.cn

[A26] 类型转换总览
来源：http://juy.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kcp.quarkkingdee.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tuv.smart0.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://url.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://yao.chenlongwang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hkb.ybcxt.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fuu.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kpb.chenzaomai.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qvq.pengpengdd.cyou

================================================================================
来源：http://rsn.yfazqb.com

B. 流程控制
来源：http://jpm.zycfv.cn

================================================================================
来源：http://tdf.ywan-chungtsiang.top

[B01] 条件判断 if / else
来源：http://qrn.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yfb.gotoacloud.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mxw.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ikf.svipenyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://niy.cdnleiting.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zdg.yj202588.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://umg.gzhubu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lpm.zhoulong.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kbu.jlsjyb.cn

[B02] 多分支 else if / elif
来源：http://jdz.c1oappe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oyq.gotoacloud.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jyv.pengpengdd.cyou

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nqy.sxryk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://foz.iojbl.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fwb.shanyushiyangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tyc.snrcjt.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ygq.xylfe.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wqy.yj20258.top

[B03] switch / match / case
来源：http://sfv.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vlc.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sja.shzxlz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tsi.hongshengwenyu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://klw.yanxiufei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gcu.tian-w.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iok.sysykeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cyi.yangfankeji.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rva.hysaishi.cn

[B04] for 计数循环
来源：http://gyt.yangfankeji.com

Py:   for i in range(10): print(i)
来源：http://ott.sxryk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://orj.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vsk.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hgw.mhx1999.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tuq.yvedp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zfx.hongshengwenyu.top

Ruby: 10.times { |i| puts i }
来源：http://oea.yj202588.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uxb.cdnleiting.top

[B05] 遍历数组 / 列表
来源：http://ivv.fehbvm.com

Py:   for item in arr: print(item)
来源：http://xdl.jqgfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uzi.xuetiantiany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cte.xylfe.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://izu.ivvv.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mhz.yonumen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vdi.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://ksr.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hjc.mhx1999.top

[B06] 遍历字典 / 对象
来源：http://riq.andypj.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://deq.316326.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ruh.pengpengdd.cyou

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fjo.guannengcc.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rpf.zhengqikj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wqf.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sac.iojbl.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tiq.sweek.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blv.sufxvd.cn

[B07] while 循环
来源：http://swn.wangshuangyany.cn

Py:   while i < 10: i += 1
来源：http://mse.fengsongda.top

PHP:  while ($i < 10) { $i++; }
来源：http://oqo.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://hog.bjfxy.top

TS:   while (i < 10) { i++; }
来源：http://ahr.yvedp.cn

Java: while (i < 10) { i++; }
来源：http://jpf.nanxuanxn.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nja.vqdsnc.cn

Ruby: while i < 10; i += 1; end
来源：http://top.dashuyun.cn

C#:   while (i < 10) { i++; }
来源：http://hwr.tian-w.cn

[B08] do-while（至少执行一次）
来源：http://wlg.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://lct.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bnr.zhiwuduotai.top

JS:   do { i++; } while (i < 10);
来源：http://kdm.iojbl.cn

TS:   do { i++; } while (i < 10);
来源：http://euw.yonumen.top

Java: do { i++; } while (i < 10);
来源：http://skq.hywenlv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pdm.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://spe.pengpengdd.cyou

C#:   do { i++; } while (i < 10);
来源：http://csh.hnxiangtu.top

[B09] break 与 continue
来源：http://baq.gogol.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lwu.cdnleiting.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cmn.xuanzx.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://isf.jlsjyb.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lkb.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zaw.bbcook.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hgi.nanxuanxn.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://isk.yj20258888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lju.iojbl.cn

[B10] 遍历同时拿索引
来源：http://dpz.fzhhl.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kco.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lzn.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lqv.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://irk.shanyushiyangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wmq.hnxiangtu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zjc.ywan-chungtsiang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cts.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rib.feifeiyinyue.top

[B11] 生成数字序列 / 区间
来源：http://jdv.ywan-chungtsiang.top

Py:   list(range(0, 10, 2))
来源：http://tme.hongshengwenyu.top

PHP:  range(0, 10, 2);
来源：http://vlf.gzhubu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bmb.c1oappe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jcf.52xcode.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jjj.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://exo.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://wfh.jinqigufen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rjm.daxiang520.top

[B12] 跳出多层循环
来源：http://itd.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://dvd.shanyushiyangtech.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://eke.jlsjyb.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zol.cqqwz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jrv.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sti.hammf.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://udz.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sjr.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fco.chenlongwang.top

[B13] 判断是否为数字
来源：http://ymg.yj20258.top

Py:   isinstance(x, (int, float))
来源：http://rtn.yvedp.cn

PHP:  is_numeric($x)
来源：http://dgb.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sqh.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://koo.gzhubu.top

Java: x instanceof Number
来源：http://uxn.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://epp.xylfe.cn

Ruby: x.is_a?(Numeric)
来源：http://jgb.andypj.xyz

C#:   x is int or double or decimal
来源：http://aht.sysykeji.top

[B14] 判断值是否在集合内
来源：http://mnf.pengpengdd.cyou

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gcq.xziqi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rsd.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://wmn.kuanghao11.cn

TS:   [1, 2, 3].includes(x)
来源：http://aqj.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mho.jqgfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rbu.sweek.top

Ruby: [1, 2, 3].include?(x)
来源：http://lwq.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rfx.feifeiyinyue.top

[B15] 布尔运算与取反
来源：http://btu.fzhhl.top

Py:   a and b or not c
来源：http://sox.yonumen.top

PHP:  $a && $b || !$c
来源：http://gwk.chenlongwang.top

JS:   a && b || !c
来源：http://rtq.ybcxt.top

TS:   a && b || !c
来源：http://qth.hysaishi.cn

Java: a && b || !c
来源：http://alb.hcnkem.com

Go:   a && b || !c
来源：http://joy.xinyue.icu

Ruby: a && b || !c
来源：http://ktz.aibaodan.cn

C#:   a && b || !c
来源：http://yyl.havefunace.top

[B16] 卫语句：不满足条件提前返回
来源：http://aey.nanxuanxn.top

Py:   if not data: return
来源：http://nao.yonumen.top

PHP:  if (!$data) { return; }
来源：http://izv.andypj.xyz

JS:   if (!data) return;
来源：http://pqy.0kj1m.cn

TS:   if (!data) return;
来源：http://ieq.fzhhl.top

Java: if (data == null) return;
来源：http://kxw.yonumen.top

Go:   if data == nil { return }
来源：http://xea.nwbrower.top

Ruby: return if data.nil?
来源：http://eyy.jiagoushi.top

C#:   if (data == null) return;
来源：http://yjn.feifeiyinyue.top

================================================================================
来源：http://aoc.shuidangran.top

C. 函数与作用域
来源：http://fvo.jinqigfzy.top

================================================================================
来源：http://bwb.redwolf501.top

[C01] 定义函数
来源：http://gmj.xziqi.cn

Py:   def add(a, b): return a + b
来源：http://abm.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uoi.zhongyouzk.top

JS:   function add(a, b) { return a + b; }
来源：http://zew.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://esq.ybcxt.top

Java: static int add(int a, int b) { return a + b; }
来源：http://eve.iojbl.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ecl.fehbvm.com

Ruby: def add(a, b); a + b; end
来源：http://lct.epnwcf.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bgt.hysaishi.cn

[C02] 默认参数
来源：http://dbz.zycfv.cn

Py:   def greet(name="World"): return name
来源：http://khv.havefunace.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zwc.shanyushiyangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://sxn.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://weu.yongpay.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gci.xingfuxueyuan.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://osm.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://cib.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://jky.cheryme.top

[C03] 可变参数
来源：http://gvd.fzhhl.top

Py:   def total(*args): return sum(args)
来源：http://gct.c1oappe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gjf.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rpf.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://paw.haohaochexian.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hjr.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qoj.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://thv.ybcxt.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://heh.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://nhi.vehdjk.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ldn.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sct.hongshengwenyu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vpx.chenzaomai.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xpz.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://aji.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://zab.wangshuangyany.cn

Ruby: f(a: 1, b: 2)
来源：http://ccl.yvedp.cn

C#:   f(a: 1, b: 2)
来源：http://qrp.xinyue.icu

[C05] 返回多个值
来源：http://aus.yuanzhike.top

Py:   return a, b
来源：http://eoe.guannengcc.top

PHP:  return [$a, $b];
来源：http://xam.ydjk.org.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bwm.pengpengdd.cyou

TS:   return { a, b };
来源：http://nrg.cdnleiting.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xdz.kuanghao11.cn

Go:   return a, b
来源：http://brk.sysykeji.top

Ruby: return a, b
来源：http://qjx.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://eri.feifeiyinyue.top

[C06] 匿名函数 / lambda
来源：http://ddz.zhoulong.xyz

Py:   square = lambda x: x * x
来源：http://htc.tian-w.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xuv.fktsv.cn

JS:   const square = x => x * x;
来源：http://xsx.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://taf.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wuw.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://shr.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://owz.yueranfly.top

C#:   Func<int, int> square = x => x * x;
来源：http://agd.mhx1999.top

[C07] 把函数作为参数传入
来源：http://hoh.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tjx.hysaishi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://umd.hysaishi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tgi.epnwcf.com

TS:   arr.map(String)
来源：http://fop.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xau.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tsb.xingfuxueyuan.xyz

Ruby: arr.map(&:upcase)
来源：http://vlr.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://sqp.sufxvd.cn

[C08] 闭包
来源：http://ozn.guannengcc.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jdl.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cqd.guowangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bha.dianchejie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://suo.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://euh.yueranfly.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tvd.iojbl.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bue.havefunace.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hzz.bbcook.cn

[C09] 递归
来源：http://xtl.bbcook.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yax.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rbv.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xex.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://phs.epnwcf.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://inq.svipenyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://shn.yueranfly.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fiv.tarul.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://emd.yj202588.top

[C10] 变量作用域
来源：http://yku.hywenlv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nvb.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kaz.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vqy.feifeiyinyue.top

TS:   同 JS
来源：http://yfi.xinyue.icu

Java: 方法内为块级作用域
来源：http://mmy.guowangkeji.top

Go:   花括号块级作用域
来源：http://fjf.xylfe.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xiz.ehwqpu.com

C#:   块级作用域
来源：http://byx.uphjek.com

[C11] 模块导入与导出
来源：http://dva.sysykeji.top

Py:   from module import func
来源：http://mps.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kbc.52xcode.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nqw.xuetiantiany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sga.ybcxt.top

Java: import java.util.List;
来源：http://wsh.vqdsnc.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gaf.svipenyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://xww.zhixingplan.top

C#:   using System.Text;
来源：http://nsd.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://fyx.hesvh.cn

Py:   (lambda: print("run"))()
来源：http://vih.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://eal.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://tyv.jinqigufen.top

TS:   (() => { console.log("run"); })();
来源：http://txh.andypj.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mki.havefunace.top

Go:   func() { fmt.Println("run") }()
来源：http://hnt.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://eym.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uwy.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://ksh.meibo888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xjr.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ull.jyoumei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ify.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xmo.yuanzhike.top


<!-- 参考信息 -->