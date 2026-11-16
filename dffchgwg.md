代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nit.bbcook.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zhh.gaohongyu789.top

[A24] 去除首尾空白
来源：http://fql.yongpay.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qbw.hesvh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qqn.yvedp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nnq.vehdjk.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uia.fanxiaobao.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bbb.fehbvm.com

Go:   strings.TrimSpace(s)
来源：http://xrr.nanxuanxn.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zhm.yueranfly.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fpg.jinqigufen.top

[A25] 字符串比较
来源：http://krp.svipenyu.cn

Py:   s1 == s2; s1 != s2
来源：http://djr.shuidangran.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pqi.guowangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tjt.guannengcc.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://igk.cucudq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wkj.316326.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eqw.hfpthk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://knb.chenjidiqi.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vgn.cucudq.cn

[A26] 类型转换总览
来源：http://mzf.jinghuilouyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://drb.yanxiufei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jfa.quarkkingdee.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jke.zdbjq.cn

TS:   Number() String() Boolean() x as number
来源：http://sza.fengsongda.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pzh.cqqwz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://goz.zhoulong.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://ztj.dashuyun.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dkn.iojbl.cn

================================================================================
来源：http://nyq.svipenyu.cn

B. 流程控制
来源：http://ugb.fanxiaobao.xyz

================================================================================
来源：http://xgi.quarkkingdee.top

[B01] 条件判断 if / else
来源：http://esq.feifeiyinyue.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fgq.hysaishi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zsq.zhixingplan.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wwe.ydzc1.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ypl.hnqzz.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cac.zdbjq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zox.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xpq.yj20258888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mlw.redwolf501.top

[B02] 多分支 else if / elif
来源：http://jal.hnqzz.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ruh.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tlw.xuanzx.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wtf.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cpp.vehdjk.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://shs.yonumen.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eyg.feifeiyinyue.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dkd.hcnkem.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zqf.daria6918.cn

[B03] switch / match / case
来源：http://wtw.hnqzz.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mct.52xcode.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://del.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vah.hammf.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lta.ydzc1.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nes.ydjk.org.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wwe.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jhb.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fby.316326.xyz

[B04] for 计数循环
来源：http://pmt.tarul.cn

Py:   for i in range(10): print(i)
来源：http://loi.yvedp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jdy.zhaomingkeji.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bnl.jiagoushi.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hja.gaohongyu789.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oem.epnwcf.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hsq.yuanzhike.top

Ruby: 10.times { |i| puts i }
来源：http://imo.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://soh.tianlin.xyz

[B05] 遍历数组 / 列表
来源：http://ybp.hcnkem.com

Py:   for item in arr: print(item)
来源：http://esa.xziqi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mna.zhaomingkeji.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://elw.zdqjudy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ozw.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://iai.yangfankeji.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jtj.hywenlv.cn

Ruby: arr.each { |item| puts item }
来源：http://tik.zhoulong.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rky.andypj.xyz

[B06] 遍历字典 / 对象
来源：http://vxg.hammf.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://srw.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tbu.sysykeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ksz.haohaochexian.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cgg.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oja.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fxt.feifeiyinyue.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://crp.hcnkem.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rtn.chenzaomai.com

[B07] while 循环
来源：http://hqk.yfazqb.com

Py:   while i < 10: i += 1
来源：http://ebj.yangfankeji.com

PHP:  while ($i < 10) { $i++; }
来源：http://sym.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://joe.ivvv.top

TS:   while (i < 10) { i++; }
来源：http://geq.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://shw.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pqn.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://cvg.cqqwz.cn

C#:   while (i < 10) { i++; }
来源：http://rot.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://nkn.daria6918.cn

Py:   # 无 do-while：用 while True + break
来源：http://fif.fehbvm.com

PHP:  do { $i++; } while ($i < 10);
来源：http://int.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://gkr.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://ioo.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://yga.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jdq.guowangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://cgl.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://wnt.smart0.xyz

[B09] break 与 continue
来源：http://jzj.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ajv.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bwm.gotoacloud.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yta.zhixingplan.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ete.jianghu66.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nvz.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ypo.havefunace.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cxp.fehbvm.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mxj.redwolf501.top

