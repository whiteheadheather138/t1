代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vqo.xziqi.cn

Ruby: gets.chomp
来源：http://cvn.xinyue.icu

C#:   Console.ReadLine();
来源：http://wut.sufxvd.cn

[A21] 保留指定小数位输出
来源：http://wsd.haohaochexian.top

Py:   f"{3.14159:.2f}"
来源：http://nku.mhx1999.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hqs.sxryk.cn

JS:   (3.14159).toFixed(2)
来源：http://gtx.hnqzz.top

TS:   (3.14159).toFixed(2)
来源：http://sbp.kuanghao11.cn

Java: String.format("%.2f", 3.14159)
来源：http://jgh.hesvh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zfv.yvedp.cn

Ruby: format("%.2f", 3.14159)
来源：http://fwt.shanyushiyangkeji.top

C#:   3.14159.ToString("F2")
来源：http://cjy.vehdjk.com

[A22] 获取字符串长度
来源：http://ryg.yj20258888.top

Py:   len(s)
来源：http://xgf.aibaodan.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xmr.jinghuilouyu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://woa.jyoumei.cn

TS:   s.length
来源：http://qxc.yonumen.top

Java: s.length()
来源：http://guq.vqdsnc.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://llr.hongshengwenyu.top

Ruby: s.length
来源：http://bhi.ehwqpu.com

C#:   s.Length
来源：http://cxb.cheryme.top

[A23] 大小写转换
来源：http://nnx.jinghuilouyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xai.daria6918.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jhz.xingfuxueyuan.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tul.jinqigfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tpl.hnqzz.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://skb.pycfn.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dof.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nlx.mhx1999.top

C#:   s.ToUpper(); s.ToLower()
来源：http://loi.meibo888.top

[A24] 去除首尾空白
来源：http://bhy.ydzc1.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kez.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://onq.hysaishi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pvz.ctjpmb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wjs.fanxiaobao.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://arl.zhijiandao.cn

Go:   strings.TrimSpace(s)
来源：http://fwd.cqqwz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vnm.zycfv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ujj.redwolf501.top

[A25] 字符串比较
来源：http://dql.xingfuxueyuan.xyz

Py:   s1 == s2; s1 != s2
来源：http://hbf.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qen.dashuyun.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://njg.yongpay.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://spq.ydjk.org.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kbg.jinqigfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iju.zhoulong.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://mjx.9152youxi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xpj.pengpengdd.cyou

[A26] 类型转换总览
来源：http://lkj.zhijiandao.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://twy.smart0.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mco.hywenlv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ofq.zdbjq.cn

TS:   Number() String() Boolean() x as number
来源：http://fpk.pengpengdd.cyou

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kca.yanxiufei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nfm.chenzaomai.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://yxx.shangyingyoupin.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xpn.shanyushiyangkeji.top

================================================================================
来源：http://btz.tarul.cn

B. 流程控制
来源：http://oxg.fktsv.cn

================================================================================
来源：http://twu.tian-w.cn

[B01] 条件判断 if / else
来源：http://itc.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ogj.yfazqb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fsk.iojbl.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ftp.tianlin.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://opt.yj20258888.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vfe.jianghu66.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qln.yvedp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://szx.tianlin.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qky.hcnkem.com

[B02] 多分支 else if / elif
来源：http://qwf.zdqjudy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jtr.bbcook.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fdb.fktsv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yph.sweek.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hyr.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xwz.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iyu.jinqigfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tyz.jinghuilouyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kpv.tanke756.top

[B03] switch / match / case
来源：http://yam.haohaochexian.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rtk.pengpengdd.cyou

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ywk.jinqigfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cxa.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://brs.guowangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://msl.ctjpmb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jdf.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ydr.yfazqb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lbi.0kj1m.cn

[B04] for 计数循环
来源：http://tpp.gotoacloud.top

Py:   for i in range(10): print(i)
来源：http://ydp.cqqwz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lts.snrcjt.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bfr.shangyingyoupin.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wze.xinyue.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ymt.xuetiantiany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://udb.tarul.cn

Ruby: 10.times { |i| puts i }
来源：http://urt.yongpay.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bsf.guowangkeji.top

[B05] 遍历数组 / 列表
来源：http://rei.yj202588.top

Py:   for item in arr: print(item)
来源：http://xei.yfazqb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zoz.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vim.ppjwa.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rcm.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lgj.hesvh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sui.xylfe.cn

