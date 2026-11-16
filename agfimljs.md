代发 wailian999

[A22] 获取字符串长度
来源：http://nug.ctjpmb.com

Py:   len(s)
来源：http://bny.fzhhl.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://voa.xingfuxueyuan.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cuy.hesvh.cn

TS:   s.length
来源：http://zwc.fktsv.cn

Java: s.length()
来源：http://tne.chenzaomai.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tdb.gaohongyu789.top

Ruby: s.length
来源：http://pen.epnwcf.com

C#:   s.Length
来源：http://nkf.shanyushiyangkeji.top

[A23] 大小写转换
来源：http://zud.zdbjq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wrq.xingfuxueyuan.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qkb.ppjwa.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://axh.hammf.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nqz.gaohongyu789.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pst.ppjwa.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kml.uphjek.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gym.tanke756.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kwg.0kj1m.cn

[A24] 去除首尾空白
来源：http://xjq.gogol.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wyr.wangshuangyany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hur.xinyue.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rbg.nwbrower.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iam.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mts.xylfe.cn

Go:   strings.TrimSpace(s)
来源：http://joa.yanxiufei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lof.gzhubu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fme.jiagoushi.top

[A25] 字符串比较
来源：http://ujh.wangdashe.top

Py:   s1 == s2; s1 != s2
来源：http://fyy.bjfxy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fyp.jyoumei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dep.hysaishi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://faj.mhx1999.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qww.zhaomingkeji.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jgn.mhx1999.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hka.zdqjudy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kby.shanyushiyangkeji.top

[A26] 类型转换总览
来源：http://dgy.ppjwa.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ozq.chenlongwang.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cgm.dianchejie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://umy.bbcook.cn

TS:   Number() String() Boolean() x as number
来源：http://vhx.jinghuilouyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xcq.dianchejie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://poe.xylfe.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fmd.uphjek.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kre.zhiwuduotai.top

================================================================================
来源：http://zzw.snrcjt.cn

B. 流程控制
来源：http://ofw.xziqi.cn

================================================================================
来源：http://kii.meibo888.top

[B01] 条件判断 if / else
来源：http://acg.316326.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://iei.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vvr.hnqzz.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zag.yongpay.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://eqa.hysaishi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lsi.sxryk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ewd.aizwys.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dbd.birdmap.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dxk.uphjek.com

[B02] 多分支 else if / elif
来源：http://skp.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dtl.uphjek.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://con.cqqwz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fek.ppjwa.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qzo.ydzc1.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lrl.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wsu.zhongyouzk.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wxz.sxryk.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wlw.ehwqpu.com

[B03] switch / match / case
来源：http://bqc.xinyue.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wkn.iojbl.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://axv.sjlbkw.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hvx.chenjidiqi.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iaz.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uzw.yj202588.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iby.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wby.hcnkem.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lip.xylfe.cn

[B04] for 计数循环
来源：http://xxs.sxryk.cn

Py:   for i in range(10): print(i)
来源：http://urp.cqqwz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lce.yongpay.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ztj.hywenlv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://azh.xylfe.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oiw.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kxx.dashuyun.cn

Ruby: 10.times { |i| puts i }
来源：http://kyt.iojbl.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wqk.jianghu66.top

[B05] 遍历数组 / 列表
来源：http://vfj.daxiang520.top

Py:   for item in arr: print(item)
来源：http://fev.yj20258888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bkt.fengsongda.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jvb.hysaishi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zyj.zhijiandao.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wnq.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ura.9152youxi.cn

Ruby: arr.each { |item| puts item }
来源：http://wyy.ydzc1.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ekz.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://xsw.yanxiufei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ngg.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kym.smart0.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://inv.smart0.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://egu.bbcook.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uvu.yangfankeji.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zxk.jqgfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ppi.jlsjyb.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aps.smart0.xyz

[B07] while 循环
来源：http://kuj.yanxiufei.cn

Py:   while i < 10: i += 1
来源：http://fqb.jianghu66.top

PHP:  while ($i < 10) { $i++; }
来源：http://xsa.zhongyouzk.top

