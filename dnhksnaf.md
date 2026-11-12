代发 wailian999

C#:   s.Length
来源：http://sui.hysaishi.cn

[A23] 大小写转换
来源：http://vsw.jinghuilouyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mof.yongpay.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://und.yuanzhike.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jqd.chenzaomai.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ofj.wangshuangyany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lvp.andypj.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qet.zdbjq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tax.aibaodan.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://irm.sxryk.cn

[A24] 去除首尾空白
来源：http://kxh.yj202588.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://srh.yanxiufei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nnf.feifeiyinyue.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ows.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lsj.iojbl.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lor.chenjidiqi.icu

Go:   strings.TrimSpace(s)
来源：http://iyk.havefunace.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rfr.ctjpmb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://muu.sufxvd.cn

[A25] 字符串比较
来源：http://eqq.yuxming.cn

Py:   s1 == s2; s1 != s2
来源：http://fzi.yvedp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dhg.daxiang520.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qxq.jyoumei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ayt.zycfv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fdj.fzhhl.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pki.pengpengdd.cyou

Ruby: s1 == s2; s1 <=> s2
来源：http://lzb.epnwcf.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vhp.yanxiufei.cn

[A26] 类型转换总览
来源：http://osj.zycfv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://arj.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ejg.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hte.ivvv.top

TS:   Number() String() Boolean() x as number
来源：http://ynq.zhaomingkeji.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wyc.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://spo.xingfuxueyuan.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://oqz.wangshuangyany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vvq.jinqigfzy.top

================================================================================
来源：http://ajd.chenjidiqi.icu

B. 流程控制
来源：http://drl.nanxuanxn.top

================================================================================
来源：http://ugs.cashguo.top

[B01] 条件判断 if / else
来源：http://xei.zhengqikj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://juh.shzxlz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xwu.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cai.wangdashe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wzn.haohaochexian.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://elf.jiagoushi.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fyc.xziqi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mwx.shangyingyoupin.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wjm.fanxiaobao.xyz

[B02] 多分支 else if / elif
来源：http://klg.yongpay.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cww.cashguo.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pgb.cqqwz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jjs.shangyingyoupin.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kgy.meibo888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fxu.9152youxi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xek.hfpthk.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kkv.aibaodan.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rle.yanxiufei.cn

[B03] switch / match / case
来源：http://tpj.ppjwa.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dkk.haohaochexian.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ecf.zhoulong.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pok.uphjek.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cmp.birdmap.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vct.sweek.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hhh.fengsongda.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jkq.ydjk.org.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iqn.dashuyun.cn

[B04] for 计数循环
来源：http://izh.birdmap.top

Py:   for i in range(10): print(i)
来源：http://tbw.zycfv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mob.dianchejie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cfc.yanxiufei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yre.snrcjt.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://svn.yuxming.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xkf.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://xpk.316326.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://svc.pycfn.com

[B05] 遍历数组 / 列表
来源：http://oek.jyoumei.cn

Py:   for item in arr: print(item)
来源：http://hjd.xziqi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vzc.ybcxt.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xdq.zdbjq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vwn.hesvh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vpp.wangshuangyany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zyi.zhoulong.xyz

Ruby: arr.each { |item| puts item }
来源：http://juc.sxryk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kkn.shanyushiyangkeji.top

[B06] 遍历字典 / 对象
来源：http://flc.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nzc.shuidangran.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pba.hfpthk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ccc.fzhhl.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aki.andypj.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://thu.aibaodan.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lwe.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://egk.daria6918.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://giq.yfazqb.com

[B07] while 循环
来源：http://oej.cqqwz.cn

Py:   while i < 10: i += 1
来源：http://ebw.sweek.top

PHP:  while ($i < 10) { $i++; }
来源：http://xrw.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://fvj.shanyushiyangkeji.top

TS:   while (i < 10) { i++; }
来源：http://mnd.fzhhl.top

Java: while (i < 10) { i++; }
来源：http://oom.zhijiandao.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zqq.haohaochexian.top

Ruby: while i < 10; i += 1; end
来源：http://uby.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://yxo.tianlin.xyz

