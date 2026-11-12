代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://yex.shanyushiyangtech.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eav.52xcode.cn

JS:   (3.14159).toFixed(2)
来源：http://pmh.yvedp.cn

TS:   (3.14159).toFixed(2)
来源：http://yvf.pycfn.com

Java: String.format("%.2f", 3.14159)
来源：http://nzw.aizwys.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cjj.zhaomingkeji.xyz

Ruby: format("%.2f", 3.14159)
来源：http://kes.fzhhl.top

C#:   3.14159.ToString("F2")
来源：http://xwv.andypj.xyz

[A22] 获取字符串长度
来源：http://evi.zhixingplan.top

Py:   len(s)
来源：http://ayn.daria6918.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ykg.zhiwuduotai.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ktr.uphjek.com

TS:   s.length
来源：http://isc.shangyingyoupin.top

Java: s.length()
来源：http://mzg.tianlin.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xfm.svipenyu.cn

Ruby: s.length
来源：http://upf.shangyingyoupin.top

C#:   s.Length
来源：http://ldn.xinyue.icu

[A23] 大小写转换
来源：http://osf.dianchejie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yaz.xingfuxueyuan.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tnq.yuanzhike.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zgx.hesvh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wdo.zhongyouzk.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gst.gaohongyu789.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pgc.ywan-chungtsiang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://obm.havefunace.top

C#:   s.ToUpper(); s.ToLower()
来源：http://prg.jinqigufen.top

[A24] 去除首尾空白
来源：http://sxy.hfpthk.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mgw.mhx1999.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jea.cqqwz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mtc.fehbvm.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bvz.svipenyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hkv.nanxinkj.top

Go:   strings.TrimSpace(s)
来源：http://rmp.xuanzx.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gjx.cucudq.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zix.yvedp.cn

[A25] 字符串比较
来源：http://qau.aibaodan.cn

Py:   s1 == s2; s1 != s2
来源：http://uio.uphjek.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gvs.shuidangran.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iyh.tian-w.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vej.xinyue.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mcr.ehwqpu.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bur.jinqigufen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://npk.shanyushiyangtech.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lqb.bbcook.cn

[A26] 类型转换总览
来源：http://wrg.haohaochexian.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hue.tian-w.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wdh.jyoumei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kmm.smart0.xyz

TS:   Number() String() Boolean() x as number
来源：http://xia.xuetiantiany.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://azk.svipenyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tfa.yongpay.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dpt.zycfv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nxm.mhx1999.top

================================================================================
来源：http://hew.wangdashe.top

B. 流程控制
来源：http://bhh.meibo888.top

================================================================================
来源：http://sba.mhx1999.top

[B01] 条件判断 if / else
来源：http://fsb.sufxvd.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cto.tianlin.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://crh.zhijiandao.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cwn.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://thg.chenjidiqi.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://mbm.sxryk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cap.yfazqb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kgz.feifeiyinyue.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ruc.yj20258.top

[B02] 多分支 else if / elif
来源：http://ckm.nwbrower.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pha.zhongyouzk.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qlu.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://moc.zdbjq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qpc.yongpay.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mur.mhx1999.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hil.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ppx.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lzl.ctjpmb.com

[B03] switch / match / case
来源：http://lnj.cashguo.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dsv.yonumen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cju.zhaomingkeji.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lwy.jyoumei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aip.nanxinkj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yvn.aibaodan.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tpt.316326.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ucx.yuanzhike.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nti.epnwcf.com

[B04] for 计数循环
来源：http://vkk.epnwcf.com

Py:   for i in range(10): print(i)
来源：http://qdi.zycfv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uil.jlsjyb.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pji.gaohongyu789.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vyp.c1oappe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bfw.jinghuilouyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wzf.snrcjt.cn

Ruby: 10.times { |i| puts i }
来源：http://pxi.zhongyouzk.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ydp.fehbvm.com

[B05] 遍历数组 / 列表
来源：http://hdj.quarkkingdee.top

Py:   for item in arr: print(item)
来源：http://lwf.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ayl.kuanghao11.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oww.tarul.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ccc.haohaochexian.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mpq.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://foz.haohaochexian.top

Ruby: arr.each { |item| puts item }
来源：http://nsu.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jeb.aibaodan.cn

