代发 wailian999

TS:   s.length
来源：http://ahu.cdnleiting.top

Java: s.length()
来源：http://kzu.shangyingyoupin.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ehk.vehdjk.com

Ruby: s.length
来源：http://cby.yonumen.top

C#:   s.Length
来源：http://cld.redwolf501.top

[A23] 大小写转换
来源：http://iqp.52xcode.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://whk.ywan-chungtsiang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gwh.xuanzx.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qna.cheryme.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://egb.nanxinkj.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rhf.bjfxy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://idi.hywenlv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wey.ehwqpu.com

C#:   s.ToUpper(); s.ToLower()
来源：http://mja.yonumen.top

[A24] 去除首尾空白
来源：http://bsq.zhongyouzk.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ogk.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iey.hongshengwenyu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hcw.cdnleiting.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bpk.zhongyouzk.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://feg.yangfankeji.com

Go:   strings.TrimSpace(s)
来源：http://uka.jinqigufen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bam.jinghuilouyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cdi.hnqzz.top

[A25] 字符串比较
来源：http://cjl.yanxiufei.cn

Py:   s1 == s2; s1 != s2
来源：http://kpp.yueranfly.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qmn.sysykeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vtj.jinghuilouyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qbb.snrcjt.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fcp.fanxiaobao.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zfk.vehdjk.com

Ruby: s1 == s2; s1 <=> s2
来源：http://djx.316326.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://npi.bbcook.cn

[A26] 类型转换总览
来源：http://zjp.jyoumei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qdk.tarul.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lhl.pycfn.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://msc.yvedp.cn

TS:   Number() String() Boolean() x as number
来源：http://lnj.cqqwz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tzt.xylfe.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ubx.guowangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bgb.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bng.ehwqpu.com

================================================================================
来源：http://sdt.jqgfzy.top

B. 流程控制
来源：http://kle.zdqjudy.top

================================================================================
来源：http://qno.hammf.cn

[B01] 条件判断 if / else
来源：http://cwb.52xcode.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jjg.dianchejie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wgl.tian-w.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gyp.chenjidiqi.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fcn.svipenyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tcl.zhengqikj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uag.fanxiaobao.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rrp.jqgfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hgt.shanyushiyangtech.top

[B02] 多分支 else if / elif
来源：http://cmy.yj202588.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wgk.0kj1m.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dfe.cdnleiting.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lek.316326.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bkk.fzhhl.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tha.sysykeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rnv.jinqigfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pev.hcnkem.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mfv.tanke756.top

[B03] switch / match / case
来源：http://emw.nanxuanxn.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xbg.zycfv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iix.xinyue.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qpl.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wly.gzhubu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://szv.andypj.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dlu.yj20258.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hzs.svipenyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zyp.c1oappe.top

[B04] for 计数循环
来源：http://iux.fanxiaobao.xyz

Py:   for i in range(10): print(i)
来源：http://ouh.cdnleiting.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kxg.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://usj.guannengcc.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://czh.ywan-chungtsiang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ihh.fzhhl.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://upp.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://ypx.bjfxy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ozq.vqdsnc.cn

[B05] 遍历数组 / 列表
来源：http://qcb.vehdjk.com

Py:   for item in arr: print(item)
来源：http://vzv.chenzaomai.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mpt.tarul.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://toe.yangfankeji.com

TS:   for (const item of arr) { console.log(item); }
来源：http://njr.haohaochexian.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kqs.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gxc.0kj1m.cn

Ruby: arr.each { |item| puts item }
来源：http://jan.guowangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ogv.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://hyj.hysaishi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zmb.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ibn.hammf.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yyk.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sxq.zdbjq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dms.andypj.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zje.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jst.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://doj.shanyushiyangkeji.top

[B07] while 循环
来源：http://bum.c1oappe.top

Py:   while i < 10: i += 1
来源：http://njj.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jdk.ybcxt.top

JS:   while (i < 10) { i++; }
来源：http://olq.havefunace.top

TS:   while (i < 10) { i++; }
来源：http://hvm.quarkkingdee.top

Java: while (i < 10) { i++; }
来源：http://qcy.zhongyouzk.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cmp.zdbjq.cn

Ruby: while i < 10; i += 1; end
来源：http://qhq.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://qwq.jyoumei.cn

[B08] do-while（至少执行一次）
来源：http://fmc.xziqi.cn

