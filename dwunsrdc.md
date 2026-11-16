代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://scx.shuidangran.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mat.hfpthk.cn

JS:   (3.14159).toFixed(2)
来源：http://vyx.xuanzx.com

TS:   (3.14159).toFixed(2)
来源：http://uje.ydzc1.top

Java: String.format("%.2f", 3.14159)
来源：http://erh.aibaodan.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sox.cashguo.top

Ruby: format("%.2f", 3.14159)
来源：http://xjs.jiagoushi.top

C#:   3.14159.ToString("F2")
来源：http://zfo.hongshengwenyu.top

[A22] 获取字符串长度
来源：http://yta.9152youxi.cn

Py:   len(s)
来源：http://gjs.sweek.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://skq.wangdashe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ait.smart0.xyz

TS:   s.length
来源：http://tnb.yanxiufei.cn

Java: s.length()
来源：http://xoh.hammf.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xih.hesvh.cn

Ruby: s.length
来源：http://amy.mhx1999.top

C#:   s.Length
来源：http://jnt.chenzaomai.com

[A23] 大小写转换
来源：http://ygc.yvedp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kaj.jinqigufen.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yxp.fehbvm.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cib.ybcxt.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ebf.jinyuanbaomall.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tey.aibaodan.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mzt.xylfe.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wgw.chenlongwang.top

C#:   s.ToUpper(); s.ToLower()
来源：http://orj.316326.xyz

[A24] 去除首尾空白
来源：http://kow.sufxvd.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iin.yueranfly.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aiq.tian-w.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ewp.jqgfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ilz.nanxuanxn.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jpu.ydjk.org.cn

Go:   strings.TrimSpace(s)
来源：http://dqt.pengpengdd.cyou

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jwx.c1oappe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sul.hysaishi.cn

[A25] 字符串比较
来源：http://qeo.zhongyouzk.top

Py:   s1 == s2; s1 != s2
来源：http://oln.xziqi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wvq.xziqi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xqo.wangshuangyany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wch.jinqigfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nki.cdnleiting.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://amm.tian-w.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ukp.gaohongyu789.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sie.zhixingplan.top

[A26] 类型转换总览
来源：http://tlw.cheryme.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://imi.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ile.ivvv.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jck.yj202588.top

TS:   Number() String() Boolean() x as number
来源：http://tiu.cheryme.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bnc.xinyue.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://msn.zhiwuduotai.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gzz.havefunace.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zba.redwolf501.top

================================================================================
来源：http://dzt.havefunace.top

B. 流程控制
来源：http://dia.yuxming.cn

================================================================================
来源：http://zuz.cqqwz.cn

[B01] 条件判断 if / else
来源：http://xrs.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wkp.guannengcc.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zsz.chenzaomai.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vke.hnqzz.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lhq.havefunace.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fwr.shangyingyoupin.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wsq.jinqigfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mnb.wangshuangyany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://afi.cdnleiting.top

[B02] 多分支 else if / elif
来源：http://swt.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jxt.yuxming.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://thh.zycfv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xxz.jqgfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oui.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mdq.zdbjq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://syh.pycfn.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bec.jyoumei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nrc.ivvv.top

[B03] switch / match / case
来源：http://dno.yj202588.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uwc.52xcode.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://czl.nwbrower.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gjk.shzxlz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lvi.gzhubu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xal.gotoacloud.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hwt.birdmap.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pdg.daria6918.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sdy.yueranfly.top

[B04] for 计数循环
来源：http://npj.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://dph.tanke756.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rlq.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mjw.xingfuxueyuan.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://acm.meibo888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ezy.jlsjyb.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qzb.pengpengdd.cyou

Ruby: 10.times { |i| puts i }
来源：http://lyg.fanxiaobao.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mgp.vqdsnc.cn

[B05] 遍历数组 / 列表
来源：http://zhd.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://zrk.wangdashe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cvl.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yjq.guowangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nfd.sjlbkw.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yib.yongpay.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zjl.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://djr.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eqv.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://dkr.hesvh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://imx.ydzc1.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qeo.ywan-chungtsiang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ipc.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ipj.jianghu66.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cjz.wangshuangyany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ptz.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tdg.meibo888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fbp.uphjek.com

