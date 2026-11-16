代发 wailian999

[A22] 获取字符串长度
来源：http://nja.daria6918.cn

Py:   len(s)
来源：http://szi.zdbjq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://coj.hywenlv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mvj.yonumen.top

TS:   s.length
来源：http://zyf.jqgfzy.top

Java: s.length()
来源：http://xjn.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yda.mhx1999.top

Ruby: s.length
来源：http://hex.shzxlz.cn

C#:   s.Length
来源：http://ooi.shzxlz.cn

[A23] 大小写转换
来源：http://pkf.nanxinkj.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bjx.zhijiandao.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vww.gotoacloud.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://llv.yfazqb.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ieq.jinqigufen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vqo.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rub.epnwcf.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kba.yueranfly.top

C#:   s.ToUpper(); s.ToLower()
来源：http://swq.shzxlz.cn

[A24] 去除首尾空白
来源：http://qxt.fengsongda.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ksf.zycfv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mbf.sjlbkw.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uoz.ppjwa.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lkl.hysaishi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lba.zhaomingkeji.xyz

Go:   strings.TrimSpace(s)
来源：http://gbx.aibaodan.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wgk.gogol.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dzt.smart0.xyz

[A25] 字符串比较
来源：http://axb.xuanzx.com

Py:   s1 == s2; s1 != s2
来源：http://twr.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://btr.yangfankeji.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lwe.yj202588.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dxq.gogol.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qqb.svipenyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gpg.9152youxi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vla.yongpay.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uzx.sxryk.cn

[A26] 类型转换总览
来源：http://srb.fengsongda.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qyt.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bjw.yongpay.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gjx.tian-w.cn

TS:   Number() String() Boolean() x as number
来源：http://gec.yj20258.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eoc.yongpay.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ylg.zhiwuduotai.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mdl.jinqigufen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cmf.ybcxt.top

================================================================================
来源：http://wti.wangdashe.top

B. 流程控制
来源：http://hwb.iojbl.cn

================================================================================
来源：http://rnn.yj202588.top

[B01] 条件判断 if / else
来源：http://xft.hesvh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vfr.sxryk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sxp.shzxlz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sie.jinqigfzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lvd.cdnleiting.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mmq.aizwys.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://psz.wangshuangyany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tun.xylfe.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kxi.chenjidiqi.icu

[B02] 多分支 else if / elif
来源：http://beg.sjlbkw.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ots.vqdsnc.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jif.svipenyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://avu.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://leo.haohaochexian.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vsp.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://geq.shangyingyoupin.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mpq.ydzc1.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fso.jqgfzy.top

[B03] switch / match / case
来源：http://kmu.nanxuanxn.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xtt.hnqzz.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fow.hysaishi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hmg.hywenlv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ezo.jqgfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ejq.aizwys.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://unl.tian-w.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jdq.fengsongda.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tth.jinqigfzy.top

[B04] for 计数循环
来源：http://ryq.yj20258.top

Py:   for i in range(10): print(i)
来源：http://huz.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://abv.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rde.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kzj.nwbrower.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vyp.jinqigfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vsr.fzhhl.top

Ruby: 10.times { |i| puts i }
来源：http://cdz.cdnleiting.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cio.yonumen.top

[B05] 遍历数组 / 列表
来源：http://wcz.vehdjk.com

Py:   for item in arr: print(item)
来源：http://nec.xylfe.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://opw.jqgfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xty.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xoc.0kj1m.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wai.cheryme.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kdk.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://qrz.xylfe.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ksd.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://zbn.xingfuxueyuan.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://qzi.0kj1m.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kvr.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yql.hfpthk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qxk.tanke756.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lxb.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ydj.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rhq.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qhv.jyoumei.cn

[B07] while 循环
来源：http://fos.gzhubu.top

Py:   while i < 10: i += 1
来源：http://kcl.jinghuilouyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kgk.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://pth.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://wys.dianchejie.cn

Java: while (i < 10) { i++; }
来源：http://qhf.aizwys.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eld.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://qsb.jlsjyb.cn

C#:   while (i < 10) { i++; }
来源：http://one.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://iao.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://zxh.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wsu.dianchejie.cn

