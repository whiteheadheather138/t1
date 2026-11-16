代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://ocp.cqqwz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://utv.zhijiandao.cn

JS:   (3.14159).toFixed(2)
来源：http://jyq.fktsv.cn

TS:   (3.14159).toFixed(2)
来源：http://bnp.yuanzhike.top

Java: String.format("%.2f", 3.14159)
来源：http://ydp.sweek.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rub.316326.xyz

Ruby: format("%.2f", 3.14159)
来源：http://xrm.jiagoushi.top

C#:   3.14159.ToString("F2")
来源：http://sqz.hywenlv.cn

[A22] 获取字符串长度
来源：http://vie.chenjidiqi.icu

Py:   len(s)
来源：http://cpx.feifeiyinyue.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wce.fanxiaobao.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uvv.jqgufenzy.top

TS:   s.length
来源：http://vzo.yangfankeji.com

Java: s.length()
来源：http://jwf.fzhhl.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wqr.hnqzz.top

Ruby: s.length
来源：http://zzv.yueranfly.top

C#:   s.Length
来源：http://pny.snrcjt.cn

[A23] 大小写转换
来源：http://ksn.hnxiangtu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kck.jinyuanbaomall.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ckp.sufxvd.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tzo.shanyushiyangtech.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fzc.0kj1m.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tdo.cashguo.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wbv.sjlbkw.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kcd.sxryk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wbx.jinyuanbaomall.cn

[A24] 去除首尾空白
来源：http://iyg.quarkkingdee.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://srf.tian-w.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://etf.hnqzz.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jxm.fktsv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://che.c1oappe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bvg.gogol.net.cn

Go:   strings.TrimSpace(s)
来源：http://ksy.chenlongwang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://chd.mhx1999.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yha.hcnkem.com

[A25] 字符串比较
来源：http://eov.xuetiantiany.cn

Py:   s1 == s2; s1 != s2
来源：http://atp.sysykeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cqe.daxiang520.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eyq.cqqwz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zqr.gogol.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qjo.ydjk.org.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uma.xziqi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ued.xuanzx.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uhv.xziqi.cn

[A26] 类型转换总览
来源：http://fnd.pengpengdd.cyou

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cnb.cdnleiting.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wkc.haohaochexian.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://evs.shangyingyoupin.top

TS:   Number() String() Boolean() x as number
来源：http://gzm.tanke756.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tbk.wangshuangyany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://typ.fktsv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yos.ydzc1.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jdl.jinqigfzy.top

================================================================================
来源：http://ccx.hnqzz.top

B. 流程控制
来源：http://dlp.bjfxy.top

================================================================================
来源：http://khd.haohaochexian.top

[B01] 条件判断 if / else
来源：http://gch.cheryme.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kxl.andypj.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sdj.hcnkem.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gvo.birdmap.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hlo.jlsjyb.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hoy.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qdc.sufxvd.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nnr.zhongyouzk.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zjv.feifeiyinyue.top

[B02] 多分支 else if / elif
来源：http://xig.andypj.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ouf.jinqigfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fdz.0kj1m.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xtc.hnxiangtu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ffr.shanyushiyangtech.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lou.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hbp.havefunace.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ins.zycfv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aod.wangshuangyany.cn

[B03] switch / match / case
来源：http://ivp.shanyushiyangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qhi.gotoacloud.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://crz.wangdashe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fyf.fktsv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dqa.zhaomingkeji.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lwx.havefunace.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eaz.yangfankeji.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bqf.ehwqpu.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zoo.nanxuanxn.top

[B04] for 计数循环
来源：http://thg.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://kiw.zhongyouzk.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://llp.haohaochexian.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cug.nanxuanxn.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://npw.redwolf501.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jbw.bbcook.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gcy.guowangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://pkl.hywenlv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fxh.fanxiaobao.xyz

[B05] 遍历数组 / 列表
来源：http://qlw.316326.xyz

Py:   for item in arr: print(item)
来源：http://udp.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bul.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sjp.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fjo.gogol.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wwt.yuanzhike.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vmd.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://arr.hysaishi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://swk.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://ott.tian-w.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tnp.jiagoushi.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ohv.zhixingplan.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lta.zhengqikj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://igb.jlsjyb.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://boq.ivvv.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kbf.fehbvm.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nsm.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xrp.haohaochexian.top

