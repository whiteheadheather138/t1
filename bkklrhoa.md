代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://agt.shanyushiyangkeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jxq.zhaomingkeji.xyz

JS:   (3.14159).toFixed(2)
来源：http://whm.nanxuanxn.top

TS:   (3.14159).toFixed(2)
来源：http://ykv.hnqzz.top

Java: String.format("%.2f", 3.14159)
来源：http://kli.xuetiantiany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jia.mhx1999.top

Ruby: format("%.2f", 3.14159)
来源：http://jsy.52xcode.cn

C#:   3.14159.ToString("F2")
来源：http://msu.wangshuangyany.cn

[A22] 获取字符串长度
来源：http://lqs.sufxvd.cn

Py:   len(s)
来源：http://meq.xingfuxueyuan.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wvr.havefunace.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://taj.shanyushiyangtech.top

TS:   s.length
来源：http://tkl.52xcode.cn

Java: s.length()
来源：http://wpe.snrcjt.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xmy.nanxuanxn.top

Ruby: s.length
来源：http://fhz.gogol.net.cn

C#:   s.Length
来源：http://ahb.nwbrower.top

[A23] 大小写转换
来源：http://hiv.gzhubu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ogo.mhx1999.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://suz.yj20258888.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aem.fzhhl.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vyz.jiagoushi.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.daria6918.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vxg.zhiwuduotai.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lnf.shzxlz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tgx.gogol.net.cn

[A24] 去除首尾空白
来源：http://fun.shuidangran.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ybx.52xcode.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fyf.zhoulong.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://voa.xingfuxueyuan.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dym.chenzaomai.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://epk.dashuyun.cn

Go:   strings.TrimSpace(s)
来源：http://opa.wangdashe.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vjs.jianghu66.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vhn.zycfv.cn

[A25] 字符串比较
来源：http://cgw.fzhhl.top

Py:   s1 == s2; s1 != s2
来源：http://doy.xingfuxueyuan.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pyc.cdnleiting.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dgf.0kj1m.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cpl.hysaishi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mbh.cdnleiting.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qqv.fktsv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gfu.nanxuanxn.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://veo.yongpay.top

[A26] 类型转换总览
来源：http://tdn.jianghu66.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jsi.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tto.zdqjudy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uyg.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://aqx.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jym.jianghu66.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ubo.cdnleiting.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wwc.nanxinkj.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nle.wangshuangyany.cn

================================================================================
来源：http://vgt.gzhubu.top

B. 流程控制
来源：http://abz.yj20258888.top

================================================================================
来源：http://scr.gzhubu.top

[B01] 条件判断 if / else
来源：http://vxx.jinqigfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cyc.hysaishi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dhi.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xpn.cheryme.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qxy.yj202588.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ppz.zhixingplan.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kgf.uphjek.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zwa.yj202588.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rrs.smart0.xyz

[B02] 多分支 else if / elif
来源：http://hmj.xuanzx.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hki.smart0.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fuj.jqgufenzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://etq.cucudq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gej.jqgfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oxq.ydzc1.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gao.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cxn.c1oappe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ruu.yj202588.top

[B03] switch / match / case
来源：http://zms.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rco.yonumen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hkm.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gjn.gotoacloud.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yyp.tarul.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dnn.jiagoushi.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gma.hfpthk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mpn.wangdashe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pft.aibaodan.cn

[B04] for 计数循环
来源：http://afg.gotoacloud.top

Py:   for i in range(10): print(i)
来源：http://tim.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://viq.hywenlv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zmy.aibaodan.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hcj.sufxvd.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tje.yj20258.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qtd.ydjk.org.cn

Ruby: 10.times { |i| puts i }
来源：http://wyb.birdmap.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dsc.jinqigfzy.top

[B05] 遍历数组 / 列表
来源：http://lcw.daxiang520.top

Py:   for item in arr: print(item)
来源：http://jls.ivvv.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://esp.aizwys.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://acq.ivvv.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fpm.sxryk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zdj.hnqzz.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qxe.gogol.net.cn

Ruby: arr.each { |item| puts item }
来源：http://nog.tarul.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zpq.hysaishi.cn

[B06] 遍历字典 / 对象
来源：http://cjp.ivvv.top

Py:   for k, v in d.items(): print(k, v)
来源：http://iba.yongpay.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kre.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yiq.zhengqikj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://olw.hongshengwenyu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yia.shangyingyoupin.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tsk.52xcode.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gep.shuidangran.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://izn.hongshengwenyu.top

