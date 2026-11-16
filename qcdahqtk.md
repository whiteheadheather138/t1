代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ehf.zhijiandao.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vnz.9152youxi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dgt.epnwcf.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lja.jiagoushi.top

Go:   strings.TrimSpace(s)
来源：http://bua.yanxiufei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://leh.feifeiyinyue.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cib.jinqigufen.top

[A25] 字符串比较
来源：http://szp.yanxiufei.cn

Py:   s1 == s2; s1 != s2
来源：http://eiy.redwolf501.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tbh.andypj.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://euf.bjfxy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ccy.ctjpmb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xqj.ctjpmb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ccv.ehwqpu.com

Ruby: s1 == s2; s1 <=> s2
来源：http://hqe.haohaochexian.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fmg.zhijiandao.cn

[A26] 类型转换总览
来源：http://ydy.chenlongwang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eea.shanyushiyangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bvw.ivvv.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://smo.jinyuanbaomall.cn

TS:   Number() String() Boolean() x as number
来源：http://lcy.dianchejie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tek.pengpengdd.cyou

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xjn.aibaodan.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fvk.wangdashe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pxh.bbcook.cn

================================================================================
来源：http://iwr.cashguo.top

B. 流程控制
来源：http://cfo.yonumen.top

================================================================================
来源：http://hlq.shzxlz.cn

[B01] 条件判断 if / else
来源：http://gfw.epnwcf.com

Py:   result = "正" if x > 0 else "非正"
来源：http://vwb.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pge.yuxming.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lef.xuanzx.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://crr.0kj1m.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://icb.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ldi.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tfk.gzhubu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jfl.jinyuanbaomall.cn

[B02] 多分支 else if / elif
来源：http://yui.xinyue.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rsq.tianlin.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aik.quarkkingdee.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vbg.hammf.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dgm.hysaishi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://byv.cdnleiting.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gcs.chenzaomai.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://usp.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yoe.ehwqpu.com

[B03] switch / match / case
来源：http://hml.jinghuilouyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hnp.yangfankeji.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ubi.svipenyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vgb.tanke756.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bow.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hqe.52xcode.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jxs.fanxiaobao.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://shm.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gzk.feifeiyinyue.top

[B04] for 计数循环
来源：http://qnm.mhx1999.top

Py:   for i in range(10): print(i)
来源：http://wbu.bbcook.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jwy.yvedp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wjf.chenjidiqi.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dps.cheryme.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xbk.jyoumei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zuz.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://ojk.shanyushiyangtech.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tum.0kj1m.cn

[B05] 遍历数组 / 列表
来源：http://sjv.shzxlz.cn

Py:   for item in arr: print(item)
来源：http://dkk.xingfuxueyuan.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wfp.kuanghao11.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yqg.zhengqikj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://pya.jinqigufen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fol.jqgufenzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dpu.hfpthk.cn

Ruby: arr.each { |item| puts item }
来源：http://ogr.zhixingplan.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fvp.hongshengwenyu.top

[B06] 遍历字典 / 对象
来源：http://kqs.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tqk.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vpx.xylfe.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wkz.bjfxy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fde.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wno.svipenyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ifs.cashguo.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qle.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://exh.havefunace.top

[B07] while 循环
来源：http://wzl.ydjk.org.cn

Py:   while i < 10: i += 1
来源：http://srs.dianchejie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://snl.cashguo.top

JS:   while (i < 10) { i++; }
来源：http://bzt.mhx1999.top

TS:   while (i < 10) { i++; }
来源：http://kus.yuanzhike.top

Java: while (i < 10) { i++; }
来源：http://tmi.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ihq.zdqjudy.top

Ruby: while i < 10; i += 1; end
来源：http://rke.jinyuanbaomall.cn

C#:   while (i < 10) { i++; }
来源：http://fei.shanyushiyangkeji.top

[B08] do-while（至少执行一次）
来源：http://yva.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://wtx.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://eyp.cdnleiting.top

JS:   do { i++; } while (i < 10);
来源：http://gip.vehdjk.com

TS:   do { i++; } while (i < 10);
来源：http://fmb.snrcjt.cn

Java: do { i++; } while (i < 10);
来源：http://cnv.jinghuilouyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jnk.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://luf.sxryk.cn

