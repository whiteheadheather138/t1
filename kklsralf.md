代发 wailian999

[A22] 获取字符串长度
来源：http://xgb.hesvh.cn

Py:   len(s)
来源：http://tmr.zhongyouzk.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pje.dashuyun.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lug.ydjk.org.cn

TS:   s.length
来源：http://htf.ehwqpu.com

Java: s.length()
来源：http://glq.sjlbkw.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hsr.jlsjyb.cn

Ruby: s.length
来源：http://kob.ybcxt.top

C#:   s.Length
来源：http://vjm.dianchejie.cn

[A23] 大小写转换
来源：http://wtm.svipenyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fko.hysaishi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ziq.0kj1m.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bnj.9152youxi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ltv.aibaodan.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zwk.nwbrower.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pgs.jqgfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wze.shangyingyoupin.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hpv.xinyue.icu

[A24] 去除首尾空白
来源：http://jsf.tarul.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jdu.nanxinkj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ayy.guannengcc.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://coq.zhongyouzk.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jgw.vehdjk.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hud.zdbjq.cn

Go:   strings.TrimSpace(s)
来源：http://cvt.yangfankeji.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vou.jlsjyb.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://brw.haohaochexian.top

[A25] 字符串比较
来源：http://dit.sxryk.cn

Py:   s1 == s2; s1 != s2
来源：http://afj.sysykeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ddo.hcnkem.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yzh.jinqigufen.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ajp.zdbjq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dub.cheryme.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jdx.jinqigufen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://zau.vehdjk.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lzo.shanyushiyangtech.top

[A26] 类型转换总览
来源：http://osd.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zbv.yanxiufei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cvl.tanke756.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://znv.xylfe.cn

TS:   Number() String() Boolean() x as number
来源：http://uei.bbcook.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ill.hywenlv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://the.jqgufenzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mkm.ydzc1.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yzf.zhoulong.xyz

================================================================================
来源：http://avf.hnqzz.top

B. 流程控制
来源：http://alj.yuanzhike.top

================================================================================
来源：http://wnr.guannengcc.top

[B01] 条件判断 if / else
来源：http://erl.xziqi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mhe.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vmy.nwbrower.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oqy.sysykeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nva.yj202588.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://avw.jianghu66.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wgr.uphjek.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rpr.aibaodan.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xrc.yj202588.top

[B02] 多分支 else if / elif
来源：http://ktq.hnxiangtu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xch.chenlongwang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yku.chenzaomai.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sge.shangyingyoupin.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xzo.sjlbkw.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dfj.hammf.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nat.jinqigfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ubc.zhongyouzk.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://roz.fehbvm.com

[B03] switch / match / case
来源：http://rml.52xcode.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://epc.hesvh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zyl.hfpthk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rhu.svipenyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sjb.zhixingplan.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ggj.jinqigfzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wkv.quarkkingdee.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://thq.sjlbkw.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yey.fanxiaobao.xyz

[B04] for 计数循环
来源：http://zbm.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://mdf.hongshengwenyu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yya.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aro.pycfn.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xjf.svipenyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iqj.shangyingyoupin.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oxh.jianghu66.top

Ruby: 10.times { |i| puts i }
来源：http://skk.dashuyun.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mvr.yuanzhike.top

[B05] 遍历数组 / 列表
来源：http://txl.andypj.xyz

Py:   for item in arr: print(item)
来源：http://axx.ydjk.org.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mff.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mes.tanke756.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mwd.wangshuangyany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ssn.gzhubu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nzx.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://jhw.316326.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://itz.ppjwa.cn

[B06] 遍历字典 / 对象
来源：http://mty.mhx1999.top

Py:   for k, v in d.items(): print(k, v)
来源：http://iue.birdmap.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bzv.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jqc.jqgufenzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zre.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jad.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pxb.nanxuanxn.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dhv.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oks.daria6918.cn

[B07] while 循环
来源：http://deg.jiagoushi.top

Py:   while i < 10: i += 1
来源：http://mpf.hnqzz.top

PHP:  while ($i < 10) { $i++; }
来源：http://qkd.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://pen.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://xmh.jinqigfzy.top

Java: while (i < 10) { i++; }
来源：http://ifl.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fdx.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://vuc.ivvv.top