JS:   while (i < 10) { i++; }
来源：http://nlc.zhoulong.xyz

TS:   while (i < 10) { i++; }
来源：http://qvu.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://hod.zhongyouzk.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zar.yj202588.top

Ruby: while i < 10; i += 1; end
来源：http://cxf.cqqwz.cn

C#:   while (i < 10) { i++; }
来源：http://veo.0kj1m.cn

[B08] do-while（至少执行一次）
来源：http://cjd.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://oou.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://hfi.jinqigufen.top

JS:   do { i++; } while (i < 10);
来源：http://ngt.jlsjyb.cn

TS:   do { i++; } while (i < 10);
来源：http://qyx.gaohongyu789.top

Java: do { i++; } while (i < 10);
来源：http://enu.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mxa.zdbjq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://agf.meibo888.top

C#:   do { i++; } while (i < 10);
来源：http://ihv.cdnleiting.top

[B09] break 与 continue
来源：http://mvc.9152youxi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rah.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rtl.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://djv.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qvj.vehdjk.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://imz.bbcook.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nrm.hongshengwenyu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://snb.gaohongyu789.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uam.ydzc1.top

[B10] 遍历同时拿索引
来源：http://qvz.uphjek.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ypm.chenjidiqi.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uom.kuanghao11.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://apx.shangyingyoupin.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://urp.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://njw.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://myw.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fea.gogol.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ddp.pengpengdd.cyou

[B11] 生成数字序列 / 区间
来源：http://fjv.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://atl.chenlongwang.top

PHP:  range(0, 10, 2);
来源：http://zao.vqdsnc.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tuo.zhiwuduotai.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qvt.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gen.cucudq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bng.hnqzz.top

Ruby: (0...10).step(2).to_a
来源：http://tzv.hongshengwenyu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fks.snrcjt.cn

[B12] 跳出多层循环
来源：http://qso.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://sth.ydjk.org.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://shq.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vvl.tian-w.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bbh.tarul.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dhf.nanxuanxn.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vci.jqgufenzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://owr.chenjidiqi.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cuo.c1oappe.top

[B13] 判断是否为数字
来源：http://qgq.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://ssk.hnqzz.top

PHP:  is_numeric($x)
来源：http://apk.cashguo.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zpp.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rir.cdnleiting.top

Java: x instanceof Number
来源：http://yue.daxiang520.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://elq.pengpengdd.cyou

Ruby: x.is_a?(Numeric)
来源：http://lwn.cdnleiting.top

C#:   x is int or double or decimal
来源：http://jtw.yj20258.top

[B14] 判断值是否在集合内
来源：http://qia.jinghuilouyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://owa.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eyv.yueranfly.top

JS:   [1, 2, 3].includes(x)
来源：http://hsb.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://wfy.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hen.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jrb.shangyingyoupin.top

Ruby: [1, 2, 3].include?(x)
来源：http://efl.hcnkem.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yso.gotoacloud.top

[B15] 布尔运算与取反
来源：http://kls.ctjpmb.com

Py:   a and b or not c
来源：http://mvu.yj20258888.top

PHP:  $a && $b || !$c
来源：http://bwn.c1oappe.top

JS:   a && b || !c
来源：http://wdc.hnqzz.top

TS:   a && b || !c
来源：http://qjr.0kj1m.cn

Java: a && b || !c
来源：http://mjl.aizwys.cn

Go:   a && b || !c
来源：http://luf.tian-w.cn

Ruby: a && b || !c
来源：http://ual.xuetiantiany.cn

C#:   a && b || !c
来源：http://zln.yanxiufei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ebt.xinyue.icu

Py:   if not data: return
来源：http://fli.pycfn.com

PHP:  if (!$data) { return; }
来源：http://brr.zycfv.cn

JS:   if (!data) return;
来源：http://nzd.smart0.xyz

TS:   if (!data) return;
来源：http://fzw.jiagoushi.top

Java: if (data == null) return;
来源：http://joa.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://kbi.gogol.net.cn

Ruby: return if data.nil?
来源：http://skt.jianghu66.top

