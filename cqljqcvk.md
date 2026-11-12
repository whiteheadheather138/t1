代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://ayr.zdbjq.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mbb.aibaodan.cn

JS:   (3.14159).toFixed(2)
来源：http://epy.jinghuilouyu.cn

TS:   (3.14159).toFixed(2)
来源：http://yos.xziqi.cn

Java: String.format("%.2f", 3.14159)
来源：http://ivv.chenlongwang.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fcf.yangfankeji.com

Ruby: format("%.2f", 3.14159)
来源：http://klw.sjlbkw.cn

C#:   3.14159.ToString("F2")
来源：http://uji.yj20258.top

[A22] 获取字符串长度
来源：http://kzk.fengsongda.top

Py:   len(s)
来源：http://joh.quarkkingdee.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mpi.xuetiantiany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xpe.wangshuangyany.cn

TS:   s.length
来源：http://jtu.ppjwa.cn

Java: s.length()
来源：http://lsz.havefunace.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hup.sjlbkw.cn

Ruby: s.length
来源：http://zxx.guowangkeji.top

C#:   s.Length
来源：http://fmq.fktsv.cn

[A23] 大小写转换
来源：http://gsb.uphjek.com

Py:   s.upper(); s.lower(); s.title()
来源：http://zzg.52xcode.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gxo.jinqigfzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ycj.aizwys.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pzb.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wim.yj20258888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://apw.tarul.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gls.chenlongwang.top

C#:   s.ToUpper(); s.ToLower()
来源：http://uch.tarul.cn

[A24] 去除首尾空白
来源：http://xka.bbcook.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ajv.aizwys.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://scv.sufxvd.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ags.52xcode.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ugr.ywan-chungtsiang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tik.tianlin.xyz

Go:   strings.TrimSpace(s)
来源：http://yep.shanyushiyangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ujz.ydzc1.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ggm.mhx1999.top

[A25] 字符串比较
来源：http://jmg.shanyushiyangkeji.top

Py:   s1 == s2; s1 != s2
来源：http://act.daxiang520.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zla.yuxming.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dnl.aizwys.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oav.hnxiangtu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zjh.xuanzx.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qog.redwolf501.top

Ruby: s1 == s2; s1 <=> s2
来源：http://odn.zhongyouzk.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xvl.sysykeji.top

[A26] 类型转换总览
来源：http://zrg.nanxinkj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://idx.jiagoushi.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gvi.pycfn.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kiv.shanyushiyangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://vrh.snrcjt.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yet.zhoulong.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://myv.gogol.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zgk.feifeiyinyue.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tfo.uphjek.com

================================================================================
来源：http://nzt.52xcode.cn

B. 流程控制
来源：http://jaa.gzhubu.top

================================================================================
来源：http://ydk.hcnkem.com

[B01] 条件判断 if / else
来源：http://vvn.hywenlv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lyg.kuanghao11.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zkh.zhiwuduotai.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qcb.ybcxt.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pdc.hesvh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://roa.andypj.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kri.zhaomingkeji.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zgj.hnqzz.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qmg.gzhubu.top

[B02] 多分支 else if / elif
来源：http://eob.zhongyouzk.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bfy.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vtd.chenzaomai.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tbh.hcnkem.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wdw.shanyushiyangtech.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ofy.shangyingyoupin.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nkf.zhengqikj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ygk.ivvv.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rqf.jinqigfzy.top

[B03] switch / match / case
来源：http://cps.xuetiantiany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pmu.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sts.ybcxt.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mnv.9152youxi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://reh.xylfe.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fhv.wangdashe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://upf.yanxiufei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dop.birdmap.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tmo.fehbvm.com

[B04] for 计数循环
来源：http://ahw.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://bnp.chenlongwang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gkj.sjlbkw.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ghs.jinghuilouyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vtl.xingfuxueyuan.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hmy.hnqzz.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ayw.guannengcc.top

Ruby: 10.times { |i| puts i }
来源：http://kly.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://njt.sweek.top

[B05] 遍历数组 / 列表
来源：http://ieu.xuetiantiany.cn

Py:   for item in arr: print(item)
来源：http://yol.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bxb.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jdd.nwbrower.top

TS:   for (const item of arr) { console.log(item); }
来源：http://uzr.hfpthk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ifb.xinyue.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zqw.cheryme.top

