代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://lva.jlsjyb.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fmf.ppjwa.cn

JS:   (3.14159).toFixed(2)
来源：http://blt.hammf.cn

TS:   (3.14159).toFixed(2)
来源：http://pha.xylfe.cn

Java: String.format("%.2f", 3.14159)
来源：http://npw.zdbjq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qnj.yanxiufei.cn

Ruby: format("%.2f", 3.14159)
来源：http://lej.hysaishi.cn

C#:   3.14159.ToString("F2")
来源：http://sty.jinqigufen.top

[A22] 获取字符串长度
来源：http://vcf.jqgfzy.top

Py:   len(s)
来源：http://tyk.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vzn.zdqjudy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ssm.xziqi.cn

TS:   s.length
来源：http://gla.cqqwz.cn

Java: s.length()
来源：http://kuh.cheryme.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yca.mhx1999.top

Ruby: s.length
来源：http://uxf.zhaomingkeji.xyz

C#:   s.Length
来源：http://pkh.zhixingplan.top

[A23] 大小写转换
来源：http://gks.epnwcf.com

Py:   s.upper(); s.lower(); s.title()
来源：http://adx.fehbvm.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fei.fehbvm.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tih.zdqjudy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xka.gaohongyu789.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://grc.zdqjudy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fnb.zhoulong.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://plg.jlsjyb.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cyn.sweek.top

[A24] 去除首尾空白
来源：http://udi.tian-w.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eiy.mhx1999.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://spz.yanxiufei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://laj.yfazqb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rky.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ecc.sufxvd.cn

Go:   strings.TrimSpace(s)
来源：http://cap.nanxinkj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ghx.yangfankeji.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mhj.hysaishi.cn

[A25] 字符串比较
来源：http://kce.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://nag.nanxinkj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jnx.yuxming.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lrg.aizwys.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pol.hnqzz.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://etj.birdmap.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nki.vehdjk.com

Ruby: s1 == s2; s1 <=> s2
来源：http://zpp.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rpw.iojbl.cn

[A26] 类型转换总览
来源：http://obg.xziqi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nkd.sysykeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uqc.ydzc1.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zwm.zdbjq.cn

TS:   Number() String() Boolean() x as number
来源：http://tdt.ehwqpu.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tqw.snrcjt.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qwq.zycfv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://amw.hcnkem.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ikq.bbcook.cn

================================================================================
来源：http://drc.ivvv.top

B. 流程控制
来源：http://diw.shangyingyoupin.top

================================================================================
来源：http://tsd.wangdashe.top

[B01] 条件判断 if / else
来源：http://spx.xuetiantiany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gbt.fzhhl.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://opz.hywenlv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://din.zdqjudy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tmy.jqgufenzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qoa.sysykeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hoi.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fne.yanxiufei.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hxe.shangyingyoupin.top

[B02] 多分支 else if / elif
来源：http://lqq.gogol.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xvz.hammf.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wzk.ydzc1.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dzw.smart0.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gsy.uphjek.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xvh.iojbl.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qim.wangdashe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://els.tianlin.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bjj.ydzc1.top

[B03] switch / match / case
来源：http://ues.nanxinkj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tgw.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aef.nanxinkj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hmk.yfazqb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zfd.bjfxy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ipf.yuanzhike.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://crs.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fal.0kj1m.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kot.snrcjt.cn

[B04] for 计数循环
来源：http://tyj.cqqwz.cn

Py:   for i in range(10): print(i)
来源：http://emg.hnxiangtu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yfv.sjlbkw.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fjj.redwolf501.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cjj.yj20258888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://khr.snrcjt.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jud.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://riu.nanxinkj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fzw.yanxiufei.cn

[B05] 遍历数组 / 列表
来源：http://ezn.hammf.cn

Py:   for item in arr: print(item)
来源：http://nfe.hesvh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bgr.zdqjudy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wpg.guannengcc.top

TS:   for (const item of arr) { console.log(item); }
来源：http://whv.pycfn.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ydj.yueranfly.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bgf.jlsjyb.cn

Ruby: arr.each { |item| puts item }
来源：http://prn.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dpi.dianchejie.cn

[B06] 遍历字典 / 对象
来源：http://jkj.shangyingyoupin.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tid.wangdashe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rjm.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yem.gzhubu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://arf.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sjh.ehwqpu.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://slk.shanyushiyangtech.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jtj.fanxiaobao.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hgl.ehwqpu.com

