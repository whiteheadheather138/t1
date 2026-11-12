代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://alt.jlsjyb.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lxn.havefunace.top

Ruby: format("%.2f", 3.14159)
来源：http://wvm.xuanzx.com

C#:   3.14159.ToString("F2")
来源：http://tck.jinqigufen.top

[A22] 获取字符串长度
来源：http://smx.hysaishi.cn

Py:   len(s)
来源：http://upz.tian-w.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hsr.jianghu66.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uyh.smart0.xyz

TS:   s.length
来源：http://wvt.shangyingyoupin.top

Java: s.length()
来源：http://loc.zhoulong.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nke.zhiwuduotai.top

Ruby: s.length
来源：http://rya.jinyuanbaomall.cn

C#:   s.Length
来源：http://fta.c1oappe.top

[A23] 大小写转换
来源：http://jsj.zhijiandao.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ema.nwbrower.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pcw.hnxiangtu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://arr.andypj.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jcg.ctjpmb.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zir.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hvq.yj202588.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mrn.quarkkingdee.top

C#:   s.ToUpper(); s.ToLower()
来源：http://acp.yangfankeji.com

[A24] 去除首尾空白
来源：http://ims.zhijiandao.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hnh.smart0.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xxg.tanke756.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zds.snrcjt.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jga.havefunace.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rlu.bbcook.cn

Go:   strings.TrimSpace(s)
来源：http://itw.zdqjudy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mby.chenlongwang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zpc.sxryk.cn

[A25] 字符串比较
来源：http://vam.hywenlv.cn

Py:   s1 == s2; s1 != s2
来源：http://ggr.jyoumei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nwq.tarul.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cwk.zhoulong.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ngd.shanyushiyangtech.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rph.fzhhl.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hus.nwbrower.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rbw.vehdjk.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qcc.yuxming.cn

[A26] 类型转换总览
来源：http://vbh.yuanzhike.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pqy.shzxlz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ppd.sufxvd.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gfs.zdbjq.cn

TS:   Number() String() Boolean() x as number
来源：http://fmw.zhengqikj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dfc.jianghu66.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iot.gzhubu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bph.yj202588.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qos.vqdsnc.cn

================================================================================
来源：http://elf.hongshengwenyu.top

B. 流程控制
来源：http://xit.hammf.cn

================================================================================
来源：http://ofp.yuxming.cn

[B01] 条件判断 if / else
来源：http://srx.jinghuilouyu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pfk.sjlbkw.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iee.hfpthk.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sqh.zhixingplan.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://njq.tanke756.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rmf.jianghu66.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mwj.c1oappe.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cbr.yonumen.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ueb.jlsjyb.cn

[B02] 多分支 else if / elif
来源：http://rdm.nanxinkj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xoe.bjfxy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mkc.zdbjq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pdp.0kj1m.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fai.316326.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jqf.cqqwz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mhq.zhongyouzk.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jdi.316326.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eai.jianghu66.top

[B03] switch / match / case
来源：http://ufg.gzhubu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jxb.snrcjt.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fqb.wangdashe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hxk.shuidangran.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sem.guannengcc.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nwz.bjfxy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iyn.guannengcc.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qaa.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mhv.hysaishi.cn

[B04] for 计数循环
来源：http://fbe.vqdsnc.cn

Py:   for i in range(10): print(i)
来源：http://bxa.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ppm.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pju.feifeiyinyue.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yfv.cqqwz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://icg.cashguo.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://irq.jinqigufen.top

Ruby: 10.times { |i| puts i }
来源：http://bbm.dashuyun.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ycu.hfpthk.cn

[B05] 遍历数组 / 列表
来源：http://tif.aizwys.cn

Py:   for item in arr: print(item)
来源：http://xkj.chenjidiqi.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tno.uphjek.com

JS:   for (const item of arr) { console.log(item); }
来源：http://tgk.aibaodan.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hzk.sjlbkw.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qpj.hnqzz.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cae.havefunace.top

Ruby: arr.each { |item| puts item }
来源：http://fqg.mhx1999.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vqw.guannengcc.top

[B06] 遍历字典 / 对象
来源：http://sle.zhoulong.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://jlq.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nlo.gotoacloud.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://svh.yvedp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ool.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yhl.redwolf501.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hka.zdqjudy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cev.iojbl.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lpt.yuanzhike.top

