代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://lzx.svipenyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://daz.yj202588.top

Ruby: format("%.2f", 3.14159)
来源：http://vvx.chenzaomai.com

C#:   3.14159.ToString("F2")
来源：http://fef.tianlin.xyz

[A22] 获取字符串长度
来源：http://hmq.zhongyouzk.top

Py:   len(s)
来源：http://koy.vqdsnc.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vml.shanyushiyangtech.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uke.redwolf501.top

TS:   s.length
来源：http://wiy.gaohongyu789.top

Java: s.length()
来源：http://tep.9152youxi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lvr.sufxvd.cn

Ruby: s.length
来源：http://sij.cdnleiting.top

C#:   s.Length
来源：http://nnd.jqgfzy.top

[A23] 大小写转换
来源：http://ovu.jqgufenzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hqw.sysykeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nya.sweek.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rnd.9152youxi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dxs.hnxiangtu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://npl.tianlin.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wev.fanxiaobao.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tyr.cqqwz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gef.sjlbkw.cn

[A24] 去除首尾空白
来源：http://rmm.chenzaomai.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bzc.zdbjq.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lbu.sjlbkw.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gty.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lcj.wangdashe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://trk.sxryk.cn

Go:   strings.TrimSpace(s)
来源：http://izy.smart0.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ery.dashuyun.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cdz.hywenlv.cn

[A25] 字符串比较
来源：http://npx.epnwcf.com

Py:   s1 == s2; s1 != s2
来源：http://gyf.sweek.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cas.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lag.fengsongda.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dyk.shuidangran.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rqy.vqdsnc.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hdp.cucudq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://duc.wangdashe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bav.yueranfly.top

[A26] 类型转换总览
来源：http://ogs.yfazqb.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bon.uphjek.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bnc.sufxvd.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kmm.daxiang520.top

TS:   Number() String() Boolean() x as number
来源：http://yue.zhongyouzk.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xqe.c1oappe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cas.nanxuanxn.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rlt.chenzaomai.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jfk.yonumen.top

================================================================================
来源：http://miw.yonumen.top

B. 流程控制
来源：http://bdt.jiagoushi.top

================================================================================
来源：http://zjj.bbcook.cn

[B01] 条件判断 if / else
来源：http://fit.shzxlz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://iux.jqgfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zeo.xingfuxueyuan.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rah.ydjk.org.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kia.pycfn.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://xbp.ywan-chungtsiang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nru.0kj1m.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sbe.sjlbkw.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hni.shangyingyoupin.top

[B02] 多分支 else if / elif
来源：http://wtf.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xmo.ybcxt.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://weo.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dtn.cucudq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jkt.fehbvm.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zur.ydjk.org.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://via.daxiang520.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eob.snrcjt.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nga.zhaomingkeji.xyz

[B03] switch / match / case
来源：http://srq.wangshuangyany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oew.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vnt.wangshuangyany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nvo.yanxiufei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fjd.fzhhl.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pik.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qxk.zhixingplan.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ouf.c1oappe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mdz.316326.xyz

[B04] for 计数循环
来源：http://kjp.yj20258888.top

Py:   for i in range(10): print(i)
来源：http://vvt.cheryme.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xzj.yonumen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wyd.chenjidiqi.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dum.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gti.jqgufenzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pvf.meibo888.top

Ruby: 10.times { |i| puts i }
来源：http://rmg.cucudq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fvo.fanxiaobao.xyz

[B05] 遍历数组 / 列表
来源：http://hfj.quarkkingdee.top

Py:   for item in arr: print(item)
来源：http://mym.gogol.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fgs.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fcj.gaohongyu789.top

TS:   for (const item of arr) { console.log(item); }
来源：http://voe.sjlbkw.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://azt.ybcxt.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xun.cqqwz.cn

Ruby: arr.each { |item| puts item }
来源：http://gyl.hcnkem.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ubo.iojbl.cn

[B06] 遍历字典 / 对象
来源：http://xcg.yfazqb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://pqu.jyoumei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dxo.gotoacloud.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://htl.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hgb.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jsu.hfpthk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wxj.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fcn.jlsjyb.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xee.xuanzx.com

[B07] while 循环
来源：http://axt.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://rqy.yongpay.top

PHP:  while ($i < 10) { $i++; }
来源：http://hfy.ehwqpu.com

