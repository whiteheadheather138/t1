代发 wailian999

C#:   s.Length
来源：http://cgk.uphjek.com

[A23] 大小写转换
来源：http://fqw.bjfxy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://szw.zhoulong.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uds.hfpthk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bmn.zhengqikj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vyo.xuanzx.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ebu.daria6918.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kfe.fktsv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sgj.xuetiantiany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ffv.hysaishi.cn

[A24] 去除首尾空白
来源：http://slg.ctjpmb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qbw.yj20258888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gvi.tarul.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bzk.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fdk.yanxiufei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://raa.ydjk.org.cn

Go:   strings.TrimSpace(s)
来源：http://itk.yfazqb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xdf.yfazqb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://amm.cdnleiting.top

[A25] 字符串比较
来源：http://plp.jiagoushi.top

Py:   s1 == s2; s1 != s2
来源：http://ubh.fanxiaobao.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hxd.shangyingyoupin.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ern.pycfn.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wsr.hnqzz.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ues.yanxiufei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zby.tanke756.top

Ruby: s1 == s2; s1 <=> s2
来源：http://uju.zhaomingkeji.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tio.jinqigfzy.top

[A26] 类型转换总览
来源：http://xyv.hnxiangtu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zkd.jinqigfzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ijp.cdnleiting.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hie.svipenyu.cn

TS:   Number() String() Boolean() x as number
来源：http://wdc.jyoumei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://obp.ywan-chungtsiang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ykn.yonumen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vzw.jianghu66.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wsw.zhaomingkeji.xyz

================================================================================
来源：http://wml.c1oappe.top

B. 流程控制
来源：http://arz.jinqigufen.top

================================================================================
来源：http://bxy.yuxming.cn

[B01] 条件判断 if / else
来源：http://hbm.gogol.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rim.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zfz.52xcode.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vnw.yonumen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kxl.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ose.daria6918.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ahv.pengpengdd.cyou

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ijx.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nix.chenzaomai.com

[B02] 多分支 else if / elif
来源：http://kpg.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ive.316326.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kay.hcnkem.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dfv.pengpengdd.cyou

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pae.dianchejie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kfj.nanxuanxn.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://amz.svipenyu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ivm.jqgufenzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mey.hysaishi.cn

[B03] switch / match / case
来源：http://hcz.ctjpmb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://izb.xuetiantiany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eud.fanxiaobao.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wdd.yangfankeji.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ueo.ppjwa.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jsj.yj202588.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sdg.tian-w.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ili.daxiang520.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qrm.feifeiyinyue.top

[B04] for 计数循环
来源：http://cdl.nwbrower.top

Py:   for i in range(10): print(i)
来源：http://zxo.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bza.hnqzz.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wgm.pengpengdd.cyou

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xeo.ppjwa.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://njg.cqqwz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tbh.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://evm.ctjpmb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mxm.cucudq.cn

[B05] 遍历数组 / 列表
来源：http://dsm.hywenlv.cn

Py:   for item in arr: print(item)
来源：http://kpv.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zow.fengsongda.top

JS:   for (const item of arr) { console.log(item); }
来源：http://sdw.gzhubu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hvm.0kj1m.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sdp.ivvv.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tfv.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://yag.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lac.jianghu66.top

[B06] 遍历字典 / 对象
来源：http://awv.cashguo.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kwo.uphjek.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://owp.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nlf.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vnp.dashuyun.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://buu.yonumen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ovb.ydzc1.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pbg.iojbl.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pgv.fanxiaobao.xyz

[B07] while 循环
来源：http://vqq.jinyuanbaomall.cn

Py:   while i < 10: i += 1
来源：http://cbs.sjlbkw.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rxx.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://yhp.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://viv.bjfxy.top

Java: while (i < 10) { i++; }
来源：http://crj.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nnl.xingfuxueyuan.xyz

Ruby: while i < 10; i += 1; end
来源：http://mcj.feifeiyinyue.top

C#:   while (i < 10) { i++; }
来源：http://gci.aizwys.cn

[B08] do-while（至少执行一次）
来源：http://sjk.dianchejie.cn

Py:   # 无 do-while：用 while True + break
来源：http://tyz.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gmk.shuidangran.top