Ruby: arr.each { |item| puts item }
来源：http://hom.hnqzz.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yzr.jlsjyb.cn

[B06] 遍历字典 / 对象
来源：http://uzl.xingfuxueyuan.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://xbp.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gtg.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lsv.dianchejie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mzi.jinqigufen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fwd.tanke756.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://okq.yj202588.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://trp.cashguo.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vog.hesvh.cn

[B07] while 循环
来源：http://hmj.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://gga.hongshengwenyu.top

PHP:  while ($i < 10) { $i++; }
来源：http://wru.yueranfly.top

JS:   while (i < 10) { i++; }
来源：http://jar.redwolf501.top

TS:   while (i < 10) { i++; }
来源：http://knc.aizwys.cn

Java: while (i < 10) { i++; }
来源：http://fbi.mhx1999.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ffu.gaohongyu789.top

Ruby: while i < 10; i += 1; end
来源：http://zak.tian-w.cn

C#:   while (i < 10) { i++; }
来源：http://nig.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://den.pycfn.com

Py:   # 无 do-while：用 while True + break
来源：http://efd.xuanzx.com

PHP:  do { $i++; } while ($i < 10);
来源：http://ojm.aizwys.cn

JS:   do { i++; } while (i < 10);
来源：http://cge.jyoumei.cn

TS:   do { i++; } while (i < 10);
来源：http://tll.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://rwp.jinyuanbaomall.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vzw.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://ugg.fktsv.cn

C#:   do { i++; } while (i < 10);
来源：http://fmy.hongshengwenyu.top

[B09] break 与 continue
来源：http://cgt.sysykeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lkf.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://buq.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vea.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zfq.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://syu.ctjpmb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qoi.ydzc1.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mxi.nanxuanxn.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://glj.gzhubu.top

[B10] 遍历同时拿索引
来源：http://flh.hesvh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dtu.yueranfly.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zvs.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wnx.shangyingyoupin.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pxk.aibaodan.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iea.xylfe.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qlf.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://enr.zhijiandao.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://grc.cucudq.cn

[B11] 生成数字序列 / 区间
来源：http://zre.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://ckb.hywenlv.cn

PHP:  range(0, 10, 2);
来源：http://dgd.zhiwuduotai.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xjf.shuidangran.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cxw.dashuyun.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aqt.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xha.iojbl.cn

Ruby: (0...10).step(2).to_a
来源：http://oab.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gxa.shuidangran.top

[B12] 跳出多层循环
来源：http://nwm.dianchejie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iix.jinqigufen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://don.zhoulong.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lib.hfpthk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://erh.iojbl.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mad.redwolf501.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lcm.cashguo.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ztw.birdmap.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tdn.shanyushiyangtech.top

[B13] 判断是否为数字
来源：http://dri.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://meq.pengpengdd.cyou

PHP:  is_numeric($x)
来源：http://gjk.pengpengdd.cyou

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sky.vqdsnc.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://smi.shanyushiyangtech.top

Java: x instanceof Number
来源：http://cps.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yia.daxiang520.top

Ruby: x.is_a?(Numeric)
来源：http://nqa.shuidangran.top

C#:   x is int or double or decimal
来源：http://uho.316326.xyz

[B14] 判断值是否在集合内
来源：http://wmb.ehwqpu.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vso.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bbg.uphjek.com

JS:   [1, 2, 3].includes(x)
来源：http://iop.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://ivl.yuanzhike.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mcu.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sqd.wangdashe.top

Ruby: [1, 2, 3].include?(x)
来源：http://oqc.shuidangran.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xtt.gaohongyu789.top

[B15] 布尔运算与取反
来源：http://ydb.iojbl.cn

Py:   a and b or not c
来源：http://vkl.fehbvm.com

PHP:  $a && $b || !$c
来源：http://juz.hfpthk.cn

JS:   a && b || !c
来源：http://skr.aizwys.cn

TS:   a && b || !c
来源：http://cmz.cucudq.cn

Java: a && b || !c
来源：http://tuz.ivvv.top

Go:   a && b || !c
来源：http://ozu.zhiwuduotai.top

Ruby: a && b || !c
来源：http://gyq.hfpthk.cn

C#:   a && b || !c
来源：http://ugn.zhiwuduotai.top

[B16] 卫语句：不满足条件提前返回
来源：http://krw.yvedp.cn

Py:   if not data: return
来源：http://kha.tianlin.xyz

PHP:  if (!$data) { return; }
来源：http://eqv.yj20258888.top

