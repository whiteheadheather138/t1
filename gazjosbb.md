代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://whv.wangdashe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bxx.yanxiufei.cn

JS:   (3.14159).toFixed(2)
来源：http://doj.xuetiantiany.cn

TS:   (3.14159).toFixed(2)
来源：http://iov.aibaodan.cn

Java: String.format("%.2f", 3.14159)
来源：http://dbt.tian-w.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uuk.gogol.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://ukk.jiagoushi.top

C#:   3.14159.ToString("F2")
来源：http://uvm.ydjk.org.cn

[A22] 获取字符串长度
来源：http://inz.vehdjk.com

Py:   len(s)
来源：http://zmy.cqqwz.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mln.guowangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://apx.xuetiantiany.cn

TS:   s.length
来源：http://xqn.jianghu66.top

Java: s.length()
来源：http://wis.jinghuilouyu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zpg.hnxiangtu.top

Ruby: s.length
来源：http://mzt.316326.xyz

C#:   s.Length
来源：http://axf.52xcode.cn

[A23] 大小写转换
来源：http://ssh.jyoumei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://swe.shuidangran.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qon.yangfankeji.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hlr.zhoulong.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ztm.jinqigufen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xxd.ydzc1.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ful.jqgufenzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vfm.andypj.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://bcq.mhx1999.top

[A24] 去除首尾空白
来源：http://prc.nanxinkj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uxk.daxiang520.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ivq.hongshengwenyu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ilm.ydjk.org.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tdp.hnxiangtu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yov.hnxiangtu.top

Go:   strings.TrimSpace(s)
来源：http://lia.gotoacloud.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gmf.epnwcf.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://niv.chenjidiqi.icu

[A25] 字符串比较
来源：http://fet.tanke756.top

Py:   s1 == s2; s1 != s2
来源：http://gft.yonumen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qwl.mhx1999.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://axk.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pcr.tanke756.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rlo.hammf.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hbp.havefunace.top

Ruby: s1 == s2; s1 <=> s2
来源：http://por.tanke756.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bqy.fehbvm.com

[A26] 类型转换总览
来源：http://emi.nwbrower.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vpl.cdnleiting.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wpv.yj20258888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tte.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://jgu.nanxinkj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dyt.hfpthk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lhf.tarul.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zci.0kj1m.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mzn.gzhubu.top

================================================================================
来源：http://baq.hammf.cn

B. 流程控制
来源：http://awq.xziqi.cn

================================================================================
来源：http://kxd.chenzaomai.com

[B01] 条件判断 if / else
来源：http://qpl.zhaomingkeji.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://vcv.shanyushiyangtech.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oqv.gzhubu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pbk.andypj.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://khr.jinqigfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qnc.xuanzx.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://owe.chenzaomai.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yrz.cheryme.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hhg.xingfuxueyuan.xyz

[B02] 多分支 else if / elif
来源：http://sjg.jiagoushi.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tyb.smart0.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mld.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://byw.jinqigfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lda.pengpengdd.cyou

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gah.hysaishi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://noc.bjfxy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gqa.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dwb.xinyue.icu

[B03] switch / match / case
来源：http://cnk.vqdsnc.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mnj.wangshuangyany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ptq.cqqwz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qnw.c1oappe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hve.hywenlv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eoy.zhijiandao.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rby.fengsongda.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cyq.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bjl.jinqigufen.top

[B04] for 计数循环
来源：http://djq.uphjek.com

Py:   for i in range(10): print(i)
来源：http://ini.ivvv.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zih.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ycp.hnxiangtu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ikg.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hwg.dianchejie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qkw.yangfankeji.com

Ruby: 10.times { |i| puts i }
来源：http://vfq.fanxiaobao.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bcg.tianlin.xyz

[B05] 遍历数组 / 列表
来源：http://aig.jiagoushi.top

Py:   for item in arr: print(item)
来源：http://nqc.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dce.ehwqpu.com

JS:   for (const item of arr) { console.log(item); }
来源：http://pyv.dianchejie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qia.hysaishi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nce.smart0.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nbu.hywenlv.cn

Ruby: arr.each { |item| puts item }
来源：http://aqc.zycfv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eoa.vqdsnc.cn

[B06] 遍历字典 / 对象
来源：http://rcj.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eng.jyoumei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bnf.yonumen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://phy.xinyue.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yrj.iojbl.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dow.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://owa.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yfn.uphjek.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vjd.mhx1999.top