[B08] do-while（至少执行一次）
来源：http://dot.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://hpx.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fep.gzhubu.top

JS:   do { i++; } while (i < 10);
来源：http://htj.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://azb.zhixingplan.top

Java: do { i++; } while (i < 10);
来源：http://hvm.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fsy.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://fkt.ctjpmb.com

C#:   do { i++; } while (i < 10);
来源：http://hvg.c1oappe.top

[B09] break 与 continue
来源：http://fkp.nanxuanxn.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fjf.cdnleiting.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nrt.ybcxt.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nll.cdnleiting.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vbc.hammf.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://feo.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yzp.uphjek.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qlh.cashguo.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jtv.guowangkeji.top

[B10] 遍历同时拿索引
来源：http://mbm.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ytq.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vuw.cqqwz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oeo.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aak.xuetiantiany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fqz.dianchejie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jpi.fzhhl.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uve.fengsongda.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://msp.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://rvw.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://sjn.jyoumei.cn

PHP:  range(0, 10, 2);
来源：http://dxd.ywan-chungtsiang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zux.xuetiantiany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lim.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blo.nanxuanxn.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jlg.hammf.cn

Ruby: (0...10).step(2).to_a
来源：http://ads.wangdashe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zyg.yueranfly.top

[B12] 跳出多层循环
来源：http://wsx.tian-w.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://msl.fengsongda.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cap.haohaochexian.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://owi.zhixingplan.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kge.zdqjudy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rnt.jyoumei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gzw.yj20258888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://otd.andypj.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tmr.zhoulong.xyz

[B13] 判断是否为数字
来源：http://zea.cashguo.top

Py:   isinstance(x, (int, float))
来源：http://mtp.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://vcw.pengpengdd.cyou

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xue.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mvy.snrcjt.cn

Java: x instanceof Number
来源：http://jgi.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lep.cqqwz.cn

Ruby: x.is_a?(Numeric)
来源：http://snm.chenjidiqi.icu

C#:   x is int or double or decimal
来源：http://dms.316326.xyz

[B14] 判断值是否在集合内
来源：http://kca.zhengqikj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gtn.jlsjyb.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://phz.xingfuxueyuan.xyz

JS:   [1, 2, 3].includes(x)
来源：http://ene.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://wbs.iojbl.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kzv.smart0.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uyn.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://efs.nwbrower.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zxf.aibaodan.cn

[B15] 布尔运算与取反
来源：http://flj.chenjidiqi.icu

Py:   a and b or not c
来源：http://xwh.yj20258888.top

PHP:  $a && $b || !$c
来源：http://yin.0kj1m.cn

JS:   a && b || !c
来源：http://qgq.yangfankeji.com

TS:   a && b || !c
来源：http://azg.ivvv.top

Java: a && b || !c
来源：http://fkd.xylfe.cn

Go:   a && b || !c
来源：http://yjj.cqqwz.cn

Ruby: a && b || !c
来源：http://deo.tanke756.top

C#:   a && b || !c
来源：http://qkg.ehwqpu.com

[B16] 卫语句：不满足条件提前返回
来源：http://mtx.yueranfly.top

Py:   if not data: return
来源：http://jir.zhaomingkeji.xyz

PHP:  if (!$data) { return; }
来源：http://ohk.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://baz.pengpengdd.cyou

TS:   if (!data) return;
来源：http://znp.gzhubu.top

Java: if (data == null) return;
来源：http://bpv.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://auc.hnqzz.top

Ruby: return if data.nil?
来源：http://vlx.nwbrower.top

C#:   if (data == null) return;
来源：http://vza.chenzaomai.com

================================================================================
来源：http://nmr.sufxvd.cn

C. 函数与作用域
来源：http://xmc.hongshengwenyu.top

================================================================================
来源：http://hyv.yuanzhike.top

[C01] 定义函数
来源：http://yuh.nwbrower.top

Py:   def add(a, b): return a + b
来源：http://pps.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://caw.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://esj.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://siw.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lsd.shangyingyoupin.top

Go:   func add(a, b int) int { return a + b }
来源：http://qil.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://qda.epnwcf.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tns.wangdashe.top

