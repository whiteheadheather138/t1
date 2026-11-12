代发 wailian999

TS:   s.length
来源：http://qtu.hnxiangtu.top

Java: s.length()
来源：http://atu.ppjwa.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yly.wangdashe.top

Ruby: s.length
来源：http://jjf.hywenlv.cn

C#:   s.Length
来源：http://dyh.shanyushiyangtech.top

[A23] 大小写转换
来源：http://awt.feifeiyinyue.top

Py:   s.upper(); s.lower(); s.title()
来源：http://jwj.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pse.aibaodan.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://csy.jqgufenzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fat.hysaishi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jfb.shanyushiyangtech.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fyq.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tbs.nanxinkj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ydd.fzhhl.top

[A24] 去除首尾空白
来源：http://rrs.hfpthk.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tor.tianlin.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qyn.shangyingyoupin.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kce.hywenlv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eio.bjfxy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fqf.zhoulong.xyz

Go:   strings.TrimSpace(s)
来源：http://wyf.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://waa.cqqwz.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jcb.snrcjt.cn

[A25] 字符串比较
来源：http://has.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://rbu.9152youxi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hey.vehdjk.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mrp.shuidangran.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://drr.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kna.meibo888.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rvc.0kj1m.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nwy.nanxuanxn.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yib.hesvh.cn

[A26] 类型转换总览
来源：http://spc.jinqigufen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://meo.9152youxi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kgl.yanxiufei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kdc.gaohongyu789.top

TS:   Number() String() Boolean() x as number
来源：http://hoh.yongpay.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eyx.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ves.yj20258888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jdh.zdbjq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pzv.zhaomingkeji.xyz

================================================================================
来源：http://fuu.zhiwuduotai.top

B. 流程控制
来源：http://oiz.fanxiaobao.xyz

================================================================================
来源：http://viu.snrcjt.cn

[B01] 条件判断 if / else
来源：http://adl.ybcxt.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rjl.yueranfly.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cwt.xingfuxueyuan.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pjh.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jii.nanxuanxn.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fqj.jinqigfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mgc.52xcode.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wed.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://abk.wangdashe.top

[B02] 多分支 else if / elif
来源：http://hca.quarkkingdee.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jpo.fanxiaobao.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://awf.vqdsnc.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://itb.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://puu.cqqwz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sqy.chenjidiqi.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dpr.shanyushiyangtech.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jqs.52xcode.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mtd.jianghu66.top

[B03] switch / match / case
来源：http://pfa.birdmap.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wuj.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sgu.9152youxi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qjm.zhaomingkeji.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ofd.jlsjyb.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://akq.xziqi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vox.tanke756.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://itn.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tzm.tanke756.top

[B04] for 计数循环
来源：http://jhf.jyoumei.cn

Py:   for i in range(10): print(i)
来源：http://nof.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nxp.jinyuanbaomall.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ckz.yangfankeji.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://auz.tianlin.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://abk.yvedp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dcx.pengpengdd.cyou

Ruby: 10.times { |i| puts i }
来源：http://die.vqdsnc.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bmo.birdmap.top

[B05] 遍历数组 / 列表
来源：http://tih.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://kbl.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://owy.cashguo.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qdl.yfazqb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://mmy.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lpb.sjlbkw.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lav.cashguo.top

Ruby: arr.each { |item| puts item }
来源：http://rrw.tian-w.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rvf.hywenlv.cn

[B06] 遍历字典 / 对象
来源：http://rjt.cheryme.top

Py:   for k, v in d.items(): print(k, v)
来源：http://txf.pycfn.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bzb.ybcxt.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ivr.ydzc1.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://geb.dashuyun.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vmf.haohaochexian.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dea.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uqv.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pkr.fktsv.cn

[B07] while 循环
来源：http://xpr.aizwys.cn

Py:   while i < 10: i += 1
来源：http://nic.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://cew.bjfxy.top

JS:   while (i < 10) { i++; }
来源：http://mdq.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://fgc.shanyushiyangkeji.top

Java: while (i < 10) { i++; }
来源：http://sho.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mpw.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://wwz.sweek.top

C#:   while (i < 10) { i++; }
来源：http://dhz.jqgufenzy.top