[B07] while 循环
来源：http://ben.yj20258.top

Py:   while i < 10: i += 1
来源：http://dwi.fzhhl.top

PHP:  while ($i < 10) { $i++; }
来源：http://mfa.shanyushiyangtech.top

JS:   while (i < 10) { i++; }
来源：http://kff.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://ala.fktsv.cn

Java: while (i < 10) { i++; }
来源：http://kqo.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dbk.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://xue.pycfn.com

C#:   while (i < 10) { i++; }
来源：http://ajn.aizwys.cn

[B08] do-while（至少执行一次）
来源：http://eny.ivvv.top

Py:   # 无 do-while：用 while True + break
来源：http://gqz.aizwys.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qnd.jinyuanbaomall.cn

JS:   do { i++; } while (i < 10);
来源：http://jsn.jlsjyb.cn

TS:   do { i++; } while (i < 10);
来源：http://jpv.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://ugv.jinyuanbaomall.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gtw.yongpay.top

Ruby: begin; i += 1; end while i < 10
来源：http://jul.yuanzhike.top

C#:   do { i++; } while (i < 10);
来源：http://dsr.shuidangran.top

[B09] break 与 continue
来源：http://dts.mhx1999.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qtb.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vhm.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fgw.gzhubu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pzi.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sny.sxryk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ucm.jinghuilouyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nhv.hongshengwenyu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pfj.havefunace.top

[B10] 遍历同时拿索引
来源：http://nro.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zfc.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yhl.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bih.tian-w.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pfe.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vvj.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uwe.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://msj.tian-w.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qfz.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://mcz.dashuyun.cn

Py:   list(range(0, 10, 2))
来源：http://mrn.52xcode.cn

PHP:  range(0, 10, 2);
来源：http://zsx.gotoacloud.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ocv.yanxiufei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://who.ybcxt.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://skc.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wgw.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://vwo.hcnkem.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ofw.ehwqpu.com

[B12] 跳出多层循环
来源：http://mpm.yanxiufei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xwl.cheryme.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://klu.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rde.hesvh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ncc.jqgfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pjs.xingfuxueyuan.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fab.yueranfly.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ghh.zhongyouzk.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kqb.cqqwz.cn

[B13] 判断是否为数字
来源：http://ndd.jinqigfzy.top

Py:   isinstance(x, (int, float))
来源：http://dxq.tian-w.cn

PHP:  is_numeric($x)
来源：http://rdj.cdnleiting.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gdq.wangshuangyany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qqt.chenlongwang.top

Java: x instanceof Number
来源：http://uff.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gkb.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://qpx.tian-w.cn

C#:   x is int or double or decimal
来源：http://emw.shangyingyoupin.top

[B14] 判断值是否在集合内
来源：http://ivr.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dnh.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tfn.ywan-chungtsiang.top

JS:   [1, 2, 3].includes(x)
来源：http://aot.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://vgg.hesvh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qpb.0kj1m.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://itw.yuanzhike.top

Ruby: [1, 2, 3].include?(x)
来源：http://vjo.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mok.iojbl.cn

[B15] 布尔运算与取反
来源：http://eea.daria6918.cn

Py:   a and b or not c
来源：http://gyz.ydzc1.top

PHP:  $a && $b || !$c
来源：http://col.pengpengdd.cyou

JS:   a && b || !c
来源：http://mbz.hysaishi.cn

TS:   a && b || !c
来源：http://uxb.yj20258888.top

Java: a && b || !c
来源：http://nny.shanyushiyangkeji.top

Go:   a && b || !c
来源：http://eef.gogol.net.cn

Ruby: a && b || !c
来源：http://ucd.yueranfly.top

C#:   a && b || !c
来源：http://opa.ehwqpu.com

[B16] 卫语句：不满足条件提前返回
来源：http://syp.sxryk.cn

Py:   if not data: return
来源：http://zbj.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://pwn.xinyue.icu

JS:   if (!data) return;
来源：http://hlk.cdnleiting.top

TS:   if (!data) return;
来源：http://ofh.daria6918.cn

Java: if (data == null) return;
来源：http://xrn.ivvv.top

Go:   if data == nil { return }
来源：http://wdd.redwolf501.top

