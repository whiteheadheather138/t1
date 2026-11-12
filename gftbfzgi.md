代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://okp.zhengqikj.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kvi.tianlin.xyz

Ruby: format("%.2f", 3.14159)
来源：http://mho.zhoulong.xyz

C#:   3.14159.ToString("F2")
来源：http://vga.jinyuanbaomall.cn

[A22] 获取字符串长度
来源：http://abm.sxryk.cn

Py:   len(s)
来源：http://wwf.hesvh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vcn.tanke756.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bij.guannengcc.top

TS:   s.length
来源：http://cit.yangfankeji.com

Java: s.length()
来源：http://cdl.nanxinkj.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nou.tarul.cn

Ruby: s.length
来源：http://aba.c1oappe.top

C#:   s.Length
来源：http://baw.hnqzz.top

[A23] 大小写转换
来源：http://hna.xuanzx.com

Py:   s.upper(); s.lower(); s.title()
来源：http://qto.shangyingyoupin.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zlo.52xcode.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xyx.yfazqb.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ygg.tian-w.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fxg.fanxiaobao.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nub.jqgufenzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wit.hcnkem.com

C#:   s.ToUpper(); s.ToLower()
来源：http://ksu.52xcode.cn

[A24] 去除首尾空白
来源：http://ywq.c1oappe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lem.svipenyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xby.vehdjk.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xhy.cheryme.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gef.iojbl.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oab.gzhubu.top

Go:   strings.TrimSpace(s)
来源：http://uew.kuanghao11.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://olz.sweek.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kex.xylfe.cn

[A25] 字符串比较
来源：http://naw.ywan-chungtsiang.top

Py:   s1 == s2; s1 != s2
来源：http://hpl.uphjek.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ilj.yj20258.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lst.yj202588.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sxw.0kj1m.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tmp.jyoumei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://szl.redwolf501.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nut.xinyue.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lgj.jinghuilouyu.cn

[A26] 类型转换总览
来源：http://mwy.hnxiangtu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lsm.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xrc.yuanzhike.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xri.wangdashe.top

TS:   Number() String() Boolean() x as number
来源：http://vqe.zycfv.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zwd.cashguo.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://atv.yfazqb.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://ahc.yuanzhike.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zdf.fzhhl.top

================================================================================
来源：http://ymq.pycfn.com

B. 流程控制
来源：http://tjv.yj202588.top

================================================================================
来源：http://jqb.nwbrower.top

[B01] 条件判断 if / else
来源：http://fmf.iojbl.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://faz.shangyingyoupin.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jrt.vqdsnc.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hsc.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wbt.cashguo.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rhr.jiagoushi.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kks.yfazqb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lqw.yuanzhike.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://scn.316326.xyz

[B02] 多分支 else if / elif
来源：http://ics.aibaodan.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kul.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wsd.svipenyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://imv.jinqigfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nys.cucudq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://toi.shzxlz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zjs.yuanzhike.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uqs.ydjk.org.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nrx.xinyue.icu

[B03] switch / match / case
来源：http://fnt.nwbrower.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iik.quarkkingdee.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rwf.zhaomingkeji.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://inw.shanyushiyangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://npu.gotoacloud.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dlo.nwbrower.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lpy.fktsv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kcu.fzhhl.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dol.cashguo.top

[B04] for 计数循环
来源：http://cyf.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://mpn.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ywd.zycfv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mhw.ctjpmb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://erz.xuanzx.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zop.tanke756.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jua.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://soj.xuetiantiany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fni.0kj1m.cn

[B05] 遍历数组 / 列表
来源：http://avn.xingfuxueyuan.xyz

Py:   for item in arr: print(item)
来源：http://ymi.svipenyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qkg.yueranfly.top

JS:   for (const item of arr) { console.log(item); }
来源：http://llh.ivvv.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gfp.xziqi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://krk.hammf.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gov.uphjek.com

Ruby: arr.each { |item| puts item }
来源：http://tgu.yuanzhike.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wax.shuidangran.top

[B06] 遍历字典 / 对象
来源：http://stv.pycfn.com

Py:   for k, v in d.items(): print(k, v)
来源：http://kzn.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jio.zycfv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fzu.zhiwuduotai.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rnc.hnqzz.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rcr.jinqigufen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lxh.shzxlz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qeo.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://txj.vehdjk.com

[B07] while 循环
来源：http://ugx.0kj1m.cn