[B07] while 循环
来源：http://aec.epnwcf.com

Py:   while i < 10: i += 1
来源：http://kfh.zhengqikj.top

PHP:  while ($i < 10) { $i++; }
来源：http://nvj.hywenlv.cn

JS:   while (i < 10) { i++; }
来源：http://ekv.gzhubu.top

TS:   while (i < 10) { i++; }
来源：http://hyj.nanxuanxn.top

Java: while (i < 10) { i++; }
来源：http://ofy.meibo888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iqd.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://nqd.yuanzhike.top

C#:   while (i < 10) { i++; }
来源：http://kzf.cdnleiting.top

[B08] do-while（至少执行一次）
来源：http://slf.cucudq.cn

Py:   # 无 do-while：用 while True + break
来源：http://iqo.xinyue.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://zpt.guowangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://ahq.snrcjt.cn

TS:   do { i++; } while (i < 10);
来源：http://mnq.chenlongwang.top

Java: do { i++; } while (i < 10);
来源：http://vel.hywenlv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pgg.yangfankeji.com

Ruby: begin; i += 1; end while i < 10
来源：http://pdq.daxiang520.top

C#:   do { i++; } while (i < 10);
来源：http://tcc.sysykeji.top

[B09] break 与 continue
来源：http://sns.xingfuxueyuan.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vky.shuidangran.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://syb.hammf.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lbw.chenlongwang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lqm.shanyushiyangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uwg.jqgufenzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mnq.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kvs.fktsv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aox.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://grp.fktsv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nkc.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zxl.yanxiufei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nxr.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hri.ybcxt.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lik.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://idg.gaohongyu789.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zxc.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cmd.tianlin.xyz

[B11] 生成数字序列 / 区间
来源：http://nun.cucudq.cn

Py:   list(range(0, 10, 2))
来源：http://gpy.hammf.cn

PHP:  range(0, 10, 2);
来源：http://urk.ppjwa.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://avl.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dvf.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hlt.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aeu.ydjk.org.cn

Ruby: (0...10).step(2).to_a
来源：http://gdb.gzhubu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yfv.0kj1m.cn

[B12] 跳出多层循环
来源：http://shb.yongpay.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vki.wangshuangyany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tyu.jqgfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qhz.andypj.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://poo.dashuyun.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zpq.dianchejie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vju.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yrq.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://agv.jinqigufen.top

[B13] 判断是否为数字
来源：http://vkj.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://tsg.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://oob.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wrb.jiagoushi.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qug.xziqi.cn

Java: x instanceof Number
来源：http://por.nanxinkj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mfl.jianghu66.top

Ruby: x.is_a?(Numeric)
来源：http://tjs.ywan-chungtsiang.top

C#:   x is int or double or decimal
来源：http://bbi.fengsongda.top

[B14] 判断值是否在集合内
来源：http://zbq.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mds.316326.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hqu.zycfv.cn

JS:   [1, 2, 3].includes(x)
来源：http://oav.ctjpmb.com

TS:   [1, 2, 3].includes(x)
来源：http://ata.yj20258888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gje.zhongyouzk.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ltf.guannengcc.top

Ruby: [1, 2, 3].include?(x)
来源：http://lbm.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iom.xinyue.icu

[B15] 布尔运算与取反
来源：http://kfm.zhiwuduotai.top

Py:   a and b or not c
来源：http://ruw.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://djk.fanxiaobao.xyz

JS:   a && b || !c
来源：http://mcy.zhengqikj.top

TS:   a && b || !c
来源：http://yfh.316326.xyz

Java: a && b || !c
来源：http://sds.ivvv.top

Go:   a && b || !c
来源：http://hdi.kuanghao11.cn

Ruby: a && b || !c
来源：http://exl.shzxlz.cn

C#:   a && b || !c
来源：http://rrm.0kj1m.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qly.ywan-chungtsiang.top

Py:   if not data: return
来源：http://xmy.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://vmn.havefunace.top

JS:   if (!data) return;
来源：http://ykc.hongshengwenyu.top

TS:   if (!data) return;
来源：http://zty.tanke756.top

Java: if (data == null) return;
来源：http://nav.haohaochexian.top

Go:   if data == nil { return }
来源：http://lgr.dashuyun.cn

Ruby: return if data.nil?
来源：http://chn.havefunace.top

C#:   if (data == null) return;
来源：http://glp.yj20258.top

