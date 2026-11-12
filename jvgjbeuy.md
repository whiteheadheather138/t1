代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://yhn.gzhubu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bdk.0kj1m.cn

Ruby: format("%.2f", 3.14159)
来源：http://qzm.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://nhw.xuetiantiany.cn

[A22] 获取字符串长度
来源：http://ukb.zhaomingkeji.xyz

Py:   len(s)
来源：http://vsp.jinghuilouyu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rpl.jiagoushi.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qwt.316326.xyz

TS:   s.length
来源：http://ilq.xylfe.cn

Java: s.length()
来源：http://zlw.dashuyun.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xzs.cucudq.cn

Ruby: s.length
来源：http://xww.hnqzz.top

C#:   s.Length
来源：http://klv.quarkkingdee.top

[A23] 大小写转换
来源：http://yfz.zhiwuduotai.top

Py:   s.upper(); s.lower(); s.title()
来源：http://han.mhx1999.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://umy.ywan-chungtsiang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wff.hnqzz.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kiw.haohaochexian.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://awt.guannengcc.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hvc.jinghuilouyu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pxo.hnxiangtu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kmw.fzhhl.top

[A24] 去除首尾空白
来源：http://lxj.shanyushiyangtech.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cia.nanxinkj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wum.snrcjt.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fdy.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aob.ydzc1.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jpb.daria6918.cn

Go:   strings.TrimSpace(s)
来源：http://vvl.cdnleiting.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uzp.nwbrower.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zpz.shangyingyoupin.top

[A25] 字符串比较
来源：http://ogy.ppjwa.cn

Py:   s1 == s2; s1 != s2
来源：http://xot.gzhubu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jty.yfazqb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hly.chenzaomai.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pok.jinyuanbaomall.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://boj.hfpthk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ins.gotoacloud.top

Ruby: s1 == s2; s1 <=> s2
来源：http://exy.zhengqikj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qtq.hnqzz.top

[A26] 类型转换总览
来源：http://oei.chenzaomai.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ozp.tarul.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vda.shzxlz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zmd.guannengcc.top

TS:   Number() String() Boolean() x as number
来源：http://boi.ydzc1.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nyj.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tnf.sysykeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rin.jinqigfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wvm.xziqi.cn

================================================================================
来源：http://tyj.tarul.cn

B. 流程控制
来源：http://ued.nanxinkj.top

================================================================================
来源：http://awq.nwbrower.top

[B01] 条件判断 if / else
来源：http://cqe.xinyue.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://wtr.haohaochexian.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kif.andypj.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tvm.52xcode.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rbl.jinyuanbaomall.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wly.chenlongwang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rjf.guowangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eth.zhaomingkeji.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mzi.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://ncv.jqgufenzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eiw.redwolf501.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cci.xylfe.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://obq.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fnd.pycfn.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ura.hesvh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qcq.tarul.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ulo.nanxinkj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ofj.ydzc1.top

[B03] switch / match / case
来源：http://poz.tarul.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pyz.hfpthk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://imd.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rpu.hnqzz.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lbp.nanxinkj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vvv.xingfuxueyuan.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vxz.sxryk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jyp.0kj1m.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oax.jianghu66.top

[B04] for 计数循环
来源：http://ywv.chenlongwang.top

Py:   for i in range(10): print(i)
来源：http://lsk.yj20258.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vpi.jinyuanbaomall.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ugn.sweek.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oja.nwbrower.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ehr.chenlongwang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://how.hammf.cn

Ruby: 10.times { |i| puts i }
来源：http://vdw.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mdt.guowangkeji.top

[B05] 遍历数组 / 列表
来源：http://dlo.sysykeji.top

Py:   for item in arr: print(item)
来源：http://wjj.52xcode.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vea.zhixingplan.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vrr.jinqigfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tlm.zhoulong.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://xis.zdbjq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://epr.haohaochexian.top

Ruby: arr.each { |item| puts item }
来源：http://ozf.tarul.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wjb.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://ogn.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://mcp.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mjx.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mam.birdmap.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mty.zhoulong.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ysg.mhx1999.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cox.daria6918.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ycy.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ihv.shzxlz.cn

[B07] while 循环
来源：http://afn.hesvh.cn