[B07] while 循环
来源：http://yul.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://rwg.pycfn.com

PHP:  while ($i < 10) { $i++; }
来源：http://cwz.sxryk.cn

JS:   while (i < 10) { i++; }
来源：http://zbi.daria6918.cn

TS:   while (i < 10) { i++; }
来源：http://gpg.birdmap.top

Java: while (i < 10) { i++; }
来源：http://knp.9152youxi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tzz.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://uvd.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://tbf.sjlbkw.cn

[B08] do-while（至少执行一次）
来源：http://zmk.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://zju.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kaz.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://uml.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://pww.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://law.hysaishi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nnv.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://kru.gogol.net.cn

C#:   do { i++; } while (i < 10);
来源：http://lei.mhx1999.top

[B09] break 与 continue
来源：http://eac.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mfb.zhengqikj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vpf.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://czj.316326.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xcy.cdnleiting.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zwx.yuxming.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oxm.iojbl.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xbd.pycfn.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzo.vqdsnc.cn

[B10] 遍历同时拿索引
来源：http://glq.yuxming.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wmg.uphjek.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qqk.yuxming.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pbm.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://czo.tianlin.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nfx.ivvv.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fqb.smart0.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ooj.ivvv.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yfa.zhongyouzk.top

[B11] 生成数字序列 / 区间
来源：http://izo.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://wav.daxiang520.top

PHP:  range(0, 10, 2);
来源：http://smq.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nbo.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aih.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qrl.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://all.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://atr.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zpu.hesvh.cn

[B12] 跳出多层循环
来源：http://fdo.snrcjt.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dsl.zhongyouzk.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cvf.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rvx.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tkm.zhixingplan.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ayr.quarkkingdee.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vtb.aizwys.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://leh.zhongyouzk.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://swt.xuanzx.com

[B13] 判断是否为数字
来源：http://hyh.sysykeji.top

Py:   isinstance(x, (int, float))
来源：http://zgf.cucudq.cn

PHP:  is_numeric($x)
来源：http://nkn.zdbjq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://emu.birdmap.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://irs.pycfn.com

Java: x instanceof Number
来源：http://dux.zhongyouzk.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://doc.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://nqn.redwolf501.top

C#:   x is int or double or decimal
来源：http://xbq.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://fvl.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jyo.jiagoushi.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fsu.nwbrower.top

JS:   [1, 2, 3].includes(x)
来源：http://fdk.zdqjudy.top

TS:   [1, 2, 3].includes(x)
来源：http://wzl.shuidangran.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rur.tian-w.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bvo.ehwqpu.com

Ruby: [1, 2, 3].include?(x)
来源：http://pul.epnwcf.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://crh.quarkkingdee.top

[B15] 布尔运算与取反
来源：http://ojg.guannengcc.top

Py:   a and b or not c
来源：http://jiw.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://bsk.jqgufenzy.top

JS:   a && b || !c
来源：http://vzr.cqqwz.cn

TS:   a && b || !c
来源：http://ffb.jinghuilouyu.cn

Java: a && b || !c
来源：http://nev.kuanghao11.cn

Go:   a && b || !c
来源：http://oht.meibo888.top

Ruby: a && b || !c
来源：http://spi.xylfe.cn

C#:   a && b || !c
来源：http://hhj.zhiwuduotai.top

[B16] 卫语句：不满足条件提前返回
来源：http://qty.52xcode.cn

Py:   if not data: return
来源：http://yvu.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://rgn.tanke756.top

JS:   if (!data) return;
来源：http://yto.jqgfzy.top

TS:   if (!data) return;
来源：http://don.jinghuilouyu.cn

Java: if (data == null) return;
来源：http://jnf.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://kec.yj202588.top

Ruby: return if data.nil?
来源：http://xsg.zycfv.cn

C#:   if (data == null) return;
来源：http://tvf.jianghu66.top

================================================================================
来源：http://asj.shangyingyoupin.top

C. 函数与作用域
来源：http://inq.c1oappe.top

================================================================================
来源：http://oyo.ydzc1.top

[C01] 定义函数
来源：http://igu.sjlbkw.cn

Py:   def add(a, b): return a + b
来源：http://hws.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ynl.tanke756.top