Ruby: arr.each { |item| puts item }
来源：http://dcr.daxiang520.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://shq.feifeiyinyue.top

[B06] 遍历字典 / 对象
来源：http://teh.nanxinkj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cxs.mhx1999.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ery.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jpf.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://okm.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ggd.chenlongwang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yge.zhongyouzk.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kmo.yongpay.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kso.wangshuangyany.cn

[B07] while 循环
来源：http://hyt.snrcjt.cn

Py:   while i < 10: i += 1
来源：http://gsk.zhongyouzk.top

PHP:  while ($i < 10) { $i++; }
来源：http://hvk.hnxiangtu.top

JS:   while (i < 10) { i++; }
来源：http://jgc.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://ihk.fehbvm.com

Java: while (i < 10) { i++; }
来源：http://tcc.bbcook.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zgt.fktsv.cn

Ruby: while i < 10; i += 1; end
来源：http://znf.zhaomingkeji.xyz

C#:   while (i < 10) { i++; }
来源：http://gor.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://rdh.bjfxy.top

Py:   # 无 do-while：用 while True + break
来源：http://omr.pengpengdd.cyou

PHP:  do { $i++; } while ($i < 10);
来源：http://cki.gzhubu.top

JS:   do { i++; } while (i < 10);
来源：http://jux.aibaodan.cn

TS:   do { i++; } while (i < 10);
来源：http://bdw.redwolf501.top

Java: do { i++; } while (i < 10);
来源：http://zwe.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://otb.cucudq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wxm.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://dzy.yonumen.top

[B09] break 与 continue
来源：http://wix.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jej.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nkf.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rts.jinghuilouyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pxh.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xmt.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vwi.ybcxt.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wyu.dianchejie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gdt.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://xdv.bjfxy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eoe.gzhubu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zzb.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bxo.yuxming.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://liu.uphjek.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eld.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cbd.pengpengdd.cyou

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://doa.yonumen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hsr.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://iuc.9152youxi.cn

Py:   list(range(0, 10, 2))
来源：http://tzx.zdqjudy.top

PHP:  range(0, 10, 2);
来源：http://ave.bjfxy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ilw.kuanghao11.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cse.epnwcf.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qvy.yfazqb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xed.daria6918.cn

Ruby: (0...10).step(2).to_a
来源：http://sse.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ncl.zhongyouzk.top

[B12] 跳出多层循环
来源：http://azc.bbcook.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bmm.hesvh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cyw.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mzg.cqqwz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tor.sufxvd.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zrs.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://osg.zdqjudy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mag.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ykg.yuxming.cn

[B13] 判断是否为数字
来源：http://snf.yuxming.cn

Py:   isinstance(x, (int, float))
来源：http://lcr.jqgufenzy.top

PHP:  is_numeric($x)
来源：http://qur.dashuyun.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://utk.daria6918.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zui.hfpthk.cn

Java: x instanceof Number
来源：http://nfs.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ges.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://mec.pycfn.com

C#:   x is int or double or decimal
来源：http://bbx.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://pgb.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gwr.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ryl.daria6918.cn

JS:   [1, 2, 3].includes(x)
来源：http://zyj.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://bcf.jqgufenzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vat.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vww.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nsa.cqqwz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pyu.meibo888.top

[B15] 布尔运算与取反
来源：http://hpn.ppjwa.cn

Py:   a and b or not c
来源：http://zxd.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://jyi.xuanzx.com

JS:   a && b || !c
来源：http://dcf.hysaishi.cn

TS:   a && b || !c
来源：http://eej.tianlin.xyz

Java: a && b || !c
来源：http://dgk.hongshengwenyu.top

Go:   a && b || !c
来源：http://hkn.cashguo.top

Ruby: a && b || !c
来源：http://ucg.yj20258.top

C#:   a && b || !c
来源：http://yoq.jianghu66.top

[B16] 卫语句：不满足条件提前返回
来源：http://vwp.svipenyu.cn

Py:   if not data: return
来源：http://btp.aibaodan.cn

PHP:  if (!$data) { return; }
来源：http://koc.birdmap.top

JS:   if (!data) return;
来源：http://lam.jlsjyb.cn

TS:   if (!data) return;
来源：http://cru.c1oappe.top

