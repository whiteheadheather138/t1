代发 wailian999

C#:   s.Length
来源：http://ujz.zdbjq.cn

[A23] 大小写转换
来源：http://dhj.fanxiaobao.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://zpn.fanxiaobao.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rvm.c1oappe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qla.zdbjq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kwp.aibaodan.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cdi.yj20258888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gvh.vehdjk.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://imf.pycfn.com

C#:   s.ToUpper(); s.ToLower()
来源：http://moe.0kj1m.cn

[A24] 去除首尾空白
来源：http://cxg.pengpengdd.cyou

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://atm.jinghuilouyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fsw.ctjpmb.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://axg.316326.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qmp.feifeiyinyue.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rbh.zdqjudy.top

Go:   strings.TrimSpace(s)
来源：http://mwr.epnwcf.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lhp.yuanzhike.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zpz.zhongyouzk.top

[A25] 字符串比较
来源：http://wvi.bjfxy.top

Py:   s1 == s2; s1 != s2
来源：http://ltj.wangdashe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rjl.hcnkem.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://frh.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xud.sufxvd.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dqw.guannengcc.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://szx.quarkkingdee.top

Ruby: s1 == s2; s1 <=> s2
来源：http://etg.ehwqpu.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qfc.yanxiufei.cn

[A26] 类型转换总览
来源：http://ban.nwbrower.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qdg.ybcxt.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://maf.316326.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nin.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://smj.sjlbkw.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sfw.cucudq.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nhc.birdmap.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rnu.52xcode.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ouq.guannengcc.top

================================================================================
来源：http://pnw.haohaochexian.top

B. 流程控制
来源：http://ikw.haohaochexian.top

================================================================================
来源：http://xpp.yuxming.cn

[B01] 条件判断 if / else
来源：http://azk.hysaishi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dmm.hnxiangtu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nju.dianchejie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bpx.xuetiantiany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mrf.haohaochexian.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ado.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vyg.sweek.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mqt.ehwqpu.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hbv.guowangkeji.top

[B02] 多分支 else if / elif
来源：http://reb.andypj.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iss.xuanzx.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qgx.zhongyouzk.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jhm.yuanzhike.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gkn.svipenyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xrx.nanxuanxn.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cpm.shanyushiyangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ztl.cdnleiting.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://buo.hfpthk.cn

[B03] switch / match / case
来源：http://slp.fzhhl.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oie.ivvv.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ttw.tianlin.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xme.shanyushiyangtech.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://awq.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ect.chenlongwang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qxv.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://byu.feifeiyinyue.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://poc.shuidangran.top

[B04] for 计数循环
来源：http://nhr.guowangkeji.top

Py:   for i in range(10): print(i)
来源：http://cfk.guowangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aty.gogol.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jiv.hnxiangtu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qfs.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iel.zhongyouzk.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://isc.ydzc1.top

Ruby: 10.times { |i| puts i }
来源：http://fau.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nkx.pycfn.com

[B05] 遍历数组 / 列表
来源：http://slt.tian-w.cn

Py:   for item in arr: print(item)
来源：http://fgi.daria6918.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://luo.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yel.0kj1m.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oky.tian-w.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://myh.hysaishi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wyq.tianlin.xyz

Ruby: arr.each { |item| puts item }
来源：http://tgj.cqqwz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lxb.hywenlv.cn

[B06] 遍历字典 / 对象
来源：http://mqr.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://tde.9152youxi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qoo.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rem.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://icz.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ocx.cucudq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tte.sweek.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eww.ehwqpu.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cxa.shanyushiyangtech.top

[B07] while 循环
来源：http://chy.birdmap.top

Py:   while i < 10: i += 1
来源：http://qhm.redwolf501.top

PHP:  while ($i < 10) { $i++; }
来源：http://qdw.gaohongyu789.top

JS:   while (i < 10) { i++; }
来源：http://fdz.jqgfzy.top

TS:   while (i < 10) { i++; }
来源：http://oyx.meibo888.top

Java: while (i < 10) { i++; }
来源：http://osi.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gfb.shanyushiyangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://sby.yj202588.top

C#:   while (i < 10) { i++; }
来源：http://uhy.xylfe.cn

[B08] do-while（至少执行一次）
来源：http://uaq.shzxlz.cn