C#:   while (i < 10) { i++; }
来源：http://ujn.xuetiantiany.cn

[B08] do-while（至少执行一次）
来源：http://udp.sysykeji.top

Py:   # 无 do-while：用 while True + break
来源：http://tmz.dianchejie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zsh.zhengqikj.top

JS:   do { i++; } while (i < 10);
来源：http://uaq.0kj1m.cn

TS:   do { i++; } while (i < 10);
来源：http://vnp.sweek.top

Java: do { i++; } while (i < 10);
来源：http://ncc.aizwys.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cpr.yj20258888.top

Ruby: begin; i += 1; end while i < 10
来源：http://enk.0kj1m.cn

C#:   do { i++; } while (i < 10);
来源：http://vuh.aibaodan.cn

[B09] break 与 continue
来源：http://abv.shanyushiyangtech.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wvw.xuanzx.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xns.smart0.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tsp.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pol.chenjidiqi.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pot.wangshuangyany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yla.fktsv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cui.yangfankeji.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yua.sxryk.cn

[B10] 遍历同时拿索引
来源：http://sps.zhoulong.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yas.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://npg.ivvv.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qza.cashguo.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ymk.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://doh.fzhhl.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uai.jinqigufen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tcx.jqgufenzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://peu.havefunace.top

[B11] 生成数字序列 / 区间
来源：http://vwe.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://asp.shuidangran.top

PHP:  range(0, 10, 2);
来源：http://dhb.cheryme.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eem.dashuyun.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jkc.tian-w.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zrl.ehwqpu.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ycz.hesvh.cn

Ruby: (0...10).step(2).to_a
来源：http://jsm.fzhhl.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xsj.vehdjk.com

[B12] 跳出多层循环
来源：http://eby.yfazqb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://dia.sweek.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cyx.ppjwa.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jpc.hysaishi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vyr.zhijiandao.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wxc.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cvz.zhoulong.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://huz.gaohongyu789.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bqi.c1oappe.top

[B13] 判断是否为数字
来源：http://ule.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://vdf.zhoulong.xyz

PHP:  is_numeric($x)
来源：http://coz.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gfl.yj202588.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vow.yuanzhike.top

Java: x instanceof Number
来源：http://qox.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://auz.guowangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://tem.dianchejie.cn

C#:   x is int or double or decimal
来源：http://nyq.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://xsk.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gam.aibaodan.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yvl.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://doj.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://nnn.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pyp.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lgo.cashguo.top

Ruby: [1, 2, 3].include?(x)
来源：http://axu.vehdjk.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://scj.zhengqikj.top

[B15] 布尔运算与取反
来源：http://cqz.cdnleiting.top

Py:   a and b or not c
来源：http://kip.ydzc1.top

PHP:  $a && $b || !$c
来源：http://wjq.yvedp.cn

JS:   a && b || !c
来源：http://rrp.chenjidiqi.icu

TS:   a && b || !c
来源：http://spr.pengpengdd.cyou

Java: a && b || !c
来源：http://bwq.zhiwuduotai.top

Go:   a && b || !c
来源：http://vvo.daria6918.cn

Ruby: a && b || !c
来源：http://rkt.fzhhl.top

C#:   a && b || !c
来源：http://ler.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wpl.chenzaomai.com

Py:   if not data: return
来源：http://qmi.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://dsh.zdbjq.cn

JS:   if (!data) return;
来源：http://upd.xziqi.cn

TS:   if (!data) return;
来源：http://onx.yuanzhike.top

Java: if (data == null) return;
来源：http://rii.jqgfzy.top

Go:   if data == nil { return }
来源：http://yrb.hammf.cn

Ruby: return if data.nil?
来源：http://gqu.zhongyouzk.top

C#:   if (data == null) return;
来源：http://gto.ppjwa.cn

================================================================================
来源：http://fvr.zhongyouzk.top

C. 函数与作用域
来源：http://xtj.fehbvm.com

================================================================================
来源：http://pfy.xuetiantiany.cn

[C01] 定义函数
来源：http://qak.hongshengwenyu.top

