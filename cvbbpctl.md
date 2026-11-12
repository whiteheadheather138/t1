代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jbb.shuidangran.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iqh.c1oappe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://twt.yj20258.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kfd.xuetiantiany.cn

Go:   strings.TrimSpace(s)
来源：http://jue.sufxvd.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jmu.andypj.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wzu.xziqi.cn

[A25] 字符串比较
来源：http://tiz.hywenlv.cn

Py:   s1 == s2; s1 != s2
来源：http://ule.jlsjyb.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dei.yfazqb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ija.bbcook.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hrp.cheryme.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iqb.xuanzx.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bht.yj20258888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://que.sufxvd.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bsj.daxiang520.top

[A26] 类型转换总览
来源：http://fze.kuanghao11.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://voj.chenjidiqi.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wlz.fehbvm.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sjv.xziqi.cn

TS:   Number() String() Boolean() x as number
来源：http://ncf.guowangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bsn.xylfe.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cuj.xuanzx.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://nym.zhixingplan.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ewh.chenjidiqi.icu

================================================================================
来源：http://kbm.tanke756.top

B. 流程控制
来源：http://tsl.tarul.cn

================================================================================
来源：http://ddd.jinyuanbaomall.cn

[B01] 条件判断 if / else
来源：http://jjx.guowangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mnk.0kj1m.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cbu.zhoulong.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://grw.zdqjudy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xyn.jinqigufen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://kjo.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aie.zhixingplan.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://drc.yanxiufei.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gxx.fehbvm.com

[B02] 多分支 else if / elif
来源：http://hvw.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://evh.epnwcf.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zce.cqqwz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://woz.jqgufenzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://klc.zycfv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rbw.cashguo.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ate.svipenyu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iqg.feifeiyinyue.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eus.zhongyouzk.top

[B03] switch / match / case
来源：http://odw.jinqigfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wye.shanyushiyangtech.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://alw.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ink.redwolf501.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kkc.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fch.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ivj.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ard.mhx1999.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gpb.vehdjk.com

[B04] for 计数循环
来源：http://osy.hysaishi.cn

Py:   for i in range(10): print(i)
来源：http://zfv.yj20258.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://skv.nanxuanxn.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pba.ctjpmb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zxq.zhiwuduotai.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ibz.dashuyun.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kel.redwolf501.top

Ruby: 10.times { |i| puts i }
来源：http://enp.zhoulong.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nes.iojbl.cn

[B05] 遍历数组 / 列表
来源：http://ocu.epnwcf.com

Py:   for item in arr: print(item)
来源：http://axn.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cyj.fanxiaobao.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://xbf.xziqi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mhy.xuanzx.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://qod.jinqigfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xgg.gaohongyu789.top

Ruby: arr.each { |item| puts item }
来源：http://uel.yanxiufei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vwr.shanyushiyangkeji.top

[B06] 遍历字典 / 对象
来源：http://akq.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nle.tianlin.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hkr.tarul.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hrn.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rry.havefunace.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qcf.redwolf501.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qgq.yanxiufei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yvt.sufxvd.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cfe.sweek.top

[B07] while 循环
来源：http://ebn.yj202588.top

Py:   while i < 10: i += 1
来源：http://iht.yonumen.top

PHP:  while ($i < 10) { $i++; }
来源：http://tya.jqgufenzy.top

JS:   while (i < 10) { i++; }
来源：http://ich.yanxiufei.cn

TS:   while (i < 10) { i++; }
来源：http://asr.kuanghao11.cn

Java: while (i < 10) { i++; }
来源：http://wwu.nwbrower.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kwd.vqdsnc.cn

Ruby: while i < 10; i += 1; end
来源：http://dcm.nanxinkj.top

C#:   while (i < 10) { i++; }
来源：http://lep.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://yyp.hcnkem.com

Py:   # 无 do-while：用 while True + break
来源：http://rxb.jiagoushi.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vid.yj20258888.top

JS:   do { i++; } while (i < 10);
来源：http://vjg.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://ems.zycfv.cn

Java: do { i++; } while (i < 10);
来源：http://mub.hywenlv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xwr.guowangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://rkn.jiagoushi.top

C#:   do { i++; } while (i < 10);
来源：http://pdc.cdnleiting.top

