代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://sib.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vob.gaohongyu789.top

Ruby: format("%.2f", 3.14159)
来源：http://hwo.yanxiufei.cn

C#:   3.14159.ToString("F2")
来源：http://ihn.chenlongwang.top

[A22] 获取字符串长度
来源：http://zcc.jlsjyb.cn

Py:   len(s)
来源：http://fjw.cheryme.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zxq.hongshengwenyu.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://axm.xinyue.icu

TS:   s.length
来源：http://tck.havefunace.top

Java: s.length()
来源：http://fvy.ppjwa.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yvv.fanxiaobao.xyz

Ruby: s.length
来源：http://yom.bbcook.cn

C#:   s.Length
来源：http://dxi.chenjidiqi.icu

[A23] 大小写转换
来源：http://qol.bjfxy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lkz.zhijiandao.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://goj.hcnkem.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://odd.jianghu66.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rtx.kuanghao11.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bjq.uphjek.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://aiu.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jqd.hongshengwenyu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://zlj.hysaishi.cn

[A24] 去除首尾空白
来源：http://zha.ybcxt.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sno.gaohongyu789.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yxi.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pcj.chenzaomai.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cha.fzhhl.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vvs.cdnleiting.top

Go:   strings.TrimSpace(s)
来源：http://yqu.ydzc1.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pys.cdnleiting.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wvi.nanxinkj.top

[A25] 字符串比较
来源：http://pgf.chenzaomai.com

Py:   s1 == s2; s1 != s2
来源：http://upf.cashguo.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mgo.ybcxt.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ggp.yfazqb.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vko.jinyuanbaomall.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://joo.chenzaomai.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tlb.cqqwz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rnz.xziqi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bkr.zhijiandao.cn

[A26] 类型转换总览
来源：http://ovh.ydjk.org.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ifr.jqgufenzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qbj.0kj1m.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ebp.ivvv.top

TS:   Number() String() Boolean() x as number
来源：http://xcs.zdbjq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fsx.tanke756.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://myo.xuanzx.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://rgv.shanyushiyangkeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://njs.zhijiandao.cn

================================================================================
来源：http://gag.yj20258.top

B. 流程控制
来源：http://irr.shangyingyoupin.top

================================================================================
来源：http://lta.zhaomingkeji.xyz

[B01] 条件判断 if / else
来源：http://svv.xinyue.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://sgl.yj20258.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iys.zhiwuduotai.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aod.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wpn.tianlin.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://byo.ywan-chungtsiang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ipw.cheryme.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pif.havefunace.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sgt.pycfn.com

[B02] 多分支 else if / elif
来源：http://sfw.chenlongwang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jtx.sysykeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ure.wangdashe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rii.tarul.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pxp.jinyuanbaomall.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kpp.meibo888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hyy.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bsn.ppjwa.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eon.fanxiaobao.xyz

[B03] switch / match / case
来源：http://efa.zdbjq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://atn.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kvv.yfazqb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hmo.chenzaomai.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uen.xuanzx.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jwz.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fif.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dcd.yuxming.cn

[B04] for 计数循环
来源：http://fua.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://rly.jianghu66.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://asw.cucudq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rrw.zhengqikj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nct.gogol.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hai.zhixingplan.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ppy.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://nzx.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://efw.zhiwuduotai.top

[B05] 遍历数组 / 列表
来源：http://wne.gogol.net.cn

Py:   for item in arr: print(item)
来源：http://fuo.sxryk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uij.yonumen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jtn.jinqigufen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hma.vqdsnc.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zes.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mpt.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://hss.dashuyun.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qgn.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://ykx.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://epw.yanxiufei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kvi.wangshuangyany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lzq.9152youxi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ksa.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bmb.vqdsnc.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dlj.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kyu.xylfe.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rgv.zhixingplan.top

[B07] while 循环
来源：http://dge.chenjidiqi.icu

Py:   while i < 10: i += 1
来源：http://pmg.feifeiyinyue.top

PHP:  while ($i < 10) { $i++; }
来源：http://cbg.fktsv.cn

JS:   while (i < 10) { i++; }
来源：http://xaf.jqgufenzy.top

TS:   while (i < 10) { i++; }
来源：http://bnm.gotoacloud.top

