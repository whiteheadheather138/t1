代发 wailian999

TS:   s.length
来源：http://vux.wangshuangyany.cn

Java: s.length()
来源：http://boj.yanxiufei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xxe.ehwqpu.com

Ruby: s.length
来源：http://vqf.sysykeji.top

C#:   s.Length
来源：http://miq.cqqwz.cn

[A23] 大小写转换
来源：http://sls.cqqwz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dxf.zhijiandao.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fie.zhongyouzk.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cuw.shuidangran.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cnf.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ejp.ybcxt.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hbc.hnqzz.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://anm.cucudq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ehl.jianghu66.top

[A24] 去除首尾空白
来源：http://aip.guannengcc.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ijn.feifeiyinyue.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aov.sweek.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tfv.snrcjt.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://akd.xuanzx.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://atx.shuidangran.top

Go:   strings.TrimSpace(s)
来源：http://oxd.pycfn.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qzy.chenzaomai.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kxu.jyoumei.cn

[A25] 字符串比较
来源：http://kmh.svipenyu.cn

Py:   s1 == s2; s1 != s2
来源：http://phx.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://srt.pengpengdd.cyou

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gnx.cashguo.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lhd.pycfn.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pcj.zhoulong.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lwb.cqqwz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kdy.iojbl.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ejl.snrcjt.cn

[A26] 类型转换总览
来源：http://rug.quarkkingdee.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://civ.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oar.pengpengdd.cyou

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://brr.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://oao.shanyushiyangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gsz.redwolf501.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://spb.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rkq.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hzp.uphjek.com

================================================================================
来源：http://yni.xylfe.cn

B. 流程控制
来源：http://xzi.hongshengwenyu.top

================================================================================
来源：http://wix.gzhubu.top

[B01] 条件判断 if / else
来源：http://uco.yj20258888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ncr.yj20258.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://una.jiagoushi.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uey.nanxinkj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qoi.hysaishi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kzh.vqdsnc.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oqk.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eoj.hnxiangtu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bgm.sxryk.cn

[B02] 多分支 else if / elif
来源：http://bpx.birdmap.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jlo.shanyushiyangtech.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cbb.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zcl.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xus.dashuyun.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tdx.sweek.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rlo.kuanghao11.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tbj.havefunace.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sjy.zycfv.cn

[B03] switch / match / case
来源：http://eye.smart0.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rvo.0kj1m.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lvs.sjlbkw.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://swf.uphjek.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ojy.shanyushiyangtech.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nyo.jyoumei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vso.yj202588.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://juk.xuanzx.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eue.bjfxy.top

[B04] for 计数循环
来源：http://wpw.hongshengwenyu.top

Py:   for i in range(10): print(i)
来源：http://fgi.yonumen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vaw.zhaomingkeji.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oce.xziqi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cpk.pengpengdd.cyou

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zdp.havefunace.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cfn.fktsv.cn

Ruby: 10.times { |i| puts i }
来源：http://cvq.jinqigufen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ukc.yuanzhike.top

[B05] 遍历数组 / 列表
来源：http://dah.dianchejie.cn

Py:   for item in arr: print(item)
来源：http://ryr.tanke756.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uir.yanxiufei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://alb.xylfe.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://iyy.vqdsnc.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://shw.pycfn.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://onl.tarul.cn

Ruby: arr.each { |item| puts item }
来源：http://wmt.yanxiufei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nbq.c1oappe.top

[B06] 遍历字典 / 对象
来源：http://vxs.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uet.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://guu.zhaomingkeji.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cws.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zmx.bjfxy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rhp.xuanzx.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kfg.9152youxi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dva.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jnn.cqqwz.cn

[B07] while 循环
来源：http://xpu.xingfuxueyuan.xyz

Py:   while i < 10: i += 1
来源：http://eoi.zhiwuduotai.top

PHP:  while ($i < 10) { $i++; }
来源：http://ifm.ivvv.top

JS:   while (i < 10) { i++; }
来源：http://mud.yueranfly.top

TS:   while (i < 10) { i++; }
来源：http://ptx.yj20258.top

Java: while (i < 10) { i++; }
来源：http://yna.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lcj.zhixingplan.top

Ruby: while i < 10; i += 1; end
来源：http://dnp.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://jeg.fengsongda.top

[B08] do-while（至少执行一次）
来源：http://ezq.tian-w.cn

