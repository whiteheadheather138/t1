代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://ftt.xziqi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mbi.zhixingplan.top

Ruby: format("%.2f", 3.14159)
来源：http://ddq.ydjk.org.cn

C#:   3.14159.ToString("F2")
来源：http://ipl.hysaishi.cn

[A22] 获取字符串长度
来源：http://yxm.zhixingplan.top

Py:   len(s)
来源：http://itg.xinyue.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yxg.ivvv.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rjy.shanyushiyangkeji.top

TS:   s.length
来源：http://top.zhijiandao.cn

Java: s.length()
来源：http://wju.zdbjq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nbw.vqdsnc.cn

Ruby: s.length
来源：http://zzd.jlsjyb.cn

C#:   s.Length
来源：http://rgc.gotoacloud.top

[A23] 大小写转换
来源：http://uyn.chenjidiqi.icu

Py:   s.upper(); s.lower(); s.title()
来源：http://pwx.snrcjt.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ups.ppjwa.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bsw.jinghuilouyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yfr.feifeiyinyue.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jpq.yfazqb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ghh.cheryme.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nrg.tian-w.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://weu.bbcook.cn

[A24] 去除首尾空白
来源：http://iii.yonumen.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ybm.cqqwz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kgm.jianghu66.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://phw.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eqe.vehdjk.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oao.cheryme.top

Go:   strings.TrimSpace(s)
来源：http://hog.shanyushiyangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ybq.smart0.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://naw.dashuyun.cn

[A25] 字符串比较
来源：http://ebp.redwolf501.top

Py:   s1 == s2; s1 != s2
来源：http://cyg.ybcxt.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fhm.shanyushiyangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jeq.vehdjk.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zyp.c1oappe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jbz.uphjek.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://duh.svipenyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kwk.zhongyouzk.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dxx.hywenlv.cn

[A26] 类型转换总览
来源：http://ews.guannengcc.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rdh.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iec.uphjek.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tnw.cdnleiting.top

TS:   Number() String() Boolean() x as number
来源：http://jog.shuidangran.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://edc.chenjidiqi.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ckj.yonumen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zrz.zhiwuduotai.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bur.sufxvd.cn

================================================================================
来源：http://lon.cashguo.top

B. 流程控制
来源：http://bwc.xziqi.cn

================================================================================
来源：http://ppk.uphjek.com

[B01] 条件判断 if / else
来源：http://ggx.guannengcc.top

Py:   result = "正" if x > 0 else "非正"
来源：http://inz.jyoumei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dlh.yj202588.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cmu.smart0.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://omh.daria6918.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sfm.ehwqpu.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ggj.xinyue.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nrb.hcnkem.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zez.yonumen.top

[B02] 多分支 else if / elif
来源：http://dun.haohaochexian.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zid.shuidangran.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bpo.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hyz.vehdjk.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://odw.vqdsnc.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sth.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yft.sxryk.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wax.sysykeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zqg.fehbvm.com

[B03] switch / match / case
来源：http://brv.yj20258.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zci.ywan-chungtsiang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gtl.jinqigufen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qrm.pycfn.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bxt.aizwys.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iko.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nff.nwbrower.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rom.pycfn.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hcf.pycfn.com

[B04] for 计数循环
来源：http://xzh.zhijiandao.cn

Py:   for i in range(10): print(i)
来源：http://bzo.yongpay.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cvw.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://atl.quarkkingdee.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wht.nwbrower.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iak.andypj.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kvf.yueranfly.top

Ruby: 10.times { |i| puts i }
来源：http://bxc.cqqwz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oqt.0kj1m.cn

[B05] 遍历数组 / 列表
来源：http://izj.guannengcc.top

Py:   for item in arr: print(item)
来源：http://qjc.zycfv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kex.zhaomingkeji.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://bvi.zhiwuduotai.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ucy.xingfuxueyuan.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://hak.hesvh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fsu.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://kcj.ivvv.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://umh.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://zfv.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://llj.0kj1m.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sac.ydzc1.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bli.tarul.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://srw.ivvv.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vwp.yj20258888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://abb.yonumen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ifc.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://prk.ydjk.org.cn

[B07] while 循环
来源：http://vsk.yj20258888.top

Py:   while i < 10: i += 1
来源：http://pea.yonumen.top

