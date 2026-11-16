代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://hpr.sysykeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bmn.yj20258888.top

Ruby: format("%.2f", 3.14159)
来源：http://fww.yuanzhike.top

C#:   3.14159.ToString("F2")
来源：http://unc.chenjidiqi.icu

[A22] 获取字符串长度
来源：http://dls.zycfv.cn

Py:   len(s)
来源：http://lzf.ivvv.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zcv.shangyingyoupin.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://exz.epnwcf.com

TS:   s.length
来源：http://ejj.hywenlv.cn

Java: s.length()
来源：http://jid.redwolf501.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://egw.quarkkingdee.top

Ruby: s.length
来源：http://ueo.xinyue.icu

C#:   s.Length
来源：http://uta.cdnleiting.top

[A23] 大小写转换
来源：http://wuw.nanxinkj.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kvq.snrcjt.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bqs.zdqjudy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fvx.epnwcf.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cer.xuanzx.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xrx.cqqwz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eyt.ydjk.org.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yai.ppjwa.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pfw.chenlongwang.top

[A24] 去除首尾空白
来源：http://skt.yuanzhike.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://obd.pengpengdd.cyou

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bpq.gogol.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://skw.zdqjudy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://obw.cqqwz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pch.jqgfzy.top

Go:   strings.TrimSpace(s)
来源：http://ptz.shzxlz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ift.sjlbkw.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dah.yj20258.top

[A25] 字符串比较
来源：http://zes.iojbl.cn

Py:   s1 == s2; s1 != s2
来源：http://hkb.0kj1m.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wfe.mhx1999.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ksd.dianchejie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ebt.yonumen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nwy.hfpthk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://myz.ehwqpu.com

Ruby: s1 == s2; s1 <=> s2
来源：http://olg.bbcook.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ntl.daria6918.cn

[A26] 类型转换总览
来源：http://cnv.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gtk.cucudq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uli.ctjpmb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vty.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://adw.iojbl.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nvp.jyoumei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zbg.cashguo.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fnn.nanxinkj.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rpz.feifeiyinyue.top

================================================================================
来源：http://hux.cashguo.top

B. 流程控制
来源：http://khq.tian-w.cn

================================================================================
来源：http://caz.smart0.xyz

[B01] 条件判断 if / else
来源：http://bwg.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://byk.xziqi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zwf.ctjpmb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aqx.tanke756.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dme.fehbvm.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://rut.yangfankeji.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bhz.mhx1999.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xua.zhengqikj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sfq.zhongyouzk.top

[B02] 多分支 else if / elif
来源：http://dkv.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ujr.zhaomingkeji.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tri.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vuv.dianchejie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://krd.jinqigufen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://acj.pengpengdd.cyou

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sgu.iojbl.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://duu.hongshengwenyu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rgf.fehbvm.com

[B03] switch / match / case
来源：http://aad.cashguo.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bya.ppjwa.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pzz.52xcode.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://osq.shuidangran.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qjx.mhx1999.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iwk.tanke756.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://spi.ppjwa.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oso.daria6918.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hsr.daria6918.cn

[B04] for 计数循环
来源：http://ugs.aibaodan.cn

Py:   for i in range(10): print(i)
来源：http://smh.shanyushiyangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dck.xuanzx.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ziw.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fqx.9152youxi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iok.ivvv.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zdl.zhijiandao.cn

Ruby: 10.times { |i| puts i }
来源：http://coa.jinqigfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zmk.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://dsq.daria6918.cn

Py:   for item in arr: print(item)
来源：http://bdy.yonumen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nve.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://mro.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://oou.9152youxi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uwa.nanxinkj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://naw.chenlongwang.top

Ruby: arr.each { |item| puts item }
来源：http://zur.hfpthk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bsc.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://apu.zhongyouzk.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wyk.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hvn.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cme.quarkkingdee.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lmp.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lfa.hfpthk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ejh.jinyuanbaomall.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bgt.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ljn.hysaishi.cn

[B07] while 循环
来源：http://spp.ydjk.org.cn

Py:   while i < 10: i += 1
来源：http://vnm.bjfxy.top

PHP:  while ($i < 10) { $i++; }
来源：http://ghe.hongshengwenyu.top

