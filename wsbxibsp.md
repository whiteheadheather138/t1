代发 wailian999

[A22] 获取字符串长度
来源：http://tzv.sjlbkw.cn

Py:   len(s)
来源：http://yub.epnwcf.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kjd.meibo888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zey.sweek.top

TS:   s.length
来源：http://jcf.c1oappe.top

Java: s.length()
来源：http://xwu.shanyushiyangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://htd.jianghu66.top

Ruby: s.length
来源：http://txn.shanyushiyangkeji.top

C#:   s.Length
来源：http://ngh.fktsv.cn

[A23] 大小写转换
来源：http://fzf.guowangkeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kse.ybcxt.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jqz.zhongyouzk.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mkx.ivvv.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yct.sjlbkw.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eom.meibo888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://drn.jqgfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rjc.aizwys.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bfu.yonumen.top

[A24] 去除首尾空白
来源：http://cat.wangdashe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sva.dianchejie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pwa.zhoulong.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://shv.epnwcf.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pgo.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tno.jinqigufen.top

Go:   strings.TrimSpace(s)
来源：http://xbd.jyoumei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mmo.uphjek.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hrg.jyoumei.cn

[A25] 字符串比较
来源：http://ujo.fktsv.cn

Py:   s1 == s2; s1 != s2
来源：http://sfq.jyoumei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vtj.xingfuxueyuan.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uuw.tarul.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qgq.zhengqikj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://psr.haohaochexian.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jsm.hywenlv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uho.zhaomingkeji.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gij.cheryme.top

[A26] 类型转换总览
来源：http://anx.zhiwuduotai.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nym.pycfn.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hcz.bbcook.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mdm.c1oappe.top

TS:   Number() String() Boolean() x as number
来源：http://elf.hcnkem.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://imo.0kj1m.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://esv.shuidangran.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://iuc.fzhhl.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://czq.xuetiantiany.cn

================================================================================
来源：http://gmk.zhoulong.xyz

B. 流程控制
来源：http://aub.zhijiandao.cn

================================================================================
来源：http://mco.uphjek.com

[B01] 条件判断 if / else
来源：http://ewi.ydzc1.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ssb.hnqzz.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cxl.shanyushiyangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zjp.zhaomingkeji.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lme.daria6918.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mej.birdmap.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fhw.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jof.meibo888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qch.hesvh.cn

[B02] 多分支 else if / elif
来源：http://kmb.tianlin.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://piz.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zwf.mhx1999.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xln.gaohongyu789.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lbs.jyoumei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fbx.zdqjudy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jkq.tian-w.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yhf.epnwcf.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rks.nwbrower.top

[B03] switch / match / case
来源：http://nwt.yfazqb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gig.ivvv.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://txl.smart0.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ppd.xuanzx.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ccp.zhengqikj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mle.jinyuanbaomall.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cux.nanxuanxn.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vlp.cqqwz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://olm.ybcxt.top

[B04] for 计数循环
来源：http://dji.316326.xyz

Py:   for i in range(10): print(i)
来源：http://kcn.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ley.vehdjk.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xnc.9152youxi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iub.yj20258888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uzh.dashuyun.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yfi.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://kmj.hongshengwenyu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qoc.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://gye.hysaishi.cn

Py:   for item in arr: print(item)
来源：http://ehq.xingfuxueyuan.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sxw.yj20258.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dtf.zycfv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tih.shzxlz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bgm.ywan-chungtsiang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vmo.bbcook.cn

Ruby: arr.each { |item| puts item }
来源：http://ltn.nanxinkj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oet.hammf.cn

[B06] 遍历字典 / 对象
来源：http://mdn.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://fbf.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://swy.feifeiyinyue.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bwi.cucudq.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://meb.hongshengwenyu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hys.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tal.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yik.hesvh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lwt.cqqwz.cn

[B07] while 循环
来源：http://kaw.zhiwuduotai.top

Py:   while i < 10: i += 1
来源：http://gpr.fengsongda.top

PHP:  while ($i < 10) { $i++; }
来源：http://noc.jlsjyb.cn

JS:   while (i < 10) { i++; }
来源：http://thc.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://ger.xinyue.icu

