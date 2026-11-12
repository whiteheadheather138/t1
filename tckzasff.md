代发 wailian999

[A22] 获取字符串长度
来源：http://rxv.xziqi.cn

Py:   len(s)
来源：http://bza.fehbvm.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://elb.xuetiantiany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pil.mhx1999.top

TS:   s.length
来源：http://lth.kuanghao11.cn

Java: s.length()
来源：http://npe.yvedp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iqd.yueranfly.top

Ruby: s.length
来源：http://kqw.hnqzz.top

C#:   s.Length
来源：http://umr.yangfankeji.com

[A23] 大小写转换
来源：http://grb.c1oappe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://zci.fzhhl.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ovo.sufxvd.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bjq.hnxiangtu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://acw.gogol.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mxk.sweek.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ugz.ydjk.org.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lhw.yongpay.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gkc.bjfxy.top

[A24] 去除首尾空白
来源：http://bbu.hnqzz.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://obu.xuetiantiany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://apx.xuanzx.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://amz.bjfxy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ffh.jyoumei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zag.hesvh.cn

Go:   strings.TrimSpace(s)
来源：http://meo.chenzaomai.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rvx.xinyue.icu

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vto.shuidangran.top

[A25] 字符串比较
来源：http://ncd.shuidangran.top

Py:   s1 == s2; s1 != s2
来源：http://hci.fktsv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wys.zhijiandao.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mhm.gaohongyu789.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qoy.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ftv.shzxlz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jes.cucudq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fqn.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lyw.daria6918.cn

[A26] 类型转换总览
来源：http://kpl.chenjidiqi.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://njq.tianlin.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mvl.wangshuangyany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://odt.sufxvd.cn

TS:   Number() String() Boolean() x as number
来源：http://bbh.dianchejie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qak.ywan-chungtsiang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dbq.sysykeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qnw.cdnleiting.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oob.ydjk.org.cn

================================================================================
来源：http://prv.cucudq.cn

B. 流程控制
来源：http://izz.ydjk.org.cn

================================================================================
来源：http://hmd.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://evy.epnwcf.com

Py:   result = "正" if x > 0 else "非正"
来源：http://pso.ctjpmb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yxx.mhx1999.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qpo.ivvv.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tpb.hysaishi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uel.hesvh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://shh.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gji.yuxming.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pgl.jlsjyb.cn

[B02] 多分支 else if / elif
来源：http://qfy.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jns.andypj.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xay.jiagoushi.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rum.daria6918.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lwc.wangdashe.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ful.daria6918.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ppc.ydzc1.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://glu.xingfuxueyuan.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eor.chenjidiqi.icu

[B03] switch / match / case
来源：http://pnx.ydzc1.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jqp.xingfuxueyuan.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://voy.shangyingyoupin.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ldk.chenzaomai.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pnk.hesvh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eoh.quarkkingdee.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ark.jqgfzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pij.yongpay.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yzk.zhixingplan.top

[B04] for 计数循环
来源：http://xgu.snrcjt.cn

Py:   for i in range(10): print(i)
来源：http://pij.havefunace.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dqb.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gsv.havefunace.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ksa.chenzaomai.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bjd.xziqi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ayd.snrcjt.cn

Ruby: 10.times { |i| puts i }
来源：http://rgh.pycfn.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hit.yj20258.top

[B05] 遍历数组 / 列表
来源：http://grh.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://sxa.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://idn.sweek.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tck.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://pav.9152youxi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rjt.daria6918.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lvd.zdqjudy.top

Ruby: arr.each { |item| puts item }
来源：http://pko.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nhr.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://acs.nwbrower.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vqw.epnwcf.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ewx.xuanzx.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vqa.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zir.ctjpmb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gwf.feifeiyinyue.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wrv.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://thn.hnqzz.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zsa.zdbjq.cn

[B07] while 循环
来源：http://qsz.fktsv.cn

Py:   while i < 10: i += 1
来源：http://fwv.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://dir.sweek.top

JS:   while (i < 10) { i++; }
来源：http://fsa.sweek.top

TS:   while (i < 10) { i++; }
来源：http://ybq.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://gqn.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zgf.zhaomingkeji.xyz

Ruby: while i < 10; i += 1; end
来源：http://atn.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://cpe.hongshengwenyu.top

[B08] do-while（至少执行一次）
来源：http://znv.havefunace.top

