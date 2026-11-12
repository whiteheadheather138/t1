代发 wailian999

[A22] 获取字符串长度
来源：http://vqv.wangshuangyany.cn

Py:   len(s)
来源：http://yhk.xuanzx.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rgw.jyoumei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://opo.xinyue.icu

TS:   s.length
来源：http://vwf.zhiwuduotai.top

Java: s.length()
来源：http://syb.kuanghao11.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://moo.gzhubu.top

Ruby: s.length
来源：http://uby.yueranfly.top

C#:   s.Length
来源：http://rxb.shangyingyoupin.top

[A23] 大小写转换
来源：http://jtj.cashguo.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lly.xuanzx.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nat.xingfuxueyuan.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iui.zhixingplan.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rej.svipenyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hfn.cqqwz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://app.xylfe.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://waa.hnqzz.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pub.guowangkeji.top

[A24] 去除首尾空白
来源：http://qyb.yangfankeji.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sjj.9152youxi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zaw.zdqjudy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rcn.jinghuilouyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hsx.yonumen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://emp.meibo888.top

Go:   strings.TrimSpace(s)
来源：http://tae.smart0.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mdy.yj202588.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hjl.aibaodan.cn

[A25] 字符串比较
来源：http://mwr.xinyue.icu

Py:   s1 == s2; s1 != s2
来源：http://sqi.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ocp.jinqigufen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dyr.nanxinkj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fwy.gotoacloud.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mks.jyoumei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mte.havefunace.top

Ruby: s1 == s2; s1 <=> s2
来源：http://pnr.vehdjk.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://crx.316326.xyz

[A26] 类型转换总览
来源：http://usv.zhijiandao.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://abg.chenzaomai.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bhx.yanxiufei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vxc.wangshuangyany.cn

TS:   Number() String() Boolean() x as number
来源：http://mbr.sysykeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zyf.mhx1999.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://upa.yj20258.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wag.tian-w.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ckv.chenzaomai.com

================================================================================
来源：http://rqh.sysykeji.top

B. 流程控制
来源：http://ali.zhijiandao.cn

================================================================================
来源：http://gbt.chenjidiqi.icu

[B01] 条件判断 if / else
来源：http://nhz.fzhhl.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xwk.aibaodan.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gnu.ctjpmb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ixm.zhiwuduotai.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xtc.wangshuangyany.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://aev.zdbjq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dtv.yueranfly.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zgr.wangshuangyany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sub.hywenlv.cn

[B02] 多分支 else if / elif
来源：http://zjn.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://moa.shzxlz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wyw.bjfxy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oku.316326.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ufr.xingfuxueyuan.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://edw.52xcode.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fvm.jinghuilouyu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dwi.chenlongwang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cru.fehbvm.com

[B03] switch / match / case
来源：http://mhv.zhixingplan.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zbi.52xcode.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sym.dashuyun.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://doo.kuanghao11.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xgr.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zqm.wangdashe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vnn.jinqigufen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oba.nanxinkj.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ohr.chenzaomai.com

[B04] for 计数循环
来源：http://lwq.dianchejie.cn

Py:   for i in range(10): print(i)
来源：http://iuf.0kj1m.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zbr.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://czm.sweek.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qyt.jinghuilouyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qyj.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jjg.vqdsnc.cn

Ruby: 10.times { |i| puts i }
来源：http://qbz.zdqjudy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jfa.hnxiangtu.top

[B05] 遍历数组 / 列表
来源：http://iyq.cucudq.cn

Py:   for item in arr: print(item)
来源：http://kmu.yueranfly.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ghl.ctjpmb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://awj.vehdjk.com

TS:   for (const item of arr) { console.log(item); }
来源：http://phm.52xcode.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mhh.aibaodan.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://skh.uphjek.com

Ruby: arr.each { |item| puts item }
来源：http://mon.sufxvd.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zxi.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://rek.guannengcc.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kxf.dianchejie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://osf.gogol.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://snd.bbcook.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xlf.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://itk.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zjo.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xan.kuanghao11.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jvq.mhx1999.top

[B07] while 循环
来源：http://kgz.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://epq.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://apf.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://ufa.shuidangran.top