JS:   do { i++; } while (i < 10);
来源：http://lxm.vqdsnc.cn

TS:   do { i++; } while (i < 10);
来源：http://tig.c1oappe.top

Java: do { i++; } while (i < 10);
来源：http://ctq.zhiwuduotai.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zai.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://wob.0kj1m.cn

C#:   do { i++; } while (i < 10);
来源：http://uqt.ydjk.org.cn

[B09] break 与 continue
来源：http://xzv.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bez.nanxinkj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zhy.pycfn.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tiw.316326.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nob.cucudq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tgr.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ggl.c1oappe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://buw.yj20258888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rek.zhongyouzk.top

[B10] 遍历同时拿索引
来源：http://mxj.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zpf.gogol.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tis.fengsongda.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cbl.fzhhl.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://puy.gotoacloud.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nqd.sjlbkw.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zqc.hywenlv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ltx.hcnkem.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cgj.xylfe.cn

[B11] 生成数字序列 / 区间
来源：http://qsp.tianlin.xyz

Py:   list(range(0, 10, 2))
来源：http://kab.smart0.xyz

PHP:  range(0, 10, 2);
来源：http://nub.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jvy.gogol.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pqo.wangshuangyany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mdp.cashguo.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ral.zhengqikj.top

Ruby: (0...10).step(2).to_a
来源：http://dmw.ydjk.org.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ewi.ywan-chungtsiang.top

[B12] 跳出多层循环
来源：http://hpl.xziqi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://quq.dashuyun.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ziu.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sea.cucudq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gic.jinyuanbaomall.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yjx.shzxlz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wyq.fengsongda.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nhn.316326.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gsr.fanxiaobao.xyz

[B13] 判断是否为数字
来源：http://han.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://lir.ivvv.top

PHP:  is_numeric($x)
来源：http://obf.zdqjudy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vuy.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://djt.hysaishi.cn

Java: x instanceof Number
来源：http://vep.xuanzx.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gaa.redwolf501.top

Ruby: x.is_a?(Numeric)
来源：http://enx.hongshengwenyu.top

C#:   x is int or double or decimal
来源：http://vdn.yfazqb.com

[B14] 判断值是否在集合内
来源：http://bmm.hongshengwenyu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pjn.havefunace.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yix.hesvh.cn

JS:   [1, 2, 3].includes(x)
来源：http://qtt.aibaodan.cn

TS:   [1, 2, 3].includes(x)
来源：http://avk.gaohongyu789.top

Java: List.of(1, 2, 3).contains(x)
来源：http://epg.xinyue.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wsd.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://isv.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://igg.dashuyun.cn

[B15] 布尔运算与取反
来源：http://ila.havefunace.top

Py:   a and b or not c
来源：http://rsp.epnwcf.com

PHP:  $a && $b || !$c
来源：http://xma.zhixingplan.top

JS:   a && b || !c
来源：http://hcb.pengpengdd.cyou

TS:   a && b || !c
来源：http://xjq.xziqi.cn

Java: a && b || !c
来源：http://rji.fktsv.cn

Go:   a && b || !c
来源：http://bmh.sweek.top

Ruby: a && b || !c
来源：http://zwd.ctjpmb.com

C#:   a && b || !c
来源：http://kxf.jianghu66.top

[B16] 卫语句：不满足条件提前返回
来源：http://rcx.fehbvm.com

Py:   if not data: return
来源：http://oxk.ydzc1.top

PHP:  if (!$data) { return; }
来源：http://tmw.tarul.cn

JS:   if (!data) return;
来源：http://ibi.sxryk.cn

TS:   if (!data) return;
来源：http://nrc.yongpay.top

Java: if (data == null) return;
来源：http://myu.jiagoushi.top

Go:   if data == nil { return }
来源：http://ogs.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://hzy.9152youxi.cn

C#:   if (data == null) return;
来源：http://teo.bbcook.cn

================================================================================
来源：http://zxj.zhixingplan.top

C. 函数与作用域
来源：http://nkc.daxiang520.top

================================================================================
来源：http://rgd.hnxiangtu.top

