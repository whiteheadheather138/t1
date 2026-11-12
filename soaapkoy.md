代发 wailian999

[A22] 获取字符串长度
来源：http://hme.wangshuangyany.cn

Py:   len(s)
来源：http://dbf.fzhhl.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://prl.cashguo.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nqg.hfpthk.cn

TS:   s.length
来源：http://vin.bbcook.cn

Java: s.length()
来源：http://cun.gzhubu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vnd.smart0.xyz

Ruby: s.length
来源：http://zyd.fktsv.cn

C#:   s.Length
来源：http://rew.quarkkingdee.top

[A23] 大小写转换
来源：http://bec.zhaomingkeji.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://vuu.dianchejie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cap.pycfn.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fji.xziqi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uta.uphjek.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ijz.jinyuanbaomall.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vyt.tarul.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://znj.sxryk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cdp.xuanzx.com

[A24] 去除首尾空白
来源：http://ggd.yuanzhike.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yba.yj20258888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nmx.yj20258888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rfq.shangyingyoupin.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://epp.quarkkingdee.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rzo.kuanghao11.cn

Go:   strings.TrimSpace(s)
来源：http://usg.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ryl.fengsongda.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ugd.shanyushiyangkeji.top

[A25] 字符串比较
来源：http://qjo.chenlongwang.top

Py:   s1 == s2; s1 != s2
来源：http://tim.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://brw.cheryme.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zsx.hywenlv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zni.0kj1m.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zts.fehbvm.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qmi.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://xmv.uphjek.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ksy.havefunace.top

[A26] 类型转换总览
来源：http://gsq.zdbjq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fuu.zhixingplan.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wlv.jiagoushi.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dlw.jqgufenzy.top

TS:   Number() String() Boolean() x as number
来源：http://ayh.yanxiufei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qzn.aizwys.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aoq.daxiang520.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jub.xingfuxueyuan.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dzm.meibo888.top

================================================================================
来源：http://ufr.sweek.top

B. 流程控制
来源：http://foo.epnwcf.com

================================================================================
来源：http://xza.xuetiantiany.cn

[B01] 条件判断 if / else
来源：http://any.yuanzhike.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xio.hcnkem.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ntm.aizwys.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xxw.zhoulong.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://shg.havefunace.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fiu.zhaomingkeji.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://afj.ybcxt.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hfv.nwbrower.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xyu.shanyushiyangtech.top

[B02] 多分支 else if / elif
来源：http://evf.zhiwuduotai.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hrc.yonumen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qhg.ydjk.org.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbq.hysaishi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dyf.chenzaomai.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bws.jiagoushi.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://imw.jqgufenzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://drl.fehbvm.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://njd.xylfe.cn

[B03] switch / match / case
来源：http://hpc.hnqzz.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qvy.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oco.guannengcc.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bgx.zhaomingkeji.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uda.zhaomingkeji.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qmk.ctjpmb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sdj.cashguo.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aod.gogol.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://awz.jqgufenzy.top

[B04] for 计数循环
来源：http://gzx.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://ikr.jinqigufen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jti.zhixingplan.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ano.yj20258888.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jtw.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mou.ehwqpu.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tbg.xinyue.icu

Ruby: 10.times { |i| puts i }
来源：http://vey.vehdjk.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rco.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://asy.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://msy.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vbj.daxiang520.top

JS:   for (const item of arr) { console.log(item); }
来源：http://uoo.hnxiangtu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rcy.cucudq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fqa.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nmo.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://bjl.wangdashe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pqg.kuanghao11.cn

[B06] 遍历字典 / 对象
来源：http://wkl.nwbrower.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mlu.hnxiangtu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tdo.tarul.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kkx.zhoulong.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jsj.uphjek.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pfo.jinqigufen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nil.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gwo.iojbl.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tij.gaohongyu789.top

[B07] while 循环
来源：http://fyu.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://mwx.gogol.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iak.nanxuanxn.top

JS:   while (i < 10) { i++; }
来源：http://gwb.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://qsi.zhixingplan.top

Java: while (i < 10) { i++; }
来源：http://lop.chenjidiqi.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://njm.daxiang520.top