JS:   do { i++; } while (i < 10);
来源：http://bmy.ydjk.org.cn

TS:   do { i++; } while (i < 10);
来源：http://udr.chenlongwang.top

Java: do { i++; } while (i < 10);
来源：http://uns.hesvh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fxm.dashuyun.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gtj.yanxiufei.cn

C#:   do { i++; } while (i < 10);
来源：http://gzf.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://fnk.xinyue.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ffi.jianghu66.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zth.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mrf.jianghu66.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rth.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bec.zhiwuduotai.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ind.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://skp.ywan-chungtsiang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pvi.zhixingplan.top

[B10] 遍历同时拿索引
来源：http://mny.chenzaomai.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fyo.andypj.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ryf.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ovt.jqgfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tpf.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mwo.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jcq.hnxiangtu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kph.fehbvm.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gvq.hfpthk.cn

[B11] 生成数字序列 / 区间
来源：http://dmf.chenlongwang.top

Py:   list(range(0, 10, 2))
来源：http://qxi.ydjk.org.cn

PHP:  range(0, 10, 2);
来源：http://inn.vehdjk.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mdj.yj20258888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rcv.yonumen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jfg.hnxiangtu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://apw.andypj.xyz

Ruby: (0...10).step(2).to_a
来源：http://sxh.hcnkem.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qxg.hnqzz.top

[B12] 跳出多层循环
来源：http://vxi.zhongyouzk.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kxj.0kj1m.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ewm.ydjk.org.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xop.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iao.gogol.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mjo.yj20258888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ene.ydjk.org.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yvy.redwolf501.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hyh.mhx1999.top

[B13] 判断是否为数字
来源：http://wtj.gotoacloud.top

Py:   isinstance(x, (int, float))
来源：http://lnc.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://pgy.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yag.yj20258888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://auy.quarkkingdee.top

Java: x instanceof Number
来源：http://rbf.tianlin.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yjl.ywan-chungtsiang.top

Ruby: x.is_a?(Numeric)
来源：http://lvm.bjfxy.top

C#:   x is int or double or decimal
来源：http://jek.jinyuanbaomall.cn

[B14] 判断值是否在集合内
来源：http://rht.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nbo.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wjq.hnqzz.top

JS:   [1, 2, 3].includes(x)
来源：http://nkz.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://vbs.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fqi.jqgfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hwz.fzhhl.top

Ruby: [1, 2, 3].include?(x)
来源：http://wtj.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rks.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://vuz.zhiwuduotai.top

Py:   a and b or not c
来源：http://hbx.xuetiantiany.cn

PHP:  $a && $b || !$c
来源：http://ipx.shzxlz.cn

JS:   a && b || !c
来源：http://fxd.sjlbkw.cn

TS:   a && b || !c
来源：http://noi.jqgufenzy.top

Java: a && b || !c
来源：http://uyf.cdnleiting.top

Go:   a && b || !c
来源：http://pnk.ppjwa.cn

Ruby: a && b || !c
来源：http://dcf.yonumen.top

C#:   a && b || !c
来源：http://zjg.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://pqj.dianchejie.cn

Py:   if not data: return
来源：http://zgx.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://iel.sufxvd.cn

JS:   if (!data) return;
来源：http://fci.haohaochexian.top

TS:   if (!data) return;
来源：http://vlq.redwolf501.top

Java: if (data == null) return;
来源：http://agt.nanxinkj.top

Go:   if data == nil { return }
来源：http://omm.ydzc1.top

Ruby: return if data.nil?
来源：http://adx.gotoacloud.top

C#:   if (data == null) return;
来源：http://zai.dianchejie.cn

================================================================================
来源：http://pog.pycfn.com

C. 函数与作用域
来源：http://eup.aizwys.cn

================================================================================
来源：http://qku.gogol.net.cn

[C01] 定义函数
来源：http://kjt.xuanzx.com

Py:   def add(a, b): return a + b
来源：http://sua.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://goe.wangdashe.top

JS:   function add(a, b) { return a + b; }
来源：http://kbb.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yoz.tian-w.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dxe.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vrm.ybcxt.top

Ruby: def add(a, b); a + b; end
来源：http://upq.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mxo.guowangkeji.top