C#:   do { i++; } while (i < 10);
来源：http://zze.0kj1m.cn

[B09] break 与 continue
来源：http://pwa.hammf.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bct.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qvq.yueranfly.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oqs.vehdjk.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vny.uphjek.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cxr.jianghu66.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lqy.feifeiyinyue.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gsx.guannengcc.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://akc.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://cve.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mne.hywenlv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nne.uphjek.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://osb.zdqjudy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tyf.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bya.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cxc.jlsjyb.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fhi.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mov.yuanzhike.top

[B11] 生成数字序列 / 区间
来源：http://vzk.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://klm.wangdashe.top

PHP:  range(0, 10, 2);
来源：http://wtf.tarul.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hts.shanyushiyangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uzi.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://php.zhijiandao.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://byt.uphjek.com

Ruby: (0...10).step(2).to_a
来源：http://aqj.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gml.sufxvd.cn

[B12] 跳出多层循环
来源：http://plt.zhijiandao.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zdg.fanxiaobao.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://aju.0kj1m.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yrc.gzhubu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xcc.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bbm.nwbrower.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nsp.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vgl.yj20258888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gky.ivvv.top

[B13] 判断是否为数字
来源：http://ipp.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://vem.dashuyun.cn

PHP:  is_numeric($x)
来源：http://kxf.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ngt.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cuh.hysaishi.cn

Java: x instanceof Number
来源：http://nkm.cashguo.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rca.zhongyouzk.top

Ruby: x.is_a?(Numeric)
来源：http://yba.dianchejie.cn

C#:   x is int or double or decimal
来源：http://urx.cdnleiting.top

[B14] 判断值是否在集合内
来源：http://bxy.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dbm.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zdh.nwbrower.top

JS:   [1, 2, 3].includes(x)
来源：http://ywp.birdmap.top

TS:   [1, 2, 3].includes(x)
来源：http://euy.tarul.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qol.aizwys.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bbe.yuxming.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jgj.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rch.zdqjudy.top

[B15] 布尔运算与取反
来源：http://xan.yongpay.top

Py:   a and b or not c
来源：http://uzm.snrcjt.cn

PHP:  $a && $b || !$c
来源：http://icn.tianlin.xyz

JS:   a && b || !c
来源：http://zxi.sysykeji.top

TS:   a && b || !c
来源：http://zep.chenzaomai.com

Java: a && b || !c
来源：http://sdr.bjfxy.top

Go:   a && b || !c
来源：http://rvk.havefunace.top

Ruby: a && b || !c
来源：http://cfa.snrcjt.cn

C#:   a && b || !c
来源：http://dug.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zzg.sysykeji.top

Py:   if not data: return
来源：http://xkb.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://frs.yj202588.top

JS:   if (!data) return;
来源：http://dfe.chenzaomai.com

TS:   if (!data) return;
来源：http://lqd.daxiang520.top

Java: if (data == null) return;
来源：http://rah.havefunace.top

Go:   if data == nil { return }
来源：http://fjg.tianlin.xyz

Ruby: return if data.nil?
来源：http://pss.guannengcc.top

C#:   if (data == null) return;
来源：http://rtq.yvedp.cn

================================================================================
来源：http://whn.gzhubu.top

C. 函数与作用域
来源：http://pkg.snrcjt.cn

================================================================================
来源：http://oge.zdqjudy.top

[C01] 定义函数
来源：http://fsw.sysykeji.top

Py:   def add(a, b): return a + b
来源：http://ysm.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oxj.jinqigfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://gsx.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://diq.jlsjyb.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sib.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://old.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://gwq.guannengcc.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fur.hcnkem.com

[C02] 默认参数
来源：http://tte.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://lzr.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fqw.zhoulong.xyz

JS:   function greet(name = "World") { return name; }
来源：http://spx.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vci.hongshengwenyu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dnl.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dyy.yueranfly.top

Ruby: def greet(name = "World") = name
来源：http://jjj.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://wrv.jinqigfzy.top

[C03] 可变参数
来源：http://itp.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://wgj.sysykeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gto.ywan-chungtsiang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yvd.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://twu.nanxinkj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ybx.yj20258.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dki.zycfv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ujh.ywan-chungtsiang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sxs.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://zua.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pjo.fehbvm.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://axt.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xpo.jyoumei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ani.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://ics.cdnleiting.top