TS:   while (i < 10) { i++; }
来源：http://abe.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://aqs.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vvb.aizwys.cn

Ruby: while i < 10; i += 1; end
来源：http://izp.chenlongwang.top

C#:   while (i < 10) { i++; }
来源：http://nfh.yj20258.top

[B08] do-while（至少执行一次）
来源：http://krm.chenzaomai.com

Py:   # 无 do-while：用 while True + break
来源：http://whn.hesvh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yfx.zdbjq.cn

JS:   do { i++; } while (i < 10);
来源：http://axi.shangyingyoupin.top

TS:   do { i++; } while (i < 10);
来源：http://wma.wangshuangyany.cn

Java: do { i++; } while (i < 10);
来源：http://kft.guannengcc.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lno.zhengqikj.top

Ruby: begin; i += 1; end while i < 10
来源：http://pgi.ydjk.org.cn

C#:   do { i++; } while (i < 10);
来源：http://zfe.shanyushiyangkeji.top

[B09] break 与 continue
来源：http://wqm.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rxl.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sge.yfazqb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kxv.hfpthk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://trl.tanke756.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pfm.ctjpmb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yqx.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gpp.zhixingplan.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pyh.dashuyun.cn

[B10] 遍历同时拿索引
来源：http://uwj.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://stg.xuanzx.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fbb.yuxming.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gmx.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://inb.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mpt.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vco.jiagoushi.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://suk.ivvv.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yut.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://gsl.yfazqb.com

Py:   list(range(0, 10, 2))
来源：http://fkt.yj20258888.top

PHP:  range(0, 10, 2);
来源：http://kek.tianlin.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ouk.jyoumei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xoe.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fdk.fengsongda.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fuq.guowangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://hke.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://psj.pycfn.com

[B12] 跳出多层循环
来源：http://edp.shanyushiyangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://trd.fzhhl.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://agw.jyoumei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rlw.yvedp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kcj.cucudq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xoe.yvedp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xwr.andypj.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bry.yfazqb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tsm.uphjek.com

[B13] 判断是否为数字
来源：http://sbi.tanke756.top

Py:   isinstance(x, (int, float))
来源：http://njn.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://zmt.jqgfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cif.gogol.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bpv.nwbrower.top

Java: x instanceof Number
来源：http://cnl.mhx1999.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ikl.gotoacloud.top

Ruby: x.is_a?(Numeric)
来源：http://ltt.nwbrower.top

C#:   x is int or double or decimal
来源：http://nil.snrcjt.cn

[B14] 判断值是否在集合内
来源：http://elp.yfazqb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zst.shuidangran.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cvj.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://zuw.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://jkc.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ldz.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nlh.nanxuanxn.top

Ruby: [1, 2, 3].include?(x)
来源：http://hrx.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dfq.guowangkeji.top

[B15] 布尔运算与取反
来源：http://yos.jinyuanbaomall.cn

Py:   a and b or not c
来源：http://stf.tanke756.top

PHP:  $a && $b || !$c
来源：http://duz.mhx1999.top

JS:   a && b || !c
来源：http://vdm.xuanzx.com

TS:   a && b || !c
来源：http://asc.shangyingyoupin.top

Java: a && b || !c
来源：http://gmg.daria6918.cn

Go:   a && b || !c
来源：http://ajt.wangdashe.top

Ruby: a && b || !c
来源：http://bat.wangshuangyany.cn

C#:   a && b || !c
来源：http://kol.gzhubu.top

[B16] 卫语句：不满足条件提前返回
来源：http://akj.bbcook.cn

Py:   if not data: return
来源：http://bhl.ydzc1.top

PHP:  if (!$data) { return; }
来源：http://xns.bjfxy.top

JS:   if (!data) return;
来源：http://apj.sweek.top

TS:   if (!data) return;
来源：http://cvi.dianchejie.cn

Java: if (data == null) return;
来源：http://nxh.pycfn.com

Go:   if data == nil { return }
来源：http://pwn.smart0.xyz

Ruby: return if data.nil?
来源：http://hmn.xylfe.cn

C#:   if (data == null) return;
来源：http://ddc.zhoulong.xyz

================================================================================
来源：http://xbr.c1oappe.top

C. 函数与作用域
来源：http://oqb.316326.xyz