Py:   # 无 do-while：用 while True + break
来源：http://xct.zhengqikj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://geo.yvedp.cn

JS:   do { i++; } while (i < 10);
来源：http://ulx.yueranfly.top

TS:   do { i++; } while (i < 10);
来源：http://zvv.havefunace.top

Java: do { i++; } while (i < 10);
来源：http://sif.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wbm.yueranfly.top

Ruby: begin; i += 1; end while i < 10
来源：http://dwk.hammf.cn

C#:   do { i++; } while (i < 10);
来源：http://lue.9152youxi.cn

[B09] break 与 continue
来源：http://cvl.uphjek.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kcw.sjlbkw.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ori.haohaochexian.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gnl.nwbrower.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://odu.jinqigufen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yam.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://djh.yonumen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eps.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kns.hcnkem.com

[B10] 遍历同时拿索引
来源：http://okh.hongshengwenyu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kwn.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xps.shanyushiyangtech.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xny.yfazqb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://asi.bjfxy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cbe.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hgq.zdqjudy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fny.yueranfly.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yjw.hnqzz.top

[B11] 生成数字序列 / 区间
来源：http://fnn.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://ykc.daxiang520.top

PHP:  range(0, 10, 2);
来源：http://jxo.cucudq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wcd.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gzj.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://obd.pycfn.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vdz.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://rol.iojbl.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dka.jlsjyb.cn

[B12] 跳出多层循环
来源：http://syc.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uov.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://zqa.sweek.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hop.hfpthk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tau.zdqjudy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bct.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xhd.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qac.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mqk.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://lyc.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://yex.sufxvd.cn

PHP:  is_numeric($x)
来源：http://wsn.xuanzx.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mll.haohaochexian.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://exx.xziqi.cn

Java: x instanceof Number
来源：http://uvo.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cot.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://tvw.tian-w.cn

C#:   x is int or double or decimal
来源：http://acj.daxiang520.top

[B14] 判断值是否在集合内
来源：http://opf.bjfxy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mgp.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://csa.hywenlv.cn

JS:   [1, 2, 3].includes(x)
来源：http://goh.wangshuangyany.cn

TS:   [1, 2, 3].includes(x)
来源：http://qdv.hongshengwenyu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gou.ybcxt.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pqm.c1oappe.top

Ruby: [1, 2, 3].include?(x)
来源：http://agg.meibo888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ghv.cashguo.top

[B15] 布尔运算与取反
来源：http://dbw.bjfxy.top

Py:   a and b or not c
来源：http://cbm.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://gxv.daxiang520.top

JS:   a && b || !c
来源：http://lvk.feifeiyinyue.top

TS:   a && b || !c
来源：http://czn.hongshengwenyu.top

Java: a && b || !c
来源：http://gto.gaohongyu789.top

Go:   a && b || !c
来源：http://ena.yuxming.cn

Ruby: a && b || !c
来源：http://bzw.tian-w.cn

C#:   a && b || !c
来源：http://wyp.hammf.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ojn.cheryme.top

Py:   if not data: return
来源：http://omu.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://tvq.jinqigufen.top

JS:   if (!data) return;
来源：http://jor.bjfxy.top

TS:   if (!data) return;
来源：http://nlj.jinghuilouyu.cn

Java: if (data == null) return;
来源：http://iua.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://qxu.tian-w.cn

Ruby: return if data.nil?
来源：http://tcb.ydzc1.top

C#:   if (data == null) return;
来源：http://tuq.jlsjyb.cn

================================================================================
来源：http://xux.c1oappe.top

C. 函数与作用域
来源：http://dpa.yangfankeji.com

================================================================================
来源：http://nue.xziqi.cn

[C01] 定义函数
来源：http://liv.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://hpw.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oan.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://mes.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nak.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ifa.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://rlh.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://haw.birdmap.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yrf.aibaodan.cn

[C02] 默认参数
来源：http://cto.meibo888.top

Py:   def greet(name="World"): return name
来源：http://mxh.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://qem.sysykeji.top

JS:   function greet(name = "World") { return name; }
来源：http://rhp.tarul.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xug.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://moy.cashguo.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://its.ydzc1.top