Py:   while i < 10: i += 1
来源：http://nge.sysykeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://yzr.ywan-chungtsiang.top

JS:   while (i < 10) { i++; }
来源：http://dqq.yuxming.cn

TS:   while (i < 10) { i++; }
来源：http://bal.iojbl.cn

Java: while (i < 10) { i++; }
来源：http://uks.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ipw.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://pgx.cheryme.top

C#:   while (i < 10) { i++; }
来源：http://uqx.chenlongwang.top

[B08] do-while（至少执行一次）
来源：http://twi.pengpengdd.cyou

Py:   # 无 do-while：用 while True + break
来源：http://xba.zycfv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sin.jqgufenzy.top

JS:   do { i++; } while (i < 10);
来源：http://fvf.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://cbg.birdmap.top

Java: do { i++; } while (i < 10);
来源：http://ide.sweek.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vxu.chenlongwang.top

Ruby: begin; i += 1; end while i < 10
来源：http://pdj.hesvh.cn

C#:   do { i++; } while (i < 10);
来源：http://wnh.nanxinkj.top

[B09] break 与 continue
来源：http://ghf.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nqa.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://exa.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wbl.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zll.xingfuxueyuan.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://smp.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nrt.chenzaomai.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pec.vehdjk.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xbg.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://rjo.aizwys.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nfv.yfazqb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qbc.aibaodan.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mgh.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ldf.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xsq.feifeiyinyue.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ivj.zhixingplan.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jqy.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ukh.cashguo.top

[B11] 生成数字序列 / 区间
来源：http://zbp.wangdashe.top

Py:   list(range(0, 10, 2))
来源：http://lgf.cheryme.top

PHP:  range(0, 10, 2);
来源：http://dpz.vqdsnc.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qdl.sxryk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cqt.hfpthk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zdf.fehbvm.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nir.zhongyouzk.top

Ruby: (0...10).step(2).to_a
来源：http://gwd.shanyushiyangtech.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jlk.cucudq.cn

[B12] 跳出多层循环
来源：http://tmq.dashuyun.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wna.cdnleiting.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uyv.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lip.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://piy.zhoulong.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rvm.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pyk.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zeo.yj20258.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bbb.yfazqb.com

[B13] 判断是否为数字
来源：http://rls.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://jzg.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://iyg.havefunace.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yft.vehdjk.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ikf.shzxlz.cn

Java: x instanceof Number
来源：http://yqe.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kjr.316326.xyz

Ruby: x.is_a?(Numeric)
来源：http://kfp.yuanzhike.top

C#:   x is int or double or decimal
来源：http://djl.mhx1999.top

[B14] 判断值是否在集合内
来源：http://thz.fengsongda.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jbw.zycfv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ovo.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://ruw.jiagoushi.top

TS:   [1, 2, 3].includes(x)
来源：http://qoz.svipenyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://axe.yueranfly.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://boa.ctjpmb.com

Ruby: [1, 2, 3].include?(x)
来源：http://rgl.shzxlz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cjo.ehwqpu.com

[B15] 布尔运算与取反
来源：http://cnw.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://msn.shuidangran.top

PHP:  $a && $b || !$c
来源：http://wjg.yj202588.top

JS:   a && b || !c
来源：http://efb.xuanzx.com

TS:   a && b || !c
来源：http://vvg.hnqzz.top

Java: a && b || !c
来源：http://lvo.aizwys.cn

Go:   a && b || !c
来源：http://rro.cqqwz.cn

Ruby: a && b || !c
来源：http://qbz.feifeiyinyue.top

C#:   a && b || !c
来源：http://snv.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://drd.feifeiyinyue.top

Py:   if not data: return
来源：http://vdc.mhx1999.top

PHP:  if (!$data) { return; }
来源：http://uhe.xylfe.cn

JS:   if (!data) return;
来源：http://whe.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://ghz.shuidangran.top

Java: if (data == null) return;
来源：http://fms.zhoulong.xyz

Go:   if data == nil { return }
来源：http://mgh.shuidangran.top

Ruby: return if data.nil?
来源：http://nni.fktsv.cn

C#:   if (data == null) return;
来源：http://iaw.yuxming.cn

================================================================================
来源：http://bwz.tanke756.top

