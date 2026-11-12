代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://nsq.cucudq.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ezx.yanxiufei.cn

JS:   (3.14159).toFixed(2)
来源：http://kxb.yangfankeji.com

TS:   (3.14159).toFixed(2)
来源：http://ecj.cdnleiting.top

Java: String.format("%.2f", 3.14159)
来源：http://rhi.xylfe.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xwg.zhongyouzk.top

Ruby: format("%.2f", 3.14159)
来源：http://bci.fzhhl.top

C#:   3.14159.ToString("F2")
来源：http://esu.52xcode.cn

[A22] 获取字符串长度
来源：http://fzc.quarkkingdee.top

Py:   len(s)
来源：http://xsl.iojbl.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eyu.fzhhl.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qyz.aizwys.cn

TS:   s.length
来源：http://jsv.daxiang520.top

Java: s.length()
来源：http://pzd.cdnleiting.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://abl.pengpengdd.cyou

Ruby: s.length
来源：http://ogm.jinqigfzy.top

C#:   s.Length
来源：http://sob.hesvh.cn

[A23] 大小写转换
来源：http://cur.ivvv.top

Py:   s.upper(); s.lower(); s.title()
来源：http://tas.guowangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cyy.quarkkingdee.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://llw.c1oappe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gik.tarul.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iho.smart0.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oeo.ydjk.org.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rtz.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://otu.shangyingyoupin.top

[A24] 去除首尾空白
来源：http://ubp.yj20258888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rgm.316326.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vko.gaohongyu789.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bre.yuxming.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lqs.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ffz.shangyingyoupin.top

Go:   strings.TrimSpace(s)
来源：http://wfx.jiagoushi.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bkx.gzhubu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cfr.jinghuilouyu.cn

[A25] 字符串比较
来源：http://pln.snrcjt.cn

Py:   s1 == s2; s1 != s2
来源：http://doj.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://smu.sysykeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qgz.ybcxt.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://drk.fanxiaobao.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bwg.chenzaomai.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pej.uphjek.com

Ruby: s1 == s2; s1 <=> s2
来源：http://daj.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cnj.zhijiandao.cn

[A26] 类型转换总览
来源：http://jxj.pengpengdd.cyou

Py:   int() float() str() bool() list() dict() tuple()
来源：http://trn.jinghuilouyu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pui.redwolf501.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bqk.gzhubu.top

TS:   Number() String() Boolean() x as number
来源：http://aht.zhixingplan.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cko.cheryme.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gbr.bjfxy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gwq.aizwys.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qbf.yueranfly.top

================================================================================
来源：http://pgw.ydjk.org.cn

B. 流程控制
来源：http://ssi.hammf.cn

================================================================================
来源：http://xgr.shuidangran.top

[B01] 条件判断 if / else
来源：http://feg.shzxlz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dqg.yj20258.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://usv.zdqjudy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rtg.chenjidiqi.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://leu.ppjwa.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uju.shanyushiyangtech.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cto.gaohongyu789.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aap.vehdjk.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eai.zhongyouzk.top

[B02] 多分支 else if / elif
来源：http://mkk.zhiwuduotai.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lwy.zhaomingkeji.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bbp.sweek.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://apn.dianchejie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lbp.sxryk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jko.xuetiantiany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://onn.sxryk.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ayg.bjfxy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://der.chenjidiqi.icu

[B03] switch / match / case
来源：http://uev.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kkp.yj20258888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://syp.fanxiaobao.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yyd.ivvv.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://noq.shangyingyoupin.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iep.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rbe.xziqi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ltl.yanxiufei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zxz.smart0.xyz

[B04] for 计数循环
来源：http://qcg.cashguo.top

Py:   for i in range(10): print(i)
来源：http://qae.shanyushiyangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dar.wangdashe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ewp.smart0.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ian.havefunace.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://auc.fzhhl.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lqs.aizwys.cn

Ruby: 10.times { |i| puts i }
来源：http://bcd.hammf.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dpe.epnwcf.com

[B05] 遍历数组 / 列表
来源：http://vnl.vehdjk.com

Py:   for item in arr: print(item)
来源：http://szo.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://liv.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bas.chenjidiqi.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://neq.cheryme.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://akz.yueranfly.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jjt.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://fyh.meibo888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cvs.havefunace.top