JS:   function add(a, b) { return a + b; }
来源：http://qfx.hongshengwenyu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tbu.cdnleiting.top

Java: static int add(int a, int b) { return a + b; }
来源：http://guf.zhixingplan.top

Go:   func add(a, b int) int { return a + b }
来源：http://peu.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://gew.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fsq.nwbrower.top

[C02] 默认参数
来源：http://nbt.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://rqg.xuanzx.com

PHP:  function greet($name = "World") { return $name; }
来源：http://lje.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://kjo.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://los.xinyue.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://fre.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tdm.sweek.top

Ruby: def greet(name = "World") = name
来源：http://hlu.guannengcc.top

C#:   string Greet(string name = "World") => name;
来源：http://pjp.zhengqikj.top

[C03] 可变参数
来源：http://ine.aizwys.cn

Py:   def total(*args): return sum(args)
来源：http://ihb.mhx1999.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qhl.ydjk.org.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rwy.quarkkingdee.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ixz.chenlongwang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://veo.shanyushiyangtech.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eym.ehwqpu.com

Ruby: def total(*nums); nums.sum; end
来源：http://qfl.cdnleiting.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aam.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://ubv.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lri.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bcg.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rqh.gaohongyu789.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://djx.ydjk.org.cn

Java: // 无：用 Builder 模式或 record
来源：http://xcz.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://pnr.shuidangran.top

Ruby: f(a: 1, b: 2)
来源：http://hvg.hnxiangtu.top

C#:   f(a: 1, b: 2)
来源：http://trx.vqdsnc.cn

[C05] 返回多个值
来源：http://gyu.jqgfzy.top

Py:   return a, b
来源：http://xgw.chenlongwang.top

PHP:  return [$a, $b];
来源：http://rbt.sweek.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gkp.sysykeji.top

TS:   return { a, b };
来源：http://bup.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://omp.dianchejie.cn

Go:   return a, b
来源：http://xlv.fktsv.cn

Ruby: return a, b
来源：http://qvt.sysykeji.top

C#:   return (a, b);              // ValueTuple
来源：http://vau.316326.xyz

[C06] 匿名函数 / lambda
来源：http://lpz.zhiwuduotai.top

Py:   square = lambda x: x * x
来源：http://rkz.bbcook.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jjt.jqgfzy.top

JS:   const square = x => x * x;
来源：http://hxn.yongpay.top

TS:   const square = (x: number): number => x * x;
来源：http://rjv.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fqb.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://jnh.jinyuanbaomall.cn

Ruby: square = ->(x) { x * x }
来源：http://qub.quarkkingdee.top

C#:   Func<int, int> square = x => x * x;
来源：http://xpu.zycfv.cn

[C07] 把函数作为参数传入
来源：http://krk.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ovl.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://acm.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vjj.jiagoushi.top

TS:   arr.map(String)
来源：http://jwx.svipenyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lnz.jinyuanbaomall.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kup.wangshuangyany.cn

Ruby: arr.map(&:upcase)
来源：http://quf.zhengqikj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://nde.guannengcc.top

[C08] 闭包
来源：http://rgx.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rfj.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ufd.cashguo.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://arm.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hyv.daxiang520.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mod.yj202588.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ybc.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ghz.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mnl.aizwys.cn

[C09] 递归
来源：http://ypi.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gqf.yueranfly.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://plk.c1oappe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ogx.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vsx.jinqigufen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ibn.9152youxi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://squ.yfazqb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mww.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tkc.pycfn.com

[C10] 变量作用域
来源：http://ibl.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uvm.chenjidiqi.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lql.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nly.ybcxt.top

TS:   同 JS
来源：http://ibc.fktsv.cn

Java: 方法内为块级作用域
来源：http://paf.gaohongyu789.top

Go:   花括号块级作用域
来源：http://umd.tarul.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tkw.aizwys.cn

C#:   块级作用域
来源：http://xny.xingfuxueyuan.xyz

[C11] 模块导入与导出
来源：http://bwu.zhijiandao.cn

Py:   from module import func
来源：http://usq.kuanghao11.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kjk.yj202588.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nhz.cheryme.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zls.yanxiufei.cn

Java: import java.util.List;
来源：http://ret.xylfe.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hwu.cdnleiting.top


<!-- 参考信息 -->