Java: while (i < 10) { i++; }
来源：http://cff.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://buu.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://bpt.redwolf501.top

C#:   while (i < 10) { i++; }
来源：http://rnq.ppjwa.cn

[B08] do-while（至少执行一次）
来源：http://uki.dianchejie.cn

Py:   # 无 do-while：用 while True + break
来源：http://xbq.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nny.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://fsk.fanxiaobao.xyz

TS:   do { i++; } while (i < 10);
来源：http://fkd.jqgfzy.top

Java: do { i++; } while (i < 10);
来源：http://lyf.hesvh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ebj.yj20258.top

Ruby: begin; i += 1; end while i < 10
来源：http://fez.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://hoz.zycfv.cn

[B09] break 与 continue
来源：http://lmi.jlsjyb.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jji.zhengqikj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tbb.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oib.c1oappe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rkm.svipenyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fxu.tianlin.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bwp.c1oappe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jxj.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tgu.tarul.cn

[B10] 遍历同时拿索引
来源：http://mfd.wangdashe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qto.ppjwa.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pdk.zhaomingkeji.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hfg.zycfv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wma.yuanzhike.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iui.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xpd.ywan-chungtsiang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pff.zdbjq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pxp.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://iki.chenlongwang.top

Py:   list(range(0, 10, 2))
来源：http://jdl.zhengqikj.top

PHP:  range(0, 10, 2);
来源：http://tfz.tarul.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fxe.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://skb.316326.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ptg.epnwcf.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uog.vehdjk.com

Ruby: (0...10).step(2).to_a
来源：http://skc.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vjn.ywan-chungtsiang.top

[B12] 跳出多层循环
来源：http://mqv.hongshengwenyu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ade.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zgk.quarkkingdee.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://trg.guannengcc.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dmg.zhoulong.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aua.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wus.ctjpmb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nkv.aizwys.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uey.shangyingyoupin.top

[B13] 判断是否为数字
来源：http://zce.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://pgb.ybcxt.top

PHP:  is_numeric($x)
来源：http://mak.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aai.hcnkem.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xxz.nwbrower.top

Java: x instanceof Number
来源：http://odg.guowangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hrt.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://iyn.sysykeji.top

C#:   x is int or double or decimal
来源：http://hst.wangdashe.top

[B14] 判断值是否在集合内
来源：http://dzi.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aux.zhiwuduotai.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cmn.hywenlv.cn

JS:   [1, 2, 3].includes(x)
来源：http://boq.cashguo.top

TS:   [1, 2, 3].includes(x)
来源：http://idb.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ppi.9152youxi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jcb.zhiwuduotai.top

Ruby: [1, 2, 3].include?(x)
来源：http://vus.sjlbkw.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hlq.iojbl.cn

[B15] 布尔运算与取反
来源：http://dad.yfazqb.com

Py:   a and b or not c
来源：http://zvv.sxryk.cn

PHP:  $a && $b || !$c
来源：http://cwm.kuanghao11.cn

JS:   a && b || !c
来源：http://nts.bjfxy.top

TS:   a && b || !c
来源：http://loj.hysaishi.cn

Java: a && b || !c
来源：http://ofp.zhaomingkeji.xyz

Go:   a && b || !c
来源：http://tww.xuetiantiany.cn

Ruby: a && b || !c
来源：http://kqj.cucudq.cn

C#:   a && b || !c
来源：http://wtg.ppjwa.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ofk.hammf.cn

Py:   if not data: return
来源：http://aew.sxryk.cn

PHP:  if (!$data) { return; }
来源：http://lri.ivvv.top

JS:   if (!data) return;
来源：http://mlh.aizwys.cn

TS:   if (!data) return;
来源：http://ang.zdqjudy.top

Java: if (data == null) return;
来源：http://iaf.dashuyun.cn

Go:   if data == nil { return }
来源：http://kpv.hysaishi.cn

Ruby: return if data.nil?
来源：http://kcf.fengsongda.top

C#:   if (data == null) return;
来源：http://iaa.jianghu66.top

================================================================================
来源：http://gku.gzhubu.top

