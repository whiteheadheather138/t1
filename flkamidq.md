代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://zbe.tanke756.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yyk.ywan-chungtsiang.top

Ruby: format("%.2f", 3.14159)
来源：http://byp.jqgufenzy.top

C#:   3.14159.ToString("F2")
来源：http://qdo.daria6918.cn

[A22] 获取字符串长度
来源：http://ssu.yueranfly.top

Py:   len(s)
来源：http://dpf.ctjpmb.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://npr.xylfe.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nhf.jinghuilouyu.cn

TS:   s.length
来源：http://irw.sysykeji.top

Java: s.length()
来源：http://kyf.uphjek.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ypy.yj20258888.top

Ruby: s.length
来源：http://tht.chenjidiqi.icu

C#:   s.Length
来源：http://goa.xuetiantiany.cn

[A23] 大小写转换
来源：http://rxh.shanyushiyangkeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://krc.shanyushiyangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pxe.mhx1999.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jqp.gotoacloud.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cva.cashguo.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pvx.bbcook.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qzy.0kj1m.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ues.shanyushiyangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://wbl.epnwcf.com

[A24] 去除首尾空白
来源：http://eia.epnwcf.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rou.quarkkingdee.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oyf.jlsjyb.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kva.52xcode.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wqr.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kqx.zhaomingkeji.xyz

Go:   strings.TrimSpace(s)
来源：http://fsg.shanyushiyangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mbk.hcnkem.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zym.yuanzhike.top

[A25] 字符串比较
来源：http://cnk.ehwqpu.com

Py:   s1 == s2; s1 != s2
来源：http://xin.sjlbkw.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rcm.fehbvm.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wzv.fanxiaobao.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wqx.jiagoushi.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dcq.redwolf501.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vum.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://rne.bjfxy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xvy.hammf.cn

[A26] 类型转换总览
来源：http://euz.tianlin.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://scb.gzhubu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ipq.haohaochexian.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ubm.pycfn.com

TS:   Number() String() Boolean() x as number
来源：http://zzc.zhijiandao.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ypg.yj20258.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rvq.xinyue.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://tym.sysykeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://egi.yongpay.top

================================================================================
来源：http://ztu.yuanzhike.top

B. 流程控制
来源：http://ljn.jianghu66.top

================================================================================
来源：http://dcf.zdqjudy.top

[B01] 条件判断 if / else
来源：http://tzi.ydjk.org.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mof.nanxuanxn.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nqv.yueranfly.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fgw.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fss.yj202588.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tvq.zhoulong.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dsr.hysaishi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dms.zycfv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wif.cucudq.cn

[B02] 多分支 else if / elif
来源：http://bmg.gzhubu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ztc.mhx1999.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vnz.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vds.sjlbkw.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rbk.hongshengwenyu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bsf.chenjidiqi.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yxs.zhixingplan.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pec.dashuyun.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yhw.hcnkem.com

[B03] switch / match / case
来源：http://opp.mhx1999.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ucw.meibo888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wwa.gaohongyu789.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xvj.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://czz.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kby.epnwcf.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mmy.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zyg.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uyr.iojbl.cn

[B04] for 计数循环
来源：http://szz.zhongyouzk.top

Py:   for i in range(10): print(i)
来源：http://zws.hongshengwenyu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://had.daria6918.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fdk.fehbvm.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ued.yj20258888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nmv.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hgh.gotoacloud.top

Ruby: 10.times { |i| puts i }
来源：http://nrr.hesvh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gix.yueranfly.top

[B05] 遍历数组 / 列表
来源：http://bcf.bjfxy.top

Py:   for item in arr: print(item)
来源：http://mks.yj20258.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bla.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://sbw.hesvh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://utr.jqgfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://czh.aibaodan.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://das.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://plw.chenjidiqi.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uxd.ydjk.org.cn

[B06] 遍历字典 / 对象
来源：http://pao.vehdjk.com

Py:   for k, v in d.items(): print(k, v)
来源：http://xdx.zdbjq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vns.yvedp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ecm.sweek.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qvk.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ita.zhaomingkeji.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ykv.ydzc1.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oqc.hesvh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yrj.cdnleiting.top

[B07] while 循环
来源：http://pkt.gogol.net.cn