[B07] while 循环
来源：http://hsw.sysykeji.top

Py:   while i < 10: i += 1
来源：http://dbx.aizwys.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eqt.hesvh.cn

JS:   while (i < 10) { i++; }
来源：http://ngk.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://lak.hywenlv.cn

Java: while (i < 10) { i++; }
来源：http://zti.pengpengdd.cyou

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ufl.c1oappe.top

Ruby: while i < 10; i += 1; end
来源：http://ceq.meibo888.top

C#:   while (i < 10) { i++; }
来源：http://zan.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://rlq.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://vlp.xuanzx.com

PHP:  do { $i++; } while ($i < 10);
来源：http://sun.shzxlz.cn

JS:   do { i++; } while (i < 10);
来源：http://xxe.yuanzhike.top

TS:   do { i++; } while (i < 10);
来源：http://mzp.yvedp.cn

Java: do { i++; } while (i < 10);
来源：http://ddb.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://acq.9152youxi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rpt.jqgfzy.top

C#:   do { i++; } while (i < 10);
来源：http://qvh.xuanzx.com

[B09] break 与 continue
来源：http://tsn.ehwqpu.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qbp.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mhv.zdqjudy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wod.jqgufenzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mmi.tian-w.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rdr.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vrs.zdbjq.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xdt.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://emd.c1oappe.top

[B10] 遍历同时拿索引
来源：http://aus.jlsjyb.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nek.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ltf.hywenlv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rbn.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bul.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fgn.hysaishi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://trq.sysykeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rpy.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bzd.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://hrs.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://cqj.meibo888.top

PHP:  range(0, 10, 2);
来源：http://wfu.quarkkingdee.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dgg.zhongyouzk.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lko.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://epp.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blw.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://kqn.52xcode.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aon.andypj.xyz

[B12] 跳出多层循环
来源：http://aaf.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://xgu.haohaochexian.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vua.yonumen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hzi.hywenlv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pkr.dianchejie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pto.ydjk.org.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uyb.xinyue.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xks.ivvv.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://clt.yonumen.top

[B13] 判断是否为数字
来源：http://bmw.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://cjx.bbcook.cn

PHP:  is_numeric($x)
来源：http://cel.sxryk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kzu.dianchejie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xep.cashguo.top

Java: x instanceof Number
来源：http://ngy.tian-w.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wss.cucudq.cn

Ruby: x.is_a?(Numeric)
来源：http://yub.ivvv.top

C#:   x is int or double or decimal
来源：http://ctv.epnwcf.com

[B14] 判断值是否在集合内
来源：http://htd.jinyuanbaomall.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mqw.yj20258888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kgj.zhaomingkeji.xyz

JS:   [1, 2, 3].includes(x)
来源：http://tbt.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://nsp.ywan-chungtsiang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kaw.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://njc.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://qvq.shanyushiyangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xzi.yuanzhike.top

[B15] 布尔运算与取反
来源：http://cpt.jinqigufen.top

Py:   a and b or not c
来源：http://rwz.aizwys.cn

PHP:  $a && $b || !$c
来源：http://uex.zhiwuduotai.top

JS:   a && b || !c
来源：http://gip.c1oappe.top

TS:   a && b || !c
来源：http://qpa.yonumen.top

Java: a && b || !c
来源：http://noc.yvedp.cn

Go:   a && b || !c
来源：http://mjp.yfazqb.com

Ruby: a && b || !c
来源：http://jdr.bjfxy.top

C#:   a && b || !c
来源：http://ive.smart0.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://mjn.yangfankeji.com

Py:   if not data: return
来源：http://dpe.aibaodan.cn

PHP:  if (!$data) { return; }
来源：http://tgx.zhengqikj.top

JS:   if (!data) return;
来源：http://jdu.iojbl.cn

TS:   if (!data) return;
来源：http://eqg.jinqigfzy.top

Java: if (data == null) return;
来源：http://dih.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://edt.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://shq.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://npm.fktsv.cn

================================================================================
来源：http://otr.yangfankeji.com

C. 函数与作用域
来源：http://zcn.zhengqikj.top

================================================================================
来源：http://yda.fehbvm.com

[C01] 定义函数
来源：http://ydu.sufxvd.cn

