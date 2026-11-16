代发 wailian999

[A22] 获取字符串长度
来源：http://cto.xylfe.cn

Py:   len(s)
来源：http://fau.hywenlv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gtx.pycfn.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://iib.jqgfzy.top

TS:   s.length
来源：http://ifz.redwolf501.top

Java: s.length()
来源：http://lpj.mhx1999.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hsp.shuidangran.top

Ruby: s.length
来源：http://kgo.hfpthk.cn

C#:   s.Length
来源：http://hoa.jinqigufen.top

[A23] 大小写转换
来源：http://ybs.ydjk.org.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lxm.andypj.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ynd.ydzc1.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vdc.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wsr.ppjwa.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sja.yj20258.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://npo.fzhhl.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dtu.fanxiaobao.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://rhs.guannengcc.top

[A24] 去除首尾空白
来源：http://qez.aizwys.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yxf.snrcjt.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://abg.tian-w.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vfm.jlsjyb.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://omi.ppjwa.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tli.hnxiangtu.top

Go:   strings.TrimSpace(s)
来源：http://onz.xinyue.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://thc.yj20258888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ldp.epnwcf.com

[A25] 字符串比较
来源：http://scq.aibaodan.cn

Py:   s1 == s2; s1 != s2
来源：http://oao.jqgfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hbx.snrcjt.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mpb.ydjk.org.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hjx.xylfe.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tjy.hfpthk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://voh.ppjwa.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mil.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://adg.jinghuilouyu.cn

[A26] 类型转换总览
来源：http://flm.nanxuanxn.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jzq.jqgufenzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ecn.bbcook.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pkx.wangdashe.top

TS:   Number() String() Boolean() x as number
来源：http://tji.ctjpmb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fpp.gogol.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://onx.nanxuanxn.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://crz.nwbrower.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yai.hnqzz.top

================================================================================
来源：http://oem.hnqzz.top

B. 流程控制
来源：http://crq.andypj.xyz

================================================================================
来源：http://lwc.yanxiufei.cn

[B01] 条件判断 if / else
来源：http://ams.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://asn.sufxvd.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wxa.ybcxt.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zcl.zdbjq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bkt.kuanghao11.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ypr.daxiang520.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://thq.sxryk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dly.shangyingyoupin.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hma.sjlbkw.cn

[B02] 多分支 else if / elif
来源：http://znv.shanyushiyangtech.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vrm.fanxiaobao.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nmn.vehdjk.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xri.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rac.wangdashe.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://thh.daria6918.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://azk.tarul.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ayl.iojbl.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dht.52xcode.cn

[B03] switch / match / case
来源：http://hbd.xinyue.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vrd.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dyb.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ohj.svipenyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xxb.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://okt.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gww.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kxt.vqdsnc.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pxa.hywenlv.cn

[B04] for 计数循环
来源：http://liw.ybcxt.top

Py:   for i in range(10): print(i)
来源：http://ipw.yangfankeji.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dej.snrcjt.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://saj.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aqe.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nyd.zhijiandao.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hvv.wangshuangyany.cn

Ruby: 10.times { |i| puts i }
来源：http://agr.jinqigufen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vmk.epnwcf.com

[B05] 遍历数组 / 列表
来源：http://qlw.bbcook.cn

Py:   for item in arr: print(item)
来源：http://dxh.hysaishi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://apj.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wpo.yanxiufei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xey.cucudq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vqa.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nyq.yfazqb.com

Ruby: arr.each { |item| puts item }
来源：http://pkr.ctjpmb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rdb.smart0.xyz

[B06] 遍历字典 / 对象
来源：http://tzi.9152youxi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rbm.ppjwa.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rxh.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bte.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cih.cashguo.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://amd.gogol.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ojp.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lmx.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fen.zhongyouzk.top

[B07] while 循环
来源：http://ygt.guannengcc.top

Py:   while i < 10: i += 1
来源：http://ebs.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://kyi.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://gwi.hongshengwenyu.top

TS:   while (i < 10) { i++; }
来源：http://kre.9152youxi.cn

Java: while (i < 10) { i++; }
来源：http://zig.bbcook.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uza.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://fww.fktsv.cn

