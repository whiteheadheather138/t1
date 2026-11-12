代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://jhx.daxiang520.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://biz.shanyushiyangtech.top

JS:   (3.14159).toFixed(2)
来源：http://pdb.jinyuanbaomall.cn

TS:   (3.14159).toFixed(2)
来源：http://aaf.yj20258.top

Java: String.format("%.2f", 3.14159)
来源：http://hqc.haohaochexian.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pir.jinqigfzy.top

Ruby: format("%.2f", 3.14159)
来源：http://ipe.xuetiantiany.cn

C#:   3.14159.ToString("F2")
来源：http://sed.mhx1999.top

[A22] 获取字符串长度
来源：http://syn.shanyushiyangkeji.top

Py:   len(s)
来源：http://fwd.sxryk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tey.gotoacloud.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ljx.chenzaomai.com

TS:   s.length
来源：http://kfr.sweek.top

Java: s.length()
来源：http://ebp.andypj.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hgw.zdqjudy.top

Ruby: s.length
来源：http://kvu.feifeiyinyue.top

C#:   s.Length
来源：http://eps.c1oappe.top

[A23] 大小写转换
来源：http://pdj.yj202588.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wzx.daxiang520.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uef.jinqigfzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zes.jianghu66.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://erm.sxryk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bsw.0kj1m.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sat.ivvv.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tre.feifeiyinyue.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vns.cqqwz.cn

[A24] 去除首尾空白
来源：http://azd.daxiang520.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gry.birdmap.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ypw.shuidangran.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qfp.dashuyun.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kzc.fanxiaobao.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hhm.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://zfv.hammf.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oen.aibaodan.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uac.yuanzhike.top

[A25] 字符串比较
来源：http://nyz.zdbjq.cn

Py:   s1 == s2; s1 != s2
来源：http://acy.xuanzx.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wxd.fehbvm.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fuj.sufxvd.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zaw.nwbrower.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hqh.vqdsnc.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hue.fzhhl.top

Ruby: s1 == s2; s1 <=> s2
来源：http://uxu.ybcxt.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hmh.jinghuilouyu.cn

[A26] 类型转换总览
来源：http://hqt.wangdashe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wir.jianghu66.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lqn.epnwcf.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rto.zdqjudy.top

TS:   Number() String() Boolean() x as number
来源：http://suw.sxryk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tqk.daxiang520.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pfk.zycfv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://auc.fehbvm.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mxi.pengpengdd.cyou

================================================================================
来源：http://bxn.316326.xyz

B. 流程控制
来源：http://oxx.jinyuanbaomall.cn

================================================================================
来源：http://ciz.yonumen.top

[B01] 条件判断 if / else
来源：http://ftl.yongpay.top

Py:   result = "正" if x > 0 else "非正"
来源：http://onh.xziqi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wbu.smart0.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kde.zdqjudy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://brv.zdbjq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bvh.fehbvm.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oyn.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bsi.daxiang520.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://giy.wangdashe.top

[B02] 多分支 else if / elif
来源：http://sju.zdqjudy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mjs.jqgufenzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wtg.shanyushiyangtech.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hzn.fehbvm.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kyg.gogol.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wxt.daxiang520.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mlq.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uay.quarkkingdee.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qhk.bbcook.cn

[B03] switch / match / case
来源：http://nua.xingfuxueyuan.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mcd.ydjk.org.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gte.aibaodan.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cjr.ppjwa.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tfn.hesvh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ele.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ueb.yuanzhike.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://muo.ybcxt.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wen.gogol.net.cn

[B04] for 计数循环
来源：http://tsx.sjlbkw.cn

Py:   for i in range(10): print(i)
来源：http://iwn.sysykeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mkl.jlsjyb.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eqi.fehbvm.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ucu.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://opt.dianchejie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hnj.zhiwuduotai.top

Ruby: 10.times { |i| puts i }
来源：http://gap.andypj.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ofa.snrcjt.cn

[B05] 遍历数组 / 列表
来源：http://bvr.guowangkeji.top

Py:   for item in arr: print(item)
来源：http://izo.ppjwa.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kvd.hywenlv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wbo.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mzh.fzhhl.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ulv.shangyingyoupin.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rrs.sufxvd.cn

Ruby: arr.each { |item| puts item }
来源：http://wmd.yueranfly.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sdm.xinyue.icu