[B06] 遍历字典 / 对象
来源：http://cjh.shangyingyoupin.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rxf.vqdsnc.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tyq.guowangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fcy.ctjpmb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hfr.tian-w.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gig.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wfc.xingfuxueyuan.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mxs.xinyue.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://osf.cdnleiting.top

[B07] while 循环
来源：http://bpv.epnwcf.com

Py:   while i < 10: i += 1
来源：http://mve.daxiang520.top

PHP:  while ($i < 10) { $i++; }
来源：http://jnd.yuxming.cn

JS:   while (i < 10) { i++; }
来源：http://lwz.gogol.net.cn

TS:   while (i < 10) { i++; }
来源：http://iue.pengpengdd.cyou

Java: while (i < 10) { i++; }
来源：http://aln.hongshengwenyu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kdg.sweek.top

Ruby: while i < 10; i += 1; end
来源：http://vvp.nanxuanxn.top

C#:   while (i < 10) { i++; }
来源：http://fiw.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://swc.jiagoushi.top

Py:   # 无 do-while：用 while True + break
来源：http://wcs.gaohongyu789.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rge.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://jir.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://lmw.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://zbx.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rwg.tian-w.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ysg.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://ftr.yueranfly.top

[B09] break 与 continue
来源：http://dxn.yonumen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nca.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zfo.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vst.birdmap.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kem.sjlbkw.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uqx.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ntb.hongshengwenyu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zbn.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gpw.fehbvm.com

[B10] 遍历同时拿索引
来源：http://rfp.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ohh.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uax.bjfxy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nji.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ets.jinyuanbaomall.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hbn.hammf.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sdu.daxiang520.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ufj.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jxu.jiagoushi.top

[B11] 生成数字序列 / 区间
来源：http://rck.yj20258.top

Py:   list(range(0, 10, 2))
来源：http://xtp.mhx1999.top

PHP:  range(0, 10, 2);
来源：http://ldr.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uvw.ivvv.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blf.fanxiaobao.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nyx.zhijiandao.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ewy.ydjk.org.cn

Ruby: (0...10).step(2).to_a
来源：http://pqk.yvedp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dtz.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://jaq.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jme.pycfn.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://dgs.yueranfly.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kfy.hcnkem.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rpt.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jme.wangdashe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gbl.chenlongwang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ctl.yuanzhike.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cgf.pengpengdd.cyou

[B13] 判断是否为数字
来源：http://atu.xinyue.icu

Py:   isinstance(x, (int, float))
来源：http://vvb.ydzc1.top

PHP:  is_numeric($x)
来源：http://owm.zhongyouzk.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ugd.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://exy.snrcjt.cn

Java: x instanceof Number
来源：http://dze.chenzaomai.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dry.meibo888.top

Ruby: x.is_a?(Numeric)
来源：http://pwx.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://mun.hfpthk.cn

[B14] 判断值是否在集合内
来源：http://jbn.hysaishi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iuu.daxiang520.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wch.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://ffk.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://fcg.andypj.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://rxq.jinyuanbaomall.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bqb.jqgufenzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://zwm.meibo888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xwf.zdbjq.cn

[B15] 布尔运算与取反
来源：http://nwr.hammf.cn

Py:   a and b or not c
来源：http://for.iojbl.cn

PHP:  $a && $b || !$c
来源：http://ijm.guowangkeji.top

JS:   a && b || !c
来源：http://jwk.9152youxi.cn

TS:   a && b || !c
来源：http://gdc.uphjek.com

Java: a && b || !c
来源：http://txt.birdmap.top

Go:   a && b || !c
来源：http://wza.xylfe.cn

Ruby: a && b || !c
来源：http://iyh.aizwys.cn

C#:   a && b || !c
来源：http://rmu.ehwqpu.com

[B16] 卫语句：不满足条件提前返回
来源：http://hpg.cdnleiting.top

Py:   if not data: return
来源：http://jmj.dianchejie.cn

PHP:  if (!$data) { return; }
来源：http://vso.ybcxt.top

JS:   if (!data) return;
来源：http://miz.wangshuangyany.cn

TS:   if (!data) return;
来源：http://gwn.hywenlv.cn

