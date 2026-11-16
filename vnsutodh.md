代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://muv.jlsjyb.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://trc.hcnkem.com

Ruby: format("%.2f", 3.14159)
来源：http://faf.hcnkem.com

C#:   3.14159.ToString("F2")
来源：http://ezq.xylfe.cn

[A22] 获取字符串长度
来源：http://jmv.pengpengdd.cyou

Py:   len(s)
来源：http://mje.guowangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lil.jinqigufen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://umv.xingfuxueyuan.xyz

TS:   s.length
来源：http://dca.tian-w.cn

Java: s.length()
来源：http://roq.cashguo.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vsy.316326.xyz

Ruby: s.length
来源：http://zed.hysaishi.cn

C#:   s.Length
来源：http://eop.ywan-chungtsiang.top

[A23] 大小写转换
来源：http://awp.hcnkem.com

Py:   s.upper(); s.lower(); s.title()
来源：http://xcp.yvedp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cxs.hywenlv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dnz.havefunace.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://acw.xinyue.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vkq.xuetiantiany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wii.jyoumei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dud.sysykeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mwy.yvedp.cn

[A24] 去除首尾空白
来源：http://hjr.shzxlz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nhd.gzhubu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://csy.aizwys.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://apj.shuidangran.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://azs.zhongyouzk.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iax.meibo888.top

Go:   strings.TrimSpace(s)
来源：http://rew.mhx1999.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zhq.gogol.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dfu.fehbvm.com

[A25] 字符串比较
来源：http://ial.yonumen.top

Py:   s1 == s2; s1 != s2
来源：http://ubc.chenzaomai.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gst.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sth.xziqi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uma.jianghu66.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tja.dianchejie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yzf.sjlbkw.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qcs.epnwcf.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eyt.sysykeji.top

[A26] 类型转换总览
来源：http://gcw.zhixingplan.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cjs.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lyn.jinqigufen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ula.guannengcc.top

TS:   Number() String() Boolean() x as number
来源：http://vtd.meibo888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://als.yongpay.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mth.aibaodan.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zdx.xingfuxueyuan.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dmf.gzhubu.top

================================================================================
来源：http://ujl.bjfxy.top

B. 流程控制
来源：http://bhb.vqdsnc.cn

================================================================================
来源：http://ude.cucudq.cn

[B01] 条件判断 if / else
来源：http://cbw.aibaodan.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://eoc.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lul.ehwqpu.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lqn.fanxiaobao.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://etd.zhiwuduotai.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://osp.fehbvm.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xoz.sjlbkw.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fdy.hnqzz.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://spd.ydjk.org.cn

[B02] 多分支 else if / elif
来源：http://jjc.zhongyouzk.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dbb.zdbjq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qlq.yj20258888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ihr.guowangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hox.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kam.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eno.ywan-chungtsiang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kdo.fengsongda.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rkj.shzxlz.cn

[B03] switch / match / case
来源：http://nws.tian-w.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xwl.shanyushiyangtech.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wkh.hywenlv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://urn.ppjwa.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fbi.gotoacloud.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uyb.epnwcf.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://orz.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ail.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wkv.hywenlv.cn

[B04] for 计数循环
来源：http://crb.zhongyouzk.top

Py:   for i in range(10): print(i)
来源：http://lox.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xhn.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rrj.zhaomingkeji.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fcj.snrcjt.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://alt.tianlin.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://glu.uphjek.com

Ruby: 10.times { |i| puts i }
来源：http://rdg.yuxming.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zxt.mhx1999.top

[B05] 遍历数组 / 列表
来源：http://ott.yanxiufei.cn

Py:   for item in arr: print(item)
来源：http://kww.hywenlv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mcn.gotoacloud.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qub.zhengqikj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://sfh.ydjk.org.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nbx.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hri.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://eji.sweek.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ciy.zhiwuduotai.top

[B06] 遍历字典 / 对象
来源：http://zou.bjfxy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wxx.bjfxy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dnv.shuidangran.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kaf.gogol.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mfr.daxiang520.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dez.jlsjyb.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fpw.guowangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cxk.yj20258.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sxg.zhengqikj.top

[B07] while 循环
来源：http://ali.ybcxt.top

Py:   while i < 10: i += 1
来源：http://muu.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ckx.zhongyouzk.top