Go:   // 无：用配置结构体参数
来源：http://onj.jinqigufen.top

Ruby: f(a: 1, b: 2)
来源：http://dyz.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://ytn.snrcjt.cn

[C05] 返回多个值
来源：http://sob.shangyingyoupin.top

Py:   return a, b
来源：http://elj.mhx1999.top

PHP:  return [$a, $b];
来源：http://pgv.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://shh.ywan-chungtsiang.top

TS:   return { a, b };
来源：http://les.yuxming.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://msf.dianchejie.cn

Go:   return a, b
来源：http://ppn.tarul.cn

Ruby: return a, b
来源：http://igm.sjlbkw.cn

C#:   return (a, b);              // ValueTuple
来源：http://hqr.zhoulong.xyz

[C06] 匿名函数 / lambda
来源：http://jlf.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://dob.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lhz.yfazqb.com

JS:   const square = x => x * x;
来源：http://bdj.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://clt.shanyushiyangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gpp.sweek.top

Go:   sq := func(x int) int { return x * x }
来源：http://tbc.hnqzz.top

Ruby: square = ->(x) { x * x }
来源：http://eud.meibo888.top

C#:   Func<int, int> square = x => x * x;
来源：http://uka.fengsongda.top

[C07] 把函数作为参数传入
来源：http://rsi.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aby.tarul.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yln.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hle.hesvh.cn

TS:   arr.map(String)
来源：http://pzg.chenjidiqi.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vym.ydjk.org.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://spd.sxryk.cn

Ruby: arr.map(&:upcase)
来源：http://trd.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ufn.epnwcf.com

[C08] 闭包
来源：http://ccl.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://clv.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ioq.hongshengwenyu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rxr.aizwys.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vdj.zhengqikj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://afr.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mye.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bcs.feifeiyinyue.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dqb.hesvh.cn

[C09] 递归
来源：http://wny.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gfx.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uri.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lbj.fengsongda.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ayt.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yel.hongshengwenyu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zmq.fengsongda.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fbw.xziqi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://emj.hongshengwenyu.top

[C10] 变量作用域
来源：http://yty.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://igc.hnxiangtu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ltd.xinyue.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://biv.zhongyouzk.top

TS:   同 JS
来源：http://wmy.chenjidiqi.icu

Java: 方法内为块级作用域
来源：http://roq.zhoulong.xyz

Go:   花括号块级作用域
来源：http://emn.hnxiangtu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lmj.cucudq.cn

C#:   块级作用域
来源：http://gnj.snrcjt.cn

[C11] 模块导入与导出
来源：http://mdz.aibaodan.cn

Py:   from module import func
来源：http://xvs.svipenyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xjb.bbcook.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bbk.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vjo.fehbvm.com

Java: import java.util.List;
来源：http://hvj.xuanzx.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fou.jianghu66.top

Ruby: require "json"; require_relative "./util"
来源：http://jfh.smart0.xyz

C#:   using System.Text;
来源：http://grm.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://lda.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://dva.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://ivm.xylfe.cn

JS:   (() => { console.log("run"); })();
来源：http://pri.shuidangran.top

TS:   (() => { console.log("run"); })();
来源：http://wrq.hesvh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rom.ehwqpu.com

Go:   func() { fmt.Println("run") }()
来源：http://esv.shzxlz.cn

Ruby: -> { puts "run" }.call
来源：http://dxn.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dde.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://hov.jyoumei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zvi.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tah.aizwys.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nni.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zst.chenzaomai.com

Java: int add(int a, int b) { return a + b; }
来源：http://dbu.zhengqikj.top

Go:   func add(a, b int) int
来源：http://azu.aibaodan.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vxi.hesvh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qeb.uphjek.com

[C14] 泛型函数
来源：http://boy.svipenyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mbq.hnqzz.top

PHP:  // 无泛型
来源：http://vgg.9152youxi.cn

JS:   // 无泛型
来源：http://hwq.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eeo.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nuw.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xaq.bbcook.cn

Ruby: # 无泛型
来源：http://cct.c1oappe.top


<!-- 参考信息 -->