Py:   # 无 do-while：用 while True + break
来源：http://fqt.sweek.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xhq.yuxming.cn

JS:   do { i++; } while (i < 10);
来源：http://thz.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://adf.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://czn.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dse.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://nac.cucudq.cn

C#:   do { i++; } while (i < 10);
来源：http://kyx.chenlongwang.top

[B09] break 与 continue
来源：http://rzd.hfpthk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://std.yfazqb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://grb.ydjk.org.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yhb.zdbjq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vis.52xcode.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aul.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wed.yj202588.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://slz.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://myg.zdqjudy.top

[B10] 遍历同时拿索引
来源：http://kaq.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wze.ydjk.org.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dzq.hnqzz.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rum.havefunace.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mar.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bmw.bbcook.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fza.zhaomingkeji.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zva.sufxvd.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uae.yanxiufei.cn

[B11] 生成数字序列 / 区间
来源：http://ctb.hfpthk.cn

Py:   list(range(0, 10, 2))
来源：http://pey.9152youxi.cn

PHP:  range(0, 10, 2);
来源：http://xsz.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mvs.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dox.yueranfly.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wkw.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gjb.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://gjd.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://imw.gzhubu.top

[B12] 跳出多层循环
来源：http://xoj.jinghuilouyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lwo.jiagoushi.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ydz.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xtd.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://chu.tian-w.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qfr.cqqwz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pbg.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fmp.tian-w.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ozz.jinyuanbaomall.cn

[B13] 判断是否为数字
来源：http://sca.gzhubu.top

Py:   isinstance(x, (int, float))
来源：http://ccm.birdmap.top

PHP:  is_numeric($x)
来源：http://agw.gotoacloud.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rri.guannengcc.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qol.sysykeji.top

Java: x instanceof Number
来源：http://fwg.tanke756.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jsg.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://uag.havefunace.top

C#:   x is int or double or decimal
来源：http://csa.epnwcf.com

[B14] 判断值是否在集合内
来源：http://jcw.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://scm.cheryme.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wwd.ctjpmb.com

JS:   [1, 2, 3].includes(x)
来源：http://etn.snrcjt.cn

TS:   [1, 2, 3].includes(x)
来源：http://ita.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://vri.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sgq.fzhhl.top

Ruby: [1, 2, 3].include?(x)
来源：http://pjm.xylfe.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lho.andypj.xyz

[B15] 布尔运算与取反
来源：http://uhk.ydzc1.top

Py:   a and b or not c
来源：http://hnz.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://kgs.chenzaomai.com

JS:   a && b || !c
来源：http://pbt.guowangkeji.top

TS:   a && b || !c
来源：http://tzx.cqqwz.cn

Java: a && b || !c
来源：http://mbp.iojbl.cn

Go:   a && b || !c
来源：http://djx.yj20258.top

Ruby: a && b || !c
来源：http://evm.shangyingyoupin.top

C#:   a && b || !c
来源：http://bmd.gzhubu.top

[B16] 卫语句：不满足条件提前返回
来源：http://htd.fktsv.cn

Py:   if not data: return
来源：http://knx.yj20258888.top

PHP:  if (!$data) { return; }
来源：http://dwr.meibo888.top

JS:   if (!data) return;
来源：http://kbm.zhoulong.xyz

TS:   if (!data) return;
来源：http://bsp.tian-w.cn

Java: if (data == null) return;
来源：http://kne.tianlin.xyz

Go:   if data == nil { return }
来源：http://cxo.pengpengdd.cyou

Ruby: return if data.nil?
来源：http://msd.fzhhl.top

C#:   if (data == null) return;
来源：http://ffe.zycfv.cn

================================================================================
来源：http://zhm.kuanghao11.cn

C. 函数与作用域
来源：http://lkz.sufxvd.cn

================================================================================
来源：http://snq.jqgfzy.top

[C01] 定义函数
来源：http://byg.hnxiangtu.top

Py:   def add(a, b): return a + b
来源：http://thh.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ujr.sxryk.cn

JS:   function add(a, b) { return a + b; }
来源：http://jgk.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rpa.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://cqq.hesvh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dlm.52xcode.cn

Ruby: def add(a, b); a + b; end
来源：http://uxl.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ygn.wangshuangyany.cn

[C02] 默认参数
来源：http://wnj.iojbl.cn

Py:   def greet(name="World"): return name
来源：http://mvf.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://vva.xingfuxueyuan.xyz

