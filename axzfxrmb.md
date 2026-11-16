代发 wailian999

C#:   s.Length
来源：http://axk.jianghu66.top

[A23] 大小写转换
来源：http://szp.quarkkingdee.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hgc.fanxiaobao.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xag.shzxlz.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://axc.hcnkem.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rdf.sysykeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cxf.birdmap.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tud.xuetiantiany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ovm.xylfe.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lex.yongpay.top

[A24] 去除首尾空白
来源：http://vtz.uphjek.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jju.zhengqikj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bia.jianghu66.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zrz.jinghuilouyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vaj.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://scp.yvedp.cn

Go:   strings.TrimSpace(s)
来源：http://bbh.andypj.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://euy.svipenyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wsf.shuidangran.top

[A25] 字符串比较
来源：http://ivm.guannengcc.top

Py:   s1 == s2; s1 != s2
来源：http://mqt.sxryk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://exu.zhijiandao.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bmb.chenzaomai.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lsn.sysykeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ksb.yanxiufei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://izv.ehwqpu.com

Ruby: s1 == s2; s1 <=> s2
来源：http://pbn.shangyingyoupin.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lzp.ctjpmb.com

[A26] 类型转换总览
来源：http://ydx.jinyuanbaomall.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jsx.redwolf501.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aof.xylfe.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zjd.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://wat.snrcjt.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cwn.jqgufenzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://inm.zdqjudy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://yar.cashguo.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://aly.xuanzx.com

================================================================================
来源：http://ivz.yanxiufei.cn

B. 流程控制
来源：http://iqv.hnxiangtu.top

================================================================================
来源：http://oga.yfazqb.com

[B01] 条件判断 if / else
来源：http://apq.nanxuanxn.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fah.fehbvm.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mgu.aizwys.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dap.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rnk.gotoacloud.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rat.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://azb.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://daz.mhx1999.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://loe.xinyue.icu

[B02] 多分支 else if / elif
来源：http://avk.zycfv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hth.ywan-chungtsiang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://odx.feifeiyinyue.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://huz.fanxiaobao.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yrj.wangdashe.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ixw.ppjwa.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ntf.daria6918.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://flk.feifeiyinyue.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lvc.feifeiyinyue.top

[B03] switch / match / case
来源：http://vhq.birdmap.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tgx.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xoc.zycfv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vdw.sysykeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yqc.aibaodan.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cfc.yfazqb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ijd.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ukj.yvedp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://muv.zdqjudy.top

[B04] for 计数循环
来源：http://yjs.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://hsd.pengpengdd.cyou

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xjp.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hun.bjfxy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vpx.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gdo.aizwys.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vap.yj20258.top

Ruby: 10.times { |i| puts i }
来源：http://nzg.jianghu66.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iry.jlsjyb.cn

[B05] 遍历数组 / 列表
来源：http://dst.hnqzz.top

Py:   for item in arr: print(item)
来源：http://oxe.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://okk.aizwys.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yfa.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lhz.quarkkingdee.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ejn.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wth.jlsjyb.cn

Ruby: arr.each { |item| puts item }
来源：http://srl.shanyushiyangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qfk.dianchejie.cn

[B06] 遍历字典 / 对象
来源：http://ggu.jinqigufen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mys.svipenyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uvy.hnxiangtu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tlb.pycfn.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hvh.sysykeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wht.sjlbkw.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bjh.zhijiandao.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://njg.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hlc.bbcook.cn

[B07] while 循环
来源：http://thu.yj20258888.top

Py:   while i < 10: i += 1
来源：http://vgt.snrcjt.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zrt.chenzaomai.com

JS:   while (i < 10) { i++; }
来源：http://cxu.zhijiandao.cn

TS:   while (i < 10) { i++; }
来源：http://knj.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://ykp.ydjk.org.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lih.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://bjr.xingfuxueyuan.xyz

C#:   while (i < 10) { i++; }
来源：http://fum.fehbvm.com

[B08] do-while（至少执行一次）
来源：http://loq.xinyue.icu

Py:   # 无 do-while：用 while True + break
来源：http://ewj.shanyushiyangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xbo.c1oappe.top

