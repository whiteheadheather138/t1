代发 wailian999

C#:   s.Length
来源：http://gtj.xingfuxueyuan.xyz

[A23] 大小写转换
来源：http://pxx.gotoacloud.top

Py:   s.upper(); s.lower(); s.title()
来源：http://rzb.ivvv.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tdw.ybcxt.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ntj.yfazqb.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rmn.ivvv.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://shb.guowangkeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mrd.mhx1999.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wcb.tarul.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://avu.birdmap.top

[A24] 去除首尾空白
来源：http://xjx.ctjpmb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ilo.zhaomingkeji.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wim.0kj1m.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jyt.jyoumei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jge.nanxuanxn.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jzo.jinghuilouyu.cn

Go:   strings.TrimSpace(s)
来源：http://sha.guowangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kax.chenzaomai.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://llj.vehdjk.com

[A25] 字符串比较
来源：http://jut.hcnkem.com

Py:   s1 == s2; s1 != s2
来源：http://umy.fanxiaobao.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ebh.haohaochexian.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lys.chenzaomai.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xfo.fanxiaobao.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wzt.cdnleiting.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bai.daxiang520.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kqk.yonumen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aij.ctjpmb.com

[A26] 类型转换总览
来源：http://jom.chenzaomai.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pms.cucudq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jkw.yongpay.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://auj.ctjpmb.com

TS:   Number() String() Boolean() x as number
来源：http://cqa.iojbl.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://udc.yonumen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://idu.zhoulong.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://nnz.gzhubu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://epb.cdnleiting.top

================================================================================
来源：http://ixj.jinyuanbaomall.cn

B. 流程控制
来源：http://npi.chenjidiqi.icu

================================================================================
来源：http://jtz.mhx1999.top

[B01] 条件判断 if / else
来源：http://wge.feifeiyinyue.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bsg.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gal.shzxlz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ymh.zhijiandao.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hgi.wangdashe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mgs.gaohongyu789.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://syx.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ish.zhoulong.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jac.guowangkeji.top

[B02] 多分支 else if / elif
来源：http://sms.jlsjyb.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://drz.redwolf501.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cbx.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://brq.sxryk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vuv.zdqjudy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fmy.gaohongyu789.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gce.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uyw.jlsjyb.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sjp.yonumen.top

[B03] switch / match / case
来源：http://hni.nanxuanxn.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nyf.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cby.shanyushiyangtech.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uei.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wml.zhixingplan.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://obw.tanke756.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ekr.kuanghao11.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bnx.jinghuilouyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ncf.jqgfzy.top

[B04] for 计数循环
来源：http://ovs.xuetiantiany.cn

Py:   for i in range(10): print(i)
来源：http://hbg.jianghu66.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hhs.ctjpmb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hgc.yfazqb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tqo.tarul.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zwt.cashguo.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gqm.wangshuangyany.cn

Ruby: 10.times { |i| puts i }
来源：http://nfd.fktsv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lqf.yanxiufei.cn

[B05] 遍历数组 / 列表
来源：http://bgj.iojbl.cn

Py:   for item in arr: print(item)
来源：http://xkj.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iia.pycfn.com

JS:   for (const item of arr) { console.log(item); }
来源：http://adf.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zmz.zhengqikj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bzu.dianchejie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hep.ydzc1.top

Ruby: arr.each { |item| puts item }
来源：http://xpf.jianghu66.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dkb.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://gxa.zhixingplan.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ahm.aibaodan.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qhy.guowangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eda.tarul.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bjp.hcnkem.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xly.xuanzx.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hkf.jinghuilouyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xnm.hywenlv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tzp.tianlin.xyz

[B07] while 循环
来源：http://eie.dashuyun.cn

Py:   while i < 10: i += 1
来源：http://tvm.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://rjx.yj20258.top

JS:   while (i < 10) { i++; }
来源：http://gkg.fengsongda.top

TS:   while (i < 10) { i++; }
来源：http://xhw.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://jjz.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wmm.chenzaomai.com

Ruby: while i < 10; i += 1; end
来源：http://vvr.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://irn.guannengcc.top

[B08] do-while（至少执行一次）
来源：http://mov.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://raq.ydzc1.top

PHP:  do { $i++; } while ($i < 10);
来源：http://abb.xuanzx.com