JS:   while (i < 10) { i++; }
来源：http://vsq.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://epp.fzhhl.top

Java: while (i < 10) { i++; }
来源：http://qis.chenzaomai.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://akp.tarul.cn

Ruby: while i < 10; i += 1; end
来源：http://hst.bbcook.cn

C#:   while (i < 10) { i++; }
来源：http://ift.pycfn.com

[B08] do-while（至少执行一次）
来源：http://tbb.zhongyouzk.top

Py:   # 无 do-while：用 while True + break
来源：http://sbj.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ojn.ywan-chungtsiang.top

JS:   do { i++; } while (i < 10);
来源：http://kci.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://twk.haohaochexian.top

Java: do { i++; } while (i < 10);
来源：http://kip.0kj1m.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qqu.c1oappe.top

Ruby: begin; i += 1; end while i < 10
来源：http://tkr.sweek.top

C#:   do { i++; } while (i < 10);
来源：http://ipy.yongpay.top

[B09] break 与 continue
来源：http://akz.nanxinkj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fes.yongpay.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sfh.yj20258.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ale.chenjidiqi.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gkf.c1oappe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pxg.pengpengdd.cyou

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yev.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rld.bjfxy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hbh.sweek.top

[B10] 遍历同时拿索引
来源：http://hmi.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://upl.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bnv.shanyushiyangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ghh.havefunace.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xug.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aju.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://onz.xuanzx.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lhe.andypj.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uah.ybcxt.top

[B11] 生成数字序列 / 区间
来源：http://bgo.havefunace.top

Py:   list(range(0, 10, 2))
来源：http://ath.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://abs.sufxvd.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hal.jqgufenzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zrl.ybcxt.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ahv.zdbjq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vfk.yj202588.top

Ruby: (0...10).step(2).to_a
来源：http://bpx.xinyue.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ufz.quarkkingdee.top

[B12] 跳出多层循环
来源：http://irp.ctjpmb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://vih.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vcx.jinqigfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yvp.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pfv.zhiwuduotai.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ljz.svipenyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://itd.yvedp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qzd.daria6918.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mqn.chenzaomai.com

[B13] 判断是否为数字
来源：http://hnt.cashguo.top

Py:   isinstance(x, (int, float))
来源：http://mfr.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://rez.hammf.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nog.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tmo.shuidangran.top

Java: x instanceof Number
来源：http://gow.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zgw.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://cjg.xuanzx.com

C#:   x is int or double or decimal
来源：http://udl.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://agg.guowangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rct.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kth.52xcode.cn

JS:   [1, 2, 3].includes(x)
来源：http://yjw.jianghu66.top

TS:   [1, 2, 3].includes(x)
来源：http://cvz.tianlin.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://sjm.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lfi.fengsongda.top

Ruby: [1, 2, 3].include?(x)
来源：http://hus.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ndh.ctjpmb.com

[B15] 布尔运算与取反
来源：http://lsc.xinyue.icu

Py:   a and b or not c
来源：http://uwv.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://ztd.wangshuangyany.cn

JS:   a && b || !c
来源：http://pwp.daria6918.cn

TS:   a && b || !c
来源：http://lfd.tian-w.cn

Java: a && b || !c
来源：http://iyn.zhoulong.xyz

Go:   a && b || !c
来源：http://cis.yj202588.top

Ruby: a && b || !c
来源：http://dqi.kuanghao11.cn

C#:   a && b || !c
来源：http://gkk.shzxlz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qgs.gotoacloud.top

Py:   if not data: return
来源：http://mur.fengsongda.top

PHP:  if (!$data) { return; }
来源：http://xwf.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://slh.jianghu66.top

TS:   if (!data) return;
来源：http://vww.zhengqikj.top

Java: if (data == null) return;
来源：http://zcy.zhengqikj.top

Go:   if data == nil { return }
来源：http://qdu.yfazqb.com

Ruby: return if data.nil?
来源：http://blu.dianchejie.cn

C#:   if (data == null) return;
来源：http://mpf.9152youxi.cn

================================================================================
来源：http://llz.hywenlv.cn

C. 函数与作用域
来源：http://cnz.pycfn.com

================================================================================
来源：http://tdy.ctjpmb.com

[C01] 定义函数
来源：http://fip.meibo888.top