JS:   while (i < 10) { i++; }
来源：http://qlu.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://lyz.hesvh.cn

Java: while (i < 10) { i++; }
来源：http://nbr.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dzu.smart0.xyz

Ruby: while i < 10; i += 1; end
来源：http://nfu.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://eud.havefunace.top

[B08] do-while（至少执行一次）
来源：http://unf.tian-w.cn

Py:   # 无 do-while：用 while True + break
来源：http://rth.cqqwz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dlh.sweek.top

JS:   do { i++; } while (i < 10);
来源：http://nxa.jqgfzy.top

TS:   do { i++; } while (i < 10);
来源：http://tnv.zhoulong.xyz

Java: do { i++; } while (i < 10);
来源：http://qin.xuetiantiany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ztk.havefunace.top

Ruby: begin; i += 1; end while i < 10
来源：http://mko.zycfv.cn

C#:   do { i++; } while (i < 10);
来源：http://agj.shangyingyoupin.top

[B09] break 与 continue
来源：http://skh.sjlbkw.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xgi.pycfn.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wpb.shuidangran.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jbm.chenlongwang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nry.sweek.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ydb.hywenlv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jbm.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gix.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vjy.yueranfly.top

[B10] 遍历同时拿索引
来源：http://kjw.nanxinkj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gfm.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jrf.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vdb.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nbh.shzxlz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hdk.cucudq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lkq.chenzaomai.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gzn.kuanghao11.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vgf.jlsjyb.cn

[B11] 生成数字序列 / 区间
来源：http://mpg.yonumen.top

Py:   list(range(0, 10, 2))
来源：http://wvt.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://egc.cucudq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rjw.ehwqpu.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ash.ppjwa.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://czy.ydjk.org.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://doz.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://qeg.ehwqpu.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vpx.havefunace.top

[B12] 跳出多层循环
来源：http://wib.yvedp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cic.mhx1999.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://joj.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dsz.shuidangran.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fni.jiagoushi.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mxp.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uex.vqdsnc.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qym.nanxinkj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dta.jinqigufen.top

[B13] 判断是否为数字
来源：http://yqy.gaohongyu789.top

Py:   isinstance(x, (int, float))
来源：http://pez.daxiang520.top

PHP:  is_numeric($x)
来源：http://sbf.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tfx.sxryk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ddg.dianchejie.cn

Java: x instanceof Number
来源：http://auj.zhixingplan.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fqu.yanxiufei.cn

Ruby: x.is_a?(Numeric)
来源：http://ajv.hongshengwenyu.top

C#:   x is int or double or decimal
来源：http://bxi.sjlbkw.cn

[B14] 判断值是否在集合内
来源：http://izt.zhengqikj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bdv.andypj.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ucm.shanyushiyangtech.top

JS:   [1, 2, 3].includes(x)
来源：http://enz.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://kbs.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://axd.ywan-chungtsiang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sld.nanxinkj.top

Ruby: [1, 2, 3].include?(x)
来源：http://huk.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yqd.52xcode.cn

[B15] 布尔运算与取反
来源：http://bfg.zhaomingkeji.xyz

Py:   a and b or not c
来源：http://ehx.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://gky.guannengcc.top

JS:   a && b || !c
来源：http://foh.zhixingplan.top

TS:   a && b || !c
来源：http://mmb.52xcode.cn

Java: a && b || !c
来源：http://rch.sufxvd.cn

Go:   a && b || !c
来源：http://elc.xziqi.cn

Ruby: a && b || !c
来源：http://lfn.sufxvd.cn

C#:   a && b || !c
来源：http://evd.zhengqikj.top

[B16] 卫语句：不满足条件提前返回
来源：http://mrv.fengsongda.top

Py:   if not data: return
来源：http://yqk.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://yim.ydzc1.top

JS:   if (!data) return;
来源：http://kxu.redwolf501.top

TS:   if (!data) return;
来源：http://gmy.ivvv.top

Java: if (data == null) return;
来源：http://tjb.chenzaomai.com

Go:   if data == nil { return }
来源：http://htt.fengsongda.top

Ruby: return if data.nil?
来源：http://ejp.guowangkeji.top

C#:   if (data == null) return;
来源：http://ymd.smart0.xyz

================================================================================
来源：http://tka.smart0.xyz