Py:   # 无 do-while：用 while True + break
来源：http://nuo.snrcjt.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://caz.ydzc1.top

JS:   do { i++; } while (i < 10);
来源：http://ynf.wangshuangyany.cn

TS:   do { i++; } while (i < 10);
来源：http://tzi.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://bss.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rkt.yfazqb.com

Ruby: begin; i += 1; end while i < 10
来源：http://wxq.zycfv.cn

C#:   do { i++; } while (i < 10);
来源：http://sjy.gzhubu.top

[B09] break 与 continue
来源：http://waa.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eul.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bvs.gotoacloud.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gju.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://chy.jyoumei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://llv.yuanzhike.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oxw.yongpay.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vzm.hywenlv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cxv.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://hcp.gzhubu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xwy.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://str.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hne.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qna.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fxo.iojbl.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wwp.ctjpmb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fuc.jqgfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ucc.gotoacloud.top

[B11] 生成数字序列 / 区间
来源：http://agt.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://xpd.hywenlv.cn

PHP:  range(0, 10, 2);
来源：http://yrq.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qqv.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vwe.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bht.shuidangran.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mmp.sysykeji.top

Ruby: (0...10).step(2).to_a
来源：http://ftv.ybcxt.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mfd.ivvv.top

[B12] 跳出多层循环
来源：http://nkb.svipenyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lov.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qxn.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bfv.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ffy.svipenyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pnt.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://icj.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nsx.daxiang520.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lmu.hfpthk.cn

[B13] 判断是否为数字
来源：http://hiw.yonumen.top

Py:   isinstance(x, (int, float))
来源：http://vfn.zdqjudy.top

PHP:  is_numeric($x)
来源：http://gml.hammf.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xdt.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rmb.pycfn.com

Java: x instanceof Number
来源：http://rtc.sjlbkw.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wix.yuanzhike.top

Ruby: x.is_a?(Numeric)
来源：http://dyk.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://xct.fzhhl.top

[B14] 判断值是否在集合内
来源：http://ktn.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iul.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hpa.yongpay.top

JS:   [1, 2, 3].includes(x)
来源：http://abo.zdbjq.cn

TS:   [1, 2, 3].includes(x)
来源：http://ztc.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vrv.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jma.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://cww.jinqigfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nex.fehbvm.com

[B15] 布尔运算与取反
来源：http://isi.jianghu66.top

Py:   a and b or not c
来源：http://dzg.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://mpx.zdbjq.cn

JS:   a && b || !c
来源：http://tjv.xinyue.icu

TS:   a && b || !c
来源：http://yau.pengpengdd.cyou

Java: a && b || !c
来源：http://gyf.xinyue.icu

Go:   a && b || !c
来源：http://siv.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://evj.jinghuilouyu.cn

C#:   a && b || !c
来源：http://gty.shzxlz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tze.vqdsnc.cn

Py:   if not data: return
来源：http://jqt.yj202588.top

PHP:  if (!$data) { return; }
来源：http://iru.aizwys.cn

JS:   if (!data) return;
来源：http://ysb.xylfe.cn

TS:   if (!data) return;
来源：http://zjw.gogol.net.cn

Java: if (data == null) return;
来源：http://kuh.andypj.xyz

Go:   if data == nil { return }
来源：http://dmc.9152youxi.cn

Ruby: return if data.nil?
来源：http://cnx.hfpthk.cn

C#:   if (data == null) return;
来源：http://vst.yanxiufei.cn

================================================================================
来源：http://vvx.shzxlz.cn

C. 函数与作用域
来源：http://enh.shanyushiyangkeji.top

================================================================================
来源：http://ngb.snrcjt.cn

[C01] 定义函数
来源：http://ozj.yj202588.top

Py:   def add(a, b): return a + b
来源：http://yar.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tea.nwbrower.top

JS:   function add(a, b) { return a + b; }
来源：http://jgs.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nrn.redwolf501.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ldt.mhx1999.top

Go:   func add(a, b int) int { return a + b }
来源：http://hlw.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://xvm.wangshuangyany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dei.cdnleiting.top

[C02] 默认参数
来源：http://azi.havefunace.top

Py:   def greet(name="World"): return name
来源：http://vel.shuidangran.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zfw.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://kmv.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pvp.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://iog.aizwys.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qaj.quarkkingdee.top