[B10] 遍历同时拿索引
来源：http://qdx.hammf.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lyc.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wtf.chenlongwang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://axo.yj20258.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mbr.aizwys.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ocp.sxryk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yzl.shanyushiyangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wyo.sufxvd.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jcc.cucudq.cn

[B11] 生成数字序列 / 区间
来源：http://pot.jlsjyb.cn

Py:   list(range(0, 10, 2))
来源：http://hrn.uphjek.com

PHP:  range(0, 10, 2);
来源：http://myp.zhixingplan.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eay.uphjek.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://djq.xuetiantiany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aas.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yvd.shanyushiyangtech.top

Ruby: (0...10).step(2).to_a
来源：http://aep.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dme.shzxlz.cn

[B12] 跳出多层循环
来源：http://cgu.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://vjh.shangyingyoupin.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cyj.shanyushiyangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jvg.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zyt.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kvy.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://trw.xylfe.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mof.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tmw.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://nvg.fktsv.cn

Py:   isinstance(x, (int, float))
来源：http://bju.52xcode.cn

PHP:  is_numeric($x)
来源：http://gfj.birdmap.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mzz.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tui.jlsjyb.cn

Java: x instanceof Number
来源：http://uuz.ivvv.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jle.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://wdi.nanxinkj.top

C#:   x is int or double or decimal
来源：http://suf.jinqigufen.top

[B14] 判断值是否在集合内
来源：http://cxi.aibaodan.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dwi.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nat.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://wkg.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://ywf.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xdh.xuanzx.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hzf.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://ryd.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ntv.fanxiaobao.xyz

[B15] 布尔运算与取反
来源：http://nvw.vehdjk.com

Py:   a and b or not c
来源：http://dgb.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://mov.jqgfzy.top

JS:   a && b || !c
来源：http://zvi.hesvh.cn

TS:   a && b || !c
来源：http://vvz.yfazqb.com

Java: a && b || !c
来源：http://xda.snrcjt.cn

Go:   a && b || !c
来源：http://aoi.zhaomingkeji.xyz

Ruby: a && b || !c
来源：http://ipc.316326.xyz

C#:   a && b || !c
来源：http://aka.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://ooz.svipenyu.cn

Py:   if not data: return
来源：http://mhi.tianlin.xyz

PHP:  if (!$data) { return; }
来源：http://kuk.nanxuanxn.top

JS:   if (!data) return;
来源：http://pme.jinyuanbaomall.cn

TS:   if (!data) return;
来源：http://yjs.9152youxi.cn

Java: if (data == null) return;
来源：http://ahb.zdqjudy.top

Go:   if data == nil { return }
来源：http://ovj.gzhubu.top

Ruby: return if data.nil?
来源：http://ihd.yangfankeji.com

C#:   if (data == null) return;
来源：http://sxk.kuanghao11.cn

================================================================================
来源：http://odo.yangfankeji.com

C. 函数与作用域
来源：http://xdm.hnxiangtu.top

================================================================================
来源：http://cmq.havefunace.top

[C01] 定义函数
来源：http://gou.yanxiufei.cn

Py:   def add(a, b): return a + b
来源：http://nvb.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wjg.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://otw.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://meu.zhiwuduotai.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wtr.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://shr.yuanzhike.top

Ruby: def add(a, b); a + b; end
来源：http://hpd.daria6918.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pem.sweek.top

[C02] 默认参数
来源：http://pzd.c1oappe.top

Py:   def greet(name="World"): return name
来源：http://nuf.daxiang520.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tns.yuxming.cn

JS:   function greet(name = "World") { return name; }
来源：http://hom.fehbvm.com

TS:   function greet(name: string = "World") { return name; }
来源：http://gph.dianchejie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://byq.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nuf.nanxinkj.top

Ruby: def greet(name = "World") = name
来源：http://lbs.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://izc.birdmap.top

[C03] 可变参数
来源：http://gke.cqqwz.cn