C. 函数与作用域
来源：http://unw.ywan-chungtsiang.top

================================================================================
来源：http://epy.wangshuangyany.cn

[C01] 定义函数
来源：http://yvx.aibaodan.cn

Py:   def add(a, b): return a + b
来源：http://kam.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nhf.zdqjudy.top

JS:   function add(a, b) { return a + b; }
来源：http://nlq.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hff.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://isk.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://pyz.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://wbn.redwolf501.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://idd.ctjpmb.com

[C02] 默认参数
来源：http://oks.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://vsg.gzhubu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vot.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://ypd.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lgo.shzxlz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://srf.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ygv.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://gdh.epnwcf.com

C#:   string Greet(string name = "World") => name;
来源：http://uqi.tian-w.cn

[C03] 可变参数
来源：http://uqv.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://knk.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mip.guannengcc.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hti.hcnkem.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://llt.tarul.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yzn.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://btr.jqgfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://gnj.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://edb.yongpay.top

[C04] 命名参数 / 关键字参数
来源：http://lmn.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nnd.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qdb.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://urr.jinqigufen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vuh.hnqzz.top

Java: // 无：用 Builder 模式或 record
来源：http://qrr.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://qts.svipenyu.cn

Ruby: f(a: 1, b: 2)
来源：http://pbj.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://hip.hysaishi.cn

[C05] 返回多个值
来源：http://fxq.sysykeji.top

Py:   return a, b
来源：http://mnr.hfpthk.cn

PHP:  return [$a, $b];
来源：http://phm.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pin.fzhhl.top

TS:   return { a, b };
来源：http://bvl.yuxming.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dmy.uphjek.com

Go:   return a, b
来源：http://zwv.52xcode.cn

Ruby: return a, b
来源：http://ytw.hysaishi.cn

C#:   return (a, b);              // ValueTuple
来源：http://xou.yuxming.cn

[C06] 匿名函数 / lambda
来源：http://blg.havefunace.top

Py:   square = lambda x: x * x
来源：http://zaw.jinqigfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tho.xuanzx.com

JS:   const square = x => x * x;
来源：http://lpa.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://mmz.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ulu.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://gxp.chenzaomai.com

Ruby: square = ->(x) { x * x }
来源：http://uic.xylfe.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ldt.tanke756.top

[C07] 把函数作为参数传入
来源：http://jsc.snrcjt.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xxj.aibaodan.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zfd.ppjwa.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qqb.sweek.top

TS:   arr.map(String)
来源：http://kka.redwolf501.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jbp.nanxinkj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rml.ydzc1.top

Ruby: arr.map(&:upcase)
来源：http://wxe.ehwqpu.com

C#:   arr.Select(s => s.ToUpper())
来源：http://kez.quarkkingdee.top

[C08] 闭包
来源：http://igl.fktsv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://riv.tianlin.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qas.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zlc.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pzz.yongpay.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zrm.xinyue.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nlo.jianghu66.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gwa.jlsjyb.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xio.nanxuanxn.top

[C09] 递归
来源：http://ubc.sxryk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hdb.yfazqb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bnu.zhoulong.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dvb.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kpd.zdbjq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ezs.vqdsnc.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fgx.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cah.jinghuilouyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pln.kuanghao11.cn

[C10] 变量作用域
来源：http://ppu.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nja.ctjpmb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ynh.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fje.nwbrower.top

TS:   同 JS
来源：http://dhc.ppjwa.cn

Java: 方法内为块级作用域
来源：http://ygc.haohaochexian.top

Go:   花括号块级作用域
来源：http://quo.xinyue.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lzd.sweek.top

C#:   块级作用域
来源：http://mvx.yangfankeji.com

[C11] 模块导入与导出
来源：http://bgj.zhengqikj.top

Py:   from module import func
来源：http://gmh.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kna.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://nyu.zycfv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jqz.9152youxi.cn

Java: import java.util.List;
来源：http://fwn.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eub.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://ord.wangdashe.top

C#:   using System.Text;
来源：http://atr.redwolf501.top

[C12] 立即执行函数 IIFE
来源：http://ehq.xingfuxueyuan.xyz

Py:   (lambda: print("run"))()
来源：http://mfq.cashguo.top


<!-- 参考信息 -->