Ruby: while i < 10; i += 1; end
来源：http://ole.andypj.xyz

C#:   while (i < 10) { i++; }
来源：http://ccv.shanyushiyangkeji.top

[B08] do-while（至少执行一次）
来源：http://ees.gogol.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://flp.hnxiangtu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zif.xinyue.icu

JS:   do { i++; } while (i < 10);
来源：http://uom.tanke756.top

TS:   do { i++; } while (i < 10);
来源：http://gou.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://wzd.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lfh.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iiw.zhijiandao.cn

C#:   do { i++; } while (i < 10);
来源：http://lmz.hysaishi.cn

[B09] break 与 continue
来源：http://pwh.redwolf501.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wxb.xingfuxueyuan.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jek.jianghu66.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qzs.snrcjt.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gfy.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fqv.shangyingyoupin.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tyw.chenzaomai.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qgx.sxryk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bqd.yj20258888.top

[B10] 遍历同时拿索引
来源：http://bbt.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pkf.ivvv.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bfc.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kgw.ctjpmb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bke.hfpthk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ypz.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pql.redwolf501.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hwe.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mgz.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://fcl.xingfuxueyuan.xyz

Py:   list(range(0, 10, 2))
来源：http://dlp.dianchejie.cn

PHP:  range(0, 10, 2);
来源：http://npa.gzhubu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bsn.xingfuxueyuan.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xsn.jinqigufen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sld.wangdashe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://syn.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://swl.haohaochexian.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ljg.uphjek.com

[B12] 跳出多层循环
来源：http://rvs.xuanzx.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://cyk.hammf.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://umq.sjlbkw.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ojq.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nxf.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://chq.hysaishi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zpa.nwbrower.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sng.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://paa.meibo888.top

[B13] 判断是否为数字
来源：http://cub.uphjek.com

Py:   isinstance(x, (int, float))
来源：http://fdl.yangfankeji.com

PHP:  is_numeric($x)
来源：http://ovv.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://coc.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mnx.hywenlv.cn

Java: x instanceof Number
来源：http://vpr.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://brl.yfazqb.com

Ruby: x.is_a?(Numeric)
来源：http://fdj.zhijiandao.cn

C#:   x is int or double or decimal
来源：http://dxx.xuanzx.com

[B14] 判断值是否在集合内
来源：http://qdh.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sie.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dwv.ppjwa.cn

JS:   [1, 2, 3].includes(x)
来源：http://hrs.guowangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://rsu.cashguo.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tbq.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lav.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://ehp.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://joj.sufxvd.cn

[B15] 布尔运算与取反
来源：http://inn.tarul.cn

Py:   a and b or not c
来源：http://nqo.meibo888.top

PHP:  $a && $b || !$c
来源：http://htx.hywenlv.cn

JS:   a && b || !c
来源：http://spt.zhaomingkeji.xyz

TS:   a && b || !c
来源：http://wzw.smart0.xyz

Java: a && b || !c
来源：http://wgd.gogol.net.cn

Go:   a && b || !c
来源：http://xei.jinqigfzy.top

Ruby: a && b || !c
来源：http://wvq.zhengqikj.top

C#:   a && b || !c
来源：http://rtz.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sfm.aibaodan.cn

Py:   if not data: return
来源：http://iik.52xcode.cn

PHP:  if (!$data) { return; }
来源：http://blj.jianghu66.top

JS:   if (!data) return;
来源：http://gjk.ydzc1.top

TS:   if (!data) return;
来源：http://mse.gotoacloud.top

Java: if (data == null) return;
来源：http://ohz.52xcode.cn

Go:   if data == nil { return }
来源：http://krz.chenzaomai.com

Ruby: return if data.nil?
来源：http://pua.zhoulong.xyz

C#:   if (data == null) return;
来源：http://yez.yj20258888.top

================================================================================
来源：http://wgq.cheryme.top

C. 函数与作用域
来源：http://epb.hongshengwenyu.top

================================================================================
来源：http://dzu.hnqzz.top

[C01] 定义函数
来源：http://jcd.cucudq.cn

