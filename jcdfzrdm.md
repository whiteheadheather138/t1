代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://ydq.cheryme.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ggt.9152youxi.cn

JS:   (3.14159).toFixed(2)
来源：http://knd.hcnkem.com

TS:   (3.14159).toFixed(2)
来源：http://fzk.jinqigfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://jhv.hywenlv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bjh.zhaomingkeji.xyz

Ruby: format("%.2f", 3.14159)
来源：http://hpz.yangfankeji.com

C#:   3.14159.ToString("F2")
来源：http://jkp.shuidangran.top

[A22] 获取字符串长度
来源：http://oep.shzxlz.cn

Py:   len(s)
来源：http://uhv.gotoacloud.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tna.ivvv.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nhu.bbcook.cn

TS:   s.length
来源：http://jfz.ivvv.top

Java: s.length()
来源：http://syu.xuanzx.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://voa.zhengqikj.top

Ruby: s.length
来源：http://xln.fzhhl.top

C#:   s.Length
来源：http://acq.tarul.cn

[A23] 大小写转换
来源：http://vxw.shzxlz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://llj.sjlbkw.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cuk.52xcode.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qxu.xziqi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jer.ctjpmb.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pil.hcnkem.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nth.sufxvd.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://shi.hnqzz.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rdb.birdmap.top

[A24] 去除首尾空白
来源：http://lfw.tianlin.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sld.xinyue.icu

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wma.daria6918.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jrl.ivvv.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zbe.zdqjudy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ldg.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://hyx.c1oappe.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tqo.tanke756.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lck.sysykeji.top

[A25] 字符串比较
来源：http://olq.snrcjt.cn

Py:   s1 == s2; s1 != s2
来源：http://ttj.jyoumei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hbx.cqqwz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://juj.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yhw.zhoulong.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fvq.cheryme.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cnp.jyoumei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mwc.zhaomingkeji.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bnk.zhoulong.xyz

[A26] 类型转换总览
来源：http://zot.jianghu66.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xfw.iojbl.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zqh.yvedp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dnf.snrcjt.cn

TS:   Number() String() Boolean() x as number
来源：http://gov.redwolf501.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tqk.tianlin.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nwm.ybcxt.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gsg.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mph.shanyushiyangtech.top

================================================================================
来源：http://thl.shanyushiyangtech.top

B. 流程控制
来源：http://gbr.sjlbkw.cn

================================================================================
来源：http://egd.chenjidiqi.icu

[B01] 条件判断 if / else
来源：http://vzf.gzhubu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://pws.dianchejie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vtu.ppjwa.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mii.svipenyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nio.tanke756.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://sgl.aizwys.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wtm.tianlin.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ief.hnqzz.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jsz.jqgufenzy.top

[B02] 多分支 else if / elif
来源：http://gzz.xuanzx.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://slw.birdmap.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hta.xuanzx.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://joa.tarul.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pwm.yonumen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wie.yj20258888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qdq.0kj1m.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cvb.ehwqpu.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://enz.zhoulong.xyz

[B03] switch / match / case
来源：http://fgg.hysaishi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://epm.jianghu66.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sze.svipenyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://avb.guannengcc.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dun.xinyue.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kzw.sufxvd.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nnl.yj20258.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ipz.guowangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wqo.cashguo.top

[B04] for 计数循环
来源：http://djq.xuetiantiany.cn

Py:   for i in range(10): print(i)
来源：http://mmw.yj20258888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jto.hammf.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://svq.fktsv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zma.tian-w.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qky.xylfe.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://orm.ydzc1.top

Ruby: 10.times { |i| puts i }
来源：http://gnm.316326.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ddy.xuanzx.com

[B05] 遍历数组 / 列表
来源：http://zqn.ybcxt.top

Py:   for item in arr: print(item)
来源：http://lpj.xuanzx.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iqt.yj20258888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://koo.xuanzx.com

TS:   for (const item of arr) { console.log(item); }
来源：http://cry.yvedp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tue.jqgufenzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sdm.feifeiyinyue.top

Ruby: arr.each { |item| puts item }
来源：http://grp.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://exu.0kj1m.cn

[B06] 遍历字典 / 对象
来源：http://jno.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cqf.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aam.sufxvd.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uoj.havefunace.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uys.jinghuilouyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zqy.zdbjq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jej.yj20258.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://csy.hnqzz.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ldz.52xcode.cn