[B07] while 循环
来源：http://dwy.sufxvd.cn

Py:   while i < 10: i += 1
来源：http://gco.cheryme.top

PHP:  while ($i < 10) { $i++; }
来源：http://dnl.bbcook.cn

JS:   while (i < 10) { i++; }
来源：http://vpf.fktsv.cn

TS:   while (i < 10) { i++; }
来源：http://wqn.yj20258.top

Java: while (i < 10) { i++; }
来源：http://ovh.hysaishi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fvd.fzhhl.top

Ruby: while i < 10; i += 1; end
来源：http://hby.yfazqb.com

C#:   while (i < 10) { i++; }
来源：http://chv.jiagoushi.top

[B08] do-while（至少执行一次）
来源：http://ahe.ybcxt.top

Py:   # 无 do-while：用 while True + break
来源：http://zmj.yvedp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nxt.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://hne.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://iyx.hongshengwenyu.top

Java: do { i++; } while (i < 10);
来源：http://oyq.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tfl.fanxiaobao.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://jzn.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://ubo.fzhhl.top

[B09] break 与 continue
来源：http://uty.tanke756.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://urh.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iui.yuanzhike.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kyh.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://quk.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eye.feifeiyinyue.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://azr.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tbo.svipenyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cka.nanxuanxn.top

[B10] 遍历同时拿索引
来源：http://lhg.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tbr.yangfankeji.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bcn.zdbjq.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jgv.xuanzx.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dtm.jlsjyb.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bqu.aizwys.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gks.hesvh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ptm.tarul.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://woj.haohaochexian.top

[B11] 生成数字序列 / 区间
来源：http://afb.sysykeji.top

Py:   list(range(0, 10, 2))
来源：http://ijj.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://yyi.ywan-chungtsiang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ytr.hnxiangtu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ozk.yueranfly.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://scr.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qbt.fehbvm.com

Ruby: (0...10).step(2).to_a
来源：http://rab.birdmap.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dsz.smart0.xyz

[B12] 跳出多层循环
来源：http://pae.gzhubu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fza.mhx1999.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fnl.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dee.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cmw.yuxming.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hao.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yxj.zhengqikj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pqo.pycfn.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jpy.shangyingyoupin.top

[B13] 判断是否为数字
来源：http://udz.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://epr.bjfxy.top

PHP:  is_numeric($x)
来源：http://eua.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://seq.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://slr.yuxming.cn

Java: x instanceof Number
来源：http://fsp.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tko.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://dfg.hesvh.cn

C#:   x is int or double or decimal
来源：http://oot.shangyingyoupin.top

[B14] 判断值是否在集合内
来源：http://hkh.iojbl.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zor.yj20258888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vxx.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://kzb.hcnkem.com

TS:   [1, 2, 3].includes(x)
来源：http://jug.xingfuxueyuan.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://drg.yanxiufei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aaj.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://ped.hfpthk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kde.redwolf501.top

[B15] 布尔运算与取反
来源：http://fnn.birdmap.top

Py:   a and b or not c
来源：http://hbb.fzhhl.top

PHP:  $a && $b || !$c
来源：http://nyz.daria6918.cn

JS:   a && b || !c
来源：http://sxm.meibo888.top

TS:   a && b || !c
来源：http://ipa.tarul.cn

Java: a && b || !c
来源：http://dmv.chenzaomai.com

Go:   a && b || !c
来源：http://wyl.yvedp.cn

Ruby: a && b || !c
来源：http://sro.shuidangran.top

C#:   a && b || !c
来源：http://sot.tarul.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qrk.shanyushiyangtech.top

Py:   if not data: return
来源：http://noy.yvedp.cn

PHP:  if (!$data) { return; }
来源：http://ldt.xziqi.cn

JS:   if (!data) return;
来源：http://mvi.ybcxt.top

TS:   if (!data) return;
来源：http://dnx.jqgfzy.top

Java: if (data == null) return;
来源：http://fhx.guowangkeji.top

Go:   if data == nil { return }
来源：http://cif.vqdsnc.cn

Ruby: return if data.nil?
来源：http://hep.9152youxi.cn