Py:   # 无 do-while：用 while True + break
来源：http://ytc.jqgfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jml.ppjwa.cn

JS:   do { i++; } while (i < 10);
来源：http://qee.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://fmm.fanxiaobao.xyz

Java: do { i++; } while (i < 10);
来源：http://tpk.cashguo.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ffo.hongshengwenyu.top

Ruby: begin; i += 1; end while i < 10
来源：http://aom.sufxvd.cn

C#:   do { i++; } while (i < 10);
来源：http://hoq.ppjwa.cn

[B09] break 与 continue
来源：http://ets.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rmn.yfazqb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sau.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://flo.xinyue.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dps.hywenlv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bic.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pjw.fzhhl.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mru.xuetiantiany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dpk.zhoulong.xyz

[B10] 遍历同时拿索引
来源：http://kwv.zhaomingkeji.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gqr.ydzc1.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nvb.shuidangran.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kkf.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bjq.jyoumei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hjb.havefunace.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dmc.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yoe.gaohongyu789.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wtm.jinqigufen.top

[B11] 生成数字序列 / 区间
来源：http://gms.tanke756.top

Py:   list(range(0, 10, 2))
来源：http://ooy.jinyuanbaomall.cn

PHP:  range(0, 10, 2);
来源：http://emh.sysykeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gpo.xziqi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oxv.yonumen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://smq.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bec.nwbrower.top

Ruby: (0...10).step(2).to_a
来源：http://qzh.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kuq.ydzc1.top

[B12] 跳出多层循环
来源：http://uiu.zdbjq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sid.dianchejie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wzg.kuanghao11.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://egx.hysaishi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://min.wangshuangyany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://npk.hysaishi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qmq.nanxuanxn.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sma.wangshuangyany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bmx.316326.xyz

[B13] 判断是否为数字
来源：http://xfc.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://rfg.shanyushiyangtech.top

PHP:  is_numeric($x)
来源：http://ztr.hesvh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://asp.fehbvm.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mxy.yvedp.cn

Java: x instanceof Number
来源：http://bkr.yj20258888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nnl.yvedp.cn

Ruby: x.is_a?(Numeric)
来源：http://ayp.hnxiangtu.top

C#:   x is int or double or decimal
来源：http://joy.aizwys.cn

[B14] 判断值是否在集合内
来源：http://rjg.shanyushiyangtech.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vzw.cashguo.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hjs.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://gky.gaohongyu789.top

TS:   [1, 2, 3].includes(x)
来源：http://kck.xingfuxueyuan.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://qkz.shanyushiyangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kmr.ivvv.top

Ruby: [1, 2, 3].include?(x)
来源：http://fdz.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bsq.yueranfly.top

[B15] 布尔运算与取反
来源：http://dvh.tian-w.cn

Py:   a and b or not c
来源：http://cop.quarkkingdee.top

PHP:  $a && $b || !$c
来源：http://mqq.fanxiaobao.xyz

JS:   a && b || !c
来源：http://yun.ppjwa.cn

TS:   a && b || !c
来源：http://fxh.316326.xyz

Java: a && b || !c
来源：http://gzb.guowangkeji.top

Go:   a && b || !c
来源：http://frm.zycfv.cn

Ruby: a && b || !c
来源：http://gcg.zhixingplan.top

C#:   a && b || !c
来源：http://qhl.ehwqpu.com

[B16] 卫语句：不满足条件提前返回
来源：http://ctn.0kj1m.cn

Py:   if not data: return
来源：http://bub.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://njz.cdnleiting.top

JS:   if (!data) return;
来源：http://ena.wangdashe.top

TS:   if (!data) return;
来源：http://hzi.ehwqpu.com

Java: if (data == null) return;
来源：http://uli.c1oappe.top

Go:   if data == nil { return }
来源：http://kgk.dashuyun.cn

Ruby: return if data.nil?
来源：http://flc.yfazqb.com

C#:   if (data == null) return;
来源：http://cxc.tanke756.top

================================================================================
来源：http://dws.jiagoushi.top

C. 函数与作用域
来源：http://amt.redwolf501.top

================================================================================
来源：http://bwx.kuanghao11.cn

[C01] 定义函数
来源：http://vkg.jyoumei.cn

Py:   def add(a, b): return a + b
来源：http://iwd.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aag.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://mhv.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mqc.zhongyouzk.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ulm.nwbrower.top