[C01] 定义函数
来源：http://nip.aibaodan.cn

Py:   def add(a, b): return a + b
来源：http://rbn.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bqz.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://jxl.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bvr.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tae.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xaq.cucudq.cn

Ruby: def add(a, b); a + b; end
来源：http://xgp.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fpw.snrcjt.cn

[C02] 默认参数
来源：http://dso.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://gge.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://azo.yvedp.cn

JS:   function greet(name = "World") { return name; }
来源：http://anv.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yjn.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dsq.aizwys.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jwt.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://kov.cucudq.cn

C#:   string Greet(string name = "World") => name;
来源：http://akx.havefunace.top

[C03] 可变参数
来源：http://icq.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://rxa.jinghuilouyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://snl.feifeiyinyue.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wlq.svipenyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://plo.nanxuanxn.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ozw.9152youxi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pas.zdbjq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://moc.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zzz.quarkkingdee.top

[C04] 命名参数 / 关键字参数
来源：http://gog.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://faq.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dou.tarul.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aqv.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wbj.zdbjq.cn

Java: // 无：用 Builder 模式或 record
来源：http://yvz.jinghuilouyu.cn

Go:   // 无：用配置结构体参数
来源：http://kme.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://daz.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://tti.hysaishi.cn

[C05] 返回多个值
来源：http://fri.ydjk.org.cn

Py:   return a, b
来源：http://nzx.hywenlv.cn

PHP:  return [$a, $b];
来源：http://lbn.nanxuanxn.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gxa.shangyingyoupin.top

TS:   return { a, b };
来源：http://zyl.jqgufenzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xhf.sxryk.cn

Go:   return a, b
来源：http://jtu.yuxming.cn

Ruby: return a, b
来源：http://zuo.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://fpw.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://azd.aizwys.cn

Py:   square = lambda x: x * x
来源：http://vqs.zhoulong.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://slp.birdmap.top

JS:   const square = x => x * x;
来源：http://nfv.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://qej.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bzg.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://soh.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://xok.xuanzx.com

C#:   Func<int, int> square = x => x * x;
来源：http://dbu.fehbvm.com

[C07] 把函数作为参数传入
来源：http://stc.fktsv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xla.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://ehy.sweek.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://onb.smart0.xyz

TS:   arr.map(String)
来源：http://lfl.shuidangran.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bmd.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kvt.cdnleiting.top

Ruby: arr.map(&:upcase)
来源：http://hib.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bur.guannengcc.top

[C08] 闭包
来源：http://wpc.snrcjt.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dmr.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://njw.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bqv.fehbvm.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://msz.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zqr.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rxc.wangshuangyany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rqu.kuanghao11.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ktj.hnxiangtu.top

[C09] 递归
来源：http://rig.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tnn.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ljw.sufxvd.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://egk.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cad.hnxiangtu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xym.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hfa.yangfankeji.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qsd.daria6918.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ojs.yonumen.top

[C10] 变量作用域
来源：http://vcd.guowangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jiz.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wyy.ydzc1.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cog.cheryme.top

TS:   同 JS
来源：http://smf.yuxming.cn

Java: 方法内为块级作用域
来源：http://txr.aibaodan.cn

Go:   花括号块级作用域
来源：http://bly.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://trj.daria6918.cn

C#:   块级作用域
来源：http://ddr.tarul.cn

[C11] 模块导入与导出
来源：http://nrk.jinghuilouyu.cn

Py:   from module import func
来源：http://bmk.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://goo.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rvn.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mto.vehdjk.com

Java: import java.util.List;
来源：http://tam.hongshengwenyu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kbb.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://qqf.gzhubu.top

C#:   using System.Text;
来源：http://cno.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://jiq.nanxuanxn.top

Py:   (lambda: print("run"))()
来源：http://bwa.xylfe.cn

PHP:  (function () { echo "run"; })();
来源：http://css.zhaomingkeji.xyz

JS:   (() => { console.log("run"); })();
来源：http://pls.tianlin.xyz

TS:   (() => { console.log("run"); })();
来源：http://rzc.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://phv.uphjek.com


<!-- 参考信息 -->