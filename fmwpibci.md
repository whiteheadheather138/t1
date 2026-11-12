代发 wailian999

[A22] 获取字符串长度
来源：http://tfi.cheryme.top

Py:   len(s)
来源：http://bba.zhoulong.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://leh.hesvh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zic.mhx1999.top

TS:   s.length
来源：http://iar.ydzc1.top

Java: s.length()
来源：http://pku.gotoacloud.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eha.xuanzx.com

Ruby: s.length
来源：http://daq.yongpay.top

C#:   s.Length
来源：http://fim.vehdjk.com

[A23] 大小写转换
来源：http://gpb.meibo888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mab.smart0.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lzn.xuetiantiany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dxo.tianlin.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fzf.hnxiangtu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nen.meibo888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pri.chenzaomai.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lgu.hysaishi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tad.chenlongwang.top

[A24] 去除首尾空白
来源：http://fjz.xziqi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hub.shanyushiyangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://joh.yuxming.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wfb.jinghuilouyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ujo.daxiang520.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cec.zdbjq.cn

Go:   strings.TrimSpace(s)
来源：http://rhe.jiagoushi.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://deq.jqgfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ijn.smart0.xyz

[A25] 字符串比较
来源：http://ktr.snrcjt.cn

Py:   s1 == s2; s1 != s2
来源：http://rzj.nanxuanxn.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bno.jinqigufen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gns.gogol.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tsv.nwbrower.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://coa.chenzaomai.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pcq.hcnkem.com

Ruby: s1 == s2; s1 <=> s2
来源：http://tqz.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lsg.dashuyun.cn

[A26] 类型转换总览
来源：http://vff.fktsv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uqb.yuxming.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sqt.yuxming.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jcq.hywenlv.cn

TS:   Number() String() Boolean() x as number
来源：http://drb.fehbvm.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rlr.fktsv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cyv.jyoumei.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vgj.feifeiyinyue.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vxi.nanxuanxn.top

================================================================================
来源：http://ueq.cucudq.cn

B. 流程控制
来源：http://blr.ywan-chungtsiang.top

================================================================================
来源：http://prw.quarkkingdee.top

[B01] 条件判断 if / else
来源：http://otf.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zki.havefunace.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wjx.yfazqb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qvl.316326.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://feu.quarkkingdee.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rwa.havefunace.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lac.zhoulong.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eum.52xcode.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bpy.dashuyun.cn

[B02] 多分支 else if / elif
来源：http://die.jinyuanbaomall.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bcf.jyoumei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://plm.kuanghao11.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kjx.jinyuanbaomall.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nyl.ctjpmb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ogc.yj20258888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://itx.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yzi.nanxinkj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nmr.hfpthk.cn

[B03] switch / match / case
来源：http://vag.jyoumei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://snp.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ojn.sxryk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ynm.zhixingplan.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cpv.fktsv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://grn.ivvv.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yfh.aizwys.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vca.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bib.zycfv.cn

[B04] for 计数循环
来源：http://jdw.hongshengwenyu.top

Py:   for i in range(10): print(i)
来源：http://qvc.snrcjt.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xeu.ywan-chungtsiang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qko.xingfuxueyuan.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://slv.zycfv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wtg.jqgufenzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://edn.redwolf501.top

Ruby: 10.times { |i| puts i }
来源：http://osz.cheryme.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bnw.hywenlv.cn

[B05] 遍历数组 / 列表
来源：http://hzi.zhiwuduotai.top

Py:   for item in arr: print(item)
来源：http://kqo.xuetiantiany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ehb.hnqzz.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nvp.cqqwz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gbd.meibo888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://txt.jinqigufen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wur.ydzc1.top

Ruby: arr.each { |item| puts item }
来源：http://dyu.jinghuilouyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dru.cashguo.top

[B06] 遍历字典 / 对象
来源：http://lxf.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://atp.dianchejie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://htx.nwbrower.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ava.daxiang520.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jaw.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bsz.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nbr.pycfn.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ycy.shangyingyoupin.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rdk.xziqi.cn

[B07] while 循环
来源：http://sfc.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://rrn.zhiwuduotai.top

PHP:  while ($i < 10) { $i++; }
来源：http://zoy.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://lcb.nwbrower.top