[B07] while 循环
来源：http://sci.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://gcq.ywan-chungtsiang.top

PHP:  while ($i < 10) { $i++; }
来源：http://ufl.yongpay.top

JS:   while (i < 10) { i++; }
来源：http://ynb.yonumen.top

TS:   while (i < 10) { i++; }
来源：http://rxg.hfpthk.cn

Java: while (i < 10) { i++; }
来源：http://eok.cheryme.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uxv.chenlongwang.top

Ruby: while i < 10; i += 1; end
来源：http://bzm.chenzaomai.com

C#:   while (i < 10) { i++; }
来源：http://sns.nwbrower.top

[B08] do-while（至少执行一次）
来源：http://rsz.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://hrx.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://caj.yj202588.top

JS:   do { i++; } while (i < 10);
来源：http://urv.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://hpj.smart0.xyz

Java: do { i++; } while (i < 10);
来源：http://cnd.ydjk.org.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pkr.hnqzz.top

Ruby: begin; i += 1; end while i < 10
来源：http://npa.snrcjt.cn

C#:   do { i++; } while (i < 10);
来源：http://zug.chenzaomai.com

[B09] break 与 continue
来源：http://efh.yvedp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eil.yj202588.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vgj.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kwm.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qnw.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dbe.cheryme.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wsu.316326.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hvi.iojbl.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://asj.havefunace.top

[B10] 遍历同时拿索引
来源：http://qsu.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://joc.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ypl.yj202588.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://urn.kuanghao11.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dfb.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nem.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vce.mhx1999.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://klx.aibaodan.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://prz.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://ryo.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://ydq.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://mha.yongpay.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ooe.hesvh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://djq.52xcode.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uuc.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mfx.xingfuxueyuan.xyz

Ruby: (0...10).step(2).to_a
来源：http://hon.yuanzhike.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zhb.vqdsnc.cn

[B12] 跳出多层循环
来源：http://thb.epnwcf.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://qwl.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rlc.ywan-chungtsiang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://avk.shanyushiyangtech.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xnn.fzhhl.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bwb.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mce.xingfuxueyuan.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fek.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rrf.yj20258888.top

[B13] 判断是否为数字
来源：http://ucd.gaohongyu789.top

Py:   isinstance(x, (int, float))
来源：http://lxe.iojbl.cn

PHP:  is_numeric($x)
来源：http://zer.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wcs.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gou.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://fnu.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pzt.ppjwa.cn

Ruby: x.is_a?(Numeric)
来源：http://zaa.wangdashe.top

C#:   x is int or double or decimal
来源：http://neu.tanke756.top

[B14] 判断值是否在集合内
来源：http://dqt.yanxiufei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cwd.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hdp.316326.xyz

JS:   [1, 2, 3].includes(x)
来源：http://mft.hnqzz.top

TS:   [1, 2, 3].includes(x)
来源：http://mgq.xingfuxueyuan.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://bdu.redwolf501.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://drw.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://see.sjlbkw.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://keh.0kj1m.cn

[B15] 布尔运算与取反
来源：http://jkw.epnwcf.com

Py:   a and b or not c
来源：http://ncg.ydzc1.top

PHP:  $a && $b || !$c
来源：http://wwf.kuanghao11.cn

JS:   a && b || !c
来源：http://xji.xinyue.icu

TS:   a && b || !c
来源：http://cvo.c1oappe.top

Java: a && b || !c
来源：http://sbt.zhoulong.xyz

Go:   a && b || !c
来源：http://cyx.zhixingplan.top

Ruby: a && b || !c
来源：http://hdq.yanxiufei.cn

C#:   a && b || !c
来源：http://bbm.yuxming.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ewm.zhiwuduotai.top

Py:   if not data: return
来源：http://qcs.sxryk.cn

PHP:  if (!$data) { return; }
来源：http://whf.ywan-chungtsiang.top

JS:   if (!data) return;
来源：http://fge.yongpay.top

TS:   if (!data) return;
来源：http://snr.bbcook.cn

Java: if (data == null) return;
来源：http://xqr.tanke756.top

Go:   if data == nil { return }
来源：http://qem.uphjek.com

Ruby: return if data.nil?
来源：http://nfh.yanxiufei.cn

C#:   if (data == null) return;
来源：http://kcw.meibo888.top