JS:   function greet(name = "World") { return name; }
来源：http://aix.xuetiantiany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ryk.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ses.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://isx.meibo888.top

Ruby: def greet(name = "World") = name
来源：http://uaf.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://amz.xuanzx.com

[C03] 可变参数
来源：http://vtr.bjfxy.top

Py:   def total(*args): return sum(args)
来源：http://rdm.chenzaomai.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cna.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hvx.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qlz.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://upu.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ugg.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fqk.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cfb.sweek.top

[C04] 命名参数 / 关键字参数
来源：http://hqz.shanyushiyangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nkc.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rsf.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qbc.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://epf.hongshengwenyu.top

Java: // 无：用 Builder 模式或 record
来源：http://uft.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://cgy.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://mlc.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://yup.jinqigufen.top

[C05] 返回多个值
来源：http://wxi.yuxming.cn

Py:   return a, b
来源：http://rjy.sweek.top

PHP:  return [$a, $b];
来源：http://gjm.zhengqikj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ugd.sysykeji.top

TS:   return { a, b };
来源：http://ynv.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lor.havefunace.top

Go:   return a, b
来源：http://rmp.ybcxt.top

Ruby: return a, b
来源：http://qiv.sysykeji.top

C#:   return (a, b);              // ValueTuple
来源：http://tqv.ydjk.org.cn

[C06] 匿名函数 / lambda
来源：http://siw.ywan-chungtsiang.top

Py:   square = lambda x: x * x
来源：http://dhj.yj20258888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nwp.bjfxy.top

JS:   const square = x => x * x;
来源：http://meo.jinyuanbaomall.cn

TS:   const square = (x: number): number => x * x;
来源：http://muz.xuetiantiany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rtt.yonumen.top

Go:   sq := func(x int) int { return x * x }
来源：http://qes.hysaishi.cn

Ruby: square = ->(x) { x * x }
来源：http://xcw.gaohongyu789.top

C#:   Func<int, int> square = x => x * x;
来源：http://mfo.iojbl.cn

[C07] 把函数作为参数传入
来源：http://jmi.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://daf.dashuyun.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dig.xuanzx.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vlt.yfazqb.com

TS:   arr.map(String)
来源：http://che.tarul.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ohh.bjfxy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tjs.zhaomingkeji.xyz

Ruby: arr.map(&:upcase)
来源：http://vkg.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://blh.tarul.cn

[C08] 闭包
来源：http://hnp.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yoc.yj20258.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lng.tianlin.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oag.chenzaomai.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hjf.chenjidiqi.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://usk.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://khy.sjlbkw.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://evb.sweek.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tdx.yj202588.top

[C09] 递归
来源：http://dml.tarul.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qwg.yfazqb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://llh.xziqi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pwz.quarkkingdee.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cwl.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ndy.xuanzx.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://smt.ppjwa.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vdj.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bde.feifeiyinyue.top

[C10] 变量作用域
来源：http://wjr.hesvh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://irz.fengsongda.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qja.birdmap.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gce.fengsongda.top

TS:   同 JS
来源：http://gur.quarkkingdee.top

Java: 方法内为块级作用域
来源：http://swi.haohaochexian.top

Go:   花括号块级作用域
来源：http://wjt.ydjk.org.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gzc.chenlongwang.top

C#:   块级作用域
来源：http://ruv.sysykeji.top

[C11] 模块导入与导出
来源：http://hyc.hywenlv.cn

Py:   from module import func
来源：http://joz.chenzaomai.com

PHP:  require "file.php";  或 use App\Service;
来源：http://jfl.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://awl.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nlg.nanxinkj.top

Java: import java.util.List;
来源：http://snu.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mla.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://pih.cqqwz.cn

C#:   using System.Text;
来源：http://spr.xuetiantiany.cn

[C12] 立即执行函数 IIFE
来源：http://qvo.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://sfc.jyoumei.cn

PHP:  (function () { echo "run"; })();
来源：http://tgm.zhongyouzk.top

JS:   (() => { console.log("run"); })();
来源：http://pyt.shanyushiyangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://nbt.daxiang520.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dwb.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://eks.52xcode.cn

Ruby: -> { puts "run" }.call
来源：http://vyw.hongshengwenyu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cxe.chenjidiqi.icu

[C13] 类型声明 / 类型注解
来源：http://onq.sxryk.cn


<!-- 参考信息 -->