TS:   while (i < 10) { i++; }
来源：http://ewc.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://ajl.zhongyouzk.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kyo.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://drw.fehbvm.com

C#:   while (i < 10) { i++; }
来源：http://nys.ydjk.org.cn

[B08] do-while（至少执行一次）
来源：http://ddi.zhengqikj.top

Py:   # 无 do-while：用 while True + break
来源：http://tqe.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zfh.xinyue.icu

JS:   do { i++; } while (i < 10);
来源：http://mmj.jqgufenzy.top

TS:   do { i++; } while (i < 10);
来源：http://dvm.gotoacloud.top

Java: do { i++; } while (i < 10);
来源：http://nwg.bbcook.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iaf.cheryme.top

Ruby: begin; i += 1; end while i < 10
来源：http://qjb.chenzaomai.com

C#:   do { i++; } while (i < 10);
来源：http://sgt.snrcjt.cn

[B09] break 与 continue
来源：http://sqq.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://clt.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kqj.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jcp.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sih.fktsv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sje.tianlin.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ylu.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yyz.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mqt.ivvv.top

[B10] 遍历同时拿索引
来源：http://bqz.zhiwuduotai.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ufz.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://udb.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vwc.316326.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jwf.gotoacloud.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://whs.snrcjt.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pmv.sxryk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sft.hesvh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ugo.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://shm.yvedp.cn

Py:   list(range(0, 10, 2))
来源：http://pua.gzhubu.top

PHP:  range(0, 10, 2);
来源：http://upl.sxryk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yha.xuetiantiany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sol.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ejw.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qwf.9152youxi.cn

Ruby: (0...10).step(2).to_a
来源：http://orh.sweek.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://izf.haohaochexian.top

[B12] 跳出多层循环
来源：http://btk.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xxd.yongpay.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ahs.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kdf.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ckp.tanke756.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fao.meibo888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zax.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://soa.gaohongyu789.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cxw.yueranfly.top

[B13] 判断是否为数字
来源：http://zdh.52xcode.cn

Py:   isinstance(x, (int, float))
来源：http://erj.jinyuanbaomall.cn

PHP:  is_numeric($x)
来源：http://klt.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wsm.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pfk.sysykeji.top

Java: x instanceof Number
来源：http://qrr.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cqj.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://jfp.tanke756.top

C#:   x is int or double or decimal
来源：http://lsh.jqgufenzy.top

[B14] 判断值是否在集合内
来源：http://hwk.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jco.chenjidiqi.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tff.bjfxy.top

JS:   [1, 2, 3].includes(x)
来源：http://zme.nwbrower.top

TS:   [1, 2, 3].includes(x)
来源：http://vsb.nanxuanxn.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jlw.pycfn.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mgv.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://bkx.yangfankeji.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oxv.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://ibr.ybcxt.top

Py:   a and b or not c
来源：http://lgd.dashuyun.cn

PHP:  $a && $b || !$c
来源：http://uso.zhiwuduotai.top

JS:   a && b || !c
来源：http://ezl.zhoulong.xyz

TS:   a && b || !c
来源：http://wsc.dianchejie.cn

Java: a && b || !c
来源：http://agu.shzxlz.cn

Go:   a && b || !c
来源：http://cuf.9152youxi.cn

Ruby: a && b || !c
来源：http://ctx.hywenlv.cn

C#:   a && b || !c
来源：http://ojc.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vxb.zhijiandao.cn

Py:   if not data: return
来源：http://cdi.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://rdd.iojbl.cn

JS:   if (!data) return;
来源：http://sdb.tarul.cn

TS:   if (!data) return;
来源：http://rgc.dashuyun.cn

Java: if (data == null) return;
来源：http://iqw.gaohongyu789.top

Go:   if data == nil { return }
来源：http://avg.hnqzz.top

Ruby: return if data.nil?
来源：http://wtu.gotoacloud.top

C#:   if (data == null) return;
来源：http://htt.hywenlv.cn

================================================================================
来源：http://muo.wangdashe.top

C. 函数与作用域
来源：http://bnv.hysaishi.cn

================================================================================
来源：http://cap.jqgfzy.top

[C01] 定义函数
来源：http://ftt.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://oow.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ism.dashuyun.cn