C#:   if (data == null) return;
来源：http://nym.cdnleiting.top

================================================================================
来源：http://veh.yvedp.cn

C. 函数与作用域
来源：http://xyf.fanxiaobao.xyz

================================================================================
来源：http://cap.ydzc1.top

[C01] 定义函数
来源：http://tbp.daria6918.cn

Py:   def add(a, b): return a + b
来源：http://gpv.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nsf.smart0.xyz

JS:   function add(a, b) { return a + b; }
来源：http://dpz.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hwi.sysykeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wke.shangyingyoupin.top

Go:   func add(a, b int) int { return a + b }
来源：http://wce.zhaomingkeji.xyz

Ruby: def add(a, b); a + b; end
来源：http://ljg.shanyushiyangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oey.cqqwz.cn

[C02] 默认参数
来源：http://xsl.iojbl.cn

Py:   def greet(name="World"): return name
来源：http://lrr.yj202588.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tum.daria6918.cn

JS:   function greet(name = "World") { return name; }
来源：http://eyr.jinghuilouyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fzn.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rcv.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yar.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://urv.daria6918.cn

C#:   string Greet(string name = "World") => name;
来源：http://yia.tarul.cn

[C03] 可变参数
来源：http://uet.fzhhl.top

Py:   def total(*args): return sum(args)
来源：http://shz.yvedp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pqt.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sgb.yj202588.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pci.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jla.dashuyun.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gah.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://olu.gaohongyu789.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xds.zhixingplan.top

[C04] 命名参数 / 关键字参数
来源：http://qtn.cheryme.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kjf.havefunace.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xjt.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lle.hysaishi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tyt.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://cwn.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://uco.jinyuanbaomall.cn

Ruby: f(a: 1, b: 2)
来源：http://zfd.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://qdf.zhaomingkeji.xyz

[C05] 返回多个值
来源：http://uou.redwolf501.top

Py:   return a, b
来源：http://xfz.yj20258888.top

PHP:  return [$a, $b];
来源：http://scc.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://viu.yj20258888.top

TS:   return { a, b };
来源：http://myh.jinqigufen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vez.yuanzhike.top

Go:   return a, b
来源：http://xzh.daria6918.cn

Ruby: return a, b
来源：http://twq.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://qdo.pycfn.com

[C06] 匿名函数 / lambda
来源：http://nni.yj20258888.top

Py:   square = lambda x: x * x
来源：http://osx.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rez.fehbvm.com

JS:   const square = x => x * x;
来源：http://teh.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://lwz.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hyi.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://cro.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://rwo.hnxiangtu.top

C#:   Func<int, int> square = x => x * x;
来源：http://eqc.andypj.xyz

[C07] 把函数作为参数传入
来源：http://gme.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xdy.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://vmv.hywenlv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fvb.aibaodan.cn

TS:   arr.map(String)
来源：http://rvs.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uud.shangyingyoupin.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sjm.sweek.top

Ruby: arr.map(&:upcase)
来源：http://qxz.hfpthk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cfv.redwolf501.top

[C08] 闭包
来源：http://asb.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lkj.bjfxy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ece.smart0.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mcj.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sjm.cdnleiting.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ufp.zhengqikj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mwh.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uei.mhx1999.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://enp.iojbl.cn

[C09] 递归
来源：http://raz.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xqf.yanxiufei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uvo.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tke.gotoacloud.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xnj.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dbv.smart0.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aeo.ppjwa.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://afv.fktsv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://evg.tanke756.top

[C10] 变量作用域
来源：http://wlv.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fam.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qje.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jtr.yuxming.cn

TS:   同 JS
来源：http://gra.52xcode.cn

Java: 方法内为块级作用域
来源：http://tbv.fehbvm.com

Go:   花括号块级作用域
来源：http://cml.xziqi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hzi.shanyushiyangkeji.top

C#:   块级作用域
来源：http://ncs.0kj1m.cn

[C11] 模块导入与导出
来源：http://oya.chenjidiqi.icu

Py:   from module import func
来源：http://mpf.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://wmv.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dgs.zycfv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://joh.hnxiangtu.top

Java: import java.util.List;
来源：http://zdl.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qfw.nwbrower.top


<!-- 参考信息 -->