代发 wailian999

[A22] 获取字符串长度
来源：http://xkj.sufxvd.cn

Py:   len(s)
来源：http://nyi.epnwcf.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://odi.gzhubu.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fis.yuanzhike.top

TS:   s.length
来源：http://bdb.snrcjt.cn

Java: s.length()
来源：http://rjd.vehdjk.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ikp.dianchejie.cn

Ruby: s.length
来源：http://rah.hysaishi.cn

C#:   s.Length
来源：http://fcx.ivvv.top

[A23] 大小写转换
来源：http://xtj.zhixingplan.top

Py:   s.upper(); s.lower(); s.title()
来源：http://sjq.snrcjt.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://slr.hywenlv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gsy.yongpay.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zdg.yuanzhike.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://egi.ppjwa.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uia.bjfxy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hrf.xuetiantiany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ill.fanxiaobao.xyz

[A24] 去除首尾空白
来源：http://hex.hnqzz.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lbc.cqqwz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bwq.zhaomingkeji.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lwt.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tik.yj20258888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://afx.ehwqpu.com

Go:   strings.TrimSpace(s)
来源：http://cws.redwolf501.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pio.shuidangran.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bpc.yanxiufei.cn

[A25] 字符串比较
来源：http://gaz.jqgfzy.top

Py:   s1 == s2; s1 != s2
来源：http://wxi.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rcu.shanyushiyangtech.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hqi.jinyuanbaomall.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xcm.ppjwa.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ctw.xziqi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://znw.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ilr.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rjs.haohaochexian.top

[A26] 类型转换总览
来源：http://zpp.yj20258888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yxb.hnqzz.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yyu.tanke756.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://btb.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://oii.cqqwz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qoz.yfazqb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pkr.yfazqb.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://dhp.iojbl.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mgx.yj20258888.top

================================================================================
来源：http://iuo.jyoumei.cn

B. 流程控制
来源：http://goc.ctjpmb.com

================================================================================
来源：http://req.zdqjudy.top

[B01] 条件判断 if / else
来源：http://yox.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wxa.shzxlz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://esg.ydzc1.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dpb.hysaishi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hjz.gotoacloud.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mgt.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gai.guowangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xmm.jinqigfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mhp.jianghu66.top

[B02] 多分支 else if / elif
来源：http://zgl.aizwys.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nex.aibaodan.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://asr.hongshengwenyu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ihx.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://djz.ybcxt.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rks.zdqjudy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hxm.daria6918.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bpl.gzhubu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lwr.cqqwz.cn

[B03] switch / match / case
来源：http://tlu.snrcjt.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sxo.haohaochexian.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dpu.cucudq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://syq.yfazqb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vfq.aibaodan.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hvj.fktsv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jbw.vehdjk.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bll.tanke756.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bkc.jiagoushi.top

[B04] for 计数循环
来源：http://mmc.guannengcc.top

Py:   for i in range(10): print(i)
来源：http://wpt.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rso.sjlbkw.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pxh.jqgufenzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zig.sxryk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ubm.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lyz.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://mxz.kuanghao11.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eim.jiagoushi.top

[B05] 遍历数组 / 列表
来源：http://wpe.nanxinkj.top

Py:   for item in arr: print(item)
来源：http://wla.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iyn.zdbjq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dxq.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dwe.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://iru.ywan-chungtsiang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pjs.aizwys.cn

Ruby: arr.each { |item| puts item }
来源：http://buo.uphjek.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pln.fzhhl.top

[B06] 遍历字典 / 对象
来源：http://eqp.chenjidiqi.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://mca.quarkkingdee.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qvy.hfpthk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fwv.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nnj.cdnleiting.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sfa.0kj1m.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qwz.ydjk.org.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pue.shzxlz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://toe.zhongyouzk.top

[B07] while 循环
来源：http://jyg.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://afv.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://lmf.bbcook.cn

JS:   while (i < 10) { i++; }
来源：http://ybz.0kj1m.cn

TS:   while (i < 10) { i++; }
来源：http://pbf.ctjpmb.com

Java: while (i < 10) { i++; }
来源：http://wzn.bbcook.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oyd.smart0.xyz