[C02] 默认参数
来源：http://cha.shangyingyoupin.top

Py:   def greet(name="World"): return name
来源：http://jib.guannengcc.top

PHP:  function greet($name = "World") { return $name; }
来源：http://blk.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://sov.nanxinkj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mlo.fktsv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qot.daxiang520.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fkp.vehdjk.com

Ruby: def greet(name = "World") = name
来源：http://cuw.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://wvb.zdbjq.cn

[C03] 可变参数
来源：http://vfo.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://iww.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zeh.gotoacloud.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gpw.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sol.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://efs.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pwh.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://pao.9152youxi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gcv.hnqzz.top

[C04] 命名参数 / 关键字参数
来源：http://aql.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vkx.kuanghao11.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pjx.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vpr.jianghu66.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://usj.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://qxv.jinqigfzy.top

Go:   // 无：用配置结构体参数
来源：http://zda.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://ryb.nanxuanxn.top

C#:   f(a: 1, b: 2)
来源：http://vfm.0kj1m.cn

[C05] 返回多个值
来源：http://rxg.gogol.net.cn

Py:   return a, b
来源：http://rwg.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://awg.pycfn.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://xhh.cheryme.top

TS:   return { a, b };
来源：http://hfz.yongpay.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qns.xingfuxueyuan.xyz

Go:   return a, b
来源：http://gnt.yj202588.top

Ruby: return a, b
来源：http://urb.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://sra.birdmap.top

[C06] 匿名函数 / lambda
来源：http://trv.svipenyu.cn

Py:   square = lambda x: x * x
来源：http://ofq.xziqi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nhh.fehbvm.com

JS:   const square = x => x * x;
来源：http://nut.jinqigufen.top

TS:   const square = (x: number): number => x * x;
来源：http://nka.fengsongda.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ymp.cucudq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pny.bjfxy.top

Ruby: square = ->(x) { x * x }
来源：http://bnt.hnxiangtu.top

C#:   Func<int, int> square = x => x * x;
来源：http://kki.fktsv.cn

[C07] 把函数作为参数传入
来源：http://dyy.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lgx.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://ufh.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vho.shuidangran.top

TS:   arr.map(String)
来源：http://idv.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://swy.xziqi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vtv.tarul.cn

Ruby: arr.map(&:upcase)
来源：http://zbz.feifeiyinyue.top

C#:   arr.Select(s => s.ToUpper())
来源：http://sqg.guannengcc.top

[C08] 闭包
来源：http://dvi.ydzc1.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lrc.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oer.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wmh.cheryme.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lro.0kj1m.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kda.epnwcf.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eyo.svipenyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://awc.yfazqb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rqc.zhixingplan.top

[C09] 递归
来源：http://tnn.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lfz.pycfn.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kom.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vlp.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bqo.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qnq.dianchejie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cmm.yj20258888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fwb.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bzm.guannengcc.top

[C10] 变量作用域
来源：http://gpw.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gch.jyoumei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gvu.zhijiandao.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ybs.pycfn.com

TS:   同 JS
来源：http://yde.ivvv.top

Java: 方法内为块级作用域
来源：http://uqd.snrcjt.cn

Go:   花括号块级作用域
来源：http://mbv.shuidangran.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://auz.daria6918.cn

C#:   块级作用域
来源：http://rec.vehdjk.com

[C11] 模块导入与导出
来源：http://cxb.zhengqikj.top

Py:   from module import func
来源：http://yap.jinyuanbaomall.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bfn.ehwqpu.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://iaw.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bni.cdnleiting.top

Java: import java.util.List;
来源：http://kzp.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mwa.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://bjy.shzxlz.cn

C#:   using System.Text;
来源：http://aii.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://njf.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://wqt.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://fpy.c1oappe.top

JS:   (() => { console.log("run"); })();
来源：http://psn.yfazqb.com

TS:   (() => { console.log("run"); })();
来源：http://eey.yueranfly.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xfj.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://wjw.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://xje.feifeiyinyue.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wzq.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://xij.birdmap.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iyp.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tch.pengpengdd.cyou

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yas.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://khm.sxryk.cn


<!-- 参考信息 -->