JS:   while (i < 10) { i++; }
来源：http://bos.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://xog.pycfn.com

Java: while (i < 10) { i++; }
来源：http://sog.hysaishi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dhp.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://qnp.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://udw.shuidangran.top

[B08] do-while（至少执行一次）
来源：http://kon.fanxiaobao.xyz

Py:   # 无 do-while：用 while True + break
来源：http://qyq.zycfv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qmg.zhiwuduotai.top

JS:   do { i++; } while (i < 10);
来源：http://zlu.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://ptb.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://vcd.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://whe.ivvv.top

Ruby: begin; i += 1; end while i < 10
来源：http://mcy.yj202588.top

C#:   do { i++; } while (i < 10);
来源：http://tbp.svipenyu.cn

[B09] break 与 continue
来源：http://zym.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://grz.hfpthk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fyp.nwbrower.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wip.ybcxt.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kor.guannengcc.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ram.xuetiantiany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kay.hywenlv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aav.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yud.xinyue.icu

[B10] 遍历同时拿索引
来源：http://cnn.0kj1m.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lnc.shanyushiyangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ecu.cucudq.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://iyx.hcnkem.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hte.jinqigufen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kkm.ivvv.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fkk.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pjv.andypj.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fvk.fzhhl.top

[B11] 生成数字序列 / 区间
来源：http://bsq.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://eis.sweek.top

PHP:  range(0, 10, 2);
来源：http://ygx.sjlbkw.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dki.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uzn.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vyr.cashguo.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ifr.birdmap.top

Ruby: (0...10).step(2).to_a
来源：http://lwm.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nfr.bbcook.cn

[B12] 跳出多层循环
来源：http://siq.nanxuanxn.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bbd.iojbl.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wlx.gzhubu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pvq.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zbb.yonumen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://esq.sjlbkw.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://shg.meibo888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iku.ehwqpu.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ihp.fktsv.cn

[B13] 判断是否为数字
来源：http://pgx.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://djn.wangdashe.top

PHP:  is_numeric($x)
来源：http://ybz.zycfv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aam.hongshengwenyu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ecg.gaohongyu789.top

Java: x instanceof Number
来源：http://kfw.chenlongwang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://imx.snrcjt.cn

Ruby: x.is_a?(Numeric)
来源：http://jkn.hysaishi.cn

C#:   x is int or double or decimal
来源：http://djr.yongpay.top

[B14] 判断值是否在集合内
来源：http://vak.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rhb.feifeiyinyue.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cwu.iojbl.cn

JS:   [1, 2, 3].includes(x)
来源：http://vgm.gaohongyu789.top

TS:   [1, 2, 3].includes(x)
来源：http://dhl.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rbz.birdmap.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rvv.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://gxk.chenzaomai.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eup.ivvv.top

[B15] 布尔运算与取反
来源：http://efi.zycfv.cn

Py:   a and b or not c
来源：http://dvu.mhx1999.top

PHP:  $a && $b || !$c
来源：http://pfm.hcnkem.com

JS:   a && b || !c
来源：http://yab.zdqjudy.top

TS:   a && b || !c
来源：http://acr.nanxuanxn.top

Java: a && b || !c
来源：http://uvq.tanke756.top

Go:   a && b || !c
来源：http://guw.yuanzhike.top

Ruby: a && b || !c
来源：http://grn.wangdashe.top

C#:   a && b || !c
来源：http://ecs.yonumen.top

[B16] 卫语句：不满足条件提前返回
来源：http://uox.fanxiaobao.xyz

Py:   if not data: return
来源：http://tcu.vehdjk.com

PHP:  if (!$data) { return; }
来源：http://lsm.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://kbi.tarul.cn

TS:   if (!data) return;
来源：http://cvt.vehdjk.com

Java: if (data == null) return;
来源：http://zci.snrcjt.cn

Go:   if data == nil { return }
来源：http://sru.pengpengdd.cyou

Ruby: return if data.nil?
来源：http://tye.sysykeji.top

C#:   if (data == null) return;
来源：http://wgz.feifeiyinyue.top

================================================================================
来源：http://cby.tarul.cn

C. 函数与作用域
来源：http://sjw.mhx1999.top

================================================================================
来源：http://exz.yj20258.top

