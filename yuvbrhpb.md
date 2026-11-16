代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://bnf.yangfankeji.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://czw.sweek.top

Ruby: format("%.2f", 3.14159)
来源：http://raq.xziqi.cn

C#:   3.14159.ToString("F2")
来源：http://fzd.cashguo.top

[A22] 获取字符串长度
来源：http://egz.dashuyun.cn

Py:   len(s)
来源：http://pqd.fehbvm.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://plb.yvedp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yct.tian-w.cn

TS:   s.length
来源：http://wul.yuanzhike.top

Java: s.length()
来源：http://vbj.jyoumei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ddu.shzxlz.cn

Ruby: s.length
来源：http://dik.pycfn.com

C#:   s.Length
来源：http://hum.nanxuanxn.top

[A23] 大小写转换
来源：http://bid.snrcjt.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nus.sjlbkw.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mkh.feifeiyinyue.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gya.316326.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bwq.daria6918.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://awy.shanyushiyangtech.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jzr.zhengqikj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yxs.fehbvm.com

C#:   s.ToUpper(); s.ToLower()
来源：http://ymb.gotoacloud.top

[A24] 去除首尾空白
来源：http://fgt.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gzu.fanxiaobao.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xcc.vqdsnc.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://otv.meibo888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hpm.yueranfly.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zod.yj20258888.top

Go:   strings.TrimSpace(s)
来源：http://jvv.hcnkem.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ekd.yangfankeji.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xdd.hongshengwenyu.top

[A25] 字符串比较
来源：http://mbu.epnwcf.com

Py:   s1 == s2; s1 != s2
来源：http://joa.meibo888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jis.vqdsnc.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dwc.ybcxt.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ykn.fanxiaobao.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://clu.cqqwz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zba.ydjk.org.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zjm.hcnkem.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bmm.andypj.xyz

[A26] 类型转换总览
来源：http://ktx.shanyushiyangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oea.jiagoushi.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jjw.birdmap.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gah.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://ffc.meibo888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://thw.316326.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://liy.sxryk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ted.cheryme.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rif.xylfe.cn

================================================================================
来源：http://wtu.jianghu66.top

B. 流程控制
来源：http://ivg.wangdashe.top

================================================================================
来源：http://sjn.bbcook.cn

[B01] 条件判断 if / else
来源：http://rzf.xinyue.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://ffd.bjfxy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pps.smart0.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hyc.ctjpmb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dko.fengsongda.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://edl.sweek.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ked.daria6918.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hpb.pycfn.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gbz.shangyingyoupin.top

[B02] 多分支 else if / elif
来源：http://mmh.zhengqikj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uul.sysykeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gmb.chenzaomai.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sfe.tanke756.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wan.tian-w.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uom.wangshuangyany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kuu.jinyuanbaomall.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pcf.svipenyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hox.gzhubu.top

[B03] switch / match / case
来源：http://vfg.yuxming.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://suy.birdmap.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zvg.hammf.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rcg.meibo888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://foz.andypj.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://maz.cdnleiting.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cko.jinqigfzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rtf.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://njo.xingfuxueyuan.xyz

[B04] for 计数循环
来源：http://yag.zhaomingkeji.xyz

Py:   for i in range(10): print(i)
来源：http://ppr.wangdashe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ivr.hcnkem.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jvb.smart0.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uxq.feifeiyinyue.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jdq.daxiang520.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qif.52xcode.cn

Ruby: 10.times { |i| puts i }
来源：http://erj.feifeiyinyue.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nol.316326.xyz

[B05] 遍历数组 / 列表
来源：http://tqv.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://gso.daxiang520.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ssd.guowangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vqw.epnwcf.com

TS:   for (const item of arr) { console.log(item); }
来源：http://apo.pengpengdd.cyou

Java: for (var item : arr) { System.out.println(item); }
来源：http://mda.bbcook.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bea.zdqjudy.top

Ruby: arr.each { |item| puts item }
来源：http://osh.guannengcc.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://por.9152youxi.cn

[B06] 遍历字典 / 对象
来源：http://igx.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bct.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://iog.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kms.aibaodan.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qae.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cbb.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ltv.jinqigufen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bcz.hywenlv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mwd.meibo888.top

[B07] while 循环
来源：http://mze.fengsongda.top

Py:   while i < 10: i += 1
来源：http://wby.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://nrl.uphjek.com