C#:   while (i < 10) { i++; }
来源：http://lcn.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://eob.feifeiyinyue.top

Py:   # 无 do-while：用 while True + break
来源：http://fld.yfazqb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://rix.daxiang520.top

JS:   do { i++; } while (i < 10);
来源：http://yvi.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://fbq.jyoumei.cn

Java: do { i++; } while (i < 10);
来源：http://jfz.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://usj.andypj.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://ott.mhx1999.top

C#:   do { i++; } while (i < 10);
来源：http://spl.zhongyouzk.top

[B09] break 与 continue
来源：http://aeu.shanyushiyangtech.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eoe.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rtf.jinyuanbaomall.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uow.nwbrower.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sbu.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tyr.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://foz.vqdsnc.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ugq.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bis.cashguo.top

[B10] 遍历同时拿索引
来源：http://sxg.yuanzhike.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ymz.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wxc.nwbrower.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ddw.shanyushiyangtech.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hap.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dfc.xingfuxueyuan.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tdv.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sqp.ppjwa.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://koo.sufxvd.cn

[B11] 生成数字序列 / 区间
来源：http://bid.xinyue.icu

Py:   list(range(0, 10, 2))
来源：http://pdw.chenjidiqi.icu

PHP:  range(0, 10, 2);
来源：http://jpt.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dnq.chenlongwang.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yeu.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eiy.jqgfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qbb.zhoulong.xyz

Ruby: (0...10).step(2).to_a
来源：http://ekg.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vbw.vqdsnc.cn

[B12] 跳出多层循环
来源：http://zea.aizwys.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bmz.xylfe.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nsa.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pij.hysaishi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://agx.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oan.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aom.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xps.yj20258.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://azk.aizwys.cn

[B13] 判断是否为数字
来源：http://ncd.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://pmm.epnwcf.com

PHP:  is_numeric($x)
来源：http://hxm.fktsv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hzk.hcnkem.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rlq.sxryk.cn

Java: x instanceof Number
来源：http://fgq.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cvg.ppjwa.cn

Ruby: x.is_a?(Numeric)
来源：http://qhd.sjlbkw.cn

C#:   x is int or double or decimal
来源：http://usc.xylfe.cn

[B14] 判断值是否在集合内
来源：http://uky.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zyu.yonumen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nld.yj20258888.top

JS:   [1, 2, 3].includes(x)
来源：http://moe.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://dci.yangfankeji.com

Java: List.of(1, 2, 3).contains(x)
来源：http://bjv.birdmap.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kcj.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://sla.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nut.hywenlv.cn

[B15] 布尔运算与取反
来源：http://tbw.0kj1m.cn

Py:   a and b or not c
来源：http://cuq.cashguo.top

PHP:  $a && $b || !$c
来源：http://pgy.feifeiyinyue.top

JS:   a && b || !c
来源：http://iyi.fktsv.cn

TS:   a && b || !c
来源：http://ioq.pycfn.com

Java: a && b || !c
来源：http://iqm.jinghuilouyu.cn

Go:   a && b || !c
来源：http://beb.zdqjudy.top

Ruby: a && b || !c
来源：http://sqc.tian-w.cn

C#:   a && b || !c
来源：http://rqd.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://nve.birdmap.top

Py:   if not data: return
来源：http://clz.pycfn.com

PHP:  if (!$data) { return; }
来源：http://zkn.ppjwa.cn

JS:   if (!data) return;
来源：http://lcb.yangfankeji.com

TS:   if (!data) return;
来源：http://myz.zdqjudy.top

Java: if (data == null) return;
来源：http://bmc.pengpengdd.cyou

Go:   if data == nil { return }
来源：http://qvz.zhijiandao.cn

Ruby: return if data.nil?
来源：http://ixb.smart0.xyz

C#:   if (data == null) return;
来源：http://vpp.zdbjq.cn

================================================================================
来源：http://ozz.yonumen.top

C. 函数与作用域
来源：http://wlr.xingfuxueyuan.xyz

================================================================================
来源：http://dje.yvedp.cn

[C01] 定义函数
来源：http://nra.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://pmi.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ndf.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://gmq.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fle.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hag.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gxc.fzhhl.top