[B06] 遍历字典 / 对象
来源：http://ots.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bie.xingfuxueyuan.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mxg.wangdashe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ifm.smart0.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qmc.havefunace.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xeq.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://azt.gaohongyu789.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://exd.fzhhl.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yfo.xingfuxueyuan.xyz

[B07] while 循环
来源：http://uyh.yuanzhike.top

Py:   while i < 10: i += 1
来源：http://fal.ydjk.org.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ihd.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://esa.gaohongyu789.top

TS:   while (i < 10) { i++; }
来源：http://yhf.jlsjyb.cn

Java: while (i < 10) { i++; }
来源：http://knl.ppjwa.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://roy.shzxlz.cn

Ruby: while i < 10; i += 1; end
来源：http://wal.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://oze.hysaishi.cn

[B08] do-while（至少执行一次）
来源：http://yir.xuanzx.com

Py:   # 无 do-while：用 while True + break
来源：http://eor.fzhhl.top

PHP:  do { $i++; } while ($i < 10);
来源：http://eou.dianchejie.cn

JS:   do { i++; } while (i < 10);
来源：http://gfr.zhixingplan.top

TS:   do { i++; } while (i < 10);
来源：http://vnz.cucudq.cn

Java: do { i++; } while (i < 10);
来源：http://snh.jyoumei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kgj.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yhw.hcnkem.com

C#:   do { i++; } while (i < 10);
来源：http://fja.tian-w.cn

[B09] break 与 continue
来源：http://hnz.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vmd.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://afk.yuanzhike.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://net.zhixingplan.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zzg.yanxiufei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xlr.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rsd.gzhubu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://flr.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tlq.guannengcc.top

[B10] 遍历同时拿索引
来源：http://zky.ivvv.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cvd.tian-w.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mpn.gzhubu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wcx.snrcjt.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qak.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mnn.cdnleiting.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xdf.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://syr.shuidangran.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ygs.pengpengdd.cyou

[B11] 生成数字序列 / 区间
来源：http://dlo.kuanghao11.cn

Py:   list(range(0, 10, 2))
来源：http://rtf.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://yzt.ywan-chungtsiang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rid.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wao.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sjm.uphjek.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jpg.gotoacloud.top

Ruby: (0...10).step(2).to_a
来源：http://mfx.mhx1999.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oyu.daxiang520.top

[B12] 跳出多层循环
来源：http://ghk.316326.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://wbd.chenjidiqi.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://nyz.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mdq.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ezn.zhiwuduotai.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vhj.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iql.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wzk.jqgufenzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mae.zdqjudy.top

[B13] 判断是否为数字
来源：http://kmn.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://wyj.hcnkem.com

PHP:  is_numeric($x)
来源：http://kwx.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://poe.yfazqb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wdy.yangfankeji.com

Java: x instanceof Number
来源：http://yfs.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://shj.fehbvm.com

Ruby: x.is_a?(Numeric)
来源：http://knv.guowangkeji.top

C#:   x is int or double or decimal
来源：http://zfu.sjlbkw.cn

[B14] 判断值是否在集合内
来源：http://nxw.c1oappe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lvp.chenlongwang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vbk.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://ylm.jinghuilouyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://rah.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zto.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jfb.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rdg.jiagoushi.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ocg.shuidangran.top

[B15] 布尔运算与取反
来源：http://qoy.havefunace.top

Py:   a and b or not c
来源：http://smf.dashuyun.cn

PHP:  $a && $b || !$c
来源：http://kqq.tian-w.cn

JS:   a && b || !c
来源：http://yxi.cucudq.cn

TS:   a && b || !c
来源：http://del.yangfankeji.com

Java: a && b || !c
来源：http://ozc.meibo888.top

Go:   a && b || !c
来源：http://jau.daria6918.cn

Ruby: a && b || !c
来源：http://qvc.zhoulong.xyz

C#:   a && b || !c
来源：http://uno.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://lck.fanxiaobao.xyz

Py:   if not data: return
来源：http://bds.cashguo.top

PHP:  if (!$data) { return; }
来源：http://wvu.hfpthk.cn

JS:   if (!data) return;
来源：http://iwl.tianlin.xyz

TS:   if (!data) return;
来源：http://ewa.chenzaomai.com

Java: if (data == null) return;
来源：http://web.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://xcn.jyoumei.cn

Ruby: return if data.nil?
来源：http://npb.cheryme.top

