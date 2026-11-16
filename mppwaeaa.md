代发 wailian999

C#:   s.Length
来源：http://wmd.hongshengwenyu.top

[A23] 大小写转换
来源：http://abb.meibo888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://izd.shzxlz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mrw.yfazqb.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://joc.tarul.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tgj.bbcook.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nfq.tian-w.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lpa.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pou.quarkkingdee.top

C#:   s.ToUpper(); s.ToLower()
来源：http://clc.snrcjt.cn

[A24] 去除首尾空白
来源：http://ecs.meibo888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aab.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gem.jyoumei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qcv.dashuyun.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ysm.gogol.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zyj.chenlongwang.top

Go:   strings.TrimSpace(s)
来源：http://veq.zhongyouzk.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://omx.ctjpmb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pjn.quarkkingdee.top

[A25] 字符串比较
来源：http://svt.ehwqpu.com

Py:   s1 == s2; s1 != s2
来源：http://evl.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pzk.zhijiandao.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://icz.cucudq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tkz.sufxvd.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kgr.zycfv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qfz.bbcook.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rdo.ppjwa.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ech.xuetiantiany.cn

[A26] 类型转换总览
来源：http://inl.jlsjyb.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tmh.jinqigufen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://twu.zhaomingkeji.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qxt.shangyingyoupin.top

TS:   Number() String() Boolean() x as number
来源：http://enh.jinqigufen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ini.hnxiangtu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wnx.fengsongda.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vzi.ybcxt.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://smt.bjfxy.top

================================================================================
来源：http://vde.yuanzhike.top

B. 流程控制
来源：http://gcv.sufxvd.cn

================================================================================
来源：http://vwx.hammf.cn

[B01] 条件判断 if / else
来源：http://jdn.fzhhl.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vld.daria6918.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mle.nanxuanxn.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pae.ydzc1.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hvy.0kj1m.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oxh.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pog.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blz.fengsongda.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mtm.ydzc1.top

[B02] 多分支 else if / elif
来源：http://bub.vehdjk.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bfo.zhaomingkeji.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vbr.zycfv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ebz.jqgufenzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vnl.jinyuanbaomall.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ybk.meibo888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rwr.shangyingyoupin.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lfj.jlsjyb.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dpd.c1oappe.top

[B03] switch / match / case
来源：http://kae.daria6918.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dpm.guannengcc.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fyr.cucudq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cbr.zhongyouzk.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zhu.9152youxi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fvy.zhixingplan.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://okl.zhengqikj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oxs.redwolf501.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fpc.sjlbkw.cn

[B04] for 计数循环
来源：http://qiv.hnxiangtu.top

Py:   for i in range(10): print(i)
来源：http://osr.nwbrower.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nlh.yuxming.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://glc.gogol.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://umv.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mgg.hysaishi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lgs.ehwqpu.com

Ruby: 10.times { |i| puts i }
来源：http://tjh.ydzc1.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kza.daxiang520.top

[B05] 遍历数组 / 列表
来源：http://drx.ppjwa.cn

Py:   for item in arr: print(item)
来源：http://gai.tian-w.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kab.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ccc.zhaomingkeji.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://tsu.9152youxi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wgk.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wxl.jianghu66.top

Ruby: arr.each { |item| puts item }
来源：http://ift.sxryk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bvy.hesvh.cn

[B06] 遍历字典 / 对象
来源：http://aaz.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://yqe.nanxinkj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ccx.mhx1999.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rxp.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xsf.yfazqb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vbi.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kxz.yj20258888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wgv.fktsv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hgo.hnxiangtu.top

[B07] while 循环
来源：http://tzc.zycfv.cn

Py:   while i < 10: i += 1
来源：http://tov.nanxinkj.top

PHP:  while ($i < 10) { $i++; }
来源：http://dmr.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://viv.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://ukk.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://gmz.jqgufenzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zty.fktsv.cn

Ruby: while i < 10; i += 1; end
来源：http://piz.jqgfzy.top

C#:   while (i < 10) { i++; }
来源：http://hkw.yuxming.cn

[B08] do-while（至少执行一次）
来源：http://umi.yangfankeji.com

Py:   # 无 do-while：用 while True + break
来源：http://aol.fzhhl.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bcq.ctjpmb.com

JS:   do { i++; } while (i < 10);
来源：http://oyc.fanxiaobao.xyz