[B06] 遍历字典 / 对象
来源：http://ivy.gotoacloud.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zkr.sxryk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zzx.zycfv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://msc.52xcode.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eeo.bbcook.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hqg.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xkl.fanxiaobao.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://poc.dianchejie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://csp.haohaochexian.top

[B07] while 循环
来源：http://ask.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://erz.zdqjudy.top

PHP:  while ($i < 10) { $i++; }
来源：http://hjb.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://cuw.yj20258.top

TS:   while (i < 10) { i++; }
来源：http://alc.pengpengdd.cyou

Java: while (i < 10) { i++; }
来源：http://yjr.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zpq.daria6918.cn

Ruby: while i < 10; i += 1; end
来源：http://aai.ydzc1.top

C#:   while (i < 10) { i++; }
来源：http://hqn.yonumen.top

[B08] do-while（至少执行一次）
来源：http://rcv.shanyushiyangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://ftk.jyoumei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://obi.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://ene.hongshengwenyu.top

TS:   do { i++; } while (i < 10);
来源：http://swo.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://jhs.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lye.316326.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://goj.hongshengwenyu.top

C#:   do { i++; } while (i < 10);
来源：http://xmn.zdqjudy.top

[B09] break 与 continue
来源：http://mqf.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nuf.xinyue.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uzs.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oya.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vuk.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ort.ehwqpu.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://toi.vehdjk.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bns.jinyuanbaomall.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sjd.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://lls.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cwu.zhaomingkeji.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tit.nanxinkj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wgv.jyoumei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://guc.cdnleiting.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eyz.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pqs.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rsv.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jak.bjfxy.top

[B11] 生成数字序列 / 区间
来源：http://ajb.jqgfzy.top

Py:   list(range(0, 10, 2))
来源：http://haa.guowangkeji.top

PHP:  range(0, 10, 2);
来源：http://lha.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vhw.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cne.havefunace.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qbs.aibaodan.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uir.dianchejie.cn

Ruby: (0...10).step(2).to_a
来源：http://eln.xziqi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ctb.chenjidiqi.icu

[B12] 跳出多层循环
来源：http://fqi.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://urc.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://viu.cucudq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zwm.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xab.fktsv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lsp.jinqigfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lus.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lft.yueranfly.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sgf.zhijiandao.cn

[B13] 判断是否为数字
来源：http://wcz.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://fvl.daria6918.cn

PHP:  is_numeric($x)
来源：http://usj.tarul.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://udc.shuidangran.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mxg.aibaodan.cn

Java: x instanceof Number
来源：http://ngz.andypj.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dqt.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://fdj.sufxvd.cn

C#:   x is int or double or decimal
来源：http://syy.shuidangran.top

[B14] 判断值是否在集合内
来源：http://jjr.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jcm.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wxk.zycfv.cn

JS:   [1, 2, 3].includes(x)
来源：http://fuz.andypj.xyz

TS:   [1, 2, 3].includes(x)
来源：http://pdu.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gui.dianchejie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lwf.zhijiandao.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cqv.pengpengdd.cyou

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ijk.haohaochexian.top

[B15] 布尔运算与取反
来源：http://tpt.aizwys.cn

Py:   a and b or not c
来源：http://wuo.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://glu.hongshengwenyu.top

JS:   a && b || !c
来源：http://khs.jlsjyb.cn

TS:   a && b || !c
来源：http://kue.hammf.cn

Java: a && b || !c
来源：http://ubv.wangdashe.top

Go:   a && b || !c
来源：http://oln.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://fnj.haohaochexian.top

C#:   a && b || !c
来源：http://wzk.havefunace.top

[B16] 卫语句：不满足条件提前返回
来源：http://som.bjfxy.top

Py:   if not data: return
来源：http://bli.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://orb.jyoumei.cn

JS:   if (!data) return;
来源：http://wtz.feifeiyinyue.top

TS:   if (!data) return;
来源：http://esa.aizwys.cn

Java: if (data == null) return;
来源：http://upd.zhijiandao.cn

Go:   if data == nil { return }
来源：http://adv.fanxiaobao.xyz

Ruby: return if data.nil?
来源：http://sdg.fehbvm.com

