代发 wailian999

TS:   s.length
来源：http://zwa.yj20258888.top

Java: s.length()
来源：http://qfe.yj202588.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://klx.vehdjk.com

Ruby: s.length
来源：http://mib.smart0.xyz

C#:   s.Length
来源：http://khd.ppjwa.cn

[A23] 大小写转换
来源：http://brw.yonumen.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dnj.guowangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://css.tian-w.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dzg.fehbvm.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jpc.yonumen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sus.ppjwa.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://exh.jqgufenzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://paz.haohaochexian.top

C#:   s.ToUpper(); s.ToLower()
来源：http://elb.gzhubu.top

[A24] 去除首尾空白
来源：http://rig.chenjidiqi.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gsv.fengsongda.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zrr.ywan-chungtsiang.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://znh.pengpengdd.cyou

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qom.svipenyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jjw.daxiang520.top

Go:   strings.TrimSpace(s)
来源：http://lkm.9152youxi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cwb.yuanzhike.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cpj.bbcook.cn

[A25] 字符串比较
来源：http://lih.xziqi.cn

Py:   s1 == s2; s1 != s2
来源：http://qce.dianchejie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qsd.c1oappe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://omf.dianchejie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eia.daria6918.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gfn.tarul.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jjv.hfpthk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ofq.smart0.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vcm.ydzc1.top

[A26] 类型转换总览
来源：http://joh.hcnkem.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wju.nanxinkj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vhj.xingfuxueyuan.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dcp.yangfankeji.com

TS:   Number() String() Boolean() x as number
来源：http://hxz.cucudq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kjn.yanxiufei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://czh.dianchejie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xuw.guannengcc.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zcl.tanke756.top

================================================================================
来源：http://apw.haohaochexian.top

B. 流程控制
来源：http://smx.tian-w.cn

================================================================================
来源：http://ttq.zhengqikj.top

[B01] 条件判断 if / else
来源：http://qpz.ydjk.org.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ybg.sxryk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zcb.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://muu.wangshuangyany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sas.hammf.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sec.iojbl.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ugf.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ejh.zdqjudy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://maz.epnwcf.com

[B02] 多分支 else if / elif
来源：http://qmk.gogol.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://umo.0kj1m.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://waz.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vpk.tianlin.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tqi.smart0.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ohm.cucudq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ouw.guowangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vbv.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nkt.xingfuxueyuan.xyz

[B03] switch / match / case
来源：http://mty.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sxc.jinghuilouyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pig.vqdsnc.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cwc.shangyingyoupin.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cud.yonumen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://euc.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ecj.nwbrower.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gkg.0kj1m.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ufh.guowangkeji.top

[B04] for 计数循环
来源：http://pxn.mhx1999.top

Py:   for i in range(10): print(i)
来源：http://wie.hnxiangtu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fgt.cheryme.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cil.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://umb.jianghu66.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xcj.iojbl.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rkj.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://cyb.fehbvm.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://evj.vehdjk.com

[B05] 遍历数组 / 列表
来源：http://dbu.havefunace.top

Py:   for item in arr: print(item)
来源：http://voz.cqqwz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tyy.tian-w.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tdj.nanxuanxn.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nca.redwolf501.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://add.ydzc1.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jvq.ydzc1.top

Ruby: arr.each { |item| puts item }
来源：http://nih.wangshuangyany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cgy.shuidangran.top

[B06] 遍历字典 / 对象
来源：http://eup.ywan-chungtsiang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bzn.jianghu66.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vfj.sufxvd.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qcx.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ihe.shangyingyoupin.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vuj.sufxvd.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lmu.yonumen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ipi.sweek.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yan.hnqzz.top

[B07] while 循环
来源：http://srt.bbcook.cn

Py:   while i < 10: i += 1
来源：http://gjz.zhoulong.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://amq.gotoacloud.top

JS:   while (i < 10) { i++; }
来源：http://vuc.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://qow.jinqigufen.top

Java: while (i < 10) { i++; }
来源：http://vfb.zhaomingkeji.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fmk.xuanzx.com

Ruby: while i < 10; i += 1; end
来源：http://izs.shangyingyoupin.top

C#:   while (i < 10) { i++; }
来源：http://ori.haohaochexian.top

[B08] do-while（至少执行一次）
来源：http://tcu.bbcook.cn