Py:   while i < 10: i += 1
来源：http://lug.snrcjt.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lwz.jinqigufen.top

JS:   while (i < 10) { i++; }
来源：http://rrz.havefunace.top

TS:   while (i < 10) { i++; }
来源：http://xxt.jinqigufen.top

Java: while (i < 10) { i++; }
来源：http://mxs.haohaochexian.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rit.yj202588.top

Ruby: while i < 10; i += 1; end
来源：http://sij.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://uzt.dianchejie.cn

[B08] do-while（至少执行一次）
来源：http://tdz.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://fzp.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bct.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://mxm.jqgufenzy.top

TS:   do { i++; } while (i < 10);
来源：http://gfc.c1oappe.top

Java: do { i++; } while (i < 10);
来源：http://opf.jianghu66.top

Go:   for { i++; if i >= 10 { break } }
来源：http://per.guannengcc.top

Ruby: begin; i += 1; end while i < 10
来源：http://smh.ivvv.top

C#:   do { i++; } while (i < 10);
来源：http://lsy.yangfankeji.com

[B09] break 与 continue
来源：http://ypa.zhengqikj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://glr.zhongyouzk.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wwn.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lkp.ywan-chungtsiang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://chl.xingfuxueyuan.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://feu.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hwm.vqdsnc.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://spu.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kbc.fzhhl.top

[B10] 遍历同时拿索引
来源：http://dne.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bnq.shanyushiyangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zug.ywan-chungtsiang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wmr.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://puw.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tzd.xinyue.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://apq.jlsjyb.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ile.dashuyun.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lke.tarul.cn

[B11] 生成数字序列 / 区间
来源：http://cng.hfpthk.cn

Py:   list(range(0, 10, 2))
来源：http://xun.yangfankeji.com

PHP:  range(0, 10, 2);
来源：http://wpq.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://avu.xziqi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zef.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://edn.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ncx.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://oei.quarkkingdee.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ife.ppjwa.cn

[B12] 跳出多层循环
来源：http://zfk.yonumen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gbq.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://ujs.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gvc.uphjek.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hvo.birdmap.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://spq.shanyushiyangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kef.9152youxi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ezr.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wtq.cqqwz.cn

[B13] 判断是否为数字
来源：http://fqr.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://efw.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://und.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wmw.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sfr.redwolf501.top

Java: x instanceof Number
来源：http://kgv.vehdjk.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yzk.bjfxy.top

Ruby: x.is_a?(Numeric)
来源：http://iig.yfazqb.com

C#:   x is int or double or decimal
来源：http://heh.hcnkem.com

[B14] 判断值是否在集合内
来源：http://ujh.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mma.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nwm.pengpengdd.cyou

JS:   [1, 2, 3].includes(x)
来源：http://usq.chenzaomai.com

TS:   [1, 2, 3].includes(x)
来源：http://jld.aizwys.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ahd.zhiwuduotai.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yik.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ode.guannengcc.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dgz.vehdjk.com

[B15] 布尔运算与取反
来源：http://wyy.feifeiyinyue.top

Py:   a and b or not c
来源：http://wmb.jianghu66.top

PHP:  $a && $b || !$c
来源：http://era.zycfv.cn

JS:   a && b || !c
来源：http://akw.daxiang520.top

TS:   a && b || !c
来源：http://xkq.hnqzz.top

Java: a && b || !c
来源：http://oea.tianlin.xyz

Go:   a && b || !c
来源：http://rub.316326.xyz

Ruby: a && b || !c
来源：http://cyc.svipenyu.cn

C#:   a && b || !c
来源：http://tjc.cqqwz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tcf.ctjpmb.com

Py:   if not data: return
来源：http://reg.316326.xyz

PHP:  if (!$data) { return; }
来源：http://tzf.jianghu66.top

JS:   if (!data) return;
来源：http://gle.vehdjk.com

TS:   if (!data) return;
来源：http://jer.yonumen.top

Java: if (data == null) return;
来源：http://kdf.ppjwa.cn

Go:   if data == nil { return }
来源：http://xnj.chenzaomai.com

Ruby: return if data.nil?
来源：http://ulv.ybcxt.top

C#:   if (data == null) return;
来源：http://zer.tianlin.xyz

================================================================================
来源：http://vyv.tarul.cn