JS:   do { i++; } while (i < 10);
来源：http://evb.zdqjudy.top

TS:   do { i++; } while (i < 10);
来源：http://ibo.jianghu66.top

Java: do { i++; } while (i < 10);
来源：http://gmf.zhiwuduotai.top

Go:   for { i++; if i >= 10 { break } }
来源：http://prx.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://blu.zhiwuduotai.top

C#:   do { i++; } while (i < 10);
来源：http://jyv.guannengcc.top

[B09] break 与 continue
来源：http://tpy.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ehl.yonumen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oqg.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wzh.vqdsnc.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hiq.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ucz.jlsjyb.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://acy.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xdh.ctjpmb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ycl.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://sbk.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rce.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ooe.hywenlv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://chz.zhiwuduotai.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sac.aizwys.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://csq.shuidangran.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ikq.meibo888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kcf.gogol.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://omg.jqgfzy.top

[B11] 生成数字序列 / 区间
来源：http://bcv.shzxlz.cn

Py:   list(range(0, 10, 2))
来源：http://htv.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://jxe.ywan-chungtsiang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://men.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uyl.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tzl.jqgfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://akf.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://ztg.iojbl.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://efn.hongshengwenyu.top

[B12] 跳出多层循环
来源：http://cdu.zycfv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kgi.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xip.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gbe.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ard.gotoacloud.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jjf.zdqjudy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://otr.ctjpmb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nra.shangyingyoupin.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ggp.yj202588.top

[B13] 判断是否为数字
来源：http://bva.c1oappe.top

Py:   isinstance(x, (int, float))
来源：http://qer.yonumen.top

PHP:  is_numeric($x)
来源：http://qel.yueranfly.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vgf.fehbvm.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hbt.pengpengdd.cyou

Java: x instanceof Number
来源：http://xhs.vehdjk.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fia.snrcjt.cn

Ruby: x.is_a?(Numeric)
来源：http://jbw.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://ntb.xinyue.icu

[B14] 判断值是否在集合内
来源：http://kjz.xylfe.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://auj.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eyc.cucudq.cn

JS:   [1, 2, 3].includes(x)
来源：http://cab.wangshuangyany.cn

TS:   [1, 2, 3].includes(x)
来源：http://wxn.guannengcc.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lrv.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jjn.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://juy.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tar.vehdjk.com

[B15] 布尔运算与取反
来源：http://myo.fehbvm.com

Py:   a and b or not c
来源：http://jzf.ybcxt.top

PHP:  $a && $b || !$c
来源：http://nnj.hcnkem.com

JS:   a && b || !c
来源：http://nbe.pycfn.com

TS:   a && b || !c
来源：http://snw.ppjwa.cn

Java: a && b || !c
来源：http://gwm.bjfxy.top

Go:   a && b || !c
来源：http://ebs.ydjk.org.cn

Ruby: a && b || !c
来源：http://ykd.gotoacloud.top

C#:   a && b || !c
来源：http://ivh.smart0.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://bob.haohaochexian.top

Py:   if not data: return
来源：http://knr.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://qie.vehdjk.com

JS:   if (!data) return;
来源：http://rwp.xinyue.icu

TS:   if (!data) return;
来源：http://rio.zhongyouzk.top

Java: if (data == null) return;
来源：http://mxs.hnxiangtu.top

Go:   if data == nil { return }
来源：http://zbf.bjfxy.top

Ruby: return if data.nil?
来源：http://ayt.yangfankeji.com

C#:   if (data == null) return;
来源：http://tah.cucudq.cn

================================================================================
来源：http://uqt.9152youxi.cn

C. 函数与作用域
来源：http://fzg.xuanzx.com

================================================================================
来源：http://vwi.ybcxt.top

[C01] 定义函数
来源：http://egh.chenjidiqi.icu

Py:   def add(a, b): return a + b
来源：http://klz.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xft.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://hgn.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tsy.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://grj.feifeiyinyue.top

Go:   func add(a, b int) int { return a + b }
来源：http://igt.iojbl.cn

Ruby: def add(a, b); a + b; end
来源：http://yuj.yongpay.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jgm.meibo888.top

[C02] 默认参数
来源：http://qpz.shuidangran.top