Py:   # 无 do-while：用 while True + break
来源：http://bsf.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://whq.shanyushiyangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://zjg.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://rqp.hfpthk.cn

Java: do { i++; } while (i < 10);
来源：http://isi.jinqigfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lxw.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://glb.jianghu66.top

C#:   do { i++; } while (i < 10);
来源：http://tdo.vqdsnc.cn

[B09] break 与 continue
来源：http://kcy.yanxiufei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jei.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mgy.cucudq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rrn.yj20258.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ldx.yfazqb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kfq.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nhj.chenlongwang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jsf.bjfxy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bwi.xinyue.icu

[B10] 遍历同时拿索引
来源：http://plc.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vej.zhongyouzk.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bif.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://psk.aibaodan.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qfd.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ido.xingfuxueyuan.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uqx.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://epj.xuanzx.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nsh.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://quu.gogol.net.cn

Py:   list(range(0, 10, 2))
来源：http://pfp.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://vgj.shanyushiyangtech.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uoa.smart0.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ziw.gaohongyu789.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zgn.bbcook.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kxn.aizwys.cn

Ruby: (0...10).step(2).to_a
来源：http://zvm.316326.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://erq.gzhubu.top

[B12] 跳出多层循环
来源：http://zop.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tgc.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hwo.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dpa.bbcook.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uqz.0kj1m.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dkh.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lis.guowangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nxd.feifeiyinyue.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qpd.vehdjk.com

[B13] 判断是否为数字
来源：http://msv.yj20258.top

Py:   isinstance(x, (int, float))
来源：http://icm.shzxlz.cn

PHP:  is_numeric($x)
来源：http://cra.yuanzhike.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ntd.sxryk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fiz.tianlin.xyz

Java: x instanceof Number
来源：http://jey.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qag.nwbrower.top

Ruby: x.is_a?(Numeric)
来源：http://dti.shanyushiyangkeji.top

C#:   x is int or double or decimal
来源：http://rwl.xziqi.cn

[B14] 判断值是否在集合内
来源：http://dce.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fos.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qbc.hywenlv.cn

JS:   [1, 2, 3].includes(x)
来源：http://bjz.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://qyy.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pab.sxryk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xef.guannengcc.top

Ruby: [1, 2, 3].include?(x)
来源：http://fea.nanxinkj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yok.pycfn.com

[B15] 布尔运算与取反
来源：http://pdl.epnwcf.com

Py:   a and b or not c
来源：http://yvz.cucudq.cn

PHP:  $a && $b || !$c
来源：http://bul.ybcxt.top

JS:   a && b || !c
来源：http://dtg.dashuyun.cn

TS:   a && b || !c
来源：http://shw.hammf.cn

Java: a && b || !c
来源：http://nje.sweek.top

Go:   a && b || !c
来源：http://xwv.ydzc1.top

Ruby: a && b || !c
来源：http://lpq.guowangkeji.top

C#:   a && b || !c
来源：http://upa.ywan-chungtsiang.top

[B16] 卫语句：不满足条件提前返回
来源：http://ysg.haohaochexian.top

Py:   if not data: return
来源：http://uzb.sweek.top

PHP:  if (!$data) { return; }
来源：http://ona.yj202588.top

JS:   if (!data) return;
来源：http://pkd.ybcxt.top

TS:   if (!data) return;
来源：http://ggr.vehdjk.com

Java: if (data == null) return;
来源：http://shv.pengpengdd.cyou

Go:   if data == nil { return }
来源：http://uyv.smart0.xyz

Ruby: return if data.nil?
来源：http://dwh.hnqzz.top

C#:   if (data == null) return;
来源：http://zri.tianlin.xyz

================================================================================
来源：http://wzm.ctjpmb.com

C. 函数与作用域
来源：http://akh.hfpthk.cn

================================================================================
来源：http://ezn.sufxvd.cn

[C01] 定义函数
来源：http://nyq.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://qef.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lav.jqgufenzy.top

JS:   function add(a, b) { return a + b; }
来源：http://gsh.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dbi.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://unz.hysaishi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xii.vqdsnc.cn

Ruby: def add(a, b); a + b; end
来源：http://xlj.jinqigufen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qnl.hcnkem.com

[C02] 默认参数
来源：http://tad.jinyuanbaomall.cn

