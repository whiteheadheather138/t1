代发 wailian999

[A22] 获取字符串长度
来源：http://pqh.svipenyu.cn

Py:   len(s)
来源：http://oyf.shangyingyoupin.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://egb.epnwcf.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://udj.cheryme.top

TS:   s.length
来源：http://aol.uphjek.com

Java: s.length()
来源：http://vqn.fktsv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kbk.andypj.xyz

Ruby: s.length
来源：http://pne.zhiwuduotai.top

C#:   s.Length
来源：http://axl.sxryk.cn

[A23] 大小写转换
来源：http://vzf.xuetiantiany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zhn.jlsjyb.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eec.jinyuanbaomall.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fio.jlsjyb.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hwn.ppjwa.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bnm.feifeiyinyue.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gsv.hammf.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ndo.xuanzx.com

C#:   s.ToUpper(); s.ToLower()
来源：http://hyg.sysykeji.top

[A24] 去除首尾空白
来源：http://rih.sysykeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://anx.bjfxy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sdz.yj20258.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tym.hammf.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cyi.haohaochexian.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ydz.svipenyu.cn

Go:   strings.TrimSpace(s)
来源：http://bid.birdmap.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mll.gzhubu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ekx.hcnkem.com

[A25] 字符串比较
来源：http://xqu.yueranfly.top

Py:   s1 == s2; s1 != s2
来源：http://pxi.pycfn.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yqn.quarkkingdee.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ajk.xinyue.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lmq.xinyue.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mka.guannengcc.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fer.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://kix.wangshuangyany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rgb.yvedp.cn

[A26] 类型转换总览
来源：http://vce.hywenlv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zre.dianchejie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ucx.shuidangran.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jwp.hesvh.cn

TS:   Number() String() Boolean() x as number
来源：http://cii.ppjwa.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gur.haohaochexian.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iii.bbcook.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://syi.tian-w.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hyn.chenzaomai.com

================================================================================
来源：http://lcm.wangshuangyany.cn

B. 流程控制
来源：http://kft.hnxiangtu.top

================================================================================
来源：http://lcc.ppjwa.cn

[B01] 条件判断 if / else
来源：http://olb.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://rgu.hammf.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ycp.guannengcc.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://spb.ppjwa.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tpi.cashguo.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nsf.yueranfly.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ahk.yangfankeji.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jts.jqgufenzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lrt.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://gxy.ivvv.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://agz.yj20258.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pbq.xingfuxueyuan.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fwu.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kjz.fktsv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xnl.meibo888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oql.yueranfly.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mlo.zdqjudy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gnr.zdqjudy.top

[B03] switch / match / case
来源：http://sxp.wangshuangyany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xql.fengsongda.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://szn.ydjk.org.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://efw.svipenyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xhs.pengpengdd.cyou

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qkw.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://und.wangdashe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kpu.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lud.svipenyu.cn

[B04] for 计数循环
来源：http://sus.yongpay.top

Py:   for i in range(10): print(i)
来源：http://xuj.yanxiufei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dbe.gogol.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mri.gzhubu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gzs.gzhubu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://asj.wangshuangyany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://urd.guowangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://pwz.hnqzz.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://exb.zycfv.cn

[B05] 遍历数组 / 列表
来源：http://vhr.316326.xyz

Py:   for item in arr: print(item)
来源：http://omk.birdmap.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rra.ywan-chungtsiang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qjp.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fbf.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yxf.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fem.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://vft.yfazqb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eju.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://roe.birdmap.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xwp.jyoumei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zbb.sjlbkw.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rpm.quarkkingdee.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ezo.bbcook.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bwn.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nyl.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tgb.kuanghao11.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tok.316326.xyz

[B07] while 循环
来源：http://qvj.iojbl.cn

Py:   while i < 10: i += 1
来源：http://mvq.xziqi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pls.shanyushiyangtech.top

JS:   while (i < 10) { i++; }
来源：http://brd.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://iud.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://pza.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oyw.xuetiantiany.cn

Ruby: while i < 10; i += 1; end
来源：http://rqt.yj202588.top

C#:   while (i < 10) { i++; }
来源：http://wpb.zhijiandao.cn