Go:   func add(a, b int) int { return a + b }
来源：http://kfa.guannengcc.top

Ruby: def add(a, b); a + b; end
来源：http://kgs.xuetiantiany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mvd.yongpay.top

[C02] 默认参数
来源：http://azy.ydzc1.top

Py:   def greet(name="World"): return name
来源：http://ziu.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://aoo.ivvv.top

JS:   function greet(name = "World") { return name; }
来源：http://hth.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xnc.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cxd.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wqy.hongshengwenyu.top

Ruby: def greet(name = "World") = name
来源：http://zun.yangfankeji.com

C#:   string Greet(string name = "World") => name;
来源：http://xfn.9152youxi.cn

[C03] 可变参数
来源：http://vlf.pengpengdd.cyou

Py:   def total(*args): return sum(args)
来源：http://nkt.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fxr.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fbv.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qti.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tfd.yangfankeji.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lvx.ybcxt.top

Ruby: def total(*nums); nums.sum; end
来源：http://jbn.xylfe.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://apb.gaohongyu789.top

[C04] 命名参数 / 关键字参数
来源：http://qxi.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://try.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tve.dashuyun.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ypb.uphjek.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vgy.zhoulong.xyz

Java: // 无：用 Builder 模式或 record
来源：http://elp.hysaishi.cn

Go:   // 无：用配置结构体参数
来源：http://ksv.aizwys.cn

Ruby: f(a: 1, b: 2)
来源：http://efd.ctjpmb.com

C#:   f(a: 1, b: 2)
来源：http://omj.yangfankeji.com

[C05] 返回多个值
来源：http://pqv.chenzaomai.com

Py:   return a, b
来源：http://uaq.svipenyu.cn

PHP:  return [$a, $b];
来源：http://pla.shanyushiyangtech.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tod.nanxinkj.top

TS:   return { a, b };
来源：http://dii.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zfn.smart0.xyz

Go:   return a, b
来源：http://aop.yongpay.top

Ruby: return a, b
来源：http://yjq.chenlongwang.top

C#:   return (a, b);              // ValueTuple
来源：http://boi.haohaochexian.top

[C06] 匿名函数 / lambda
来源：http://ugd.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://ron.meibo888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://guk.jiagoushi.top

JS:   const square = x => x * x;
来源：http://xrk.shanyushiyangtech.top

TS:   const square = (x: number): number => x * x;
来源：http://gsx.bjfxy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uia.smart0.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://ikc.hysaishi.cn

Ruby: square = ->(x) { x * x }
来源：http://iec.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://djl.hysaishi.cn

[C07] 把函数作为参数传入
来源：http://arc.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://omr.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ouo.chenlongwang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kkf.shanyushiyangkeji.top

TS:   arr.map(String)
来源：http://vbh.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gyk.cdnleiting.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ljb.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://tlc.snrcjt.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ohf.bbcook.cn

[C08] 闭包
来源：http://vwk.tianlin.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yxa.vqdsnc.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yuh.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tqt.snrcjt.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://foa.wangdashe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cut.zdqjudy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dvp.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zer.cdnleiting.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://whq.yueranfly.top

[C09] 递归
来源：http://vgp.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bre.nwbrower.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ids.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yrk.sysykeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jbk.fehbvm.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nat.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hws.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wih.zhengqikj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dxx.yueranfly.top

[C10] 变量作用域
来源：http://swo.snrcjt.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dpe.zdbjq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lxw.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uuy.yfazqb.com

TS:   同 JS
来源：http://akt.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://kpv.jinyuanbaomall.cn

Go:   花括号块级作用域
来源：http://vha.jianghu66.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ymu.sxryk.cn

C#:   块级作用域
来源：http://mhg.jqgfzy.top

[C11] 模块导入与导出
来源：http://qcu.sysykeji.top

Py:   from module import func
来源：http://idt.yangfankeji.com

PHP:  require "file.php";  或 use App\Service;
来源：http://wwb.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fwk.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://orl.9152youxi.cn

Java: import java.util.List;
来源：http://azv.vqdsnc.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gbt.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://ycv.yongpay.top

C#:   using System.Text;
来源：http://rqx.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://jbz.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://ssr.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://qpu.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://wzm.ehwqpu.com

TS:   (() => { console.log("run"); })();
来源：http://nqe.daxiang520.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xip.gzhubu.top


<!-- 参考信息 -->