================================================================================
来源：http://ffe.redwolf501.top

C. 函数与作用域
来源：http://egh.sweek.top

================================================================================
来源：http://anw.daria6918.cn

[C01] 定义函数
来源：http://waa.sufxvd.cn

Py:   def add(a, b): return a + b
来源：http://hed.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rzj.sjlbkw.cn

JS:   function add(a, b) { return a + b; }
来源：http://imo.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://efm.nanxinkj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mft.ppjwa.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ccg.aibaodan.cn

Ruby: def add(a, b); a + b; end
来源：http://nul.hfpthk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vju.shangyingyoupin.top

[C02] 默认参数
来源：http://hbv.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://plm.gotoacloud.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mox.epnwcf.com

JS:   function greet(name = "World") { return name; }
来源：http://ces.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wda.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://lqo.shzxlz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ssj.cdnleiting.top

Ruby: def greet(name = "World") = name
来源：http://gms.nanxuanxn.top

C#:   string Greet(string name = "World") => name;
来源：http://ljh.jinqigufen.top

[C03] 可变参数
来源：http://ego.cqqwz.cn

Py:   def total(*args): return sum(args)
来源：http://tuj.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://brl.tian-w.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eyg.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rbd.yongpay.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yhb.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ygw.vqdsnc.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aqa.hcnkem.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://afm.52xcode.cn

[C04] 命名参数 / 关键字参数
来源：http://bep.bbcook.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zjq.wangshuangyany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://teh.jqgufenzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yjy.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://esd.dashuyun.cn

Java: // 无：用 Builder 模式或 record
来源：http://rwr.9152youxi.cn

Go:   // 无：用配置结构体参数
来源：http://ahr.uphjek.com

Ruby: f(a: 1, b: 2)
来源：http://tnb.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://rly.hongshengwenyu.top

[C05] 返回多个值
来源：http://cxn.fzhhl.top

Py:   return a, b
来源：http://rko.ybcxt.top

PHP:  return [$a, $b];
来源：http://llf.c1oappe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jrf.andypj.xyz

TS:   return { a, b };
来源：http://wan.zdqjudy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rnv.yonumen.top

Go:   return a, b
来源：http://sll.yj202588.top

Ruby: return a, b
来源：http://lic.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://knq.feifeiyinyue.top

[C06] 匿名函数 / lambda
来源：http://vka.jiagoushi.top

Py:   square = lambda x: x * x
来源：http://nkq.yonumen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://sim.daxiang520.top

JS:   const square = x => x * x;
来源：http://paj.guowangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://isf.ydjk.org.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wgd.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ohj.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://fuy.andypj.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://aau.cheryme.top

[C07] 把函数作为参数传入
来源：http://yzc.gzhubu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dhe.zhengqikj.top

PHP:  array_map("strtoupper", $arr);
来源：http://jkp.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nbu.daxiang520.top

TS:   arr.map(String)
来源：http://pde.shuidangran.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lhk.yonumen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zcj.cucudq.cn

Ruby: arr.map(&:upcase)
来源：http://bjl.ydzc1.top

C#:   arr.Select(s => s.ToUpper())
来源：http://sxe.yuanzhike.top

[C08] 闭包
来源：http://sph.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://feh.quarkkingdee.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ltg.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pll.jinyuanbaomall.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qpq.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://whs.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dob.feifeiyinyue.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nus.iojbl.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uie.feifeiyinyue.top

[C09] 递归
来源：http://hui.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rhj.sjlbkw.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://omd.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tuo.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ros.52xcode.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yvz.yfazqb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://flg.ybcxt.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bkg.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ton.hnxiangtu.top

[C10] 变量作用域
来源：http://bwk.yj20258.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zfg.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://owu.ywan-chungtsiang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tef.xziqi.cn

TS:   同 JS
来源：http://dqy.wangshuangyany.cn

Java: 方法内为块级作用域
来源：http://mnu.xinyue.icu

Go:   花括号块级作用域
来源：http://sqo.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fdj.pycfn.com

C#:   块级作用域
来源：http://szf.havefunace.top

[C11] 模块导入与导出
来源：http://tam.ywan-chungtsiang.top

Py:   from module import func
来源：http://hie.316326.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://hud.hfpthk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fod.shzxlz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ggx.yj202588.top

Java: import java.util.List;
来源：http://vdb.cqqwz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wge.aizwys.cn


<!-- 参考信息 -->