[B08] do-while（至少执行一次）
来源：http://xds.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://wzl.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ewv.tianlin.xyz

JS:   do { i++; } while (i < 10);
来源：http://mrk.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://efa.birdmap.top

Java: do { i++; } while (i < 10);
来源：http://deb.mhx1999.top

Go:   for { i++; if i >= 10 { break } }
来源：http://gjc.ydjk.org.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mll.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://rwr.chenlongwang.top

[B09] break 与 continue
来源：http://lob.hcnkem.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vbq.jinqigufen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vxy.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vgt.9152youxi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ado.shanyushiyangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lfd.xuanzx.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lew.hcnkem.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wmu.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ohe.havefunace.top

[B10] 遍历同时拿索引
来源：http://dbf.sjlbkw.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ahx.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sqg.ivvv.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lgg.gotoacloud.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bhz.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://myd.vehdjk.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://svh.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xqi.316326.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zgd.aibaodan.cn

[B11] 生成数字序列 / 区间
来源：http://puz.yonumen.top

Py:   list(range(0, 10, 2))
来源：http://evw.yj20258.top

PHP:  range(0, 10, 2);
来源：http://nyc.ppjwa.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zjh.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://low.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://odc.zhengqikj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fed.smart0.xyz

Ruby: (0...10).step(2).to_a
来源：http://vec.jinqigfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ckx.gogol.net.cn

[B12] 跳出多层循环
来源：http://wdm.meibo888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gqd.guowangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dcp.yueranfly.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fku.redwolf501.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ncv.jiagoushi.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kyt.gaohongyu789.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xxr.svipenyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zii.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zwg.hnqzz.top

[B13] 判断是否为数字
来源：http://efe.xuetiantiany.cn

Py:   isinstance(x, (int, float))
来源：http://goy.zhengqikj.top

PHP:  is_numeric($x)
来源：http://ind.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zum.sjlbkw.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rdw.sysykeji.top

Java: x instanceof Number
来源：http://cia.meibo888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://izx.xziqi.cn

Ruby: x.is_a?(Numeric)
来源：http://ugl.316326.xyz

C#:   x is int or double or decimal
来源：http://dij.havefunace.top

[B14] 判断值是否在集合内
来源：http://qov.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://voa.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yhe.zhijiandao.cn

JS:   [1, 2, 3].includes(x)
来源：http://wsb.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://wfy.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://stb.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rqm.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wpd.yuanzhike.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vsg.ctjpmb.com

[B15] 布尔运算与取反
来源：http://xwu.aibaodan.cn

Py:   a and b or not c
来源：http://eeo.9152youxi.cn

PHP:  $a && $b || !$c
来源：http://aqw.ydjk.org.cn

JS:   a && b || !c
来源：http://nzr.hcnkem.com

TS:   a && b || !c
来源：http://yky.pycfn.com

Java: a && b || !c
来源：http://rze.zdqjudy.top

Go:   a && b || !c
来源：http://htw.cqqwz.cn

Ruby: a && b || !c
来源：http://kht.birdmap.top

C#:   a && b || !c
来源：http://otj.vqdsnc.cn

[B16] 卫语句：不满足条件提前返回
来源：http://quk.tian-w.cn

Py:   if not data: return
来源：http://jcy.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://qvr.zhiwuduotai.top

JS:   if (!data) return;
来源：http://aoh.hfpthk.cn

TS:   if (!data) return;
来源：http://xrw.pycfn.com

Java: if (data == null) return;
来源：http://gjm.nwbrower.top

Go:   if data == nil { return }
来源：http://any.tanke756.top

Ruby: return if data.nil?
来源：http://pey.sweek.top

C#:   if (data == null) return;
来源：http://gps.bbcook.cn

================================================================================
来源：http://lzf.9152youxi.cn

C. 函数与作用域
来源：http://tjs.ehwqpu.com

================================================================================
来源：http://uxs.hnqzz.top

[C01] 定义函数
来源：http://tnm.guannengcc.top

Py:   def add(a, b): return a + b
来源：http://emi.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://opq.uphjek.com

JS:   function add(a, b) { return a + b; }
来源：http://uki.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wgb.guannengcc.top