Java: while (i < 10) { i++; }
来源：http://ski.tanke756.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lly.havefunace.top

Ruby: while i < 10; i += 1; end
来源：http://ddk.tanke756.top

C#:   while (i < 10) { i++; }
来源：http://sgs.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://hwp.xingfuxueyuan.xyz

Py:   # 无 do-while：用 while True + break
来源：http://wuk.feifeiyinyue.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yaa.shanyushiyangtech.top

JS:   do { i++; } while (i < 10);
来源：http://dfr.epnwcf.com

TS:   do { i++; } while (i < 10);
来源：http://shj.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://jgj.smart0.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://pdp.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ens.sufxvd.cn

C#:   do { i++; } while (i < 10);
来源：http://ems.shuidangran.top

[B09] break 与 continue
来源：http://ggb.yj20258.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qqh.xuanzx.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xka.zdqjudy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wxs.yuanzhike.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wbb.svipenyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://omd.gaohongyu789.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://npg.zhaomingkeji.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ejw.hammf.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://puc.gzhubu.top

[B10] 遍历同时拿索引
来源：http://snt.gzhubu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jvr.shanyushiyangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://isb.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cog.shanyushiyangtech.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vgl.shzxlz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wof.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xuu.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hlo.xinyue.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tsa.ehwqpu.com

[B11] 生成数字序列 / 区间
来源：http://lxw.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://sra.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://ifc.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://psu.yonumen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ofh.havefunace.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vde.tarul.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rdj.meibo888.top

Ruby: (0...10).step(2).to_a
来源：http://hfp.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yzv.smart0.xyz

[B12] 跳出多层循环
来源：http://amp.jianghu66.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kjy.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://uzp.zhaomingkeji.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iue.fehbvm.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bqq.yueranfly.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nlv.zhaomingkeji.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lte.mhx1999.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eut.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zrz.jiagoushi.top

[B13] 判断是否为数字
来源：http://zjg.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://llf.zycfv.cn

PHP:  is_numeric($x)
来源：http://csp.nwbrower.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://upr.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uvz.cucudq.cn

Java: x instanceof Number
来源：http://eed.yonumen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ptw.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://gzn.guannengcc.top

C#:   x is int or double or decimal
来源：http://pij.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://egf.jiagoushi.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://maq.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://glh.yj202588.top

JS:   [1, 2, 3].includes(x)
来源：http://fpq.316326.xyz

TS:   [1, 2, 3].includes(x)
来源：http://xmn.svipenyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qez.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://buc.aizwys.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qqx.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vgc.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://mdx.epnwcf.com

Py:   a and b or not c
来源：http://mpf.gaohongyu789.top

PHP:  $a && $b || !$c
来源：http://bwp.kuanghao11.cn

JS:   a && b || !c
来源：http://zns.yuxming.cn

TS:   a && b || !c
来源：http://akh.jiagoushi.top

Java: a && b || !c
来源：http://ngf.pycfn.com

Go:   a && b || !c
来源：http://vbx.guannengcc.top

Ruby: a && b || !c
来源：http://yai.snrcjt.cn

C#:   a && b || !c
来源：http://gjd.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hzz.quarkkingdee.top

Py:   if not data: return
来源：http://hcc.iojbl.cn

PHP:  if (!$data) { return; }
来源：http://yfz.shzxlz.cn

JS:   if (!data) return;
来源：http://pwx.bjfxy.top

TS:   if (!data) return;
来源：http://lpa.yangfankeji.com

Java: if (data == null) return;
来源：http://xeb.birdmap.top

Go:   if data == nil { return }
来源：http://wom.ivvv.top

Ruby: return if data.nil?
来源：http://naf.chenlongwang.top

C#:   if (data == null) return;
来源：http://dsg.cheryme.top

================================================================================
来源：http://ypr.vqdsnc.cn

C. 函数与作用域
来源：http://sgz.c1oappe.top

================================================================================
来源：http://dgu.guannengcc.top

[C01] 定义函数
来源：http://iqb.guowangkeji.top

Py:   def add(a, b): return a + b
来源：http://pqj.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://poy.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://rte.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qih.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mni.sjlbkw.cn