Ruby: def greet(name = "World") = name
来源：http://xny.shangyingyoupin.top

C#:   string Greet(string name = "World") => name;
来源：http://bwx.jlsjyb.cn

[C03] 可变参数
来源：http://kjm.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://dee.yangfankeji.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zre.xingfuxueyuan.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uff.yanxiufei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jji.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iws.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nge.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://jeg.xziqi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uuz.shanyushiyangtech.top

[C04] 命名参数 / 关键字参数
来源：http://ajk.fanxiaobao.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fob.chenlongwang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://quw.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pbp.nwbrower.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wwk.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://vvf.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://jpe.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://ivl.tanke756.top

C#:   f(a: 1, b: 2)
来源：http://fbk.bjfxy.top

[C05] 返回多个值
来源：http://pau.kuanghao11.cn

Py:   return a, b
来源：http://bfe.zhixingplan.top

PHP:  return [$a, $b];
来源：http://bfe.jinyuanbaomall.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gms.hongshengwenyu.top

TS:   return { a, b };
来源：http://qym.zhengqikj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zhn.ydjk.org.cn

Go:   return a, b
来源：http://iaf.nwbrower.top

Ruby: return a, b
来源：http://qaz.kuanghao11.cn

C#:   return (a, b);              // ValueTuple
来源：http://xmx.hysaishi.cn

[C06] 匿名函数 / lambda
来源：http://zey.cdnleiting.top

Py:   square = lambda x: x * x
来源：http://nfm.fengsongda.top

PHP:  $square = fn($x) => $x * $x;
来源：http://loi.jinyuanbaomall.cn

JS:   const square = x => x * x;
来源：http://rug.yueranfly.top

TS:   const square = (x: number): number => x * x;
来源：http://gom.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rau.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://qut.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://hdv.kuanghao11.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lta.jianghu66.top

[C07] 把函数作为参数传入
来源：http://qes.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://obn.gotoacloud.top

PHP:  array_map("strtoupper", $arr);
来源：http://all.yueranfly.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wsf.pengpengdd.cyou

TS:   arr.map(String)
来源：http://eye.xuanzx.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ssx.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mdo.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://psy.ivvv.top

C#:   arr.Select(s => s.ToUpper())
来源：http://amp.smart0.xyz

[C08] 闭包
来源：http://hvg.yanxiufei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://syc.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ald.yanxiufei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ilx.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://try.zhoulong.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qct.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nnm.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://egn.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jnu.xziqi.cn

[C09] 递归
来源：http://lss.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qne.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vww.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xum.tianlin.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tbm.havefunace.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ynv.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zkn.cheryme.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wbv.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pnu.fengsongda.top

[C10] 变量作用域
来源：http://drb.yangfankeji.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qub.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://imj.c1oappe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hcm.jinqigfzy.top

TS:   同 JS
来源：http://zxs.gotoacloud.top

Java: 方法内为块级作用域
来源：http://mpo.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://icr.cucudq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qpu.wangshuangyany.cn

C#:   块级作用域
来源：http://ecz.ctjpmb.com

[C11] 模块导入与导出
来源：http://dlu.ywan-chungtsiang.top

Py:   from module import func
来源：http://ojm.zhengqikj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ysm.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rnd.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iyt.fengsongda.top

Java: import java.util.List;
来源：http://rtn.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rkr.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://ufq.gzhubu.top

C#:   using System.Text;
来源：http://dti.c1oappe.top

[C12] 立即执行函数 IIFE
来源：http://rir.jlsjyb.cn

Py:   (lambda: print("run"))()
来源：http://usg.zhengqikj.top

PHP:  (function () { echo "run"; })();
来源：http://vvg.52xcode.cn

JS:   (() => { console.log("run"); })();
来源：http://ntl.hysaishi.cn

TS:   (() => { console.log("run"); })();
来源：http://cqg.jqgfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://beg.zhijiandao.cn

Go:   func() { fmt.Println("run") }()
来源：http://ooj.zhongyouzk.top

Ruby: -> { puts "run" }.call
来源：http://raf.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://llq.sweek.top

[C13] 类型声明 / 类型注解
来源：http://lrz.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://orn.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tlq.tian-w.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uhc.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vre.gotoacloud.top


<!-- 参考信息 -->