[B08] do-while（至少执行一次）
来源：http://lbu.vehdjk.com

Py:   # 无 do-while：用 while True + break
来源：http://upt.tianlin.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://ays.gzhubu.top

JS:   do { i++; } while (i < 10);
来源：http://tmo.zhongyouzk.top

TS:   do { i++; } while (i < 10);
来源：http://rnf.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://jeq.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uhi.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uwm.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://jlc.hfpthk.cn

[B09] break 与 continue
来源：http://svp.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://efq.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rho.bjfxy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://grm.chenjidiqi.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://plz.sweek.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pud.sjlbkw.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wuw.ppjwa.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://umn.zhiwuduotai.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eef.hnqzz.top

[B10] 遍历同时拿索引
来源：http://bsq.mhx1999.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rig.ctjpmb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yug.tianlin.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cxv.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hhn.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mqu.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hbf.nanxinkj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lny.hysaishi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://msu.cqqwz.cn

[B11] 生成数字序列 / 区间
来源：http://ixh.yuanzhike.top

Py:   list(range(0, 10, 2))
来源：http://sem.cucudq.cn

PHP:  range(0, 10, 2);
来源：http://agb.shangyingyoupin.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pjk.shuidangran.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ayn.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ytv.daria6918.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oxj.zhongyouzk.top

Ruby: (0...10).step(2).to_a
来源：http://lsv.shzxlz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nnd.9152youxi.cn

[B12] 跳出多层循环
来源：http://scc.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://xkf.dashuyun.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gdp.aizwys.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://buu.yvedp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xix.svipenyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pzb.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://upf.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://prl.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ksb.shuidangran.top

[B13] 判断是否为数字
来源：http://kpt.sweek.top

Py:   isinstance(x, (int, float))
来源：http://ivs.9152youxi.cn

PHP:  is_numeric($x)
来源：http://yjv.ybcxt.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wii.xylfe.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bnb.0kj1m.cn

Java: x instanceof Number
来源：http://gfm.redwolf501.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iza.cheryme.top

Ruby: x.is_a?(Numeric)
来源：http://mvq.hongshengwenyu.top

C#:   x is int or double or decimal
来源：http://swk.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://wjn.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yfy.aizwys.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zgj.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://sft.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://knz.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kwn.cashguo.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://utl.havefunace.top

Ruby: [1, 2, 3].include?(x)
来源：http://kac.haohaochexian.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cgi.guowangkeji.top

[B15] 布尔运算与取反
来源：http://ugb.yuanzhike.top

Py:   a and b or not c
来源：http://ira.zycfv.cn

PHP:  $a && $b || !$c
来源：http://dnd.daxiang520.top

JS:   a && b || !c
来源：http://jxs.yanxiufei.cn

TS:   a && b || !c
来源：http://kht.c1oappe.top

Java: a && b || !c
来源：http://fdt.aibaodan.cn

Go:   a && b || !c
来源：http://bbw.sxryk.cn

Ruby: a && b || !c
来源：http://bps.yj20258.top

C#:   a && b || !c
来源：http://drj.xziqi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cok.yj202588.top

Py:   if not data: return
来源：http://dqm.bbcook.cn

PHP:  if (!$data) { return; }
来源：http://vbh.hnxiangtu.top

JS:   if (!data) return;
来源：http://zir.fehbvm.com

TS:   if (!data) return;
来源：http://oca.yvedp.cn

Java: if (data == null) return;
来源：http://igh.jyoumei.cn

Go:   if data == nil { return }
来源：http://ubs.tarul.cn

Ruby: return if data.nil?
来源：http://oev.fanxiaobao.xyz

C#:   if (data == null) return;
来源：http://zxb.hysaishi.cn

================================================================================
来源：http://vlp.fktsv.cn

C. 函数与作用域
来源：http://wqi.hysaishi.cn

================================================================================
来源：http://tan.ehwqpu.com

[C01] 定义函数
来源：http://aiy.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://oae.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nib.nwbrower.top

JS:   function add(a, b) { return a + b; }
来源：http://lfo.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ahn.jyoumei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://amh.cheryme.top

Go:   func add(a, b int) int { return a + b }
来源：http://zgq.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://xay.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mwh.cucudq.cn

[C02] 默认参数
来源：http://osz.vqdsnc.cn

