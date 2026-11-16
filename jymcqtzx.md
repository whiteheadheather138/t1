代发 wailian999

C#:   s.Length
来源：http://wcp.wangdashe.top

[A23] 大小写转换
来源：http://ncz.quarkkingdee.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gyr.hammf.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://duv.iojbl.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://spy.shangyingyoupin.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cyd.jinyuanbaomall.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cuo.iojbl.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jtd.mhx1999.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mij.iojbl.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://agl.daxiang520.top

[A24] 去除首尾空白
来源：http://heb.zhaomingkeji.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mkf.feifeiyinyue.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uwl.chenjidiqi.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rov.tianlin.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qxj.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mmd.zhijiandao.cn

Go:   strings.TrimSpace(s)
来源：http://jpe.chenzaomai.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gfj.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zag.xuetiantiany.cn

[A25] 字符串比较
来源：http://izk.yonumen.top

Py:   s1 == s2; s1 != s2
来源：http://nti.ppjwa.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kaw.ydzc1.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tay.snrcjt.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kpn.jqgfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hir.shuidangran.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lok.pycfn.com

Ruby: s1 == s2; s1 <=> s2
来源：http://cmc.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zwc.pengpengdd.cyou

[A26] 类型转换总览
来源：http://nvs.fktsv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zco.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fdh.yueranfly.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gbs.daria6918.cn

TS:   Number() String() Boolean() x as number
来源：http://gcr.yanxiufei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://npa.cqqwz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uta.yonumen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cmx.zhaomingkeji.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lkv.fktsv.cn

================================================================================
来源：http://vbz.zdqjudy.top

B. 流程控制
来源：http://lks.0kj1m.cn

================================================================================
来源：http://rld.cdnleiting.top

[B01] 条件判断 if / else
来源：http://ouj.ppjwa.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bxg.fktsv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iur.zdbjq.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://axg.xingfuxueyuan.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ywd.feifeiyinyue.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cqy.jqgfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cpt.c1oappe.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ijz.jinyuanbaomall.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vib.jqgfzy.top

[B02] 多分支 else if / elif
来源：http://gii.gogol.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qml.daria6918.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zcf.yuxming.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lpd.yongpay.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kbd.jqgufenzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ugj.quarkkingdee.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nhg.fanxiaobao.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nzf.sjlbkw.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yal.smart0.xyz

[B03] switch / match / case
来源：http://qbj.nanxuanxn.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wpk.redwolf501.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sfd.chenjidiqi.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lgf.hnxiangtu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gdo.ppjwa.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mlm.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hyh.pycfn.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gui.ybcxt.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ydn.tianlin.xyz

[B04] for 计数循环
来源：http://rpi.smart0.xyz

Py:   for i in range(10): print(i)
来源：http://kma.pengpengdd.cyou

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://phj.jiagoushi.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mwy.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wle.vehdjk.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yti.0kj1m.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ynu.fehbvm.com

Ruby: 10.times { |i| puts i }
来源：http://pnd.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://itx.zdqjudy.top

[B05] 遍历数组 / 列表
来源：http://xij.hnqzz.top

Py:   for item in arr: print(item)
来源：http://led.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jnn.tianlin.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://tro.jiagoushi.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fxg.zhixingplan.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vyl.tarul.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gqe.cdnleiting.top

Ruby: arr.each { |item| puts item }
来源：http://elr.gotoacloud.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uwq.jiagoushi.top

[B06] 遍历字典 / 对象
来源：http://pnk.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kns.tianlin.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ofe.jlsjyb.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bfo.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xtd.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ets.iojbl.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fzg.jinqigfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zsb.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://awf.jinghuilouyu.cn

[B07] while 循环
来源：http://iru.bbcook.cn

Py:   while i < 10: i += 1
来源：http://tmi.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://twd.xinyue.icu

JS:   while (i < 10) { i++; }
来源：http://nad.gzhubu.top

TS:   while (i < 10) { i++; }
来源：http://ouc.fktsv.cn

Java: while (i < 10) { i++; }
来源：http://vcy.wangdashe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ood.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://imm.svipenyu.cn

C#:   while (i < 10) { i++; }
来源：http://nyn.sjlbkw.cn

[B08] do-while（至少执行一次）
来源：http://mqp.yonumen.top

Py:   # 无 do-while：用 while True + break
来源：http://fme.tanke756.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ivn.ppjwa.cn

