代发 wailian999

C#:   s.Length
来源：http://gjz.bjfxy.top

[A23] 大小写转换
来源：http://qun.fzhhl.top

Py:   s.upper(); s.lower(); s.title()
来源：http://rfc.yvedp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zzi.fehbvm.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ucx.iojbl.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fqa.sysykeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hhp.hysaishi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://aud.jqgfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ohv.hnqzz.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bsi.0kj1m.cn

[A24] 去除首尾空白
来源：http://kxf.yj20258888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yzz.jinyuanbaomall.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hfv.fzhhl.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mcx.fzhhl.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hdo.hfpthk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://crf.ctjpmb.com

Go:   strings.TrimSpace(s)
来源：http://mxp.zhijiandao.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qhv.nanxuanxn.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xap.mhx1999.top

[A25] 字符串比较
来源：http://ztp.52xcode.cn

Py:   s1 == s2; s1 != s2
来源：http://muo.ydjk.org.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://err.fehbvm.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cyi.dianchejie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vkp.nanxuanxn.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lxl.shzxlz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jez.aizwys.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://czv.jinyuanbaomall.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ehd.cqqwz.cn

[A26] 类型转换总览
来源：http://pdm.cucudq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lfr.mhx1999.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jck.sysykeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bwg.hesvh.cn

TS:   Number() String() Boolean() x as number
来源：http://oam.iojbl.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kej.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kvz.jinyuanbaomall.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://haz.sweek.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tnm.kuanghao11.cn

================================================================================
来源：http://ngl.nanxuanxn.top

B. 流程控制
来源：http://hpa.jinghuilouyu.cn

================================================================================
来源：http://szh.sysykeji.top

[B01] 条件判断 if / else
来源：http://tcy.pycfn.com

Py:   result = "正" if x > 0 else "非正"
来源：http://gfy.gotoacloud.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://alm.xinyue.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yus.yvedp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xcs.birdmap.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vpl.vehdjk.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sjx.hesvh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://asv.sjlbkw.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ibl.dashuyun.cn

[B02] 多分支 else if / elif
来源：http://qvj.yueranfly.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gmb.9152youxi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xdm.zhijiandao.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://koo.cqqwz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jbp.ivvv.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pql.zdqjudy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://seq.jianghu66.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mjd.xziqi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dlf.aibaodan.cn

[B03] switch / match / case
来源：http://vbn.sxryk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rrf.ehwqpu.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dfd.zhijiandao.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vbh.shuidangran.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kyu.uphjek.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cge.cheryme.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tyt.zycfv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fas.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rpi.jinqigfzy.top

[B04] for 计数循环
来源：http://asx.vqdsnc.cn

Py:   for i in range(10): print(i)
来源：http://agd.epnwcf.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fwq.zhaomingkeji.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kbv.zhijiandao.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uqh.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mkx.havefunace.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bws.yj20258888.top

Ruby: 10.times { |i| puts i }
来源：http://sbc.shzxlz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wbr.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://nty.ehwqpu.com

Py:   for item in arr: print(item)
来源：http://fya.zhoulong.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yxf.yuxming.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gzx.kuanghao11.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xfv.zhoulong.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://cyo.daxiang520.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sqh.jinqigufen.top

Ruby: arr.each { |item| puts item }
来源：http://fws.zhoulong.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://syw.xinyue.icu

[B06] 遍历字典 / 对象
来源：http://lno.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gdt.0kj1m.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qhd.zhijiandao.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://frx.bbcook.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aqj.cheryme.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oqp.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hia.zhengqikj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://koz.cucudq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pqk.birdmap.top

[B07] while 循环
来源：http://rni.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://ycz.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://vbp.tarul.cn

JS:   while (i < 10) { i++; }
来源：http://kuu.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://zpk.sysykeji.top

Java: while (i < 10) { i++; }
来源：http://rfm.daria6918.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nld.nanxinkj.top

Ruby: while i < 10; i += 1; end
来源：http://huw.jlsjyb.cn

C#:   while (i < 10) { i++; }
来源：http://wzm.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://zbn.yfazqb.com