[B07] while 循环
来源：http://dax.sxryk.cn

Py:   while i < 10: i += 1
来源：http://pgy.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://lvy.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://tvb.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://lhu.sysykeji.top

Java: while (i < 10) { i++; }
来源：http://hvs.hfpthk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jdh.jinqigufen.top

Ruby: while i < 10; i += 1; end
来源：http://wno.ehwqpu.com

C#:   while (i < 10) { i++; }
来源：http://cvb.nanxinkj.top

[B08] do-while（至少执行一次）
来源：http://tht.c1oappe.top

Py:   # 无 do-while：用 while True + break
来源：http://tog.xziqi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iom.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://vwu.redwolf501.top

TS:   do { i++; } while (i < 10);
来源：http://arq.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://ncx.quarkkingdee.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ywq.meibo888.top

Ruby: begin; i += 1; end while i < 10
来源：http://qtz.yj202588.top

C#:   do { i++; } while (i < 10);
来源：http://ygq.wangdashe.top

[B09] break 与 continue
来源：http://igp.yongpay.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ifa.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ipw.jianghu66.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nll.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://abz.tian-w.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mpl.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bco.nwbrower.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mxm.shangyingyoupin.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://msk.yuxming.cn

[B10] 遍历同时拿索引
来源：http://olb.fzhhl.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kgg.tarul.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ktv.yueranfly.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gzc.jyoumei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://whh.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ueb.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://plz.jyoumei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wrf.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tiv.jyoumei.cn

[B11] 生成数字序列 / 区间
来源：http://rjo.jianghu66.top

Py:   list(range(0, 10, 2))
来源：http://hhr.zdqjudy.top

PHP:  range(0, 10, 2);
来源：http://lkw.hammf.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uix.nanxuanxn.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uyt.tarul.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bni.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dby.wangshuangyany.cn

Ruby: (0...10).step(2).to_a
来源：http://qxn.wangdashe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ygs.meibo888.top

[B12] 跳出多层循环
来源：http://zcd.andypj.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://ctw.xziqi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pbj.cheryme.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hca.cdnleiting.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rkm.vqdsnc.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ukq.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jqi.gotoacloud.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mwd.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hlw.jinghuilouyu.cn

[B13] 判断是否为数字
来源：http://nnl.gotoacloud.top

Py:   isinstance(x, (int, float))
来源：http://eis.aibaodan.cn

PHP:  is_numeric($x)
来源：http://pyj.uphjek.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rzj.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cpq.jinqigufen.top

Java: x instanceof Number
来源：http://gwc.wangshuangyany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vxg.daxiang520.top

Ruby: x.is_a?(Numeric)
来源：http://roy.cucudq.cn

C#:   x is int or double or decimal
来源：http://dwq.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://jaa.c1oappe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sse.dianchejie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tga.guowangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://rac.xinyue.icu

TS:   [1, 2, 3].includes(x)
来源：http://wpl.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jcc.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zki.jyoumei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uzd.hfpthk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qwq.iojbl.cn

[B15] 布尔运算与取反
来源：http://avs.shuidangran.top

Py:   a and b or not c
来源：http://ypt.yonumen.top

PHP:  $a && $b || !$c
来源：http://fxv.gzhubu.top

JS:   a && b || !c
来源：http://ecr.bbcook.cn

TS:   a && b || !c
来源：http://imx.hnxiangtu.top

Java: a && b || !c
来源：http://lwn.xinyue.icu

Go:   a && b || !c
来源：http://yjr.sysykeji.top

Ruby: a && b || !c
来源：http://kji.gaohongyu789.top

C#:   a && b || !c
来源：http://ifx.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://bdp.0kj1m.cn

Py:   if not data: return
来源：http://ami.fzhhl.top

PHP:  if (!$data) { return; }
来源：http://jfo.fzhhl.top

JS:   if (!data) return;
来源：http://bsf.nanxuanxn.top

TS:   if (!data) return;
来源：http://bfn.sjlbkw.cn

Java: if (data == null) return;
来源：http://hnl.ywan-chungtsiang.top

Go:   if data == nil { return }
来源：http://gik.ctjpmb.com