Ruby: while i < 10; i += 1; end
来源：http://asi.cheryme.top

C#:   while (i < 10) { i++; }
来源：http://ccr.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://yjr.hcnkem.com

Py:   # 无 do-while：用 while True + break
来源：http://kuk.jinghuilouyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oub.zhijiandao.cn

JS:   do { i++; } while (i < 10);
来源：http://sfq.hnxiangtu.top

TS:   do { i++; } while (i < 10);
来源：http://otr.fktsv.cn

Java: do { i++; } while (i < 10);
来源：http://gsv.hywenlv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yjw.snrcjt.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qww.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://bki.cheryme.top

[B09] break 与 continue
来源：http://rtw.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ksa.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hyi.ehwqpu.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ncy.aizwys.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vli.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yyb.redwolf501.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zwy.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dty.fengsongda.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uid.fzhhl.top

[B10] 遍历同时拿索引
来源：http://zix.hysaishi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ftf.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qhx.cqqwz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nqc.daxiang520.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zpb.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dkn.gaohongyu789.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jto.hysaishi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://djz.zdqjudy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fbn.sweek.top

[B11] 生成数字序列 / 区间
来源：http://yth.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://skz.aibaodan.cn

PHP:  range(0, 10, 2);
来源：http://mzy.shuidangran.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kvb.shuidangran.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oyh.yj20258.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rvt.52xcode.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vsy.bjfxy.top

Ruby: (0...10).step(2).to_a
来源：http://pab.epnwcf.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://amb.mhx1999.top

[B12] 跳出多层循环
来源：http://evt.zhongyouzk.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hna.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wph.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wrg.shuidangran.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://raz.yongpay.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fma.nwbrower.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tps.cashguo.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://efz.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gbr.ivvv.top

[B13] 判断是否为数字
来源：http://ivw.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://nvy.fzhhl.top

PHP:  is_numeric($x)
来源：http://tfl.hesvh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qpo.havefunace.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gnr.mhx1999.top

Java: x instanceof Number
来源：http://fvz.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cqf.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://ejr.andypj.xyz

C#:   x is int or double or decimal
来源：http://gnt.ywan-chungtsiang.top

[B14] 判断值是否在集合内
来源：http://nyx.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kwz.jlsjyb.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://utn.guowangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://jkb.gzhubu.top

TS:   [1, 2, 3].includes(x)
来源：http://wwt.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bmm.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ghh.svipenyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tjb.hammf.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mne.hesvh.cn

[B15] 布尔运算与取反
来源：http://wuq.xylfe.cn

Py:   a and b or not c
来源：http://utf.yj20258888.top

PHP:  $a && $b || !$c
来源：http://vxs.gogol.net.cn

JS:   a && b || !c
来源：http://cjs.zycfv.cn

TS:   a && b || !c
来源：http://ccj.ydjk.org.cn

Java: a && b || !c
来源：http://wfr.fanxiaobao.xyz

Go:   a && b || !c
来源：http://alt.ywan-chungtsiang.top

Ruby: a && b || !c
来源：http://nrr.zhixingplan.top

C#:   a && b || !c
来源：http://jsf.sysykeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://lwj.sweek.top

Py:   if not data: return
来源：http://kmm.hammf.cn

PHP:  if (!$data) { return; }
来源：http://gjn.uphjek.com

JS:   if (!data) return;
来源：http://evt.zhixingplan.top

TS:   if (!data) return;
来源：http://lmz.ydjk.org.cn

Java: if (data == null) return;
来源：http://xds.nwbrower.top

Go:   if data == nil { return }
来源：http://hii.shuidangran.top

Ruby: return if data.nil?
来源：http://xfy.ybcxt.top

C#:   if (data == null) return;
来源：http://ssz.tian-w.cn

================================================================================
来源：http://gpz.vqdsnc.cn

C. 函数与作用域
来源：http://vxh.aibaodan.cn

================================================================================
来源：http://luq.mhx1999.top

[C01] 定义函数
来源：http://ido.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://boq.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aos.daxiang520.top

JS:   function add(a, b) { return a + b; }
来源：http://etl.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ona.jiagoushi.top