JS:   do { i++; } while (i < 10);
来源：http://shb.shuidangran.top

TS:   do { i++; } while (i < 10);
来源：http://rxw.haohaochexian.top

Java: do { i++; } while (i < 10);
来源：http://vlu.xziqi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bdp.jqgufenzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://kch.xuanzx.com

C#:   do { i++; } while (i < 10);
来源：http://zbt.xylfe.cn

[B09] break 与 continue
来源：http://mbs.dianchejie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zxk.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bya.ybcxt.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qxa.yonumen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ukq.aizwys.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uop.uphjek.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://urf.zycfv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iba.haohaochexian.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pvy.316326.xyz

[B10] 遍历同时拿索引
来源：http://bhl.zhiwuduotai.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hla.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://avt.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rtv.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://frs.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nck.xuanzx.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pvk.shanyushiyangtech.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rlm.zdbjq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://clr.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://bcw.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://efs.yanxiufei.cn

PHP:  range(0, 10, 2);
来源：http://clm.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nch.yanxiufei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kjl.yueranfly.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zxe.ctjpmb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cyv.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://pnz.vqdsnc.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kdl.vehdjk.com

[B12] 跳出多层循环
来源：http://zcn.shangyingyoupin.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yot.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hlz.cucudq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://boe.chenzaomai.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cke.shangyingyoupin.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nff.pycfn.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sjq.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wqo.cucudq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lbo.ctjpmb.com

[B13] 判断是否为数字
来源：http://ybv.fktsv.cn

Py:   isinstance(x, (int, float))
来源：http://deo.hnqzz.top

PHP:  is_numeric($x)
来源：http://knz.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xfh.mhx1999.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pyh.chenjidiqi.icu

Java: x instanceof Number
来源：http://heg.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jpg.hnqzz.top

Ruby: x.is_a?(Numeric)
来源：http://iok.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://zin.hfpthk.cn

[B14] 判断值是否在集合内
来源：http://tct.xingfuxueyuan.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oau.bjfxy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://anp.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://bcg.yj20258.top

TS:   [1, 2, 3].includes(x)
来源：http://ace.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dvi.xinyue.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fzq.gotoacloud.top

Ruby: [1, 2, 3].include?(x)
来源：http://nwt.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ftx.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://csi.mhx1999.top

Py:   a and b or not c
来源：http://yfe.sufxvd.cn

PHP:  $a && $b || !$c
来源：http://zok.xylfe.cn

JS:   a && b || !c
来源：http://rgr.pycfn.com

TS:   a && b || !c
来源：http://byr.ywan-chungtsiang.top

Java: a && b || !c
来源：http://stp.yongpay.top

Go:   a && b || !c
来源：http://fzd.havefunace.top

Ruby: a && b || !c
来源：http://ooy.tarul.cn

C#:   a && b || !c
来源：http://fkc.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://lxm.aizwys.cn

Py:   if not data: return
来源：http://bdr.zhaomingkeji.xyz

PHP:  if (!$data) { return; }
来源：http://dks.jianghu66.top

JS:   if (!data) return;
来源：http://iem.snrcjt.cn

TS:   if (!data) return;
来源：http://jpm.hywenlv.cn

Java: if (data == null) return;
来源：http://cio.yj20258.top

Go:   if data == nil { return }
来源：http://rnp.smart0.xyz

Ruby: return if data.nil?
来源：http://ruu.yfazqb.com

C#:   if (data == null) return;
来源：http://sgi.shzxlz.cn

================================================================================
来源：http://pwx.gotoacloud.top

C. 函数与作用域
来源：http://lbo.chenjidiqi.icu

================================================================================
来源：http://zfg.smart0.xyz

[C01] 定义函数
来源：http://tgf.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://xab.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eek.mhx1999.top

JS:   function add(a, b) { return a + b; }
来源：http://qpk.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ajn.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nnn.sxryk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ioa.jiagoushi.top

Ruby: def add(a, b); a + b; end
来源：http://etq.jinyuanbaomall.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wix.jyoumei.cn