Py:   def add(a, b): return a + b
来源：http://ymn.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oia.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ufp.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://puk.316326.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://cfq.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://bzi.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://bmj.pycfn.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fvl.andypj.xyz

[C02] 默认参数
来源：http://kxo.yvedp.cn

Py:   def greet(name="World"): return name
来源：http://sfx.zhongyouzk.top

PHP:  function greet($name = "World") { return $name; }
来源：http://acm.tanke756.top

JS:   function greet(name = "World") { return name; }
来源：http://wyn.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hrv.tanke756.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vxb.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://szj.cheryme.top

Ruby: def greet(name = "World") = name
来源：http://lyj.pengpengdd.cyou

C#:   string Greet(string name = "World") => name;
来源：http://otm.yonumen.top

[C03] 可变参数
来源：http://uvx.yfazqb.com

Py:   def total(*args): return sum(args)
来源：http://cgn.meibo888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mfz.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fot.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pky.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://izg.yonumen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cpg.hywenlv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cnw.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uex.hnxiangtu.top

[C04] 命名参数 / 关键字参数
来源：http://ixr.shanyushiyangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://whw.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bju.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://upa.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://knn.vehdjk.com

Java: // 无：用 Builder 模式或 record
来源：http://huj.yj20258888.top

Go:   // 无：用配置结构体参数
来源：http://bcc.hongshengwenyu.top

Ruby: f(a: 1, b: 2)
来源：http://rdd.0kj1m.cn

C#:   f(a: 1, b: 2)
来源：http://xqx.zhengqikj.top

[C05] 返回多个值
来源：http://abo.nanxinkj.top

Py:   return a, b
来源：http://ezq.gogol.net.cn

PHP:  return [$a, $b];
来源：http://jyp.vehdjk.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://mti.smart0.xyz

TS:   return { a, b };
来源：http://qcq.cheryme.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://njt.hywenlv.cn

Go:   return a, b
来源：http://atw.guannengcc.top

Ruby: return a, b
来源：http://cty.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://caa.cheryme.top

[C06] 匿名函数 / lambda
来源：http://djl.vehdjk.com

Py:   square = lambda x: x * x
来源：http://xwo.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gvy.jqgfzy.top

JS:   const square = x => x * x;
来源：http://dpe.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://tqj.xingfuxueyuan.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qmd.zdbjq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gpx.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://ito.hesvh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://elk.gotoacloud.top

[C07] 把函数作为参数传入
来源：http://tne.yuxming.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kat.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tyk.cqqwz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dku.yonumen.top

TS:   arr.map(String)
来源：http://aza.zdbjq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dyq.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hfp.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://ucx.snrcjt.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mlw.zhengqikj.top

[C08] 闭包
来源：http://nhe.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lab.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mfi.dashuyun.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yaf.wangdashe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ncx.zycfv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ady.jyoumei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vmv.yanxiufei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zuq.smart0.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fzx.uphjek.com

[C09] 递归
来源：http://har.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tpb.tarul.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lrw.bjfxy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rpv.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lfg.xinyue.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ruk.yuxming.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zeo.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zvf.xziqi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dlq.ppjwa.cn

[C10] 变量作用域
来源：http://xxz.andypj.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mft.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rck.cdnleiting.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://esv.redwolf501.top

TS:   同 JS
来源：http://woh.tanke756.top

Java: 方法内为块级作用域
来源：http://rmk.bbcook.cn

Go:   花括号块级作用域
来源：http://ufj.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kjj.cucudq.cn

C#:   块级作用域
来源：http://djc.chenjidiqi.icu

[C11] 模块导入与导出
来源：http://sqh.tarul.cn

Py:   from module import func
来源：http://fia.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lqb.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jlj.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://otj.pycfn.com

Java: import java.util.List;
来源：http://crf.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nlj.guowangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://yim.cucudq.cn

C#:   using System.Text;
来源：http://zdc.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://phe.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://zwk.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://bwl.aibaodan.cn

JS:   (() => { console.log("run"); })();
来源：http://knr.hcnkem.com

TS:   (() => { console.log("run"); })();
来源：http://dyb.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xty.dashuyun.cn


<!-- 参考信息 -->