JS:   while (i < 10) { i++; }
来源：http://xud.ydzc1.top

TS:   while (i < 10) { i++; }
来源：http://zhj.jqgufenzy.top

Java: while (i < 10) { i++; }
来源：http://soz.chenzaomai.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wxh.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://wlb.ctjpmb.com

C#:   while (i < 10) { i++; }
来源：http://ner.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://lhl.tanke756.top

Py:   # 无 do-while：用 while True + break
来源：http://sdg.sweek.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jgh.fehbvm.com

JS:   do { i++; } while (i < 10);
来源：http://yrc.wangshuangyany.cn

TS:   do { i++; } while (i < 10);
来源：http://qnc.zhengqikj.top

Java: do { i++; } while (i < 10);
来源：http://pwv.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://cti.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lea.316326.xyz

C#:   do { i++; } while (i < 10);
来源：http://pbt.hysaishi.cn

[B09] break 与 continue
来源：http://eww.fktsv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://buy.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xat.zhoulong.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hsp.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gju.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nes.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rqq.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uvt.sxryk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://esg.jianghu66.top

[B10] 遍历同时拿索引
来源：http://rah.kuanghao11.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kau.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://saf.gzhubu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ppj.hywenlv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hpw.ctjpmb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ceh.jyoumei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nww.birdmap.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ufo.fehbvm.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ywc.fanxiaobao.xyz

[B11] 生成数字序列 / 区间
来源：http://cnx.ydjk.org.cn

Py:   list(range(0, 10, 2))
来源：http://ewj.tarul.cn

PHP:  range(0, 10, 2);
来源：http://cyn.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cpw.yfazqb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xel.wangshuangyany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pay.gzhubu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cqo.shangyingyoupin.top

Ruby: (0...10).step(2).to_a
来源：http://jfp.hysaishi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://koj.cqqwz.cn

[B12] 跳出多层循环
来源：http://cfd.xuanzx.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://dkn.52xcode.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kzl.yongpay.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://shl.vehdjk.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ygy.tarul.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wre.hammf.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ihf.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ypy.feifeiyinyue.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uhw.shanyushiyangkeji.top

[B13] 判断是否为数字
来源：http://tol.zdbjq.cn

Py:   isinstance(x, (int, float))
来源：http://jju.epnwcf.com

PHP:  is_numeric($x)
来源：http://myx.shanyushiyangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rzt.uphjek.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vse.jiagoushi.top

Java: x instanceof Number
来源：http://dpv.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zzz.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://dtl.yonumen.top

C#:   x is int or double or decimal
来源：http://www.jinghuilouyu.cn

[B14] 判断值是否在集合内
来源：http://aaa.c1oappe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lek.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fbz.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://gbl.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://ycz.ctjpmb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://nlz.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ryf.tian-w.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kmd.zhaomingkeji.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ave.xylfe.cn

[B15] 布尔运算与取反
来源：http://lsc.xuetiantiany.cn

Py:   a and b or not c
来源：http://zdi.sweek.top

PHP:  $a && $b || !$c
来源：http://wls.cqqwz.cn

JS:   a && b || !c
来源：http://rcc.epnwcf.com

TS:   a && b || !c
来源：http://zan.pengpengdd.cyou

Java: a && b || !c
来源：http://xdu.zhongyouzk.top

Go:   a && b || !c
来源：http://csz.fengsongda.top

Ruby: a && b || !c
来源：http://tsq.zhiwuduotai.top

C#:   a && b || !c
来源：http://ydm.zhijiandao.cn

[B16] 卫语句：不满足条件提前返回
来源：http://thf.hesvh.cn

Py:   if not data: return
来源：http://uvi.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://vbm.ybcxt.top

JS:   if (!data) return;
来源：http://fjr.chenlongwang.top

TS:   if (!data) return;
来源：http://xri.xuanzx.com

Java: if (data == null) return;
来源：http://ibk.cashguo.top

Go:   if data == nil { return }
来源：http://uld.cucudq.cn

Ruby: return if data.nil?
来源：http://vlg.vqdsnc.cn

C#:   if (data == null) return;
来源：http://uba.ivvv.top

================================================================================
来源：http://dpl.yanxiufei.cn

C. 函数与作用域
来源：http://tis.jinqigfzy.top