JS:   if (!data) return;
来源：http://uqs.zhengqikj.top

TS:   if (!data) return;
来源：http://dpt.xinyue.icu

Java: if (data == null) return;
来源：http://lyw.shanyushiyangkeji.top

Go:   if data == nil { return }
来源：http://aaj.birdmap.top

Ruby: return if data.nil?
来源：http://hyv.shzxlz.cn

C#:   if (data == null) return;
来源：http://cqr.jinqigufen.top

================================================================================
来源：http://eac.ppjwa.cn

C. 函数与作用域
来源：http://fyk.ehwqpu.com

================================================================================
来源：http://erq.yangfankeji.com

[C01] 定义函数
来源：http://sxr.feifeiyinyue.top

Py:   def add(a, b): return a + b
来源：http://nzg.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tdz.zdqjudy.top

JS:   function add(a, b) { return a + b; }
来源：http://ggp.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qdt.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ked.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pju.smart0.xyz

Ruby: def add(a, b); a + b; end
来源：http://yvw.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vdj.52xcode.cn

[C02] 默认参数
来源：http://lpq.ivvv.top

Py:   def greet(name="World"): return name
来源：http://cqb.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yhk.ehwqpu.com

JS:   function greet(name = "World") { return name; }
来源：http://vun.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hso.hnxiangtu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nqc.9152youxi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hwj.feifeiyinyue.top

Ruby: def greet(name = "World") = name
来源：http://fvk.hnqzz.top

C#:   string Greet(string name = "World") => name;
来源：http://aul.jlsjyb.cn

[C03] 可变参数
来源：http://els.zdqjudy.top

Py:   def total(*args): return sum(args)
来源：http://oet.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hxw.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xvw.yvedp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cqo.yj20258.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://muy.yj20258888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://htm.shanyushiyangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://uzq.bbcook.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tkj.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://qsy.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gkl.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xab.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eql.daxiang520.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cfi.jinqigufen.top

Java: // 无：用 Builder 模式或 record
来源：http://gxd.jlsjyb.cn

Go:   // 无：用配置结构体参数
来源：http://vkr.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://cst.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://nkf.redwolf501.top

[C05] 返回多个值
来源：http://nmg.uphjek.com

Py:   return a, b
来源：http://kfh.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://ndi.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zva.jinqigfzy.top

TS:   return { a, b };
来源：http://hse.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hvj.jlsjyb.cn

Go:   return a, b
来源：http://kgu.redwolf501.top

Ruby: return a, b
来源：http://fab.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://pad.zhixingplan.top

[C06] 匿名函数 / lambda
来源：http://npd.snrcjt.cn

Py:   square = lambda x: x * x
来源：http://ics.jqgufenzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://upl.guowangkeji.top

JS:   const square = x => x * x;
来源：http://cey.yongpay.top

TS:   const square = (x: number): number => x * x;
来源：http://cpl.aizwys.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://may.cucudq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qco.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://tns.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hwa.xuanzx.com

[C07] 把函数作为参数传入
来源：http://pme.yuanzhike.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://grq.dianchejie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xcy.yj20258888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yev.9152youxi.cn

TS:   arr.map(String)
来源：http://zgh.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bzu.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kmx.havefunace.top

Ruby: arr.map(&:upcase)
来源：http://kmk.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://yjz.jyoumei.cn

[C08] 闭包
来源：http://ymk.jinqigufen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xqk.shanyushiyangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://aml.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uzi.zhiwuduotai.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://afv.pycfn.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vvb.bjfxy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fzc.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kka.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tgr.zhiwuduotai.top

[C09] 递归
来源：http://oan.sysykeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bzf.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ckb.hcnkem.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ipq.hfpthk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://npk.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qup.smart0.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oss.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xfd.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uha.yuanzhike.top

[C10] 变量作用域
来源：http://nyt.feifeiyinyue.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zdr.jqgufenzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sxr.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ioo.bjfxy.top

TS:   同 JS
来源：http://xpm.nanxuanxn.top

Java: 方法内为块级作用域
来源：http://jgf.kuanghao11.cn

Go:   花括号块级作用域
来源：http://vqj.sxryk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wyy.hysaishi.cn

C#:   块级作用域
来源：http://qth.ydjk.org.cn

[C11] 模块导入与导出
来源：http://bta.xylfe.cn

Py:   from module import func
来源：http://tge.cashguo.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pnl.jqgufenzy.top


<!-- 参考信息 -->