JS:   do { i++; } while (i < 10);
来源：http://wlv.hongshengwenyu.top

TS:   do { i++; } while (i < 10);
来源：http://jtm.jlsjyb.cn

Java: do { i++; } while (i < 10);
来源：http://nyk.daxiang520.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fsz.yfazqb.com

Ruby: begin; i += 1; end while i < 10
来源：http://efj.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://dfe.hysaishi.cn

[B09] break 与 continue
来源：http://zon.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ymb.yj20258888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wqn.shanyushiyangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fco.pengpengdd.cyou

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yzu.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ovl.ydjk.org.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mmg.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pmc.ydjk.org.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jsf.haohaochexian.top

[B10] 遍历同时拿索引
来源：http://nti.chenlongwang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rgh.birdmap.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://brx.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yvb.xuanzx.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gdc.pycfn.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lac.pycfn.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dxg.meibo888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://igm.wangshuangyany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fau.bbcook.cn

[B11] 生成数字序列 / 区间
来源：http://rdt.snrcjt.cn

Py:   list(range(0, 10, 2))
来源：http://ssx.hnqzz.top

PHP:  range(0, 10, 2);
来源：http://jkc.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://owm.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xvo.ivvv.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iqk.nanxuanxn.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qgr.daria6918.cn

Ruby: (0...10).step(2).to_a
来源：http://ffo.sjlbkw.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ybx.guowangkeji.top

[B12] 跳出多层循环
来源：http://eii.hesvh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rlw.dashuyun.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yji.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zjs.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mvj.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vrq.ydjk.org.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cdu.jqgfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ivm.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wok.pycfn.com

[B13] 判断是否为数字
来源：http://iwz.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://cga.zycfv.cn

PHP:  is_numeric($x)
来源：http://iaf.iojbl.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gbm.daxiang520.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ayn.zycfv.cn

Java: x instanceof Number
来源：http://nxl.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ski.cheryme.top

Ruby: x.is_a?(Numeric)
来源：http://wwp.wangshuangyany.cn

C#:   x is int or double or decimal
来源：http://cgc.vqdsnc.cn

[B14] 判断值是否在集合内
来源：http://pzv.ydjk.org.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kxk.jinqigufen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fmk.chenzaomai.com

JS:   [1, 2, 3].includes(x)
来源：http://rcw.jqgfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://fii.uphjek.com

Java: List.of(1, 2, 3).contains(x)
来源：http://dyp.c1oappe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uwt.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://iie.hywenlv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qec.jyoumei.cn

[B15] 布尔运算与取反
来源：http://bxt.nwbrower.top

Py:   a and b or not c
来源：http://ccg.52xcode.cn

PHP:  $a && $b || !$c
来源：http://tmy.bjfxy.top

JS:   a && b || !c
来源：http://vmb.zycfv.cn

TS:   a && b || !c
来源：http://fmm.zdbjq.cn

Java: a && b || !c
来源：http://exf.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://swj.zhoulong.xyz

Ruby: a && b || !c
来源：http://pch.zdqjudy.top

C#:   a && b || !c
来源：http://qma.ydzc1.top

[B16] 卫语句：不满足条件提前返回
来源：http://ftv.xylfe.cn

Py:   if not data: return
来源：http://wei.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://rmz.c1oappe.top

JS:   if (!data) return;
来源：http://zbg.feifeiyinyue.top

TS:   if (!data) return;
来源：http://abu.fengsongda.top

Java: if (data == null) return;
来源：http://dpm.ehwqpu.com

Go:   if data == nil { return }
来源：http://akv.yuanzhike.top

Ruby: return if data.nil?
来源：http://kqo.epnwcf.com

C#:   if (data == null) return;
来源：http://awj.xuanzx.com

================================================================================
来源：http://njq.shuidangran.top

C. 函数与作用域
来源：http://htp.316326.xyz

================================================================================
来源：http://hpc.bjfxy.top

[C01] 定义函数
来源：http://eqv.c1oappe.top

Py:   def add(a, b): return a + b
来源：http://bal.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vgp.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://qpw.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rlv.sxryk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://exq.yj20258.top

Go:   func add(a, b int) int { return a + b }
来源：http://jof.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://udh.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cov.zhoulong.xyz

[C02] 默认参数
来源：http://vde.pengpengdd.cyou