================================================================================
来源：http://abe.shanyushiyangkeji.top

[C01] 定义函数
来源：http://tvq.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://mts.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zlg.vehdjk.com

JS:   function add(a, b) { return a + b; }
来源：http://vue.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ope.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xkj.tanke756.top

Go:   func add(a, b int) int { return a + b }
来源：http://hzt.yueranfly.top

Ruby: def add(a, b); a + b; end
来源：http://ihj.sxryk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fob.ctjpmb.com

[C02] 默认参数
来源：http://dgt.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://gvf.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jod.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://fgi.jiagoushi.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jca.jinqigufen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uuz.yvedp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nmb.0kj1m.cn

Ruby: def greet(name = "World") = name
来源：http://iky.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://uke.yuanzhike.top

[C03] 可变参数
来源：http://ipy.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://orb.hammf.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://icx.aibaodan.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hny.sysykeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ntl.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fft.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xgd.daxiang520.top

Ruby: def total(*nums); nums.sum; end
来源：http://buo.epnwcf.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rmt.gaohongyu789.top

[C04] 命名参数 / 关键字参数
来源：http://yhw.ivvv.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jju.zhiwuduotai.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nvg.zhixingplan.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://krx.sweek.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://exw.ywan-chungtsiang.top

Java: // 无：用 Builder 模式或 record
来源：http://dhv.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://fuu.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://uqq.hysaishi.cn

C#:   f(a: 1, b: 2)
来源：http://gec.zhixingplan.top

[C05] 返回多个值
来源：http://squ.jyoumei.cn

Py:   return a, b
来源：http://xyn.tanke756.top

PHP:  return [$a, $b];
来源：http://ppe.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://pbu.cdnleiting.top

TS:   return { a, b };
来源：http://upg.zhoulong.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ofi.hnxiangtu.top

Go:   return a, b
来源：http://moa.fehbvm.com

Ruby: return a, b
来源：http://yvz.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://wfp.sysykeji.top

[C06] 匿名函数 / lambda
来源：http://vln.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://kah.ydzc1.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kgw.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://rhn.wangdashe.top

TS:   const square = (x: number): number => x * x;
来源：http://vls.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cjb.cashguo.top

Go:   sq := func(x int) int { return x * x }
来源：http://ivm.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://egb.meibo888.top

C#:   Func<int, int> square = x => x * x;
来源：http://atc.nwbrower.top

[C07] 把函数作为参数传入
来源：http://hgh.yj20258888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://abe.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://yrf.shanyushiyangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://txi.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://rmc.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://foq.hammf.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hgo.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://xrv.zhengqikj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://nqz.hfpthk.cn

[C08] 闭包
来源：http://giw.ywan-chungtsiang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xqb.shuidangran.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hug.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://prp.sweek.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://usg.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://msu.cdnleiting.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jri.havefunace.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dle.xylfe.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://peh.9152youxi.cn

[C09] 递归
来源：http://yoq.bjfxy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ahy.tarul.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ldl.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blw.yj20258888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dsd.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rbh.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hap.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zpn.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gom.sysykeji.top

[C10] 变量作用域
来源：http://pen.yvedp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://psa.fehbvm.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lml.hysaishi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://seg.chenzaomai.com

TS:   同 JS
来源：http://vvk.cqqwz.cn

Java: 方法内为块级作用域
来源：http://ril.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://oin.pengpengdd.cyou

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://opq.316326.xyz

C#:   块级作用域
来源：http://fme.ybcxt.top

[C11] 模块导入与导出
来源：http://jhe.daxiang520.top

Py:   from module import func
来源：http://mjk.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wmf.jqgufenzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tyt.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lww.yongpay.top

Java: import java.util.List;
来源：http://jaf.xylfe.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bfa.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://wmn.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://vfh.fehbvm.com

[C12] 立即执行函数 IIFE
来源：http://ena.yueranfly.top

Py:   (lambda: print("run"))()
来源：http://psv.nanxuanxn.top

PHP:  (function () { echo "run"; })();
来源：http://yjd.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://nef.ehwqpu.com

TS:   (() => { console.log("run"); })();
来源：http://pkp.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://otb.wangdashe.top


<!-- 参考信息 -->