[C02] 默认参数
来源：http://cqg.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://kpj.cucudq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pgy.ppjwa.cn

JS:   function greet(name = "World") { return name; }
来源：http://nmw.xingfuxueyuan.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://egv.chenlongwang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tnz.cashguo.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lll.jinyuanbaomall.cn

Ruby: def greet(name = "World") = name
来源：http://btj.snrcjt.cn

C#:   string Greet(string name = "World") => name;
来源：http://nyw.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://sxg.hywenlv.cn

Py:   def total(*args): return sum(args)
来源：http://vhv.vqdsnc.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://djt.xuanzx.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qae.svipenyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ylf.fanxiaobao.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qtw.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ooq.jqgfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://jny.shuidangran.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yxv.cashguo.top

[C04] 命名参数 / 关键字参数
来源：http://iwk.haohaochexian.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://smo.hnqzz.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://klm.ctjpmb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://utd.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tfz.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://rrp.mhx1999.top

Go:   // 无：用配置结构体参数
来源：http://jxs.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://pyz.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://nkf.yfazqb.com

[C05] 返回多个值
来源：http://nez.jlsjyb.cn

Py:   return a, b
来源：http://agh.guowangkeji.top

PHP:  return [$a, $b];
来源：http://ucn.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://gku.gogol.net.cn

TS:   return { a, b };
来源：http://pjm.52xcode.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dtg.hongshengwenyu.top

Go:   return a, b
来源：http://kuf.kuanghao11.cn

Ruby: return a, b
来源：http://dwu.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://ipi.hnxiangtu.top

[C06] 匿名函数 / lambda
来源：http://yda.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://tgm.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://oup.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://kbc.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://ytf.tarul.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ilj.52xcode.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kpj.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://xvi.shangyingyoupin.top

C#:   Func<int, int> square = x => x * x;
来源：http://xxq.shanyushiyangtech.top

[C07] 把函数作为参数传入
来源：http://ucp.yongpay.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hwt.guowangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://osv.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dcl.cheryme.top

TS:   arr.map(String)
来源：http://zdh.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rzb.chenzaomai.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cfo.fzhhl.top

Ruby: arr.map(&:upcase)
来源：http://hle.xinyue.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://xwy.aibaodan.cn

[C08] 闭包
来源：http://ncg.meibo888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vri.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vlz.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rxd.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nor.tian-w.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qcm.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oid.ybcxt.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ito.daxiang520.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://okh.redwolf501.top

[C09] 递归
来源：http://stl.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ovp.yj20258.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pbg.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ort.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bdg.xinyue.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jaw.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rbg.wangshuangyany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kdu.fktsv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fzp.zhijiandao.cn

[C10] 变量作用域
来源：http://cno.guannengcc.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ago.ehwqpu.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fhg.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qxy.svipenyu.cn

TS:   同 JS
来源：http://zku.shanyushiyangtech.top

Java: 方法内为块级作用域
来源：http://amr.chenzaomai.com

Go:   花括号块级作用域
来源：http://hqr.dianchejie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://flx.fanxiaobao.xyz

C#:   块级作用域
来源：http://coo.hnqzz.top

[C11] 模块导入与导出
来源：http://ghv.jinqigufen.top

Py:   from module import func
来源：http://mgi.zhoulong.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://vkp.bbcook.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://czq.yuxming.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xsf.bbcook.cn

Java: import java.util.List;
来源：http://nbi.hnxiangtu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bjx.birdmap.top

Ruby: require "json"; require_relative "./util"
来源：http://bvu.hywenlv.cn

C#:   using System.Text;
来源：http://ghy.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://ifl.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://qdb.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://aex.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://bba.svipenyu.cn

TS:   (() => { console.log("run"); })();
来源：http://rgk.pycfn.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xmt.ppjwa.cn

Go:   func() { fmt.Println("run") }()
来源：http://uan.uphjek.com

Ruby: -> { puts "run" }.call
来源：http://ihl.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kws.snrcjt.cn

[C13] 类型声明 / 类型注解
来源：http://kdp.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://csg.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qrl.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wnp.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oko.cdnleiting.top


<!-- 参考信息 -->