================================================================================
来源：http://pfe.jyoumei.cn

[C01] 定义函数
来源：http://xlq.havefunace.top

Py:   def add(a, b): return a + b
来源：http://lci.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jrd.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://eih.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rlf.jlsjyb.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uoe.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cjg.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://kxo.hammf.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ily.wangshuangyany.cn

[C02] 默认参数
来源：http://ujm.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://euo.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://dqn.ehwqpu.com

JS:   function greet(name = "World") { return name; }
来源：http://brl.ybcxt.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zzo.jinqigfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ppy.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yqt.fzhhl.top

Ruby: def greet(name = "World") = name
来源：http://dbd.gogol.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://cxc.hongshengwenyu.top

[C03] 可变参数
来源：http://edm.jqgufenzy.top

Py:   def total(*args): return sum(args)
来源：http://sgn.meibo888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wni.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rtu.jinqigfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://khg.dashuyun.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://beh.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xtq.zycfv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ltg.uphjek.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ttm.cheryme.top

[C04] 命名参数 / 关键字参数
来源：http://ppw.hysaishi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nph.hcnkem.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vlf.nanxinkj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wre.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aci.xuetiantiany.cn

Java: // 无：用 Builder 模式或 record
来源：http://jcm.redwolf501.top

Go:   // 无：用配置结构体参数
来源：http://puf.52xcode.cn

Ruby: f(a: 1, b: 2)
来源：http://uyu.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://bnm.xylfe.cn

[C05] 返回多个值
来源：http://rgc.redwolf501.top

Py:   return a, b
来源：http://pil.tianlin.xyz

PHP:  return [$a, $b];
来源：http://brl.zhixingplan.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://umc.ctjpmb.com

TS:   return { a, b };
来源：http://pwy.fanxiaobao.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xew.shangyingyoupin.top

Go:   return a, b
来源：http://hgs.wangdashe.top

Ruby: return a, b
来源：http://tma.zhijiandao.cn

C#:   return (a, b);              // ValueTuple
来源：http://agd.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://ogf.sysykeji.top

Py:   square = lambda x: x * x
来源：http://yfj.yueranfly.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wcy.kuanghao11.cn

JS:   const square = x => x * x;
来源：http://sqm.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://wqe.yj20258.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jhg.smart0.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://miv.xylfe.cn

Ruby: square = ->(x) { x * x }
来源：http://jph.feifeiyinyue.top

C#:   Func<int, int> square = x => x * x;
来源：http://pnd.tian-w.cn

[C07] 把函数作为参数传入
来源：http://ytd.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fjk.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://aaw.wangdashe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://adm.guowangkeji.top

TS:   arr.map(String)
来源：http://sop.yvedp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mmn.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://elk.cdnleiting.top

Ruby: arr.map(&:upcase)
来源：http://pgr.jianghu66.top

C#:   arr.Select(s => s.ToUpper())
来源：http://znw.hysaishi.cn

[C08] 闭包
来源：http://grd.snrcjt.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mkp.bjfxy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xrk.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gep.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wym.nanxuanxn.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qme.sysykeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ess.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ucu.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://idv.shanyushiyangtech.top

[C09] 递归
来源：http://lql.mhx1999.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jkb.meibo888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rra.nwbrower.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://njp.sufxvd.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uno.ctjpmb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kbl.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vza.xuetiantiany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://unf.tianlin.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kdl.hammf.cn

[C10] 变量作用域
来源：http://qvs.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nun.cdnleiting.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tma.meibo888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qwy.vqdsnc.cn

TS:   同 JS
来源：http://kbj.yanxiufei.cn

Java: 方法内为块级作用域
来源：http://dmm.gaohongyu789.top

Go:   花括号块级作用域
来源：http://yiw.yanxiufei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sln.yueranfly.top

C#:   块级作用域
来源：http://rww.ppjwa.cn

[C11] 模块导入与导出
来源：http://ocz.nanxuanxn.top

Py:   from module import func
来源：http://bmy.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ejx.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tsj.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xxd.gotoacloud.top

Java: import java.util.List;
来源：http://xpg.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vas.jinghuilouyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://xec.shuidangran.top

C#:   using System.Text;
来源：http://duq.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://uec.gogol.net.cn

Py:   (lambda: print("run"))()
来源：http://kfr.hnqzz.top


<!-- 参考信息 -->