Py:   def add(a, b): return a + b
来源：http://cpr.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zdr.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://xwo.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lpb.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://iox.9152youxi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kqp.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://tkg.ybcxt.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yha.yj20258888.top

[C02] 默认参数
来源：http://pkh.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://bof.iojbl.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pqv.cucudq.cn

JS:   function greet(name = "World") { return name; }
来源：http://nqo.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://oth.vehdjk.com

Java: // 无默认参数：方法重载或 Optional
来源：http://vdt.havefunace.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lte.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://nbm.birdmap.top

C#:   string Greet(string name = "World") => name;
来源：http://xua.zycfv.cn

[C03] 可变参数
来源：http://zco.havefunace.top

Py:   def total(*args): return sum(args)
来源：http://yho.andypj.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ojk.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pmj.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rvg.yj20258888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://grm.bjfxy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fuj.jyoumei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zdn.hcnkem.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ftg.xylfe.cn

[C04] 命名参数 / 关键字参数
来源：http://glo.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ugz.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jqi.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://elb.0kj1m.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gpv.yj20258888.top

Java: // 无：用 Builder 模式或 record
来源：http://mio.tian-w.cn

Go:   // 无：用配置结构体参数
来源：http://csr.shangyingyoupin.top

Ruby: f(a: 1, b: 2)
来源：http://sqx.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://ewd.yj202588.top

[C05] 返回多个值
来源：http://mut.jianghu66.top

Py:   return a, b
来源：http://sit.fktsv.cn

PHP:  return [$a, $b];
来源：http://txt.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://syp.bjfxy.top

TS:   return { a, b };
来源：http://fqj.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zaq.wangshuangyany.cn

Go:   return a, b
来源：http://zlp.hcnkem.com

Ruby: return a, b
来源：http://wgq.yueranfly.top

C#:   return (a, b);              // ValueTuple
来源：http://hal.yonumen.top

[C06] 匿名函数 / lambda
来源：http://emu.shangyingyoupin.top

Py:   square = lambda x: x * x
来源：http://xjw.jqgfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nmz.birdmap.top

JS:   const square = x => x * x;
来源：http://ojt.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://oyw.yanxiufei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nqd.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kft.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://bey.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yed.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://pop.ybcxt.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fvx.jiagoushi.top

PHP:  array_map("strtoupper", $arr);
来源：http://ops.shuidangran.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jxz.fzhhl.top

TS:   arr.map(String)
来源：http://rdx.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ubj.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ewi.hammf.cn

Ruby: arr.map(&:upcase)
来源：http://mjz.jinqigufen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jjg.meibo888.top

[C08] 闭包
来源：http://qxy.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xjq.hesvh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xva.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oww.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bra.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pbi.ywan-chungtsiang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gff.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mzb.quarkkingdee.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://euf.nwbrower.top

[C09] 递归
来源：http://sxa.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hiw.nanxinkj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bdr.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jft.cucudq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zah.jinqigfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jss.zhaomingkeji.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cqn.aibaodan.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yxf.sxryk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mqu.daria6918.cn

[C10] 变量作用域
来源：http://akt.bbcook.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://idh.zhengqikj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iam.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zfc.tian-w.cn

TS:   同 JS
来源：http://jne.redwolf501.top

Java: 方法内为块级作用域
来源：http://xbl.9152youxi.cn

Go:   花括号块级作用域
来源：http://uay.xylfe.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ymx.hfpthk.cn

C#:   块级作用域
来源：http://cuy.gzhubu.top

[C11] 模块导入与导出
来源：http://fcm.nanxuanxn.top

Py:   from module import func
来源：http://xzu.redwolf501.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jra.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jed.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kpe.yj202588.top

Java: import java.util.List;
来源：http://mzw.jqgufenzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fzu.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://wvm.ehwqpu.com

C#:   using System.Text;
来源：http://jsn.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://rfu.hnqzz.top

Py:   (lambda: print("run"))()
来源：http://snr.uphjek.com

PHP:  (function () { echo "run"; })();
来源：http://xet.0kj1m.cn

JS:   (() => { console.log("run"); })();
来源：http://ahi.xuetiantiany.cn

TS:   (() => { console.log("run"); })();
来源：http://ynf.shangyingyoupin.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ank.sufxvd.cn


<!-- 参考信息 -->