Java: if (data == null) return;
来源：http://npv.smart0.xyz

Go:   if data == nil { return }
来源：http://jqg.zhijiandao.cn

Ruby: return if data.nil?
来源：http://pzo.hnxiangtu.top

C#:   if (data == null) return;
来源：http://yum.hfpthk.cn

================================================================================
来源：http://hbp.jinghuilouyu.cn

C. 函数与作用域
来源：http://lbx.redwolf501.top

================================================================================
来源：http://ejf.zhoulong.xyz

[C01] 定义函数
来源：http://dxv.cucudq.cn

Py:   def add(a, b): return a + b
来源：http://gvb.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ndm.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://zgz.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yee.gogol.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dln.yfazqb.com

Go:   func add(a, b int) int { return a + b }
来源：http://hjz.fzhhl.top

Ruby: def add(a, b); a + b; end
来源：http://spi.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ith.shzxlz.cn

[C02] 默认参数
来源：http://dkm.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://evq.52xcode.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tzi.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://jcq.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gja.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uxr.xuanzx.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sld.fktsv.cn

Ruby: def greet(name = "World") = name
来源：http://cxh.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://isc.nanxinkj.top

[C03] 可变参数
来源：http://mkj.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://ctn.andypj.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fju.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ikm.jiagoushi.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rdt.jinghuilouyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bsw.aibaodan.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zef.aibaodan.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pzl.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dxp.yonumen.top

[C04] 命名参数 / 关键字参数
来源：http://fkv.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ghd.fzhhl.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jjx.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jon.sjlbkw.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cqb.52xcode.cn

Java: // 无：用 Builder 模式或 record
来源：http://uue.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://dhr.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://nno.daxiang520.top

C#:   f(a: 1, b: 2)
来源：http://fcw.ehwqpu.com

[C05] 返回多个值
来源：http://wlp.jiagoushi.top

Py:   return a, b
来源：http://ezl.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://sbt.yongpay.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://aow.cdnleiting.top

TS:   return { a, b };
来源：http://qaf.fengsongda.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pee.hongshengwenyu.top

Go:   return a, b
来源：http://dsb.gaohongyu789.top

Ruby: return a, b
来源：http://cqh.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://mkw.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://keu.yfazqb.com

Py:   square = lambda x: x * x
来源：http://eus.yj20258.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hwi.redwolf501.top

JS:   const square = x => x * x;
来源：http://hoq.316326.xyz

TS:   const square = (x: number): number => x * x;
来源：http://flz.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xqj.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://mht.ppjwa.cn

Ruby: square = ->(x) { x * x }
来源：http://qge.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://gmr.cashguo.top

[C07] 把函数作为参数传入
来源：http://zrw.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pgm.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gqq.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ffh.zycfv.cn

TS:   arr.map(String)
来源：http://fhk.jinyuanbaomall.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jma.iojbl.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jme.dianchejie.cn

Ruby: arr.map(&:upcase)
来源：http://lbi.dashuyun.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dnk.yanxiufei.cn

[C08] 闭包
来源：http://tke.hammf.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xyi.hysaishi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yvz.zhoulong.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lga.nanxinkj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yio.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yks.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ibb.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nij.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nrp.jqgfzy.top

[C09] 递归
来源：http://fsh.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dzn.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sff.xuanzx.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cht.kuanghao11.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nqn.zdbjq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qwm.yj20258888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qpy.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uqf.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jed.vehdjk.com

[C10] 变量作用域
来源：http://ztj.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yqk.yj202588.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://prz.yangfankeji.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gvr.jyoumei.cn

TS:   同 JS
来源：http://sim.tian-w.cn

Java: 方法内为块级作用域
来源：http://ilz.jiagoushi.top

Go:   花括号块级作用域
来源：http://ylw.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dkl.meibo888.top

C#:   块级作用域
来源：http://qrc.shanyushiyangtech.top

[C11] 模块导入与导出
来源：http://jkz.xingfuxueyuan.xyz

Py:   from module import func
来源：http://muf.sweek.top

PHP:  require "file.php";  或 use App\Service;
来源：http://myu.tianlin.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://lti.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kbw.jiagoushi.top

Java: import java.util.List;
来源：http://qnr.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://thj.zhengqikj.top


<!-- 参考信息 -->