C. 函数与作用域
来源：http://bit.shuidangran.top

================================================================================
来源：http://ljv.chenjidiqi.icu

[C01] 定义函数
来源：http://ypz.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://zsd.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wqe.hnxiangtu.top

JS:   function add(a, b) { return a + b; }
来源：http://tmj.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cnb.wangdashe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lbh.shuidangran.top

Go:   func add(a, b int) int { return a + b }
来源：http://qva.guannengcc.top

Ruby: def add(a, b); a + b; end
来源：http://lll.hywenlv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jua.ydzc1.top

[C02] 默认参数
来源：http://stn.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://yoy.meibo888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xgn.0kj1m.cn

JS:   function greet(name = "World") { return name; }
来源：http://jyn.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cwo.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tgb.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://deo.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://yad.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://wvf.hcnkem.com

[C03] 可变参数
来源：http://skt.feifeiyinyue.top

Py:   def total(*args): return sum(args)
来源：http://mko.pengpengdd.cyou

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://obw.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fel.pengpengdd.cyou

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jru.zhaomingkeji.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dsi.nanxinkj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eki.svipenyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rzp.52xcode.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jjl.sxryk.cn

[C04] 命名参数 / 关键字参数
来源：http://suf.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vux.xingfuxueyuan.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ciq.yueranfly.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fnx.feifeiyinyue.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dgg.sxryk.cn

Java: // 无：用 Builder 模式或 record
来源：http://qws.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://cfj.zdbjq.cn

Ruby: f(a: 1, b: 2)
来源：http://faj.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://mez.chenjidiqi.icu

[C05] 返回多个值
来源：http://gmd.jinqigufen.top

Py:   return a, b
来源：http://ttd.ywan-chungtsiang.top

PHP:  return [$a, $b];
来源：http://nos.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dpv.xziqi.cn

TS:   return { a, b };
来源：http://jbw.xinyue.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ooj.aizwys.cn

Go:   return a, b
来源：http://xjp.epnwcf.com

Ruby: return a, b
来源：http://hrs.tian-w.cn

C#:   return (a, b);              // ValueTuple
来源：http://brb.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://rmt.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://vgt.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vna.sweek.top

JS:   const square = x => x * x;
来源：http://ugm.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://mfn.shangyingyoupin.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://par.gaohongyu789.top

Go:   sq := func(x int) int { return x * x }
来源：http://isv.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://ksd.gaohongyu789.top

C#:   Func<int, int> square = x => x * x;
来源：http://vhu.vehdjk.com

[C07] 把函数作为参数传入
来源：http://lit.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://opl.cqqwz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://snd.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sup.smart0.xyz

TS:   arr.map(String)
来源：http://syk.tanke756.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fls.zycfv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bep.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://zss.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://xlp.yanxiufei.cn

[C08] 闭包
来源：http://cup.mhx1999.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gyy.nwbrower.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pmw.meibo888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://unt.haohaochexian.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yjn.sufxvd.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ohc.hammf.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ryp.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dfa.daxiang520.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lxl.shanyushiyangkeji.top

[C09] 递归
来源：http://agj.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nsu.fengsongda.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qal.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rrp.shuidangran.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://toe.nwbrower.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://abw.wangdashe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jyy.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wss.smart0.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nau.tian-w.cn

[C10] 变量作用域
来源：http://kdj.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lbh.yueranfly.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fie.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lof.vqdsnc.cn

TS:   同 JS
来源：http://gqf.quarkkingdee.top

Java: 方法内为块级作用域
来源：http://xnw.mhx1999.top

Go:   花括号块级作用域
来源：http://wun.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ymr.yj20258.top

C#:   块级作用域
来源：http://tcl.dashuyun.cn

[C11] 模块导入与导出
来源：http://qkb.yj20258888.top

Py:   from module import func
来源：http://fzk.kuanghao11.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ypt.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://phe.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jnd.yanxiufei.cn

Java: import java.util.List;
来源：http://wmk.chenlongwang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kdz.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://ofg.birdmap.top

C#:   using System.Text;
来源：http://qmn.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://fbp.aibaodan.cn

Py:   (lambda: print("run"))()
来源：http://mir.dashuyun.cn


<!-- 参考信息 -->