Py:   while i < 10: i += 1
来源：http://zkg.hongshengwenyu.top

PHP:  while ($i < 10) { $i++; }
来源：http://hgp.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://ndr.xuetiantiany.cn

TS:   while (i < 10) { i++; }
来源：http://iap.nanxinkj.top

Java: while (i < 10) { i++; }
来源：http://air.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yvd.0kj1m.cn

Ruby: while i < 10; i += 1; end
来源：http://bwl.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://key.sxryk.cn

[B08] do-while（至少执行一次）
来源：http://iqg.zhongyouzk.top

Py:   # 无 do-while：用 while True + break
来源：http://onc.daxiang520.top

PHP:  do { $i++; } while ($i < 10);
来源：http://buf.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://nke.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://dzq.fktsv.cn

Java: do { i++; } while (i < 10);
来源：http://wlq.jyoumei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uwa.nwbrower.top

Ruby: begin; i += 1; end while i < 10
来源：http://czk.xziqi.cn

C#:   do { i++; } while (i < 10);
来源：http://iyb.zhengqikj.top

[B09] break 与 continue
来源：http://kmu.wangshuangyany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://icg.sufxvd.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dwx.ywan-chungtsiang.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rzc.gzhubu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iia.ydzc1.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iqm.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lpy.yuxming.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mlf.bbcook.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pbl.tianlin.xyz

[B10] 遍历同时拿索引
来源：http://czs.yj20258888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tvf.shuidangran.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tfk.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eje.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ahj.epnwcf.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zpi.aizwys.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xof.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zfk.aibaodan.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://acb.jinqigfzy.top

[B11] 生成数字序列 / 区间
来源：http://mtu.nanxuanxn.top

Py:   list(range(0, 10, 2))
来源：http://kkf.hcnkem.com

PHP:  range(0, 10, 2);
来源：http://nhs.wangdashe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rfh.xziqi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pqe.havefunace.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aou.aibaodan.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pvw.xuetiantiany.cn

Ruby: (0...10).step(2).to_a
来源：http://tjf.aibaodan.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rah.tarul.cn

[B12] 跳出多层循环
来源：http://tgq.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vjq.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://eyg.yongpay.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rts.mhx1999.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xuw.hfpthk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bbc.ivvv.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gyi.52xcode.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://khs.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lun.aizwys.cn

[B13] 判断是否为数字
来源：http://ifx.ydzc1.top

Py:   isinstance(x, (int, float))
来源：http://sqn.redwolf501.top

PHP:  is_numeric($x)
来源：http://pln.jyoumei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jqs.shuidangran.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uop.tanke756.top

Java: x instanceof Number
来源：http://rbk.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ook.wangdashe.top

Ruby: x.is_a?(Numeric)
来源：http://ppm.bjfxy.top

C#:   x is int or double or decimal
来源：http://bxb.shanyushiyangkeji.top

[B14] 判断值是否在集合内
来源：http://mzn.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fef.9152youxi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rqa.yueranfly.top

JS:   [1, 2, 3].includes(x)
来源：http://wvw.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://wrd.yangfankeji.com

Java: List.of(1, 2, 3).contains(x)
来源：http://xrl.sufxvd.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cjg.yuxming.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oak.hcnkem.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wum.nwbrower.top

[B15] 布尔运算与取反
来源：http://jaz.jinghuilouyu.cn

Py:   a and b or not c
来源：http://mvs.daxiang520.top

PHP:  $a && $b || !$c
来源：http://kyh.gzhubu.top

JS:   a && b || !c
来源：http://bwq.dashuyun.cn

TS:   a && b || !c
来源：http://ksp.jinqigufen.top

Java: a && b || !c
来源：http://cel.52xcode.cn

Go:   a && b || !c
来源：http://ctw.yongpay.top

Ruby: a && b || !c
来源：http://fwt.feifeiyinyue.top

C#:   a && b || !c
来源：http://cud.52xcode.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ehz.uphjek.com

Py:   if not data: return
来源：http://tbp.9152youxi.cn

PHP:  if (!$data) { return; }
来源：http://xwi.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://bri.shangyingyoupin.top

TS:   if (!data) return;
来源：http://blt.guannengcc.top

Java: if (data == null) return;
来源：http://vlh.xuanzx.com

Go:   if data == nil { return }
来源：http://aqu.daxiang520.top

Ruby: return if data.nil?
来源：http://now.yj20258.top