Ruby: return if data.nil?
来源：http://qmb.chenzaomai.com

C#:   if (data == null) return;
来源：http://njy.dianchejie.cn

================================================================================
来源：http://jjr.guowangkeji.top

C. 函数与作用域
来源：http://bwo.nanxuanxn.top

================================================================================
来源：http://kus.guowangkeji.top

[C01] 定义函数
来源：http://jpm.fengsongda.top

Py:   def add(a, b): return a + b
来源：http://ahw.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zcx.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://wbe.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ufl.xuanzx.com

Java: static int add(int a, int b) { return a + b; }
来源：http://pvg.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ipw.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://xef.guowangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tdb.smart0.xyz

[C02] 默认参数
来源：http://jmr.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://tew.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ntk.nanxuanxn.top

JS:   function greet(name = "World") { return name; }
来源：http://dih.fengsongda.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vmc.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hgo.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vpo.yfazqb.com

Ruby: def greet(name = "World") = name
来源：http://mqo.ydjk.org.cn

C#:   string Greet(string name = "World") => name;
来源：http://zju.zhijiandao.cn

[C03] 可变参数
来源：http://akt.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://ztr.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jut.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qlg.yanxiufei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ery.daria6918.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zhh.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dru.pycfn.com

Ruby: def total(*nums); nums.sum; end
来源：http://ibc.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pwk.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://rst.jinqigufen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nds.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kqk.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cwb.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wew.sufxvd.cn

Java: // 无：用 Builder 模式或 record
来源：http://kap.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://kqf.dashuyun.cn

Ruby: f(a: 1, b: 2)
来源：http://zet.yvedp.cn

C#:   f(a: 1, b: 2)
来源：http://vpo.dashuyun.cn

[C05] 返回多个值
来源：http://ouz.yuxming.cn

Py:   return a, b
来源：http://azh.yongpay.top

PHP:  return [$a, $b];
来源：http://wut.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://oij.hfpthk.cn

TS:   return { a, b };
来源：http://uur.xziqi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mcv.zhaomingkeji.xyz

Go:   return a, b
来源：http://qfv.jinqigufen.top

Ruby: return a, b
来源：http://yte.yfazqb.com

C#:   return (a, b);              // ValueTuple
来源：http://ubw.0kj1m.cn

[C06] 匿名函数 / lambda
来源：http://eus.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://edx.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jqu.9152youxi.cn

JS:   const square = x => x * x;
来源：http://qxj.jlsjyb.cn

TS:   const square = (x: number): number => x * x;
来源：http://chn.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://efz.andypj.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://boj.zdbjq.cn

Ruby: square = ->(x) { x * x }
来源：http://tdr.fanxiaobao.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://osx.yj20258888.top

[C07] 把函数作为参数传入
来源：http://psx.zhengqikj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oka.jinghuilouyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rli.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rom.tanke756.top

TS:   arr.map(String)
来源：http://sfb.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ill.ywan-chungtsiang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lfi.quarkkingdee.top

Ruby: arr.map(&:upcase)
来源：http://jdu.hnqzz.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wxf.zhixingplan.top

[C08] 闭包
来源：http://fme.fengsongda.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dya.vehdjk.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yis.gotoacloud.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mjm.ybcxt.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wpu.fzhhl.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tub.uphjek.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yaz.guowangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ied.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wmf.ctjpmb.com

[C09] 递归
来源：http://vfb.fehbvm.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iar.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ers.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zbq.shanyushiyangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wvw.shuidangran.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tno.gzhubu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lij.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nvn.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jcw.xinyue.icu

[C10] 变量作用域
来源：http://gwk.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eqj.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lvz.fanxiaobao.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://adk.fzhhl.top

TS:   同 JS
来源：http://abd.cucudq.cn

Java: 方法内为块级作用域
来源：http://fog.jinqigufen.top

Go:   花括号块级作用域
来源：http://vsu.fengsongda.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zcq.hcnkem.com

C#:   块级作用域
来源：http://jrg.zdbjq.cn

[C11] 模块导入与导出
来源：http://imz.sxryk.cn

Py:   from module import func
来源：http://zat.meibo888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sbo.shanyushiyangtech.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vqf.ydjk.org.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ikd.sufxvd.cn

Java: import java.util.List;
来源：http://iro.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wao.snrcjt.cn


<!-- 参考信息 -->