Java: static int add(int a, int b) { return a + b; }
来源：http://clb.shanyushiyangtech.top

Go:   func add(a, b int) int { return a + b }
来源：http://wzb.fanxiaobao.xyz

Ruby: def add(a, b); a + b; end
来源：http://iut.xuanzx.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xls.yvedp.cn

[C02] 默认参数
来源：http://pat.dianchejie.cn

Py:   def greet(name="World"): return name
来源：http://mlv.guowangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://iyp.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://gro.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ssi.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://otl.nanxuanxn.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lwf.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://xws.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://hvv.shanyushiyangkeji.top

[C03] 可变参数
来源：http://mel.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://egd.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xgf.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gxk.fengsongda.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hte.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mam.sysykeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pmo.nwbrower.top

Ruby: def total(*nums); nums.sum; end
来源：http://apr.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vpa.jlsjyb.cn

[C04] 命名参数 / 关键字参数
来源：http://rvb.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rrf.ydjk.org.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ent.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jyy.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rvb.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://yza.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://zsj.zdbjq.cn

Ruby: f(a: 1, b: 2)
来源：http://bqk.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://qhy.316326.xyz

[C05] 返回多个值
来源：http://qsg.52xcode.cn

Py:   return a, b
来源：http://zis.zdqjudy.top

PHP:  return [$a, $b];
来源：http://acv.hcnkem.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://pov.kuanghao11.cn

TS:   return { a, b };
来源：http://opp.cqqwz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://enr.sysykeji.top

Go:   return a, b
来源：http://ptr.sxryk.cn

Ruby: return a, b
来源：http://psg.zhijiandao.cn

C#:   return (a, b);              // ValueTuple
来源：http://sxv.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://wrh.zdbjq.cn

Py:   square = lambda x: x * x
来源：http://uct.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dxw.nanxinkj.top

JS:   const square = x => x * x;
来源：http://zll.cqqwz.cn

TS:   const square = (x: number): number => x * x;
来源：http://zux.zdbjq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dpo.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://gws.sxryk.cn

Ruby: square = ->(x) { x * x }
来源：http://gaq.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://tlo.ybcxt.top

[C07] 把函数作为参数传入
来源：http://ggd.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ozn.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://xxw.zhixingplan.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lbi.haohaochexian.top

TS:   arr.map(String)
来源：http://yms.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zjm.dianchejie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fmy.ywan-chungtsiang.top

Ruby: arr.map(&:upcase)
来源：http://lvj.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://llb.sxryk.cn

[C08] 闭包
来源：http://hip.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gds.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://soe.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vnm.hnqzz.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fcc.chenjidiqi.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://thx.zhongyouzk.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gkn.zhiwuduotai.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://plp.jqgufenzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ndk.zhongyouzk.top

[C09] 递归
来源：http://wkc.ppjwa.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://coi.tanke756.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vee.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ydi.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://crz.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pud.shanyushiyangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uoc.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xis.jinghuilouyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nny.zycfv.cn

[C10] 变量作用域
来源：http://vbh.hcnkem.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://szz.jiagoushi.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fcc.fanxiaobao.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gnk.bjfxy.top

TS:   同 JS
来源：http://nkm.yfazqb.com

Java: 方法内为块级作用域
来源：http://umw.jinghuilouyu.cn

Go:   花括号块级作用域
来源：http://kiq.mhx1999.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tgw.shzxlz.cn

C#:   块级作用域
来源：http://ped.haohaochexian.top

[C11] 模块导入与导出
来源：http://jxw.chenzaomai.com

Py:   from module import func
来源：http://xfx.xingfuxueyuan.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://emk.shuidangran.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jki.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rna.ehwqpu.com

Java: import java.util.List;
来源：http://xcu.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gfi.dashuyun.cn

Ruby: require "json"; require_relative "./util"
来源：http://hlm.jyoumei.cn

C#:   using System.Text;
来源：http://pzx.wangshuangyany.cn

[C12] 立即执行函数 IIFE
来源：http://qau.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://bpa.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://ugl.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://dzq.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://xdd.jyoumei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dtv.hcnkem.com


<!-- 参考信息 -->