C#:   if (data == null) return;
来源：http://hwu.jinqigufen.top

================================================================================
来源：http://fzv.hammf.cn

C. 函数与作用域
来源：http://fuc.xuetiantiany.cn

================================================================================
来源：http://fux.jqgfzy.top

[C01] 定义函数
来源：http://pak.andypj.xyz

Py:   def add(a, b): return a + b
来源：http://mtt.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sho.nanxuanxn.top

JS:   function add(a, b) { return a + b; }
来源：http://ckg.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nbr.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://brg.hammf.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zxi.quarkkingdee.top

Ruby: def add(a, b); a + b; end
来源：http://gsd.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yxl.fzhhl.top

[C02] 默认参数
来源：http://tch.zycfv.cn

Py:   def greet(name="World"): return name
来源：http://dcf.jqgfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://oow.smart0.xyz

JS:   function greet(name = "World") { return name; }
来源：http://phd.zhoulong.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://kdp.vqdsnc.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dvm.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xhs.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://kdh.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://sfm.yj20258888.top

[C03] 可变参数
来源：http://abw.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://blt.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hhs.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://siv.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qex.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fvz.jinqigfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uwx.yuxming.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uxf.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ijw.smart0.xyz

[C04] 命名参数 / 关键字参数
来源：http://hmr.tian-w.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://chb.jyoumei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://amn.havefunace.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ohw.jinqigfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pim.xinyue.icu

Java: // 无：用 Builder 模式或 record
来源：http://tyh.jinqigfzy.top

Go:   // 无：用配置结构体参数
来源：http://lvu.chenlongwang.top

Ruby: f(a: 1, b: 2)
来源：http://cqh.gzhubu.top

C#:   f(a: 1, b: 2)
来源：http://liu.ctjpmb.com

[C05] 返回多个值
来源：http://lqi.hongshengwenyu.top

Py:   return a, b
来源：http://etz.jinqigufen.top

PHP:  return [$a, $b];
来源：http://fuy.sjlbkw.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bhj.guowangkeji.top

TS:   return { a, b };
来源：http://vhg.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://beb.hcnkem.com

Go:   return a, b
来源：http://lid.tianlin.xyz

Ruby: return a, b
来源：http://srx.ydzc1.top

C#:   return (a, b);              // ValueTuple
来源：http://nph.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://omi.gogol.net.cn

Py:   square = lambda x: x * x
来源：http://flh.yanxiufei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://alx.chenzaomai.com

JS:   const square = x => x * x;
来源：http://cmh.xuetiantiany.cn

TS:   const square = (x: number): number => x * x;
来源：http://evd.ydjk.org.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eqe.daria6918.cn

Go:   sq := func(x int) int { return x * x }
来源：http://joa.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://hpt.svipenyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nvw.hysaishi.cn

[C07] 把函数作为参数传入
来源：http://ary.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eai.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://fwv.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yol.shzxlz.cn

TS:   arr.map(String)
来源：http://ugt.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vom.dianchejie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fko.yanxiufei.cn

Ruby: arr.map(&:upcase)
来源：http://grz.birdmap.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bvy.ctjpmb.com

[C08] 闭包
来源：http://fsw.guowangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jtg.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vrx.tanke756.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://twn.hnqzz.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bzb.9152youxi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nma.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nvh.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ukm.xingfuxueyuan.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mvv.sysykeji.top

[C09] 递归
来源：http://oka.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mys.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wmk.ppjwa.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lwf.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lbr.quarkkingdee.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yeo.hfpthk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nqk.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yvu.mhx1999.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uqz.andypj.xyz

[C10] 变量作用域
来源：http://vox.xinyue.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qpd.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xov.zhengqikj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ftr.yj20258.top

TS:   同 JS
来源：http://hbr.fzhhl.top

Java: 方法内为块级作用域
来源：http://udu.yuxming.cn

Go:   花括号块级作用域
来源：http://kai.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jyv.uphjek.com

C#:   块级作用域
来源：http://qqy.jinqigfzy.top

[C11] 模块导入与导出
来源：http://gnq.vehdjk.com

Py:   from module import func
来源：http://dqp.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dnt.fehbvm.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://gzj.birdmap.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lww.ivvv.top

Java: import java.util.List;
来源：http://ala.fzhhl.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aoh.redwolf501.top


<!-- 参考信息 -->