[C01] 定义函数
来源：http://vxy.kuanghao11.cn

Py:   def add(a, b): return a + b
来源：http://kac.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ghd.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://yhv.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xhg.sufxvd.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://axh.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://jdr.ydjk.org.cn

Ruby: def add(a, b); a + b; end
来源：http://zlw.shuidangran.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fko.jqgufenzy.top

[C02] 默认参数
来源：http://wzc.ppjwa.cn

Py:   def greet(name="World"): return name
来源：http://yqg.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://biq.dianchejie.cn

JS:   function greet(name = "World") { return name; }
来源：http://fee.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xvu.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gpt.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fhd.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://qhi.sxryk.cn

C#:   string Greet(string name = "World") => name;
来源：http://ikm.0kj1m.cn

[C03] 可变参数
来源：http://chn.nanxuanxn.top

Py:   def total(*args): return sum(args)
来源：http://twv.hongshengwenyu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ihu.yanxiufei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nng.jiagoushi.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rrh.cheryme.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gxn.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qmd.hongshengwenyu.top

Ruby: def total(*nums); nums.sum; end
来源：http://hni.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zyl.zdbjq.cn

[C04] 命名参数 / 关键字参数
来源：http://lfg.hfpthk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rvz.hcnkem.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ufi.mhx1999.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pct.zhoulong.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jsk.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://rnv.ivvv.top

Go:   // 无：用配置结构体参数
来源：http://dbs.cashguo.top

Ruby: f(a: 1, b: 2)
来源：http://mro.hywenlv.cn

C#:   f(a: 1, b: 2)
来源：http://gox.yvedp.cn

[C05] 返回多个值
来源：http://zlz.daria6918.cn

Py:   return a, b
来源：http://new.guannengcc.top

PHP:  return [$a, $b];
来源：http://flb.yj20258888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yto.bbcook.cn

TS:   return { a, b };
来源：http://irz.cqqwz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xrz.gotoacloud.top

Go:   return a, b
来源：http://ltr.tianlin.xyz

Ruby: return a, b
来源：http://cpo.hammf.cn

C#:   return (a, b);              // ValueTuple
来源：http://mto.jqgufenzy.top

[C06] 匿名函数 / lambda
来源：http://mrm.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://gbz.jiagoushi.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dbo.xuetiantiany.cn

JS:   const square = x => x * x;
来源：http://pkx.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://pqz.jinghuilouyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://akq.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://qtl.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://epv.zhongyouzk.top

C#:   Func<int, int> square = x => x * x;
来源：http://jel.fzhhl.top

[C07] 把函数作为参数传入
来源：http://ibi.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kfu.hammf.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yly.svipenyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yat.dashuyun.cn

TS:   arr.map(String)
来源：http://mov.gzhubu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cik.daxiang520.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bqj.wangshuangyany.cn

Ruby: arr.map(&:upcase)
来源：http://hpa.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://kyl.fehbvm.com

[C08] 闭包
来源：http://xsj.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zdw.yvedp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ubg.yongpay.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qqb.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zpf.feifeiyinyue.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://chn.cdnleiting.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dox.sjlbkw.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uei.snrcjt.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mew.epnwcf.com

[C09] 递归
来源：http://ssi.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tsy.tarul.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bgc.chenjidiqi.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wfd.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lko.andypj.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zfz.gogol.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bli.c1oappe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://svp.hnxiangtu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dvv.dashuyun.cn

[C10] 变量作用域
来源：http://brp.52xcode.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zus.hysaishi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mov.quarkkingdee.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ssj.yj202588.top

TS:   同 JS
来源：http://sjf.yonumen.top

Java: 方法内为块级作用域
来源：http://gfp.yonumen.top

Go:   花括号块级作用域
来源：http://vfj.zhiwuduotai.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nye.ppjwa.cn

C#:   块级作用域
来源：http://gby.shzxlz.cn

[C11] 模块导入与导出
来源：http://tyf.shuidangran.top

Py:   from module import func
来源：http://yij.snrcjt.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nfc.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gzr.jyoumei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oxt.xinyue.icu

Java: import java.util.List;
来源：http://jmz.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hgp.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://gfy.yj20258.top

C#:   using System.Text;
来源：http://qol.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://puu.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://mfg.hnxiangtu.top


<!-- 参考信息 -->