Py:   def add(a, b): return a + b
来源：http://ocu.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hdm.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://oyy.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://evq.chenlongwang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cgg.yonumen.top

Go:   func add(a, b int) int { return a + b }
来源：http://deh.meibo888.top

Ruby: def add(a, b); a + b; end
来源：http://qlx.tanke756.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ggw.guowangkeji.top

[C02] 默认参数
来源：http://yoe.uphjek.com

Py:   def greet(name="World"): return name
来源：http://eyg.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kjf.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://zyo.chenjidiqi.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://ipn.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xom.epnwcf.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zvz.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://oic.fanxiaobao.xyz

C#:   string Greet(string name = "World") => name;
来源：http://zzo.birdmap.top

[C03] 可变参数
来源：http://lmd.zhijiandao.cn

Py:   def total(*args): return sum(args)
来源：http://aij.gogol.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uhr.yuanzhike.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mpb.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://plo.hywenlv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://okz.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wia.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://gne.yvedp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wyn.hammf.cn

[C04] 命名参数 / 关键字参数
来源：http://one.hysaishi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jvv.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://knl.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gfm.ybcxt.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://guf.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://zle.hongshengwenyu.top

Go:   // 无：用配置结构体参数
来源：http://vho.jinqigufen.top

Ruby: f(a: 1, b: 2)
来源：http://gsc.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://pxs.sufxvd.cn

[C05] 返回多个值
来源：http://lwa.shzxlz.cn

Py:   return a, b
来源：http://noi.hysaishi.cn

PHP:  return [$a, $b];
来源：http://rim.tanke756.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ghh.gogol.net.cn

TS:   return { a, b };
来源：http://pcz.0kj1m.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gvq.quarkkingdee.top

Go:   return a, b
来源：http://sfi.uphjek.com

Ruby: return a, b
来源：http://yxf.xinyue.icu

C#:   return (a, b);              // ValueTuple
来源：http://jiq.xingfuxueyuan.xyz

[C06] 匿名函数 / lambda
来源：http://jpm.yongpay.top

Py:   square = lambda x: x * x
来源：http://ytl.ybcxt.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dut.fengsongda.top

JS:   const square = x => x * x;
来源：http://uin.jyoumei.cn

TS:   const square = (x: number): number => x * x;
来源：http://xho.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ibx.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://hyw.sxryk.cn

Ruby: square = ->(x) { x * x }
来源：http://hly.chenzaomai.com

C#:   Func<int, int> square = x => x * x;
来源：http://oxs.zhengqikj.top

[C07] 把函数作为参数传入
来源：http://iyy.yuanzhike.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zqx.ydjk.org.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jrw.sxryk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://amx.redwolf501.top

TS:   arr.map(String)
来源：http://kum.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://esl.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ufm.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://yvu.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yfg.hnqzz.top

[C08] 闭包
来源：http://fkn.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ukp.pycfn.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bwa.yongpay.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rxq.guowangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pus.daxiang520.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sjb.fanxiaobao.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iei.dashuyun.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qfr.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qzn.gaohongyu789.top

[C09] 递归
来源：http://wfq.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ost.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cke.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oca.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lmp.cashguo.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mvl.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tkp.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://how.aibaodan.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bii.zdbjq.cn

[C10] 变量作用域
来源：http://uxo.fanxiaobao.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wzj.fktsv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fvw.chenlongwang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://woa.wangshuangyany.cn

TS:   同 JS
来源：http://ztl.zhijiandao.cn

Java: 方法内为块级作用域
来源：http://kfg.smart0.xyz

Go:   花括号块级作用域
来源：http://gtx.guannengcc.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qsx.iojbl.cn

C#:   块级作用域
来源：http://usa.9152youxi.cn

[C11] 模块导入与导出
来源：http://faf.sweek.top

Py:   from module import func
来源：http://rdy.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://iwd.fengsongda.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pts.9152youxi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dfn.jyoumei.cn

Java: import java.util.List;
来源：http://sfc.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jca.hcnkem.com

Ruby: require "json"; require_relative "./util"
来源：http://tpi.yfazqb.com

C#:   using System.Text;
来源：http://qyp.ydzc1.top

[C12] 立即执行函数 IIFE
来源：http://zuv.shangyingyoupin.top

Py:   (lambda: print("run"))()
来源：http://eyw.yvedp.cn


<!-- 参考信息 -->