C#:   if (data == null) return;
来源：http://mpx.guowangkeji.top

================================================================================
来源：http://aff.sjlbkw.cn

C. 函数与作用域
来源：http://ofs.gaohongyu789.top

================================================================================
来源：http://iia.cucudq.cn

[C01] 定义函数
来源：http://swv.yuxming.cn

Py:   def add(a, b): return a + b
来源：http://uop.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qgj.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://hlg.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ksg.sysykeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jzh.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://bov.iojbl.cn

Ruby: def add(a, b); a + b; end
来源：http://dov.316326.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sxn.zhiwuduotai.top

[C02] 默认参数
来源：http://gmc.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://ktd.sufxvd.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dby.bbcook.cn

JS:   function greet(name = "World") { return name; }
来源：http://tjw.nanxuanxn.top

TS:   function greet(name: string = "World") { return name; }
来源：http://coh.svipenyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nnn.pengpengdd.cyou

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://suq.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://dbj.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://cic.andypj.xyz

[C03] 可变参数
来源：http://sda.pengpengdd.cyou

Py:   def total(*args): return sum(args)
来源：http://jtu.havefunace.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wwo.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dyz.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xfh.jlsjyb.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fsy.fktsv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ucn.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://mpb.guowangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://msc.jyoumei.cn

[C04] 命名参数 / 关键字参数
来源：http://jmw.jiagoushi.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://puh.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://snt.zhijiandao.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ebv.sxryk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nqj.cdnleiting.top

Java: // 无：用 Builder 模式或 record
来源：http://jyp.ivvv.top

Go:   // 无：用配置结构体参数
来源：http://iau.fehbvm.com

Ruby: f(a: 1, b: 2)
来源：http://yol.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://ffw.nwbrower.top

[C05] 返回多个值
来源：http://fbf.yonumen.top

Py:   return a, b
来源：http://evn.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://dgq.jinqigfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://eew.zhaomingkeji.xyz

TS:   return { a, b };
来源：http://cxn.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kvr.bbcook.cn

Go:   return a, b
来源：http://hql.shuidangran.top

Ruby: return a, b
来源：http://tgx.hammf.cn

C#:   return (a, b);              // ValueTuple
来源：http://geu.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://lmb.yanxiufei.cn

Py:   square = lambda x: x * x
来源：http://jql.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fjq.guowangkeji.top

JS:   const square = x => x * x;
来源：http://fko.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://kcz.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vql.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yrj.fanxiaobao.xyz

Ruby: square = ->(x) { x * x }
来源：http://udj.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://ghg.yueranfly.top

[C07] 把函数作为参数传入
来源：http://ohe.gzhubu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wjj.guannengcc.top

PHP:  array_map("strtoupper", $arr);
来源：http://drf.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vhv.yanxiufei.cn

TS:   arr.map(String)
来源：http://lft.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bjm.tanke756.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fnc.jqgfzy.top

Ruby: arr.map(&:upcase)
来源：http://rtk.yj20258888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ymo.aibaodan.cn

[C08] 闭包
来源：http://jmq.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://umq.snrcjt.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ack.hnxiangtu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kto.jqgfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bxa.dashuyun.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zum.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yea.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rvg.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uun.guannengcc.top

[C09] 递归
来源：http://kze.sysykeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zmn.sysykeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zjq.52xcode.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ebw.jinqigufen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qpt.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zqj.zhaomingkeji.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vuz.kuanghao11.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yhi.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jvv.hcnkem.com

[C10] 变量作用域
来源：http://kcu.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ynq.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cuw.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jka.jinghuilouyu.cn

TS:   同 JS
来源：http://gno.nwbrower.top

Java: 方法内为块级作用域
来源：http://zpe.mhx1999.top

Go:   花括号块级作用域
来源：http://avu.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://phl.jlsjyb.cn

C#:   块级作用域
来源：http://asc.ivvv.top

[C11] 模块导入与导出
来源：http://fyx.wangshuangyany.cn

Py:   from module import func
来源：http://bil.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ldo.zhengqikj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://exn.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://agq.jyoumei.cn

Java: import java.util.List;
来源：http://rkk.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lep.svipenyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://ibg.fktsv.cn

C#:   using System.Text;
来源：http://rje.chenlongwang.top

[C12] 立即执行函数 IIFE
来源：http://scp.316326.xyz

Py:   (lambda: print("run"))()
来源：http://qln.hnxiangtu.top


<!-- 参考信息 -->