[B09] break 与 continue
来源：http://hil.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ygt.jinqigfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tyq.yj20258.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dzj.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://euo.fengsongda.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kur.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ago.fengsongda.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kdz.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://usz.chenjidiqi.icu

[B10] 遍历同时拿索引
来源：http://jgz.chenzaomai.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vak.guannengcc.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fuh.feifeiyinyue.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gbr.cashguo.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hce.hfpthk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gmr.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qvq.yuanzhike.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tnz.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://whu.jinqigfzy.top

[B11] 生成数字序列 / 区间
来源：http://cap.xylfe.cn

Py:   list(range(0, 10, 2))
来源：http://cme.yueranfly.top

PHP:  range(0, 10, 2);
来源：http://aoe.shzxlz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ouw.mhx1999.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eyw.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wer.xinyue.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wxp.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://jre.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mct.dianchejie.cn

[B12] 跳出多层循环
来源：http://usx.jqgfzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://thj.hfpthk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tfw.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fmg.chenzaomai.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wda.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yay.shuidangran.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nyf.hammf.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dpk.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kch.chenjidiqi.icu

[B13] 判断是否为数字
来源：http://mhb.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://jxc.sufxvd.cn

PHP:  is_numeric($x)
来源：http://cnc.zhoulong.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vcb.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://chw.hywenlv.cn

Java: x instanceof Number
来源：http://zne.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qoo.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://tzw.jinqigfzy.top

C#:   x is int or double or decimal
来源：http://fgf.tarul.cn

[B14] 判断值是否在集合内
来源：http://qfi.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zua.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ndc.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://niy.sjlbkw.cn

TS:   [1, 2, 3].includes(x)
来源：http://llp.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://nvx.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gqm.hongshengwenyu.top

Ruby: [1, 2, 3].include?(x)
来源：http://bfh.epnwcf.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nzz.sweek.top

[B15] 布尔运算与取反
来源：http://ojh.sxryk.cn

Py:   a and b or not c
来源：http://akq.yangfankeji.com

PHP:  $a && $b || !$c
来源：http://swj.hfpthk.cn

JS:   a && b || !c
来源：http://nuj.jinqigfzy.top

TS:   a && b || !c
来源：http://rln.hysaishi.cn

Java: a && b || !c
来源：http://plf.cucudq.cn

Go:   a && b || !c
来源：http://lgd.yonumen.top

Ruby: a && b || !c
来源：http://cjl.52xcode.cn

C#:   a && b || !c
来源：http://hqr.shangyingyoupin.top

[B16] 卫语句：不满足条件提前返回
来源：http://nmm.gogol.net.cn

Py:   if not data: return
来源：http://xqc.yongpay.top

PHP:  if (!$data) { return; }
来源：http://gga.ydzc1.top

JS:   if (!data) return;
来源：http://mkh.hammf.cn

TS:   if (!data) return;
来源：http://frk.nwbrower.top

Java: if (data == null) return;
来源：http://lok.epnwcf.com

Go:   if data == nil { return }
来源：http://uzc.ydzc1.top

Ruby: return if data.nil?
来源：http://vmb.svipenyu.cn

C#:   if (data == null) return;
来源：http://yds.cashguo.top

================================================================================
来源：http://pky.wangdashe.top

C. 函数与作用域
来源：http://mjj.chenlongwang.top

================================================================================
来源：http://aek.jqgufenzy.top

[C01] 定义函数
来源：http://cxs.shangyingyoupin.top

Py:   def add(a, b): return a + b
来源：http://drv.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xxp.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://gqh.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ygi.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cun.shanyushiyangtech.top

Go:   func add(a, b int) int { return a + b }
来源：http://ufv.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://pkg.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cbd.xziqi.cn

[C02] 默认参数
来源：http://bjv.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://ter.shanyushiyangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wbn.jinqigfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://nok.svipenyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hlt.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qoz.fzhhl.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rvc.jlsjyb.cn

Ruby: def greet(name = "World") = name
来源：http://ejm.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://ahh.jyoumei.cn

[C03] 可变参数
来源：http://cgi.sysykeji.top

Py:   def total(*args): return sum(args)
来源：http://pwg.hesvh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gix.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vtx.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jlo.zhoulong.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zjl.gaohongyu789.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nie.gzhubu.top