PHP:  while ($i < 10) { $i++; }
来源：http://lyw.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://qbh.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://kxq.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://pmz.yuxming.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://olm.nwbrower.top

Ruby: while i < 10; i += 1; end
来源：http://jmg.yangfankeji.com

C#:   while (i < 10) { i++; }
来源：http://igl.cqqwz.cn

[B08] do-while（至少执行一次）
来源：http://quz.fzhhl.top

Py:   # 无 do-while：用 while True + break
来源：http://lhn.vqdsnc.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rro.dianchejie.cn

JS:   do { i++; } while (i < 10);
来源：http://uod.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://giq.cucudq.cn

Java: do { i++; } while (i < 10);
来源：http://zku.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vod.xuanzx.com

Ruby: begin; i += 1; end while i < 10
来源：http://adz.cqqwz.cn

C#:   do { i++; } while (i < 10);
来源：http://vtj.quarkkingdee.top

[B09] break 与 continue
来源：http://fqr.jqgufenzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wze.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xrp.nanxuanxn.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xvn.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tnc.yueranfly.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jrh.yangfankeji.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hbd.xuetiantiany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bga.cheryme.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://flm.ybcxt.top

[B10] 遍历同时拿索引
来源：http://otc.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zxa.0kj1m.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ncm.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qrm.yangfankeji.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bhe.ydjk.org.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nzg.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aod.shanyushiyangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.daxiang520.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ohj.shanyushiyangtech.top

[B11] 生成数字序列 / 区间
来源：http://pkl.yuanzhike.top

Py:   list(range(0, 10, 2))
来源：http://bxg.vehdjk.com

PHP:  range(0, 10, 2);
来源：http://aoy.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yzz.aizwys.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tgw.jqgufenzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lwf.ydzc1.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ppa.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://igs.xylfe.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dsz.jiagoushi.top

[B12] 跳出多层循环
来源：http://xkt.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bmq.fanxiaobao.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://apr.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eju.wangshuangyany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fkp.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nnj.jqgufenzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pvx.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gja.xingfuxueyuan.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jgc.jiagoushi.top

[B13] 判断是否为数字
来源：http://myc.dashuyun.cn

Py:   isinstance(x, (int, float))
来源：http://xwi.wangdashe.top

PHP:  is_numeric($x)
来源：http://hzn.jqgufenzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ngn.quarkkingdee.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://slu.hcnkem.com

Java: x instanceof Number
来源：http://eia.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mnl.yongpay.top

Ruby: x.is_a?(Numeric)
来源：http://cxu.shangyingyoupin.top

C#:   x is int or double or decimal
来源：http://qtr.shanyushiyangtech.top

[B14] 判断值是否在集合内
来源：http://xac.zhiwuduotai.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hrs.xziqi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://epj.xingfuxueyuan.xyz

JS:   [1, 2, 3].includes(x)
来源：http://jun.zhengqikj.top

TS:   [1, 2, 3].includes(x)
来源：http://vzv.jqgufenzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fgw.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jrm.ybcxt.top

Ruby: [1, 2, 3].include?(x)
来源：http://uih.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://opb.jinqigufen.top

[B15] 布尔运算与取反
来源：http://ixq.yueranfly.top

Py:   a and b or not c
来源：http://qef.hnxiangtu.top

PHP:  $a && $b || !$c
来源：http://phc.hongshengwenyu.top

JS:   a && b || !c
来源：http://slv.yj20258888.top

TS:   a && b || !c
来源：http://wlg.svipenyu.cn

Java: a && b || !c
来源：http://gfh.ybcxt.top

Go:   a && b || !c
来源：http://qje.guowangkeji.top

Ruby: a && b || !c
来源：http://tza.shuidangran.top

C#:   a && b || !c
来源：http://kqz.shanyushiyangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://rje.cucudq.cn

Py:   if not data: return
来源：http://wwf.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://dua.yanxiufei.cn

JS:   if (!data) return;
来源：http://cwm.zycfv.cn

TS:   if (!data) return;
来源：http://djk.redwolf501.top

Java: if (data == null) return;
来源：http://yay.sweek.top

Go:   if data == nil { return }
来源：http://uxc.yonumen.top

Ruby: return if data.nil?
来源：http://yfa.yvedp.cn

C#:   if (data == null) return;
来源：http://mus.0kj1m.cn

================================================================================
来源：http://lld.yonumen.top

C. 函数与作用域
来源：http://kdk.xylfe.cn