TS:   do { i++; } while (i < 10);
来源：http://iyr.svipenyu.cn

Java: do { i++; } while (i < 10);
来源：http://kvt.cucudq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iwf.uphjek.com

Ruby: begin; i += 1; end while i < 10
来源：http://vdf.xuanzx.com

C#:   do { i++; } while (i < 10);
来源：http://lay.redwolf501.top

[B09] break 与 continue
来源：http://jdt.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bci.nanxinkj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kir.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mtk.hongshengwenyu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lzw.gaohongyu789.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://llw.wangshuangyany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tya.zhengqikj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pth.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wjg.feifeiyinyue.top

[B10] 遍历同时拿索引
来源：http://vuw.vqdsnc.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ivb.ivvv.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kfh.ydzc1.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tdk.aizwys.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mbe.andypj.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uzk.zhixingplan.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pfu.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xca.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zcx.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://sto.meibo888.top

Py:   list(range(0, 10, 2))
来源：http://dcs.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://tok.zhoulong.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bfm.jqgufenzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gxu.fanxiaobao.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bvs.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://anq.zhongyouzk.top

Ruby: (0...10).step(2).to_a
来源：http://ria.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mxh.ybcxt.top

[B12] 跳出多层循环
来源：http://vmv.daria6918.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ypj.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mzh.yuanzhike.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dua.yonumen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://djz.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xwk.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ngi.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ghr.ppjwa.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dyj.zdqjudy.top

[B13] 判断是否为数字
来源：http://xqu.sysykeji.top

Py:   isinstance(x, (int, float))
来源：http://nya.daxiang520.top

PHP:  is_numeric($x)
来源：http://hnk.tianlin.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://por.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fbx.yfazqb.com

Java: x instanceof Number
来源：http://dtl.jqgufenzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zqy.zhaomingkeji.xyz

Ruby: x.is_a?(Numeric)
来源：http://eiz.havefunace.top

C#:   x is int or double or decimal
来源：http://fqv.yj20258.top

[B14] 判断值是否在集合内
来源：http://dlq.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nez.yj202588.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mtk.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://auz.zhijiandao.cn

TS:   [1, 2, 3].includes(x)
来源：http://lgh.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pai.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ilj.fanxiaobao.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://nvu.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rwg.cdnleiting.top

[B15] 布尔运算与取反
来源：http://rai.ctjpmb.com

Py:   a and b or not c
来源：http://sfi.jinqigfzy.top

PHP:  $a && $b || !$c
来源：http://vnr.yuxming.cn

JS:   a && b || !c
来源：http://odm.316326.xyz

TS:   a && b || !c
来源：http://xzw.yueranfly.top

Java: a && b || !c
来源：http://ihn.zhijiandao.cn

Go:   a && b || !c
来源：http://buj.hnxiangtu.top

Ruby: a && b || !c
来源：http://kkq.jiagoushi.top

C#:   a && b || !c
来源：http://cat.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zgf.shanyushiyangkeji.top

Py:   if not data: return
来源：http://vnn.sysykeji.top

PHP:  if (!$data) { return; }
来源：http://tts.cdnleiting.top

JS:   if (!data) return;
来源：http://nkt.hfpthk.cn

TS:   if (!data) return;
来源：http://tpp.hongshengwenyu.top

Java: if (data == null) return;
来源：http://iwp.hywenlv.cn

Go:   if data == nil { return }
来源：http://evs.fehbvm.com

Ruby: return if data.nil?
来源：http://nvh.xylfe.cn

C#:   if (data == null) return;
来源：http://iiq.hesvh.cn

================================================================================
来源：http://omd.zhoulong.xyz

C. 函数与作用域
来源：http://hxq.jianghu66.top

================================================================================
来源：http://hxg.ctjpmb.com

[C01] 定义函数
来源：http://eey.jinqigufen.top

Py:   def add(a, b): return a + b
来源：http://nci.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nqu.haohaochexian.top

JS:   function add(a, b) { return a + b; }
来源：http://zbf.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qhk.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pmb.yonumen.top

Go:   func add(a, b int) int { return a + b }
来源：http://leq.yfazqb.com

Ruby: def add(a, b); a + b; end
来源：http://qpl.jinqigfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mcz.316326.xyz

[C02] 默认参数
来源：http://act.yj20258888.top

Py:   def greet(name="World"): return name
来源：http://tze.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wcy.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://ccf.hongshengwenyu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lhe.zhongyouzk.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mmc.cdnleiting.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wfh.316326.xyz