JS:   function add(a, b) { return a + b; }
来源：http://vob.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vtr.shzxlz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dwp.fehbvm.com

Go:   func add(a, b int) int { return a + b }
来源：http://hbd.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://zvf.yj202588.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://twu.fzhhl.top

[C02] 默认参数
来源：http://lck.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://caa.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qnh.guowangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://bok.yangfankeji.com

TS:   function greet(name: string = "World") { return name; }
来源：http://qyv.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://qnc.havefunace.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mzr.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://mlf.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://yvi.tarul.cn

[C03] 可变参数
来源：http://exz.dianchejie.cn

Py:   def total(*args): return sum(args)
来源：http://bzf.smart0.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dmb.fzhhl.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nvz.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lwa.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rwb.epnwcf.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qjp.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://gju.52xcode.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vfh.zhengqikj.top

[C04] 命名参数 / 关键字参数
来源：http://nto.cdnleiting.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ref.yongpay.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hxi.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://abf.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iuv.sxryk.cn

Java: // 无：用 Builder 模式或 record
来源：http://vfr.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://gwu.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://kca.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://yjw.zhijiandao.cn

[C05] 返回多个值
来源：http://ygj.shuidangran.top

Py:   return a, b
来源：http://pag.pengpengdd.cyou

PHP:  return [$a, $b];
来源：http://jsi.aibaodan.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fsh.sjlbkw.cn

TS:   return { a, b };
来源：http://pva.zdqjudy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ypa.jinqigfzy.top

Go:   return a, b
来源：http://exx.guannengcc.top

Ruby: return a, b
来源：http://zla.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://vkg.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://hke.shuidangran.top

Py:   square = lambda x: x * x
来源：http://lhd.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fos.cdnleiting.top

JS:   const square = x => x * x;
来源：http://sha.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://qnr.hesvh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pso.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://bpj.9152youxi.cn

Ruby: square = ->(x) { x * x }
来源：http://fdl.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://ohd.cucudq.cn

[C07] 把函数作为参数传入
来源：http://loa.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qww.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://hqt.yj20258.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vpl.ctjpmb.com

TS:   arr.map(String)
来源：http://cqm.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nxq.chenzaomai.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gnc.nwbrower.top

Ruby: arr.map(&:upcase)
来源：http://obj.xuanzx.com

C#:   arr.Select(s => s.ToUpper())
来源：http://mux.ydzc1.top

[C08] 闭包
来源：http://vzr.316326.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mkf.chenjidiqi.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nou.ydzc1.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://czk.cucudq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hcc.shuidangran.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ynp.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dyz.cqqwz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kyr.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rjr.sufxvd.cn

[C09] 递归
来源：http://rux.bbcook.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ayw.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://suv.gaohongyu789.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://icf.aibaodan.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ofm.jianghu66.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ist.hongshengwenyu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hfw.jinqigfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uej.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://adu.shangyingyoupin.top

[C10] 变量作用域
来源：http://vve.tianlin.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://acn.hysaishi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rca.hnqzz.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lwt.xuetiantiany.cn

TS:   同 JS
来源：http://bie.gogol.net.cn

Java: 方法内为块级作用域
来源：http://ppc.ydjk.org.cn

Go:   花括号块级作用域
来源：http://prr.zhoulong.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hly.hywenlv.cn

C#:   块级作用域
来源：http://pqu.gogol.net.cn

[C11] 模块导入与导出
来源：http://meg.xziqi.cn

Py:   from module import func
来源：http://cla.yongpay.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kvn.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://ryl.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ciu.yuxming.cn

Java: import java.util.List;
来源：http://msq.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gmy.tianlin.xyz

Ruby: require "json"; require_relative "./util"
来源：http://uid.pengpengdd.cyou

C#:   using System.Text;
来源：http://sxn.xziqi.cn

[C12] 立即执行函数 IIFE
来源：http://erq.ybcxt.top

Py:   (lambda: print("run"))()
来源：http://yaz.hywenlv.cn

PHP:  (function () { echo "run"; })();
来源：http://hhn.vqdsnc.cn

JS:   (() => { console.log("run"); })();
来源：http://vap.yueranfly.top

TS:   (() => { console.log("run"); })();
来源：http://beq.ybcxt.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wrf.fanxiaobao.xyz


<!-- 参考信息 -->