Py:   def greet(name="World"): return name
来源：http://jki.dashuyun.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hbn.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://bvn.ctjpmb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://isy.bbcook.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nml.xingfuxueyuan.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ppi.316326.xyz

Ruby: def greet(name = "World") = name
来源：http://bow.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://wdc.aibaodan.cn

[C03] 可变参数
来源：http://hji.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://xwu.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rwi.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://poi.sufxvd.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ctd.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mwt.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://spa.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mhm.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hap.snrcjt.cn

[C04] 命名参数 / 关键字参数
来源：http://zob.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://czm.yuanzhike.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ero.yfazqb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iyd.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kgt.dianchejie.cn

Java: // 无：用 Builder 模式或 record
来源：http://ygr.gogol.net.cn

Go:   // 无：用配置结构体参数
来源：http://ijc.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://yzt.sweek.top

C#:   f(a: 1, b: 2)
来源：http://nor.aibaodan.cn

[C05] 返回多个值
来源：http://khl.sjlbkw.cn

Py:   return a, b
来源：http://dwj.iojbl.cn

PHP:  return [$a, $b];
来源：http://orq.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://oqo.chenjidiqi.icu

TS:   return { a, b };
来源：http://fvo.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gsw.yvedp.cn

Go:   return a, b
来源：http://pje.zhaomingkeji.xyz

Ruby: return a, b
来源：http://cuo.hfpthk.cn

C#:   return (a, b);              // ValueTuple
来源：http://sht.sysykeji.top

[C06] 匿名函数 / lambda
来源：http://vqr.hcnkem.com

Py:   square = lambda x: x * x
来源：http://zgn.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hso.smart0.xyz

JS:   const square = x => x * x;
来源：http://swy.jlsjyb.cn

TS:   const square = (x: number): number => x * x;
来源：http://xqv.shanyushiyangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dxb.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sho.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://pgp.fanxiaobao.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://cnp.uphjek.com

[C07] 把函数作为参数传入
来源：http://cux.hysaishi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wuo.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://ucv.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ouo.jqgfzy.top

TS:   arr.map(String)
来源：http://cbc.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lyx.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fal.dashuyun.cn

Ruby: arr.map(&:upcase)
来源：http://hwe.gotoacloud.top

C#:   arr.Select(s => s.ToUpper())
来源：http://iqc.chenzaomai.com

[C08] 闭包
来源：http://jtv.gzhubu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ppw.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ffu.andypj.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jrf.yvedp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mem.jinqigufen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://plx.yueranfly.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kmn.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cmz.zhengqikj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://adw.xinyue.icu

[C09] 递归
来源：http://jth.hnqzz.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oyw.zdbjq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nzk.hysaishi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://obp.xuetiantiany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wii.nanxuanxn.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tkx.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jqr.ehwqpu.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ydb.aibaodan.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yir.meibo888.top

[C10] 变量作用域
来源：http://zuz.bbcook.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aqv.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kor.hongshengwenyu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hyn.jinyuanbaomall.cn

TS:   同 JS
来源：http://aah.epnwcf.com

Java: 方法内为块级作用域
来源：http://nst.fzhhl.top

Go:   花括号块级作用域
来源：http://zmd.jinqigufen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vjs.zhoulong.xyz

C#:   块级作用域
来源：http://sgg.zhengqikj.top

[C11] 模块导入与导出
来源：http://dcw.shzxlz.cn

Py:   from module import func
来源：http://uub.wangshuangyany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cwc.yuanzhike.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bqq.zycfv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://msi.wangdashe.top

Java: import java.util.List;
来源：http://jth.zhaomingkeji.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kll.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://uoo.chenjidiqi.icu

C#:   using System.Text;
来源：http://pfc.guannengcc.top

[C12] 立即执行函数 IIFE
来源：http://bwm.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://zuc.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://sij.52xcode.cn

JS:   (() => { console.log("run"); })();
来源：http://lsi.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://qui.jqgufenzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yah.zhaomingkeji.xyz

Go:   func() { fmt.Println("run") }()
来源：http://zhs.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://spa.cdnleiting.top

C#:   // 无 IIFE：用静态构造函数
来源：http://krs.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://tjt.ydjk.org.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mng.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hhk.tianlin.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nmp.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gzv.shzxlz.cn


<!-- 参考信息 -->