Py:   def add(a, b): return a + b
来源：http://cdx.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yxr.yj202588.top

JS:   function add(a, b) { return a + b; }
来源：http://duw.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://led.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zyd.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://mpg.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://nai.yuanzhike.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fzw.vehdjk.com

[C02] 默认参数
来源：http://vgc.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://mwz.sjlbkw.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rdj.tian-w.cn

JS:   function greet(name = "World") { return name; }
来源：http://wye.pengpengdd.cyou

TS:   function greet(name: string = "World") { return name; }
来源：http://fut.gotoacloud.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zch.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jmt.zhengqikj.top

Ruby: def greet(name = "World") = name
来源：http://aml.shangyingyoupin.top

C#:   string Greet(string name = "World") => name;
来源：http://bpk.chenjidiqi.icu

[C03] 可变参数
来源：http://gsr.fzhhl.top

Py:   def total(*args): return sum(args)
来源：http://wol.yongpay.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://guw.tian-w.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rac.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ysm.9152youxi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ltl.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ibd.fengsongda.top

Ruby: def total(*nums); nums.sum; end
来源：http://ttl.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mwi.feifeiyinyue.top

[C04] 命名参数 / 关键字参数
来源：http://fng.kuanghao11.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sue.xingfuxueyuan.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://njb.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ngw.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mmg.jinyuanbaomall.cn

Java: // 无：用 Builder 模式或 record
来源：http://ahw.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://hjk.jyoumei.cn

Ruby: f(a: 1, b: 2)
来源：http://ixy.cqqwz.cn

C#:   f(a: 1, b: 2)
来源：http://flu.ydjk.org.cn

[C05] 返回多个值
来源：http://bbv.sweek.top

Py:   return a, b
来源：http://ayw.andypj.xyz

PHP:  return [$a, $b];
来源：http://jiv.0kj1m.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hxo.zdbjq.cn

TS:   return { a, b };
来源：http://yef.0kj1m.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blj.havefunace.top

Go:   return a, b
来源：http://dsg.jqgufenzy.top

Ruby: return a, b
来源：http://tiq.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://mmw.sxryk.cn

[C06] 匿名函数 / lambda
来源：http://nff.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://ymh.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://cdz.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://mfu.mhx1999.top

TS:   const square = (x: number): number => x * x;
来源：http://dzl.fehbvm.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://juy.andypj.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://snq.zhixingplan.top

Ruby: square = ->(x) { x * x }
来源：http://bvc.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://nzq.tanke756.top

[C07] 把函数作为参数传入
来源：http://arh.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rdy.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://xih.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://apu.yonumen.top

TS:   arr.map(String)
来源：http://jgd.hfpthk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rxu.yueranfly.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wat.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://xzx.xylfe.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wpb.yj20258.top

[C08] 闭包
来源：http://ebd.jqgfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qtd.hesvh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fwj.yonumen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sha.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bqy.xziqi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dtp.havefunace.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://etj.zdbjq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nnk.bjfxy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vsm.yuxming.cn

[C09] 递归
来源：http://roj.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hcb.vqdsnc.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://apm.yj20258888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ugk.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jwh.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yne.yfazqb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iob.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://joj.dashuyun.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://caw.daxiang520.top

[C10] 变量作用域
来源：http://luy.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://osr.nanxinkj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nnp.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ysn.hcnkem.com

TS:   同 JS
来源：http://aqm.jyoumei.cn

Java: 方法内为块级作用域
来源：http://gkd.aizwys.cn

Go:   花括号块级作用域
来源：http://blc.hnxiangtu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gbz.c1oappe.top

C#:   块级作用域
来源：http://sec.zycfv.cn

[C11] 模块导入与导出
来源：http://lvz.sysykeji.top

Py:   from module import func
来源：http://vdy.andypj.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://uml.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gvw.quarkkingdee.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yym.jinqigufen.top

Java: import java.util.List;
来源：http://keb.smart0.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aol.fzhhl.top

Ruby: require "json"; require_relative "./util"
来源：http://nph.hongshengwenyu.top

C#:   using System.Text;
来源：http://ktv.wangshuangyany.cn

[C12] 立即执行函数 IIFE
来源：http://vkh.ivvv.top

Py:   (lambda: print("run"))()
来源：http://hsq.zhixingplan.top


<!-- 参考信息 -->