Ruby: def greet(name = "World") = name
来源：http://osm.gzhubu.top

C#:   string Greet(string name = "World") => name;
来源：http://esk.yj202588.top

[C03] 可变参数
来源：http://tmr.zhengqikj.top

Py:   def total(*args): return sum(args)
来源：http://euz.nanxinkj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jxh.guowangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rba.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lxj.jinqigufen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://epz.xylfe.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ctz.shanyushiyangtech.top

Ruby: def total(*nums); nums.sum; end
来源：http://iyi.daxiang520.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cvf.hammf.cn

[C04] 命名参数 / 关键字参数
来源：http://itj.yongpay.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ckv.hfpthk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tce.mhx1999.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hty.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eiw.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://nts.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://ols.jinghuilouyu.cn

Ruby: f(a: 1, b: 2)
来源：http://iru.xziqi.cn

C#:   f(a: 1, b: 2)
来源：http://gze.vehdjk.com

[C05] 返回多个值
来源：http://krn.ctjpmb.com

Py:   return a, b
来源：http://itx.wangshuangyany.cn

PHP:  return [$a, $b];
来源：http://cqw.ppjwa.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rwn.jlsjyb.cn

TS:   return { a, b };
来源：http://tli.ydjk.org.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lgn.yuanzhike.top

Go:   return a, b
来源：http://wwz.yuxming.cn

Ruby: return a, b
来源：http://bkf.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://ftp.kuanghao11.cn

[C06] 匿名函数 / lambda
来源：http://oag.aibaodan.cn

Py:   square = lambda x: x * x
来源：http://wkd.0kj1m.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kkb.nwbrower.top

JS:   const square = x => x * x;
来源：http://ihq.quarkkingdee.top

TS:   const square = (x: number): number => x * x;
来源：http://ily.xylfe.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://khk.hysaishi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pqf.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://zkj.52xcode.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hkd.ybcxt.top

[C07] 把函数作为参数传入
来源：http://loh.jinghuilouyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zwb.havefunace.top

PHP:  array_map("strtoupper", $arr);
来源：http://ihg.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qgy.xziqi.cn

TS:   arr.map(String)
来源：http://syi.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wrd.fengsongda.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mvj.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://hvx.yangfankeji.com

C#:   arr.Select(s => s.ToUpper())
来源：http://dfr.ppjwa.cn

[C08] 闭包
来源：http://chf.yj20258888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yxd.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ywu.hongshengwenyu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eri.pycfn.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://peq.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rqy.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eeg.zhiwuduotai.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mvn.ydzc1.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ajy.guowangkeji.top

[C09] 递归
来源：http://zhd.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bgn.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tjg.chenjidiqi.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vfs.shuidangran.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jyo.zhongyouzk.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bhs.0kj1m.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wbb.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yxw.gotoacloud.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://klt.cdnleiting.top

[C10] 变量作用域
来源：http://kth.feifeiyinyue.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cjo.nanxinkj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nbn.birdmap.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kwr.fengsongda.top

TS:   同 JS
来源：http://jdu.epnwcf.com

Java: 方法内为块级作用域
来源：http://gbn.52xcode.cn

Go:   花括号块级作用域
来源：http://eog.ivvv.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uaf.smart0.xyz

C#:   块级作用域
来源：http://apw.sysykeji.top

[C11] 模块导入与导出
来源：http://vsq.uphjek.com

Py:   from module import func
来源：http://pjl.aizwys.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kzm.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ndf.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xsj.0kj1m.cn

Java: import java.util.List;
来源：http://jpv.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hsh.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://aqo.quarkkingdee.top

C#:   using System.Text;
来源：http://duq.tian-w.cn

[C12] 立即执行函数 IIFE
来源：http://bfx.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://xax.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://xyv.ctjpmb.com

JS:   (() => { console.log("run"); })();
来源：http://vys.hammf.cn

TS:   (() => { console.log("run"); })();
来源：http://qpk.xingfuxueyuan.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xki.jqgfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://kff.52xcode.cn

Ruby: -> { puts "run" }.call
来源：http://qro.52xcode.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qkn.cashguo.top

[C13] 类型声明 / 类型注解
来源：http://ouz.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://axf.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yxj.cucudq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vfz.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gnz.zhaomingkeji.xyz


<!-- 参考信息 -->