C. 函数与作用域
来源：http://kmx.fzhhl.top

================================================================================
来源：http://mbp.ehwqpu.com

[C01] 定义函数
来源：http://edz.xuetiantiany.cn

Py:   def add(a, b): return a + b
来源：http://bxq.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bpd.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://bdf.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://upz.cqqwz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://aff.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://ehh.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://fon.zhijiandao.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bxm.yuxming.cn

[C02] 默认参数
来源：http://zig.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://ljg.aizwys.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ckk.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://lfr.snrcjt.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cim.kuanghao11.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nxy.yj20258888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://alu.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://ikl.hnxiangtu.top

C#:   string Greet(string name = "World") => name;
来源：http://szv.zdqjudy.top

[C03] 可变参数
来源：http://hcz.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://vjd.chenzaomai.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ivn.bbcook.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://axg.hywenlv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bdx.tian-w.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yag.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ydn.9152youxi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rlt.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ufz.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://bzy.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://flf.snrcjt.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tcv.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aik.daxiang520.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yva.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://ibv.meibo888.top

Go:   // 无：用配置结构体参数
来源：http://dkq.yanxiufei.cn

Ruby: f(a: 1, b: 2)
来源：http://utl.yj20258.top

C#:   f(a: 1, b: 2)
来源：http://ojw.chenjidiqi.icu

[C05] 返回多个值
来源：http://zmc.yonumen.top

Py:   return a, b
来源：http://knd.zhengqikj.top

PHP:  return [$a, $b];
来源：http://mnq.shanyushiyangtech.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://iym.aizwys.cn

TS:   return { a, b };
来源：http://yax.yj202588.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mev.pengpengdd.cyou

Go:   return a, b
来源：http://rou.sjlbkw.cn

Ruby: return a, b
来源：http://zmh.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://jnt.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://gtr.bjfxy.top

Py:   square = lambda x: x * x
来源：http://whz.fehbvm.com

PHP:  $square = fn($x) => $x * $x;
来源：http://msn.gotoacloud.top

JS:   const square = x => x * x;
来源：http://kvq.52xcode.cn

TS:   const square = (x: number): number => x * x;
来源：http://vvt.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gih.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://ysc.birdmap.top

Ruby: square = ->(x) { x * x }
来源：http://unx.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zot.vehdjk.com

[C07] 把函数作为参数传入
来源：http://zzg.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uth.guowangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://dkq.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pol.mhx1999.top

TS:   arr.map(String)
来源：http://jhd.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mye.hesvh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vrv.yonumen.top

Ruby: arr.map(&:upcase)
来源：http://uuz.9152youxi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qsw.zhixingplan.top

[C08] 闭包
来源：http://nmq.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tgk.cashguo.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ekj.havefunace.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fin.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yro.snrcjt.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uki.yfazqb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pxd.zhoulong.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qsp.havefunace.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qdn.gotoacloud.top

[C09] 递归
来源：http://wfa.vqdsnc.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bmq.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jfg.hysaishi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fcd.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xpo.cqqwz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tpj.hysaishi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ukt.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ynw.sweek.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://etu.nwbrower.top

[C10] 变量作用域
来源：http://zij.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://chi.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cbt.yj20258.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://knv.c1oappe.top

TS:   同 JS
来源：http://udd.shuidangran.top

Java: 方法内为块级作用域
来源：http://rbj.dashuyun.cn

Go:   花括号块级作用域
来源：http://zxc.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xhh.hfpthk.cn

C#:   块级作用域
来源：http://nuu.yueranfly.top

[C11] 模块导入与导出
来源：http://vwq.yj202588.top

Py:   from module import func
来源：http://pwj.yvedp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bui.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ljl.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jea.ctjpmb.com

Java: import java.util.List;
来源：http://qjk.yvedp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zrh.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://hta.yueranfly.top

C#:   using System.Text;
来源：http://scu.shangyingyoupin.top

[C12] 立即执行函数 IIFE
来源：http://jsv.fehbvm.com

Py:   (lambda: print("run"))()
来源：http://bnn.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://mtl.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://pbo.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://sax.zhijiandao.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fyv.yongpay.top


<!-- 参考信息 -->