================================================================================
来源：http://jei.tarul.cn

C. 函数与作用域
来源：http://muq.daxiang520.top

================================================================================
来源：http://iia.xuetiantiany.cn

[C01] 定义函数
来源：http://lla.nanxuanxn.top

Py:   def add(a, b): return a + b
来源：http://uhe.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wnk.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://rwn.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vwh.fehbvm.com

Java: static int add(int a, int b) { return a + b; }
来源：http://plo.chenlongwang.top

Go:   func add(a, b int) int { return a + b }
来源：http://rnh.gogol.net.cn

Ruby: def add(a, b); a + b; end
来源：http://eox.hesvh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zko.quarkkingdee.top

[C02] 默认参数
来源：http://rgr.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://fgs.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fzy.zhongyouzk.top

JS:   function greet(name = "World") { return name; }
来源：http://awm.bbcook.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zqg.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ouf.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://usu.ydjk.org.cn

Ruby: def greet(name = "World") = name
来源：http://slg.yangfankeji.com

C#:   string Greet(string name = "World") => name;
来源：http://cix.ehwqpu.com

[C03] 可变参数
来源：http://wcc.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://dcx.hammf.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ien.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zbc.jqgfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jkp.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fxb.yuanzhike.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mfe.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://jlx.wangshuangyany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://myh.ybcxt.top

[C04] 命名参数 / 关键字参数
来源：http://fvd.gotoacloud.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sjl.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ogs.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ymx.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xpw.andypj.xyz

Java: // 无：用 Builder 模式或 record
来源：http://ziq.chenzaomai.com

Go:   // 无：用配置结构体参数
来源：http://drj.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://asm.kuanghao11.cn

C#:   f(a: 1, b: 2)
来源：http://wmd.fktsv.cn

[C05] 返回多个值
来源：http://lsr.hcnkem.com

Py:   return a, b
来源：http://ngu.andypj.xyz

PHP:  return [$a, $b];
来源：http://wmy.tanke756.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zbw.ydzc1.top

TS:   return { a, b };
来源：http://cdv.zhiwuduotai.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://urh.zhengqikj.top

Go:   return a, b
来源：http://bny.jinqigufen.top

Ruby: return a, b
来源：http://mow.shangyingyoupin.top

C#:   return (a, b);              // ValueTuple
来源：http://ruj.jyoumei.cn

[C06] 匿名函数 / lambda
来源：http://aof.meibo888.top

Py:   square = lambda x: x * x
来源：http://qii.chenlongwang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://eeg.fengsongda.top

JS:   const square = x => x * x;
来源：http://not.fanxiaobao.xyz

TS:   const square = (x: number): number => x * x;
来源：http://lew.jiagoushi.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://exc.ivvv.top

Go:   sq := func(x int) int { return x * x }
来源：http://hzz.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://ayi.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://bur.yj202588.top

[C07] 把函数作为参数传入
来源：http://quf.gotoacloud.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wet.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://hqr.cqqwz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wui.gzhubu.top

TS:   arr.map(String)
来源：http://fgf.yonumen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lip.ywan-chungtsiang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uip.yuxming.cn

Ruby: arr.map(&:upcase)
来源：http://odg.tarul.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wkn.yfazqb.com

[C08] 闭包
来源：http://flq.jlsjyb.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rfu.gzhubu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ksa.shuidangran.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hht.yuxming.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ccb.birdmap.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ttn.jiagoushi.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yuj.yj202588.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gcp.tarul.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yts.316326.xyz

[C09] 递归
来源：http://pfa.pengpengdd.cyou

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vah.ivvv.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ydj.ydzc1.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ati.cucudq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://akt.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aku.c1oappe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dtq.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kca.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aaw.zycfv.cn

[C10] 变量作用域
来源：http://cnv.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zbs.cucudq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sao.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dxr.hysaishi.cn

TS:   同 JS
来源：http://yxb.jinyuanbaomall.cn

Java: 方法内为块级作用域
来源：http://aoh.316326.xyz

Go:   花括号块级作用域
来源：http://nhy.ybcxt.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ojx.andypj.xyz

C#:   块级作用域
来源：http://fgt.mhx1999.top

[C11] 模块导入与导出
来源：http://syu.mhx1999.top

Py:   from module import func
来源：http://bfi.nanxinkj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zro.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bzg.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mmn.xziqi.cn

Java: import java.util.List;
来源：http://qip.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tyw.cqqwz.cn


<!-- 参考信息 -->