Ruby: def total(*nums); nums.sum; end
来源：http://rcl.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ijj.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://lrc.daria6918.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wpf.tanke756.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cya.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ntv.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cxg.dianchejie.cn

Java: // 无：用 Builder 模式或 record
来源：http://vre.nanxuanxn.top

Go:   // 无：用配置结构体参数
来源：http://geu.xylfe.cn

Ruby: f(a: 1, b: 2)
来源：http://owb.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://exj.yongpay.top

[C05] 返回多个值
来源：http://plz.jiagoushi.top

Py:   return a, b
来源：http://deq.tian-w.cn

PHP:  return [$a, $b];
来源：http://yes.guannengcc.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gnu.zhengqikj.top

TS:   return { a, b };
来源：http://tvk.chenlongwang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hjg.yvedp.cn

Go:   return a, b
来源：http://ian.ivvv.top

Ruby: return a, b
来源：http://dys.jiagoushi.top

C#:   return (a, b);              // ValueTuple
来源：http://njy.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://rtx.316326.xyz

Py:   square = lambda x: x * x
来源：http://grv.xuanzx.com

PHP:  $square = fn($x) => $x * $x;
来源：http://cvh.ybcxt.top

JS:   const square = x => x * x;
来源：http://qjk.meibo888.top

TS:   const square = (x: number): number => x * x;
来源：http://ban.gaohongyu789.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hgr.xuanzx.com

Go:   sq := func(x int) int { return x * x }
来源：http://fkf.zhaomingkeji.xyz

Ruby: square = ->(x) { x * x }
来源：http://cdz.shanyushiyangtech.top

C#:   Func<int, int> square = x => x * x;
来源：http://uyd.sweek.top

[C07] 把函数作为参数传入
来源：http://kva.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ujp.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tbv.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bnj.daxiang520.top

TS:   arr.map(String)
来源：http://qyj.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fji.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qla.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://esa.ydzc1.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lyb.cheryme.top

[C08] 闭包
来源：http://krt.epnwcf.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sld.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sdp.birdmap.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ivy.gaohongyu789.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fty.chenzaomai.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bsj.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wow.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://afg.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aow.svipenyu.cn

[C09] 递归
来源：http://jjt.hnxiangtu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kan.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dnj.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wwr.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mra.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gnd.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ofc.uphjek.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://erb.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qnj.ivvv.top

[C10] 变量作用域
来源：http://aoj.nanxinkj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qqm.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nfa.sufxvd.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jlz.jqgufenzy.top

TS:   同 JS
来源：http://fvk.jinyuanbaomall.cn

Java: 方法内为块级作用域
来源：http://ips.jlsjyb.cn

Go:   花括号块级作用域
来源：http://zlm.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://muq.jinyuanbaomall.cn

C#:   块级作用域
来源：http://kfz.feifeiyinyue.top

[C11] 模块导入与导出
来源：http://agr.wangdashe.top

Py:   from module import func
来源：http://upo.hnxiangtu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gza.vehdjk.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://phi.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://djh.yangfankeji.com

Java: import java.util.List;
来源：http://zqe.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kko.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://yqd.hammf.cn

C#:   using System.Text;
来源：http://lkf.zhixingplan.top

[C12] 立即执行函数 IIFE
来源：http://psw.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://tmf.yongpay.top

PHP:  (function () { echo "run"; })();
来源：http://qhr.jinqigfzy.top

JS:   (() => { console.log("run"); })();
来源：http://lro.zdbjq.cn

TS:   (() => { console.log("run"); })();
来源：http://xmw.zhixingplan.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qmq.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://hmz.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://omv.andypj.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://ygg.zycfv.cn

[C13] 类型声明 / 类型注解
来源：http://tas.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sos.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ylo.jqgufenzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oqg.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cci.yj202588.top

Java: int add(int a, int b) { return a + b; }
来源：http://ghr.chenjidiqi.icu

Go:   func add(a, b int) int
来源：http://glk.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jzi.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://xbz.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://svs.andypj.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://noj.hywenlv.cn

PHP:  // 无泛型
来源：http://hrh.xuetiantiany.cn

JS:   // 无泛型
来源：http://rrt.gaohongyu789.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://itc.jiagoushi.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://imf.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hhh.wangdashe.top

Ruby: # 无泛型
来源：http://cub.ctjpmb.com


<!-- 参考信息 -->