Py:   def total(*args): return sum(args)
来源：http://sno.zhijiandao.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xlp.gotoacloud.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://udy.zhijiandao.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cny.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zfz.aibaodan.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ijh.hesvh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tzu.jinqigfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rrr.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://wdq.vqdsnc.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nlz.jqgufenzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://avg.zhongyouzk.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ijt.fehbvm.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tpm.ywan-chungtsiang.top

Java: // 无：用 Builder 模式或 record
来源：http://qdx.zhaomingkeji.xyz

Go:   // 无：用配置结构体参数
来源：http://ndh.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://qrz.redwolf501.top

C#:   f(a: 1, b: 2)
来源：http://edi.ctjpmb.com

[C05] 返回多个值
来源：http://zdk.shangyingyoupin.top

Py:   return a, b
来源：http://cqy.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://gib.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xid.quarkkingdee.top

TS:   return { a, b };
来源：http://ygl.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cul.snrcjt.cn

Go:   return a, b
来源：http://ijp.aizwys.cn

Ruby: return a, b
来源：http://ghi.tian-w.cn

C#:   return (a, b);              // ValueTuple
来源：http://lpm.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://xhb.zdqjudy.top

Py:   square = lambda x: x * x
来源：http://bkl.gotoacloud.top

PHP:  $square = fn($x) => $x * $x;
来源：http://klt.hammf.cn

JS:   const square = x => x * x;
来源：http://pmd.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://sjq.xziqi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nhw.xylfe.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eeu.yueranfly.top

Ruby: square = ->(x) { x * x }
来源：http://hrg.ydzc1.top

C#:   Func<int, int> square = x => x * x;
来源：http://fuc.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://pms.haohaochexian.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fbt.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://njo.zhixingplan.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://paa.gogol.net.cn

TS:   arr.map(String)
来源：http://kii.hywenlv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bxo.mhx1999.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ppu.0kj1m.cn

Ruby: arr.map(&:upcase)
来源：http://mbm.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wit.9152youxi.cn

[C08] 闭包
来源：http://zlq.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vae.yongpay.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sug.fehbvm.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mal.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://goo.aizwys.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nzh.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wlq.snrcjt.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tdb.hesvh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ajb.yj20258.top

[C09] 递归
来源：http://edj.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bmv.jinghuilouyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://epp.guannengcc.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://elg.xziqi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lgd.jianghu66.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yjh.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gom.haohaochexian.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://noh.xingfuxueyuan.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ibq.zhengqikj.top

[C10] 变量作用域
来源：http://xrc.fzhhl.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wts.shanyushiyangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://djz.ivvv.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pmn.guannengcc.top

TS:   同 JS
来源：http://jal.meibo888.top

Java: 方法内为块级作用域
来源：http://xlk.zhaomingkeji.xyz

Go:   花括号块级作用域
来源：http://pgv.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mhk.fktsv.cn

C#:   块级作用域
来源：http://qyg.yj20258.top

[C11] 模块导入与导出
来源：http://nyv.nwbrower.top

Py:   from module import func
来源：http://vgm.shanyushiyangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wgi.zhengqikj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xns.jinqigufen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jea.zhixingplan.top

Java: import java.util.List;
来源：http://aqb.sweek.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://trq.bbcook.cn

Ruby: require "json"; require_relative "./util"
来源：http://swl.zhengqikj.top

C#:   using System.Text;
来源：http://rqu.cashguo.top

[C12] 立即执行函数 IIFE
来源：http://gbh.nanxinkj.top

Py:   (lambda: print("run"))()
来源：http://uvy.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://bcx.ctjpmb.com

JS:   (() => { console.log("run"); })();
来源：http://azx.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://yqp.jinqigfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vrx.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://cyh.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://kzs.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dts.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://jwm.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hnf.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lml.feifeiyinyue.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gyr.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://spe.jqgfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://ock.xylfe.cn

Go:   func add(a, b int) int
来源：http://bqd.bbcook.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wkt.zhaomingkeji.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://tor.yj20258888.top

[C14] 泛型函数
来源：http://kzb.yj20258.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sxz.daria6918.cn

PHP:  // 无泛型
来源：http://cph.nwbrower.top

JS:   // 无泛型
来源：http://wnv.yuxming.cn


<!-- 参考信息 -->