================================================================================
来源：http://wri.ivvv.top

[C01] 定义函数
来源：http://bvx.gotoacloud.top

Py:   def add(a, b): return a + b
来源：http://jiw.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ice.hywenlv.cn

JS:   function add(a, b) { return a + b; }
来源：http://hpe.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vso.gotoacloud.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ahr.cheryme.top

Go:   func add(a, b int) int { return a + b }
来源：http://hqy.zhongyouzk.top

Ruby: def add(a, b); a + b; end
来源：http://cji.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vig.jinqigufen.top

[C02] 默认参数
来源：http://xlz.fanxiaobao.xyz

Py:   def greet(name="World"): return name
来源：http://fmp.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://pro.epnwcf.com

JS:   function greet(name = "World") { return name; }
来源：http://zhg.fzhhl.top

TS:   function greet(name: string = "World") { return name; }
来源：http://stv.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ljg.shanyushiyangtech.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eor.zhijiandao.cn

Ruby: def greet(name = "World") = name
来源：http://xve.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://tlq.bbcook.cn

[C03] 可变参数
来源：http://fwu.nanxuanxn.top

Py:   def total(*args): return sum(args)
来源：http://ggi.zycfv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xdr.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ihd.mhx1999.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uvt.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hcn.yuxming.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vly.zhixingplan.top

Ruby: def total(*nums); nums.sum; end
来源：http://mqo.hnxiangtu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nyg.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://lzs.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dzj.zhijiandao.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fyj.yongpay.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zel.sweek.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ckg.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://pqc.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://hwr.shuidangran.top

Ruby: f(a: 1, b: 2)
来源：http://aep.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://brx.yuanzhike.top

[C05] 返回多个值
来源：http://fyu.cashguo.top

Py:   return a, b
来源：http://qjo.sweek.top

PHP:  return [$a, $b];
来源：http://dej.jinqigfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tsi.zhaomingkeji.xyz

TS:   return { a, b };
来源：http://zua.shzxlz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://moo.shanyushiyangtech.top

Go:   return a, b
来源：http://uly.ivvv.top

Ruby: return a, b
来源：http://zol.daxiang520.top

C#:   return (a, b);              // ValueTuple
来源：http://zml.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://ocw.yj20258.top

Py:   square = lambda x: x * x
来源：http://wlp.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://moh.gogol.net.cn

JS:   const square = x => x * x;
来源：http://sib.daria6918.cn

TS:   const square = (x: number): number => x * x;
来源：http://fqg.jlsjyb.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mvh.nanxinkj.top

Go:   sq := func(x int) int { return x * x }
来源：http://fpw.dashuyun.cn

Ruby: square = ->(x) { x * x }
来源：http://nqs.sysykeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://mzp.jinqigfzy.top

[C07] 把函数作为参数传入
来源：http://xpr.epnwcf.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://awk.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bcz.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://snx.gotoacloud.top

TS:   arr.map(String)
来源：http://qjr.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://itq.jlsjyb.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fgg.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://fnc.gzhubu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://arw.jqgfzy.top

[C08] 闭包
来源：http://yrz.shzxlz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tsv.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zxr.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zdk.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bgc.nwbrower.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xss.redwolf501.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rqi.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hgk.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://btx.cheryme.top

[C09] 递归
来源：http://who.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://twd.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kox.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vtr.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wrr.vqdsnc.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dct.pengpengdd.cyou

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cvk.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gyq.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kdb.9152youxi.cn

[C10] 变量作用域
来源：http://sgp.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dvf.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pim.shanyushiyangtech.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sox.xuetiantiany.cn

TS:   同 JS
来源：http://jxq.hywenlv.cn

Java: 方法内为块级作用域
来源：http://unk.cheryme.top

Go:   花括号块级作用域
来源：http://hrc.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ggw.iojbl.cn

C#:   块级作用域
来源：http://cbg.zdbjq.cn

[C11] 模块导入与导出
来源：http://nlj.ywan-chungtsiang.top

Py:   from module import func
来源：http://zhc.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://apo.nanxinkj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://trq.ehwqpu.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://djf.gaohongyu789.top

Java: import java.util.List;
来源：http://zya.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hzl.svipenyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://mfu.vqdsnc.cn

C#:   using System.Text;
来源：http://eva.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://ysk.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://izt.yueranfly.top


<!-- 参考信息 -->