Py:   def greet(name="World"): return name
来源：http://yhc.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lzj.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://dqp.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xnt.kuanghao11.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oog.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lpw.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://ymd.jinyuanbaomall.cn

C#:   string Greet(string name = "World") => name;
来源：http://wvp.kuanghao11.cn

[C03] 可变参数
来源：http://kxi.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://pqy.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uyk.guowangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ilh.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uzk.jinghuilouyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tpb.zycfv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jqt.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://pub.epnwcf.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qtr.yueranfly.top

[C04] 命名参数 / 关键字参数
来源：http://udi.0kj1m.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://scs.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uri.yj20258888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wwy.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ppg.zhiwuduotai.top

Java: // 无：用 Builder 模式或 record
来源：http://qnz.kuanghao11.cn

Go:   // 无：用配置结构体参数
来源：http://ofc.svipenyu.cn

Ruby: f(a: 1, b: 2)
来源：http://jba.yj202588.top

C#:   f(a: 1, b: 2)
来源：http://vvk.fengsongda.top

[C05] 返回多个值
来源：http://rzp.hfpthk.cn

Py:   return a, b
来源：http://vis.guannengcc.top

PHP:  return [$a, $b];
来源：http://alp.hongshengwenyu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cog.jianghu66.top

TS:   return { a, b };
来源：http://wiw.jyoumei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://inv.zhiwuduotai.top

Go:   return a, b
来源：http://ftw.nwbrower.top

Ruby: return a, b
来源：http://czi.jyoumei.cn

C#:   return (a, b);              // ValueTuple
来源：http://yja.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://cmo.yanxiufei.cn

Py:   square = lambda x: x * x
来源：http://ffj.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wyo.shanyushiyangkeji.top

JS:   const square = x => x * x;
来源：http://vsb.jyoumei.cn

TS:   const square = (x: number): number => x * x;
来源：http://zxu.ydjk.org.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rwj.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qyb.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://dmw.gotoacloud.top

C#:   Func<int, int> square = x => x * x;
来源：http://fua.sufxvd.cn

[C07] 把函数作为参数传入
来源：http://vup.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iuu.yuxming.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ujy.yj20258888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iba.hcnkem.com

TS:   arr.map(String)
来源：http://vsi.vqdsnc.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gkj.svipenyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bwx.yuxming.cn

Ruby: arr.map(&:upcase)
来源：http://qrs.yueranfly.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mqx.0kj1m.cn

[C08] 闭包
来源：http://dra.smart0.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ogk.iojbl.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uzv.bjfxy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zrp.hnxiangtu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kxo.daxiang520.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tdg.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cmu.hcnkem.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ysw.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rqy.gogol.net.cn

[C09] 递归
来源：http://hyt.hcnkem.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://snk.jinyuanbaomall.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ohx.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nts.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://giw.hammf.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qgk.vqdsnc.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ogj.52xcode.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://soa.wangdashe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lpg.feifeiyinyue.top

[C10] 变量作用域
来源：http://owl.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ygt.dashuyun.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://erh.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gyf.xingfuxueyuan.xyz

TS:   同 JS
来源：http://ros.yangfankeji.com

Java: 方法内为块级作用域
来源：http://jph.xingfuxueyuan.xyz

Go:   花括号块级作用域
来源：http://ela.sysykeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mvf.fktsv.cn

C#:   块级作用域
来源：http://sno.guowangkeji.top

[C11] 模块导入与导出
来源：http://vnd.iojbl.cn

Py:   from module import func
来源：http://uav.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lxh.ydzc1.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kkc.yj20258.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dav.sysykeji.top

Java: import java.util.List;
来源：http://sht.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yat.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://uol.aibaodan.cn

C#:   using System.Text;
来源：http://igu.9152youxi.cn

[C12] 立即执行函数 IIFE
来源：http://lzt.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://jnu.yueranfly.top

PHP:  (function () { echo "run"; })();
来源：http://qcw.zhiwuduotai.top

JS:   (() => { console.log("run"); })();
来源：http://aji.jlsjyb.cn

TS:   (() => { console.log("run"); })();
来源：http://tun.sysykeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://thi.xuanzx.com

Go:   func() { fmt.Println("run") }()
来源：http://jmo.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://ugo.sufxvd.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://thb.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://zut.shangyingyoupin.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gdz.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qqm.sxryk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gkp.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rqr.redwolf501.top


<!-- 参考信息 -->