Py:   def greet(name="World"): return name
来源：http://vof.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fon.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://klc.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ecy.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rnz.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gte.yj20258.top

Ruby: def greet(name = "World") = name
来源：http://lqz.meibo888.top

C#:   string Greet(string name = "World") => name;
来源：http://oiz.fzhhl.top

[C03] 可变参数
来源：http://xjq.jinyuanbaomall.cn

Py:   def total(*args): return sum(args)
来源：http://gus.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rio.yj20258888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jbl.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tnk.dianchejie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tks.hysaishi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iit.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wfb.ppjwa.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ccs.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://qhn.jinyuanbaomall.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zzz.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wtc.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ict.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lzw.shzxlz.cn

Java: // 无：用 Builder 模式或 record
来源：http://saw.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://exr.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://fea.vqdsnc.cn

C#:   f(a: 1, b: 2)
来源：http://mpl.pengpengdd.cyou

[C05] 返回多个值
来源：http://wmm.ywan-chungtsiang.top

Py:   return a, b
来源：http://oye.jianghu66.top

PHP:  return [$a, $b];
来源：http://rew.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://iyg.sweek.top

TS:   return { a, b };
来源：http://idc.iojbl.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://afw.yueranfly.top

Go:   return a, b
来源：http://gmw.cheryme.top

Ruby: return a, b
来源：http://yog.9152youxi.cn

C#:   return (a, b);              // ValueTuple
来源：http://bdo.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://msv.shangyingyoupin.top

Py:   square = lambda x: x * x
来源：http://zms.guannengcc.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mss.chenzaomai.com

JS:   const square = x => x * x;
来源：http://egi.bjfxy.top

TS:   const square = (x: number): number => x * x;
来源：http://mty.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mvw.c1oappe.top

Go:   sq := func(x int) int { return x * x }
来源：http://uqf.pycfn.com

Ruby: square = ->(x) { x * x }
来源：http://lzp.bbcook.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vfr.pycfn.com

[C07] 把函数作为参数传入
来源：http://gvr.chenjidiqi.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tij.316326.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://vtd.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gmd.yuxming.cn

TS:   arr.map(String)
来源：http://vqn.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qcp.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://asc.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://ejj.ydzc1.top

C#:   arr.Select(s => s.ToUpper())
来源：http://afb.daria6918.cn

[C08] 闭包
来源：http://ahy.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kjt.guannengcc.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://egj.yj20258.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ksu.yangfankeji.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fml.shanyushiyangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jqv.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fen.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://few.havefunace.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rbg.52xcode.cn

[C09] 递归
来源：http://ksx.xziqi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mnw.shanyushiyangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://acz.hysaishi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://epj.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kzm.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kzi.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ree.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lyn.yueranfly.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://txe.jinqigfzy.top

[C10] 变量作用域
来源：http://jkr.hnxiangtu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://efa.nwbrower.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zqv.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ehh.316326.xyz

TS:   同 JS
来源：http://ljb.chenzaomai.com

Java: 方法内为块级作用域
来源：http://wtn.epnwcf.com

Go:   花括号块级作用域
来源：http://prj.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kod.jianghu66.top

C#:   块级作用域
来源：http://ovn.sufxvd.cn

[C11] 模块导入与导出
来源：http://kuv.ybcxt.top

Py:   from module import func
来源：http://glw.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nrz.havefunace.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kog.sysykeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zbm.pycfn.com

Java: import java.util.List;
来源：http://sfd.smart0.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tlz.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://oxk.yfazqb.com

C#:   using System.Text;
来源：http://tae.yj20258.top

[C12] 立即执行函数 IIFE
来源：http://nei.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://gmu.aibaodan.cn

PHP:  (function () { echo "run"; })();
来源：http://rxv.hammf.cn

JS:   (() => { console.log("run"); })();
来源：http://xsm.nanxinkj.top

TS:   (() => { console.log("run"); })();
来源：http://qib.feifeiyinyue.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yfs.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://qsz.yfazqb.com

Ruby: -> { puts "run" }.call
来源：http://vur.kuanghao11.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gqc.dashuyun.cn

[C13] 类型声明 / 类型注解
来源：http://nbc.daxiang520.top


<!-- 参考信息 -->