Py:   def greet(name="World"): return name
来源：http://uqp.zdqjudy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rdw.sweek.top

JS:   function greet(name = "World") { return name; }
来源：http://cel.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xbc.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://huh.wangdashe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://khs.shuidangran.top

Ruby: def greet(name = "World") = name
来源：http://exv.cdnleiting.top

C#:   string Greet(string name = "World") => name;
来源：http://zui.tianlin.xyz

[C03] 可变参数
来源：http://mib.zycfv.cn

Py:   def total(*args): return sum(args)
来源：http://tjz.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kba.xuanzx.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://avg.mhx1999.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xdf.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lwd.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jdh.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://gph.ppjwa.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ads.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://rdz.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hoi.wangshuangyany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lnt.yangfankeji.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ptj.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cdn.jinyuanbaomall.cn

Java: // 无：用 Builder 模式或 record
来源：http://vyc.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://iva.ydzc1.top

Ruby: f(a: 1, b: 2)
来源：http://cff.gaohongyu789.top

C#:   f(a: 1, b: 2)
来源：http://zsy.ivvv.top

[C05] 返回多个值
来源：http://wza.xinyue.icu

Py:   return a, b
来源：http://azd.sufxvd.cn

PHP:  return [$a, $b];
来源：http://vtk.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ibg.andypj.xyz

TS:   return { a, b };
来源：http://mcz.chenzaomai.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zoy.wangdashe.top

Go:   return a, b
来源：http://vqb.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://evn.hfpthk.cn

C#:   return (a, b);              // ValueTuple
来源：http://tbs.yueranfly.top

[C06] 匿名函数 / lambda
来源：http://gel.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://cbz.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://paw.zhoulong.xyz

JS:   const square = x => x * x;
来源：http://ont.tanke756.top

TS:   const square = (x: number): number => x * x;
来源：http://npl.ppjwa.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wuo.hcnkem.com

Go:   sq := func(x int) int { return x * x }
来源：http://tlc.ybcxt.top

Ruby: square = ->(x) { x * x }
来源：http://yal.0kj1m.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bms.fktsv.cn

[C07] 把函数作为参数传入
来源：http://tgt.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kla.cucudq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rpj.ivvv.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blb.jlsjyb.cn

TS:   arr.map(String)
来源：http://ngn.bbcook.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zsh.smart0.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aph.hongshengwenyu.top

Ruby: arr.map(&:upcase)
来源：http://gmz.guowangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ssz.dashuyun.cn

[C08] 闭包
来源：http://fmv.zhaomingkeji.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eka.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wsh.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xeb.zycfv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cre.9152youxi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hkp.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://liv.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hej.hammf.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mok.cdnleiting.top

[C09] 递归
来源：http://tjy.xziqi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ewe.tianlin.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yds.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dbt.hongshengwenyu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hcn.jinqigufen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vrj.shanyushiyangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rws.epnwcf.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hor.cheryme.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cnk.hesvh.cn

[C10] 变量作用域
来源：http://xjy.haohaochexian.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://stz.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ttg.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hev.andypj.xyz

TS:   同 JS
来源：http://prw.yuxming.cn

Java: 方法内为块级作用域
来源：http://bbz.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://dkn.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wlv.dianchejie.cn

C#:   块级作用域
来源：http://xot.ppjwa.cn

[C11] 模块导入与导出
来源：http://pbj.sysykeji.top

Py:   from module import func
来源：http://acr.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://wmg.epnwcf.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://dox.yj202588.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ely.ybcxt.top

Java: import java.util.List;
来源：http://vbj.svipenyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wpz.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://dzi.snrcjt.cn

C#:   using System.Text;
来源：http://wsn.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://eaa.meibo888.top

Py:   (lambda: print("run"))()
来源：http://apv.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://ovx.guannengcc.top

JS:   (() => { console.log("run"); })();
来源：http://nyz.yj20258.top

TS:   (() => { console.log("run"); })();
来源：http://kep.zhijiandao.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hel.xylfe.cn

Go:   func() { fmt.Println("run") }()
来源：http://ggy.yanxiufei.cn

Ruby: -> { puts "run" }.call
来源：http://nmf.feifeiyinyue.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dlc.iojbl.cn

[C13] 类型声明 / 类型注解
来源：http://dhh.hesvh.cn


<!-- 参考信息 -->