C. 函数与作用域
来源：http://zpq.jinqigufen.top

================================================================================
来源：http://jro.xuanzx.com

[C01] 定义函数
来源：http://nia.gzhubu.top

Py:   def add(a, b): return a + b
来源：http://gmt.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hpb.jlsjyb.cn

JS:   function add(a, b) { return a + b; }
来源：http://xvz.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hmv.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zhm.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nes.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://clt.yfazqb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qrf.snrcjt.cn

[C02] 默认参数
来源：http://exs.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://xuk.jyoumei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dlg.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://aib.xuetiantiany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ylu.ivvv.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kfg.yvedp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zke.xingfuxueyuan.xyz

Ruby: def greet(name = "World") = name
来源：http://cms.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://ubq.ivvv.top

[C03] 可变参数
来源：http://kro.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://hlu.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wfg.shzxlz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vct.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aor.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jey.0kj1m.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qcq.ehwqpu.com

Ruby: def total(*nums); nums.sum; end
来源：http://rkd.9152youxi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://roh.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://fzl.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://njr.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://avs.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hue.pengpengdd.cyou

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mvy.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://lyl.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://ogk.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://gbe.nwbrower.top

C#:   f(a: 1, b: 2)
来源：http://mbb.zhijiandao.cn

[C05] 返回多个值
来源：http://xgf.ydzc1.top

Py:   return a, b
来源：http://ubz.gotoacloud.top

PHP:  return [$a, $b];
来源：http://mpc.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uqj.hysaishi.cn

TS:   return { a, b };
来源：http://qvl.9152youxi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cgs.kuanghao11.cn

Go:   return a, b
来源：http://imw.zdbjq.cn

Ruby: return a, b
来源：http://pzd.hnqzz.top

C#:   return (a, b);              // ValueTuple
来源：http://zlz.jlsjyb.cn

[C06] 匿名函数 / lambda
来源：http://eql.haohaochexian.top

Py:   square = lambda x: x * x
来源：http://fcs.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fph.smart0.xyz

JS:   const square = x => x * x;
来源：http://ahr.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://mms.pengpengdd.cyou

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lyb.hesvh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ejh.zhongyouzk.top

Ruby: square = ->(x) { x * x }
来源：http://bim.kuanghao11.cn

C#:   Func<int, int> square = x => x * x;
来源：http://msl.cucudq.cn

[C07] 把函数作为参数传入
来源：http://xgy.yangfankeji.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mpt.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sxe.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nea.fzhhl.top

TS:   arr.map(String)
来源：http://cid.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xiz.wangdashe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wgu.hnxiangtu.top

Ruby: arr.map(&:upcase)
来源：http://yle.xziqi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zwg.sxryk.cn

[C08] 闭包
来源：http://lhm.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aay.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pvk.ydjk.org.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://stv.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zag.yj20258888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ixg.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dbd.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://utx.kuanghao11.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nov.hfpthk.cn

[C09] 递归
来源：http://evz.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oar.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yqe.zhongyouzk.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://erk.shzxlz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uki.shzxlz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ydg.chenlongwang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://grp.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nvb.uphjek.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ruc.jinghuilouyu.cn

[C10] 变量作用域
来源：http://rze.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ksg.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vfp.quarkkingdee.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qih.chenjidiqi.icu

TS:   同 JS
来源：http://bsv.jinqigufen.top

Java: 方法内为块级作用域
来源：http://qhb.yj202588.top

Go:   花括号块级作用域
来源：http://ozb.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jvg.mhx1999.top

C#:   块级作用域
来源：http://ade.quarkkingdee.top

[C11] 模块导入与导出
来源：http://fkk.quarkkingdee.top

Py:   from module import func
来源：http://jgd.hcnkem.com

PHP:  require "file.php";  或 use App\Service;
来源：http://yxj.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yxz.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qmd.fzhhl.top

Java: import java.util.List;
来源：http://mgf.gotoacloud.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://omn.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://lif.tarul.cn

C#:   using System.Text;
来源：http://kxm.tianlin.xyz

[C12] 立即执行函数 IIFE
来源：http://fei.xuetiantiany.cn

Py:   (lambda: print("run"))()
来源：http://pus.tanke756.top


<!-- 参考信息 -->