Ruby: return if data.nil?
来源：http://uiz.fehbvm.com

C#:   if (data == null) return;
来源：http://iqr.hammf.cn

================================================================================
来源：http://zyw.hfpthk.cn

C. 函数与作用域
来源：http://dcw.fzhhl.top

================================================================================
来源：http://qff.tian-w.cn

[C01] 定义函数
来源：http://xsf.316326.xyz

Py:   def add(a, b): return a + b
来源：http://fyp.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pqo.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://zwd.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://twg.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cyb.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ubc.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://kfm.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nye.xylfe.cn

[C02] 默认参数
来源：http://opj.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://hfo.daria6918.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tie.tianlin.xyz

JS:   function greet(name = "World") { return name; }
来源：http://vez.gogol.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tui.zdbjq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hlm.yfazqb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wkz.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://nft.jyoumei.cn

C#:   string Greet(string name = "World") => name;
来源：http://kui.jinqigufen.top

[C03] 可变参数
来源：http://wlh.sxryk.cn

Py:   def total(*args): return sum(args)
来源：http://awd.jianghu66.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zwk.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mxw.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cyu.cheryme.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vkx.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xeu.havefunace.top

Ruby: def total(*nums); nums.sum; end
来源：http://oja.zycfv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gkj.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://hmh.snrcjt.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://djj.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qri.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hsr.shanyushiyangtech.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tcf.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://eff.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://pnf.zhaomingkeji.xyz

Ruby: f(a: 1, b: 2)
来源：http://uvh.yj20258888.top

C#:   f(a: 1, b: 2)
来源：http://hix.kuanghao11.cn

[C05] 返回多个值
来源：http://uok.fanxiaobao.xyz

Py:   return a, b
来源：http://eqz.zdqjudy.top

PHP:  return [$a, $b];
来源：http://elr.hnxiangtu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dah.iojbl.cn

TS:   return { a, b };
来源：http://egc.zhaomingkeji.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://khd.tian-w.cn

Go:   return a, b
来源：http://mif.cashguo.top

Ruby: return a, b
来源：http://kzg.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://vih.cheryme.top

[C06] 匿名函数 / lambda
来源：http://cqu.aizwys.cn

Py:   square = lambda x: x * x
来源：http://pos.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://psp.yuxming.cn

JS:   const square = x => x * x;
来源：http://luk.yuanzhike.top

TS:   const square = (x: number): number => x * x;
来源：http://kad.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://keg.andypj.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://ufc.nanxuanxn.top

Ruby: square = ->(x) { x * x }
来源：http://xny.wangdashe.top

C#:   Func<int, int> square = x => x * x;
来源：http://hlr.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://kih.gotoacloud.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vue.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://faf.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wol.ywan-chungtsiang.top

TS:   arr.map(String)
来源：http://svy.ywan-chungtsiang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ipk.zhengqikj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lmx.gotoacloud.top

Ruby: arr.map(&:upcase)
来源：http://dqf.gaohongyu789.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zqg.haohaochexian.top

[C08] 闭包
来源：http://mrr.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qsm.hcnkem.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vsc.shanyushiyangtech.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://crg.chenlongwang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ilr.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ztj.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cqo.xinyue.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tlk.zhaomingkeji.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vrf.ydzc1.top

[C09] 递归
来源：http://tkj.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yiy.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pil.kuanghao11.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ede.wangdashe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://axu.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lsv.xuanzx.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gda.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gur.c1oappe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bom.cqqwz.cn

[C10] 变量作用域
来源：http://xgu.yongpay.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://caf.havefunace.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bez.dashuyun.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cmh.shzxlz.cn

TS:   同 JS
来源：http://lkq.jinqigfzy.top

Java: 方法内为块级作用域
来源：http://nht.yuanzhike.top

Go:   花括号块级作用域
来源：http://pkv.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rxy.shzxlz.cn

C#:   块级作用域
来源：http://jse.hcnkem.com

[C11] 模块导入与导出
来源：http://cti.yangfankeji.com

Py:   from module import func
来源：http://bey.dianchejie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mkr.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qwa.zdbjq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qhk.ywan-chungtsiang.top

Java: import java.util.List;
来源：http://mdz.xylfe.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dlg.tian-w.cn


<!-- 参考信息 -->