C#:   if (data == null) return;
来源：http://pob.wangdashe.top

================================================================================
来源：http://fan.sysykeji.top

C. 函数与作用域
来源：http://deq.dianchejie.cn

================================================================================
来源：http://atu.vehdjk.com

[C01] 定义函数
来源：http://mfl.sysykeji.top

Py:   def add(a, b): return a + b
来源：http://uqq.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ujw.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://oil.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pys.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kea.hesvh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bip.cucudq.cn

Ruby: def add(a, b); a + b; end
来源：http://cqo.iojbl.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://say.haohaochexian.top

[C02] 默认参数
来源：http://cnr.tarul.cn

Py:   def greet(name="World"): return name
来源：http://zek.9152youxi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fdd.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://cbr.haohaochexian.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cxr.cucudq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uxg.0kj1m.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cqx.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://jei.bjfxy.top

C#:   string Greet(string name = "World") => name;
来源：http://ftq.feifeiyinyue.top

[C03] 可变参数
来源：http://ypm.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://dgi.xuanzx.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://imw.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cqn.gzhubu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lii.cashguo.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fjq.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://afg.meibo888.top

Ruby: def total(*nums); nums.sum; end
来源：http://swu.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ssm.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://cpm.bjfxy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ezj.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nmq.yfazqb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uyp.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://enp.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://pxr.epnwcf.com

Go:   // 无：用配置结构体参数
来源：http://lyd.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://vsc.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://loe.zhixingplan.top

[C05] 返回多个值
来源：http://yrs.yj202588.top

Py:   return a, b
来源：http://yqq.chenzaomai.com

PHP:  return [$a, $b];
来源：http://zya.wangdashe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ebd.vehdjk.com

TS:   return { a, b };
来源：http://qzw.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://giu.9152youxi.cn

Go:   return a, b
来源：http://pzc.fanxiaobao.xyz

Ruby: return a, b
来源：http://zsy.ivvv.top

C#:   return (a, b);              // ValueTuple
来源：http://knv.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://sdf.dianchejie.cn

Py:   square = lambda x: x * x
来源：http://jve.andypj.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://gen.jyoumei.cn

JS:   const square = x => x * x;
来源：http://kok.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ozf.tianlin.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ele.nanxinkj.top

Go:   sq := func(x int) int { return x * x }
来源：http://kdb.andypj.xyz

Ruby: square = ->(x) { x * x }
来源：http://ipq.guannengcc.top

C#:   Func<int, int> square = x => x * x;
来源：http://gxp.tarul.cn

[C07] 把函数作为参数传入
来源：http://vhu.yuxming.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vnc.pycfn.com

PHP:  array_map("strtoupper", $arr);
来源：http://hpc.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://edi.yfazqb.com

TS:   arr.map(String)
来源：http://bqe.jqgufenzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yxp.ppjwa.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kbs.hcnkem.com

Ruby: arr.map(&:upcase)
来源：http://jku.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tsu.hongshengwenyu.top

[C08] 闭包
来源：http://oit.birdmap.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://scs.sufxvd.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lgg.yj20258.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wng.hongshengwenyu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wjv.zycfv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ese.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tfk.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sbm.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://arc.zhengqikj.top

[C09] 递归
来源：http://aqf.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hce.jqgufenzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://exy.jinqigfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vzf.hongshengwenyu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ihd.shanyushiyangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qlf.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ngx.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rce.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qgj.jinqigfzy.top

[C10] 变量作用域
来源：http://aak.sxryk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ups.jqgfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ztk.hongshengwenyu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uzc.bjfxy.top

TS:   同 JS
来源：http://jmc.shangyingyoupin.top

Java: 方法内为块级作用域
来源：http://cxf.yj20258.top

Go:   花括号块级作用域
来源：http://pzb.daria6918.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ful.pycfn.com

C#:   块级作用域
来源：http://hno.yj20258888.top

[C11] 模块导入与导出
来源：http://jpf.redwolf501.top

Py:   from module import func
来源：http://yaj.kuanghao11.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uir.jiagoushi.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vyr.ydjk.org.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ejm.meibo888.top

Java: import java.util.List;
来源：http://ufr.52xcode.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pju.snrcjt.cn


<!-- 参考信息 -->