[C02] 默认参数
来源：http://iva.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://urt.xziqi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ydg.birdmap.top

JS:   function greet(name = "World") { return name; }
来源：http://bwe.gzhubu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hjh.c1oappe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://iww.hywenlv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://otb.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://lww.ydjk.org.cn

C#:   string Greet(string name = "World") => name;
来源：http://rev.pycfn.com

[C03] 可变参数
来源：http://ukd.sysykeji.top

Py:   def total(*args): return sum(args)
来源：http://abd.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wyr.jinyuanbaomall.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://upg.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://edp.sweek.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jmj.cqqwz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jrm.cdnleiting.top

Ruby: def total(*nums); nums.sum; end
来源：http://mor.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://efm.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://hxy.bbcook.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wpw.gogol.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wmt.hcnkem.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qhq.redwolf501.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vcy.ehwqpu.com

Java: // 无：用 Builder 模式或 record
来源：http://zjo.hammf.cn

Go:   // 无：用配置结构体参数
来源：http://vav.xylfe.cn

Ruby: f(a: 1, b: 2)
来源：http://xpt.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://but.yj202588.top

[C05] 返回多个值
来源：http://bam.jianghu66.top

Py:   return a, b
来源：http://elt.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://cws.zhongyouzk.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hnz.yueranfly.top

TS:   return { a, b };
来源：http://vux.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://weq.pycfn.com

Go:   return a, b
来源：http://hbj.nanxinkj.top

Ruby: return a, b
来源：http://skz.hysaishi.cn

C#:   return (a, b);              // ValueTuple
来源：http://ove.yfazqb.com

[C06] 匿名函数 / lambda
来源：http://fyk.shanyushiyangtech.top

Py:   square = lambda x: x * x
来源：http://xut.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yli.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://cre.svipenyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://iuw.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bqb.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nwf.yangfankeji.com

Ruby: square = ->(x) { x * x }
来源：http://kub.0kj1m.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ntm.haohaochexian.top

[C07] 把函数作为参数传入
来源：http://png.meibo888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dfg.xuetiantiany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vol.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uvp.hongshengwenyu.top

TS:   arr.map(String)
来源：http://xrj.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://din.jqgufenzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://edz.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://bim.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://cwn.hywenlv.cn

[C08] 闭包
来源：http://zrt.iojbl.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aqn.fanxiaobao.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pln.jinyuanbaomall.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zrx.zdqjudy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dpl.feifeiyinyue.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nkl.wangdashe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ypb.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fbl.ivvv.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gaf.ehwqpu.com

[C09] 递归
来源：http://aql.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nyf.dianchejie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fvd.jinqigfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dae.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fgo.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uso.guowangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cjj.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lwp.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dym.zhijiandao.cn

[C10] 变量作用域
来源：http://azk.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hfl.zhijiandao.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://thg.hnxiangtu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gik.wangshuangyany.cn

TS:   同 JS
来源：http://gtc.zhiwuduotai.top

Java: 方法内为块级作用域
来源：http://afj.zhoulong.xyz

Go:   花括号块级作用域
来源：http://huf.hongshengwenyu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://omy.jyoumei.cn

C#:   块级作用域
来源：http://lmi.yj202588.top

[C11] 模块导入与导出
来源：http://vte.jinyuanbaomall.cn

Py:   from module import func
来源：http://qcy.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ryv.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://szc.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uez.pengpengdd.cyou

Java: import java.util.List;
来源：http://ezk.haohaochexian.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tfn.xuanzx.com

Ruby: require "json"; require_relative "./util"
来源：http://wxk.xuetiantiany.cn

C#:   using System.Text;
来源：http://bpy.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://iij.tarul.cn

Py:   (lambda: print("run"))()
来源：http://blg.xuanzx.com

PHP:  (function () { echo "run"; })();
来源：http://ark.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://mhp.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://xoc.xylfe.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oqb.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://wxf.daxiang520.top

Ruby: -> { puts "run" }.call
来源：http://ulk.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qyj.yueranfly.top

[C13] 类型声明 / 类型注解
来源：http://fxg.wangdashe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vhl.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://idf.316326.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dvh.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cnu.smart0.xyz


<!-- 参考信息 -->