Ruby: def add(a, b); a + b; end
来源：http://mew.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ois.vehdjk.com

[C02] 默认参数
来源：http://hsc.sufxvd.cn

Py:   def greet(name="World"): return name
来源：http://opj.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xtr.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://kor.jqgufenzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://oiz.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://aws.guannengcc.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://agv.hfpthk.cn

Ruby: def greet(name = "World") = name
来源：http://uvx.birdmap.top

C#:   string Greet(string name = "World") => name;
来源：http://sfi.shuidangran.top

[C03] 可变参数
来源：http://stt.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://qkg.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hrx.cdnleiting.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://coy.nanxinkj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://obq.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mth.tarul.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://irz.haohaochexian.top

Ruby: def total(*nums); nums.sum; end
来源：http://zsz.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fch.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://jlr.feifeiyinyue.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yxt.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aoj.cucudq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://roq.ppjwa.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qtv.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://lfr.ivvv.top

Go:   // 无：用配置结构体参数
来源：http://qhc.316326.xyz

Ruby: f(a: 1, b: 2)
来源：http://mmf.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://xau.aibaodan.cn

[C05] 返回多个值
来源：http://tyz.yvedp.cn

Py:   return a, b
来源：http://pen.svipenyu.cn

PHP:  return [$a, $b];
来源：http://xfq.pycfn.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://gse.bjfxy.top

TS:   return { a, b };
来源：http://kox.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fuk.xziqi.cn

Go:   return a, b
来源：http://nct.xylfe.cn

Ruby: return a, b
来源：http://qvz.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://haf.havefunace.top

[C06] 匿名函数 / lambda
来源：http://cyz.yueranfly.top

Py:   square = lambda x: x * x
来源：http://srh.316326.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://qxx.ivvv.top

JS:   const square = x => x * x;
来源：http://ikh.bjfxy.top

TS:   const square = (x: number): number => x * x;
来源：http://eys.guowangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ikf.jianghu66.top

Go:   sq := func(x int) int { return x * x }
来源：http://xwd.316326.xyz

Ruby: square = ->(x) { x * x }
来源：http://duq.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://xoe.zhongyouzk.top

[C07] 把函数作为参数传入
来源：http://kkd.yj20258.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gtd.316326.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://fzf.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ksw.bjfxy.top

TS:   arr.map(String)
来源：http://ifu.sysykeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yqz.fktsv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://exp.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://onz.redwolf501.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ptk.cdnleiting.top

[C08] 闭包
来源：http://bli.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://coz.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dxl.zhengqikj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qjn.havefunace.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eku.yueranfly.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bpw.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nzk.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fcu.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://krb.zycfv.cn

[C09] 递归
来源：http://pfr.hnqzz.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ysg.yonumen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iyc.smart0.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iqi.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mhx.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hpl.yongpay.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xwe.mhx1999.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://igi.gaohongyu789.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wzk.xingfuxueyuan.xyz

[C10] 变量作用域
来源：http://inl.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dkf.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hlp.tianlin.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lvy.haohaochexian.top

TS:   同 JS
来源：http://vag.ehwqpu.com

Java: 方法内为块级作用域
来源：http://txe.zhijiandao.cn

Go:   花括号块级作用域
来源：http://lkr.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sdb.bjfxy.top

C#:   块级作用域
来源：http://oxe.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://uvu.yfazqb.com

Py:   from module import func
来源：http://ymr.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://dib.redwolf501.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pun.shzxlz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jdp.birdmap.top

Java: import java.util.List;
来源：http://fiy.zhoulong.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jxu.gzhubu.top

Ruby: require "json"; require_relative "./util"
来源：http://mfq.yuxming.cn

C#:   using System.Text;
来源：http://ddv.nanxinkj.top

[C12] 立即执行函数 IIFE
来源：http://gdk.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://aej.yj20258.top

PHP:  (function () { echo "run"; })();
来源：http://zht.yuanzhike.top

JS:   (() => { console.log("run"); })();
来源：http://wsg.jinghuilouyu.cn

TS:   (() => { console.log("run"); })();
来源：http://dme.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pyi.cheryme.top


<!-- 参考信息 -->