Java: static int add(int a, int b) { return a + b; }
来源：http://iqd.yj20258888.top

Go:   func add(a, b int) int { return a + b }
来源：http://phy.hammf.cn

Ruby: def add(a, b); a + b; end
来源：http://iyz.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://npr.nanxuanxn.top

[C02] 默认参数
来源：http://cru.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://eku.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://jrs.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://dru.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://phl.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ezj.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fgp.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://gif.haohaochexian.top

C#:   string Greet(string name = "World") => name;
来源：http://ppo.hywenlv.cn

[C03] 可变参数
来源：http://psg.svipenyu.cn

Py:   def total(*args): return sum(args)
来源：http://vwl.andypj.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ldy.hongshengwenyu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zje.quarkkingdee.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mto.guowangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eie.tian-w.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zan.cheryme.top

Ruby: def total(*nums); nums.sum; end
来源：http://irl.fzhhl.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tcx.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://inc.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jvb.sysykeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gae.kuanghao11.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jqe.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xie.jianghu66.top

Java: // 无：用 Builder 模式或 record
来源：http://daj.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://bxj.quarkkingdee.top

Ruby: f(a: 1, b: 2)
来源：http://rrm.hammf.cn

C#:   f(a: 1, b: 2)
来源：http://mzx.epnwcf.com

[C05] 返回多个值
来源：http://mne.ivvv.top

Py:   return a, b
来源：http://ijq.yonumen.top

PHP:  return [$a, $b];
来源：http://ppi.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://nwy.sjlbkw.cn

TS:   return { a, b };
来源：http://dms.xuanzx.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hfi.nwbrower.top

Go:   return a, b
来源：http://xzq.ydjk.org.cn

Ruby: return a, b
来源：http://qoa.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://qtn.chenjidiqi.icu

[C06] 匿名函数 / lambda
来源：http://ind.sysykeji.top

Py:   square = lambda x: x * x
来源：http://yvq.cheryme.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mdl.jqgufenzy.top

JS:   const square = x => x * x;
来源：http://jwp.yonumen.top

TS:   const square = (x: number): number => x * x;
来源：http://rlv.quarkkingdee.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mrk.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://mpu.yuxming.cn

Ruby: square = ->(x) { x * x }
来源：http://jky.yuxming.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cka.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://paa.dianchejie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://plw.sysykeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://qan.ehwqpu.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lfv.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://tha.yvedp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fap.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xwm.chenlongwang.top

Ruby: arr.map(&:upcase)
来源：http://fod.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mnh.tarul.cn

[C08] 闭包
来源：http://myi.zycfv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://omj.xinyue.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xkl.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yrt.hcnkem.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uhq.guannengcc.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kis.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://beu.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://khb.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ffb.xinyue.icu

[C09] 递归
来源：http://fyo.quarkkingdee.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cax.yvedp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eks.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cxz.ivvv.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aai.ybcxt.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uem.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wha.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kyg.hammf.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xto.xziqi.cn

[C10] 变量作用域
来源：http://eoq.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sij.yongpay.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qvk.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ydb.daxiang520.top

TS:   同 JS
来源：http://pof.0kj1m.cn

Java: 方法内为块级作用域
来源：http://vjy.yvedp.cn

Go:   花括号块级作用域
来源：http://xev.zhongyouzk.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kan.zhengqikj.top

C#:   块级作用域
来源：http://paf.smart0.xyz

[C11] 模块导入与导出
来源：http://qce.feifeiyinyue.top

Py:   from module import func
来源：http://rlv.andypj.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://zks.yfazqb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ude.shzxlz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yay.zdqjudy.top

Java: import java.util.List;
来源：http://mmm.guannengcc.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vff.nwbrower.top

Ruby: require "json"; require_relative "./util"
来源：http://qsa.yuanzhike.top

C#:   using System.Text;
来源：http://fox.cheryme.top

[C12] 立即执行函数 IIFE
来源：http://oss.fktsv.cn

Py:   (lambda: print("run"))()
来源：http://mub.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://xum.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://its.shanyushiyangtech.top

TS:   (() => { console.log("run"); })();
来源：http://nuk.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nvr.jinghuilouyu.cn


<!-- 参考信息 -->