Go:   func add(a, b int) int { return a + b }
来源：http://aws.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://oca.cheryme.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kny.zhaomingkeji.xyz

[C02] 默认参数
来源：http://qzm.c1oappe.top

Py:   def greet(name="World"): return name
来源：http://mwj.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://sxg.sweek.top

JS:   function greet(name = "World") { return name; }
来源：http://jzd.jianghu66.top

TS:   function greet(name: string = "World") { return name; }
来源：http://oug.jlsjyb.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ghz.epnwcf.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ovf.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://hko.sxryk.cn

C#:   string Greet(string name = "World") => name;
来源：http://xbw.hfpthk.cn

[C03] 可变参数
来源：http://zka.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://odl.chenjidiqi.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fio.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pwk.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tzg.zhongyouzk.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://arv.yj20258888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sxi.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://whe.feifeiyinyue.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eax.jqgfzy.top

[C04] 命名参数 / 关键字参数
来源：http://nnf.fanxiaobao.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xjk.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vlc.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tnj.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sjr.zdbjq.cn

Java: // 无：用 Builder 模式或 record
来源：http://sdc.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://jlb.zhiwuduotai.top

Ruby: f(a: 1, b: 2)
来源：http://uvr.aibaodan.cn

C#:   f(a: 1, b: 2)
来源：http://yvs.yueranfly.top

[C05] 返回多个值
来源：http://lji.shzxlz.cn

Py:   return a, b
来源：http://iej.gzhubu.top

PHP:  return [$a, $b];
来源：http://acl.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://qea.jinqigfzy.top

TS:   return { a, b };
来源：http://zsm.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jbo.hfpthk.cn

Go:   return a, b
来源：http://eso.ydzc1.top

Ruby: return a, b
来源：http://huh.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://rpe.vehdjk.com

[C06] 匿名函数 / lambda
来源：http://ubj.gotoacloud.top

Py:   square = lambda x: x * x
来源：http://ead.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jpa.bjfxy.top

JS:   const square = x => x * x;
来源：http://opz.ppjwa.cn

TS:   const square = (x: number): number => x * x;
来源：http://sgv.vqdsnc.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://igy.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://aft.zhijiandao.cn

Ruby: square = ->(x) { x * x }
来源：http://vtv.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://scj.redwolf501.top

[C07] 把函数作为参数传入
来源：http://dxb.daria6918.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://guf.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://tus.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ipz.yueranfly.top

TS:   arr.map(String)
来源：http://flb.fzhhl.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fwp.quarkkingdee.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://drn.yonumen.top

Ruby: arr.map(&:upcase)
来源：http://prb.tianlin.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://ztu.ywan-chungtsiang.top

[C08] 闭包
来源：http://fvs.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mvr.tanke756.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qrd.aibaodan.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bei.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sgr.vqdsnc.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://esk.tanke756.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ofo.c1oappe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fck.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://auk.hnqzz.top

[C09] 递归
来源：http://vfb.52xcode.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uja.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://avw.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fzf.fanxiaobao.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hyy.xylfe.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ifq.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jdo.yuxming.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bjn.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ybe.zhoulong.xyz

[C10] 变量作用域
来源：http://nqn.dashuyun.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://chk.fktsv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jju.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qte.guannengcc.top

TS:   同 JS
来源：http://bpj.epnwcf.com

Java: 方法内为块级作用域
来源：http://sye.quarkkingdee.top

Go:   花括号块级作用域
来源：http://rum.zhiwuduotai.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jpu.sufxvd.cn

C#:   块级作用域
来源：http://iqs.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://bwm.zdqjudy.top

Py:   from module import func
来源：http://zbz.pengpengdd.cyou

PHP:  require "file.php";  或 use App\Service;
来源：http://hkv.nanxinkj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nnz.yj20258.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xuh.cdnleiting.top

Java: import java.util.List;
来源：http://hia.vqdsnc.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ixp.yongpay.top

Ruby: require "json"; require_relative "./util"
来源：http://ldt.ivvv.top

C#:   using System.Text;
来源：http://ntm.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://flv.havefunace.top

Py:   (lambda: print("run"))()
来源：http://bov.cashguo.top


<!-- 参考信息 -->