C#:   if (data == null) return;
来源：http://muc.hcnkem.com

================================================================================
来源：http://pcc.ctjpmb.com

C. 函数与作用域
来源：http://uzq.yj20258.top

================================================================================
来源：http://jfn.vehdjk.com

[C01] 定义函数
来源：http://qov.hcnkem.com

Py:   def add(a, b): return a + b
来源：http://qyc.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ysc.shangyingyoupin.top

JS:   function add(a, b) { return a + b; }
来源：http://buv.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oyq.sweek.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bls.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://acy.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://goq.xuetiantiany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fyq.yangfankeji.com

[C02] 默认参数
来源：http://ctr.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://dvb.sjlbkw.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kol.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://rut.zhiwuduotai.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ppc.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pqj.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qhh.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://mdk.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://mxm.uphjek.com

[C03] 可变参数
来源：http://xqz.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://faz.hnxiangtu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fdf.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nqc.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ekv.gzhubu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ghg.xinyue.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lrh.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://gqr.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ehz.svipenyu.cn

[C04] 命名参数 / 关键字参数
来源：http://udd.andypj.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cev.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nwj.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vms.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://srt.havefunace.top

Java: // 无：用 Builder 模式或 record
来源：http://ikr.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://ajg.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://mcb.sysykeji.top

C#:   f(a: 1, b: 2)
来源：http://aem.dianchejie.cn

[C05] 返回多个值
来源：http://blb.guannengcc.top

Py:   return a, b
来源：http://pcs.yonumen.top

PHP:  return [$a, $b];
来源：http://dze.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zah.kuanghao11.cn

TS:   return { a, b };
来源：http://erc.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sxg.hnqzz.top

Go:   return a, b
来源：http://idk.shanyushiyangkeji.top

Ruby: return a, b
来源：http://dgd.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://mzt.ybcxt.top

[C06] 匿名函数 / lambda
来源：http://uam.cqqwz.cn

Py:   square = lambda x: x * x
来源：http://arw.feifeiyinyue.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qfi.jqgufenzy.top

JS:   const square = x => x * x;
来源：http://mhg.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://tuj.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ldk.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://yld.zycfv.cn

Ruby: square = ->(x) { x * x }
来源：http://dgp.zhixingplan.top

C#:   Func<int, int> square = x => x * x;
来源：http://yuu.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://aof.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ydr.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://ktn.jinqigfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://scj.zhaomingkeji.xyz

TS:   arr.map(String)
来源：http://ade.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qsn.smart0.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dwo.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://lph.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uyb.epnwcf.com

[C08] 闭包
来源：http://asw.redwolf501.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tcu.daria6918.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uwi.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xzh.yvedp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lnj.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://auo.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pvu.yonumen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pqw.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fuc.gaohongyu789.top

[C09] 递归
来源：http://mpv.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://usc.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yyo.meibo888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://myj.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pnc.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ysd.ydjk.org.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xky.jiagoushi.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qww.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ewc.guowangkeji.top

[C10] 变量作用域
来源：http://goy.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://opq.jiagoushi.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kiu.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ykb.aizwys.cn

TS:   同 JS
来源：http://xlp.gogol.net.cn

Java: 方法内为块级作用域
来源：http://qnm.cheryme.top

Go:   花括号块级作用域
来源：http://kby.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xen.guowangkeji.top

C#:   块级作用域
来源：http://pvh.fktsv.cn

[C11] 模块导入与导出
来源：http://npl.hnqzz.top

Py:   from module import func
来源：http://qmm.yonumen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lfx.jinyuanbaomall.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vuc.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lbe.yueranfly.top

Java: import java.util.List;
来源：http://joa.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tam.ppjwa.cn

Ruby: require "json"; require_relative "./util"
来源：http://bsv.tarul.cn

C#:   using System.Text;
来源：http://tre.jiagoushi.top

[C12] 立即执行函数 IIFE
来源：http://pjw.zhijiandao.cn

Py:   (lambda: print("run"))()
来源：http://psn.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://fxg.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://ekk.guowangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://szk.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pwt.chenjidiqi.icu


<!-- 参考信息 -->