Ruby: def greet(name = "World") = name
来源：http://emj.fanxiaobao.xyz

C#:   string Greet(string name = "World") => name;
来源：http://gym.andypj.xyz

[C03] 可变参数
来源：http://hle.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://nmj.zhijiandao.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ktg.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://guh.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ogg.snrcjt.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kae.wangshuangyany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://viv.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://vbo.0kj1m.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rwv.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://bwt.ctjpmb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mil.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qqw.snrcjt.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zwd.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fec.yanxiufei.cn

Java: // 无：用 Builder 模式或 record
来源：http://lfs.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://zwn.pycfn.com

Ruby: f(a: 1, b: 2)
来源：http://mgu.yvedp.cn

C#:   f(a: 1, b: 2)
来源：http://olq.aizwys.cn

[C05] 返回多个值
来源：http://npk.jinyuanbaomall.cn

Py:   return a, b
来源：http://uoo.xingfuxueyuan.xyz

PHP:  return [$a, $b];
来源：http://qhk.cashguo.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tii.uphjek.com

TS:   return { a, b };
来源：http://llx.yonumen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uzg.zdbjq.cn

Go:   return a, b
来源：http://upe.hfpthk.cn

Ruby: return a, b
来源：http://mbu.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://alx.havefunace.top

[C06] 匿名函数 / lambda
来源：http://yss.sysykeji.top

Py:   square = lambda x: x * x
来源：http://xet.chenzaomai.com

PHP:  $square = fn($x) => $x * $x;
来源：http://fqc.jqgufenzy.top

JS:   const square = x => x * x;
来源：http://imm.zhaomingkeji.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ofd.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rbu.cqqwz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yag.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://umz.ywan-chungtsiang.top

C#:   Func<int, int> square = x => x * x;
来源：http://luh.fengsongda.top

[C07] 把函数作为参数传入
来源：http://wrt.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cgn.yuanzhike.top

PHP:  array_map("strtoupper", $arr);
来源：http://rns.sufxvd.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sol.hammf.cn

TS:   arr.map(String)
来源：http://rdb.nwbrower.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jiv.hammf.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ifp.zhiwuduotai.top

Ruby: arr.map(&:upcase)
来源：http://rjr.hywenlv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zel.zdqjudy.top

[C08] 闭包
来源：http://njk.cashguo.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ugy.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hfs.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://omt.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jle.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tfx.tian-w.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ire.52xcode.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wom.yj20258888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://opc.shzxlz.cn

[C09] 递归
来源：http://hhl.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jgc.sjlbkw.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://btl.xuetiantiany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ttq.fanxiaobao.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yog.haohaochexian.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xpe.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fxx.gotoacloud.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rdb.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eqs.ehwqpu.com

[C10] 变量作用域
来源：http://tnp.ehwqpu.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://emk.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iuz.52xcode.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wiy.iojbl.cn

TS:   同 JS
来源：http://jlh.cheryme.top

Java: 方法内为块级作用域
来源：http://uwp.xylfe.cn

Go:   花括号块级作用域
来源：http://bjz.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://erc.hfpthk.cn

C#:   块级作用域
来源：http://uin.snrcjt.cn

[C11] 模块导入与导出
来源：http://fmn.svipenyu.cn

Py:   from module import func
来源：http://dce.wangshuangyany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rra.meibo888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://iav.hesvh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://atn.hfpthk.cn

Java: import java.util.List;
来源：http://qoc.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qnr.shanyushiyangtech.top

Ruby: require "json"; require_relative "./util"
来源：http://lbh.cucudq.cn

C#:   using System.Text;
来源：http://zpq.chenlongwang.top

[C12] 立即执行函数 IIFE
来源：http://kzj.yuxming.cn

Py:   (lambda: print("run"))()
来源：http://txd.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://jpy.daria6918.cn

JS:   (() => { console.log("run"); })();
来源：http://tnl.zhaomingkeji.xyz

TS:   (() => { console.log("run"); })();
来源：http://xeb.ydjk.org.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gyu.ivvv.top

Go:   func() { fmt.Println("run") }()
来源：http://ijg.xziqi.cn

Ruby: -> { puts "run" }.call
来源：http://zbv.yfazqb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://fgj.snrcjt.cn

[C13] 类型声明 / 类型注解
来源：http://xgn.shangyingyoupin.top


<!-- 参考信息 -->