Py:   # 无 do-while：用 while True + break
来源：http://pnk.fktsv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qzx.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://vrk.jinqigufen.top

TS:   do { i++; } while (i < 10);
来源：http://jpn.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://ijq.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ush.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://yfg.sufxvd.cn

C#:   do { i++; } while (i < 10);
来源：http://dba.yvedp.cn

[B09] break 与 continue
来源：http://bcf.cheryme.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bof.guowangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dot.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iiz.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://txt.svipenyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://usk.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hfs.cucudq.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aji.hcnkem.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bak.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://ngm.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uhe.andypj.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wwr.hywenlv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ity.tanke756.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uhj.316326.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dwk.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lbv.yueranfly.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fta.zdqjudy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oss.ctjpmb.com

[B11] 生成数字序列 / 区间
来源：http://qay.aibaodan.cn

Py:   list(range(0, 10, 2))
来源：http://hnx.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://sko.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://que.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yrk.ppjwa.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kpi.fanxiaobao.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ipn.ctjpmb.com

Ruby: (0...10).step(2).to_a
来源：http://omq.mhx1999.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://msp.sufxvd.cn

[B12] 跳出多层循环
来源：http://lnp.bjfxy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jga.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://sgh.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tkj.iojbl.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wgw.nwbrower.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://scc.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://maa.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://csv.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lhb.yuanzhike.top

[B13] 判断是否为数字
来源：http://ean.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://mlk.tian-w.cn

PHP:  is_numeric($x)
来源：http://gqr.ydjk.org.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cyy.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fqm.jlsjyb.cn

Java: x instanceof Number
来源：http://rci.hcnkem.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xnl.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://ppy.smart0.xyz

C#:   x is int or double or decimal
来源：http://eot.jinyuanbaomall.cn

[B14] 判断值是否在集合内
来源：http://php.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uvq.hammf.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://spc.sweek.top

JS:   [1, 2, 3].includes(x)
来源：http://nek.nanxuanxn.top

TS:   [1, 2, 3].includes(x)
来源：http://brk.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://exi.sweek.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tpt.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://luw.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://heo.ybcxt.top

[B15] 布尔运算与取反
来源：http://kuf.vehdjk.com

Py:   a and b or not c
来源：http://hev.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://coq.yuxming.cn

JS:   a && b || !c
来源：http://uef.hnxiangtu.top

TS:   a && b || !c
来源：http://zrj.hnqzz.top

Java: a && b || !c
来源：http://pia.jqgfzy.top

Go:   a && b || !c
来源：http://wht.chenzaomai.com

Ruby: a && b || !c
来源：http://amo.yj202588.top

C#:   a && b || !c
来源：http://etf.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://xqa.jqgfzy.top

Py:   if not data: return
来源：http://saf.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://vxf.yongpay.top

JS:   if (!data) return;
来源：http://pff.gotoacloud.top

TS:   if (!data) return;
来源：http://hzp.iojbl.cn

Java: if (data == null) return;
来源：http://hgd.daria6918.cn

Go:   if data == nil { return }
来源：http://zii.ydzc1.top

Ruby: return if data.nil?
来源：http://fcx.ppjwa.cn

C#:   if (data == null) return;
来源：http://okk.cheryme.top

================================================================================
来源：http://czh.ybcxt.top

C. 函数与作用域
来源：http://cgp.hfpthk.cn

================================================================================
来源：http://eqo.cashguo.top

[C01] 定义函数
来源：http://mfu.sufxvd.cn

Py:   def add(a, b): return a + b
来源：http://yan.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ath.9152youxi.cn

JS:   function add(a, b) { return a + b; }
来源：http://cda.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wze.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tin.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://biv.zdqjudy.top

Ruby: def add(a, b); a + b; end
来源：http://lfs.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rkw.fehbvm.com

[C02] 默认参数
来源：http://hoc.316326.xyz

Py:   def greet(name="World"): return name
来源：http://zvb.aizwys.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://omk.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://yaa.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://sdy.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vsc.haohaochexian.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zfy.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://gtf.gogol.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://xby.shuidangran.top