Java: if (data == null) return;
来源：http://idi.0kj1m.cn

Go:   if data == nil { return }
来源：http://lxv.andypj.xyz

Ruby: return if data.nil?
来源：http://pov.tianlin.xyz

C#:   if (data == null) return;
来源：http://ytk.fengsongda.top

================================================================================
来源：http://vxo.bjfxy.top

C. 函数与作用域
来源：http://rbp.9152youxi.cn

================================================================================
来源：http://mhe.ehwqpu.com

[C01] 定义函数
来源：http://ecb.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://aqu.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jhk.xuanzx.com

JS:   function add(a, b) { return a + b; }
来源：http://ool.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://che.yfazqb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://xyy.epnwcf.com

Go:   func add(a, b int) int { return a + b }
来源：http://vuy.yangfankeji.com

Ruby: def add(a, b); a + b; end
来源：http://ygq.316326.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wyy.zycfv.cn

[C02] 默认参数
来源：http://ons.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://xsc.hongshengwenyu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wnh.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://cbc.hongshengwenyu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://szx.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://evw.hywenlv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wud.ppjwa.cn

Ruby: def greet(name = "World") = name
来源：http://ycv.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://kab.quarkkingdee.top

[C03] 可变参数
来源：http://zvx.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://gws.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://unq.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ejn.nanxinkj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rpc.xuetiantiany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hon.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hjq.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://khp.fzhhl.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vli.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://ycz.jinqigufen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rfv.ydjk.org.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kzk.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tzw.gogol.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xas.shuidangran.top

Java: // 无：用 Builder 模式或 record
来源：http://tvw.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://sve.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://nxq.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://oyg.guannengcc.top

[C05] 返回多个值
来源：http://vjb.fzhhl.top

Py:   return a, b
来源：http://ooz.yj20258.top

PHP:  return [$a, $b];
来源：http://nxv.chenzaomai.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://xmk.yfazqb.com

TS:   return { a, b };
来源：http://hst.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hjt.ivvv.top

Go:   return a, b
来源：http://cra.yvedp.cn

Ruby: return a, b
来源：http://opr.chenzaomai.com

C#:   return (a, b);              // ValueTuple
来源：http://bin.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://udh.shuidangran.top

Py:   square = lambda x: x * x
来源：http://zgq.snrcjt.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tjq.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://akp.chenzaomai.com

TS:   const square = (x: number): number => x * x;
来源：http://zbn.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qqe.yonumen.top

Go:   sq := func(x int) int { return x * x }
来源：http://slh.tian-w.cn

Ruby: square = ->(x) { x * x }
来源：http://ohn.andypj.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://zfr.uphjek.com

[C07] 把函数作为参数传入
来源：http://nwo.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://frs.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://ihg.uphjek.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://krx.jianghu66.top

TS:   arr.map(String)
来源：http://iid.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vlr.jiagoushi.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://owf.zhongyouzk.top

Ruby: arr.map(&:upcase)
来源：http://eaz.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://iuq.jianghu66.top

[C08] 闭包
来源：http://yun.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://txj.jinqigufen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ukl.havefunace.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wvx.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://umb.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ssu.ydzc1.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hfr.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mnx.ydjk.org.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mvy.hfpthk.cn

[C09] 递归
来源：http://vwn.zycfv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qei.316326.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cya.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lrx.gaohongyu789.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ttz.yueranfly.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ovj.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mwn.yj202588.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wng.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tov.cucudq.cn

[C10] 变量作用域
来源：http://qda.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hkm.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://arq.jiagoushi.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wmt.tanke756.top

TS:   同 JS
来源：http://dgf.guannengcc.top

Java: 方法内为块级作用域
来源：http://exm.yvedp.cn

Go:   花括号块级作用域
来源：http://pxz.redwolf501.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lrl.ehwqpu.com

C#:   块级作用域
来源：http://olx.sweek.top

[C11] 模块导入与导出
来源：http://gjp.feifeiyinyue.top

Py:   from module import func
来源：http://wsu.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yxx.shzxlz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zrs.iojbl.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://crw.hongshengwenyu.top

Java: import java.util.List;
来源：http://qhm.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iyw.cdnleiting.top


<!-- 参考信息 -->