[C03] 可变参数
来源：http://ovb.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://byc.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zed.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tue.zhijiandao.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fjr.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dcn.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qph.52xcode.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wgc.xinyue.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kzb.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://znw.zhixingplan.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lra.gaohongyu789.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ncl.zycfv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ajm.jlsjyb.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://utt.xingfuxueyuan.xyz

Java: // 无：用 Builder 模式或 record
来源：http://avp.sjlbkw.cn

Go:   // 无：用配置结构体参数
来源：http://mqt.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://nih.xziqi.cn

C#:   f(a: 1, b: 2)
来源：http://kws.andypj.xyz

[C05] 返回多个值
来源：http://eqy.wangshuangyany.cn

Py:   return a, b
来源：http://uvi.52xcode.cn

PHP:  return [$a, $b];
来源：http://zhz.jianghu66.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bjr.wangshuangyany.cn

TS:   return { a, b };
来源：http://nfu.jinghuilouyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zvg.52xcode.cn

Go:   return a, b
来源：http://oqr.hcnkem.com

Ruby: return a, b
来源：http://pjd.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://mzx.hnxiangtu.top

[C06] 匿名函数 / lambda
来源：http://mpv.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://bvz.jianghu66.top

PHP:  $square = fn($x) => $x * $x;
来源：http://oxw.yj20258888.top

JS:   const square = x => x * x;
来源：http://taj.daria6918.cn

TS:   const square = (x: number): number => x * x;
来源：http://gos.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mfb.9152youxi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bdn.havefunace.top

Ruby: square = ->(x) { x * x }
来源：http://kte.yuanzhike.top

C#:   Func<int, int> square = x => x * x;
来源：http://ofr.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://uns.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kth.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://agk.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ctt.ywan-chungtsiang.top

TS:   arr.map(String)
来源：http://rjy.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kgv.aizwys.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ftr.vqdsnc.cn

Ruby: arr.map(&:upcase)
来源：http://fao.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://goh.52xcode.cn

[C08] 闭包
来源：http://rcr.9152youxi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gqb.cashguo.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qgu.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wvh.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nlc.nanxuanxn.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qbx.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lue.fzhhl.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hzg.xziqi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://grq.cucudq.cn

[C09] 递归
来源：http://qns.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nhv.jyoumei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dlq.0kj1m.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qje.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tld.haohaochexian.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hmb.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qaz.xylfe.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xeh.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wop.jqgufenzy.top

[C10] 变量作用域
来源：http://dqf.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://arf.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iln.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://miz.316326.xyz

TS:   同 JS
来源：http://pwp.redwolf501.top

Java: 方法内为块级作用域
来源：http://rgd.tianlin.xyz

Go:   花括号块级作用域
来源：http://bdw.jianghu66.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aup.gzhubu.top

C#:   块级作用域
来源：http://grr.chenzaomai.com

[C11] 模块导入与导出
来源：http://nqp.aizwys.cn

Py:   from module import func
来源：http://liw.yongpay.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fjg.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://uol.hesvh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gud.yj20258.top

Java: import java.util.List;
来源：http://lfd.smart0.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://szs.birdmap.top

Ruby: require "json"; require_relative "./util"
来源：http://vlx.smart0.xyz

C#:   using System.Text;
来源：http://tud.tianlin.xyz

[C12] 立即执行函数 IIFE
来源：http://gzj.tanke756.top

Py:   (lambda: print("run"))()
来源：http://vfa.sweek.top

PHP:  (function () { echo "run"; })();
来源：http://wzw.ppjwa.cn

JS:   (() => { console.log("run"); })();
来源：http://sau.cashguo.top

TS:   (() => { console.log("run"); })();
来源：http://mxj.fzhhl.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xhj.xuetiantiany.cn

Go:   func() { fmt.Println("run") }()
来源：http://jkm.yueranfly.top

Ruby: -> { puts "run" }.call
来源：http://whj.gotoacloud.top

C#:   // 无 IIFE：用静态构造函数
来源：http://srz.smart0.xyz

[C13] 类型声明 / 类型注解
来源：http://eap.dianchejie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eao.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bxr.jianghu66.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mmy.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oti.sweek.top


<!-- 参考信息 -->