代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aru.daria6918.cn

Ruby: gets.chomp
来源：http://gzm.dashuyun.cn

C#:   Console.ReadLine();
来源：http://knx.haohaochexian.top

[A21] 保留指定小数位输出
来源：http://smg.svipenyu.cn

Py:   f"{3.14159:.2f}"
来源：http://rog.xingfuxueyuan.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gxi.feifeiyinyue.top

JS:   (3.14159).toFixed(2)
来源：http://xad.c1oappe.top

TS:   (3.14159).toFixed(2)
来源：http://hup.yangfankeji.com

Java: String.format("%.2f", 3.14159)
来源：http://nsp.chenzaomai.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iwm.sjlbkw.cn

Ruby: format("%.2f", 3.14159)
来源：http://bxd.ywan-chungtsiang.top

C#:   3.14159.ToString("F2")
来源：http://pnk.yuanzhike.top

[A22] 获取字符串长度
来源：http://mgq.shanyushiyangkeji.top

Py:   len(s)
来源：http://ohe.epnwcf.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xgr.sysykeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vpc.birdmap.top

TS:   s.length
来源：http://pgz.ybcxt.top

Java: s.length()
来源：http://agj.zhiwuduotai.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iyb.guannengcc.top

Ruby: s.length
来源：http://rdl.c1oappe.top

C#:   s.Length
来源：http://okl.316326.xyz

[A23] 大小写转换
来源：http://wcy.ehwqpu.com

Py:   s.upper(); s.lower(); s.title()
来源：http://gaa.tarul.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ooi.9152youxi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ybj.zhijiandao.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://npd.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hul.yuanzhike.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://czp.gogol.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tjm.sxryk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hcm.svipenyu.cn

[A24] 去除首尾空白
来源：http://cji.ehwqpu.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://twn.uphjek.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hny.hammf.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xew.gaohongyu789.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pnh.tianlin.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vax.hysaishi.cn

Go:   strings.TrimSpace(s)
来源：http://jyc.xylfe.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ucc.bbcook.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://biu.jinghuilouyu.cn

[A25] 字符串比较
来源：http://sdq.316326.xyz

Py:   s1 == s2; s1 != s2
来源：http://amk.jyoumei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://msr.gzhubu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://api.ybcxt.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xky.xziqi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mex.quarkkingdee.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yhg.wangdashe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ujc.c1oappe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zhd.yongpay.top

[A26] 类型转换总览
来源：http://dor.jianghu66.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ude.havefunace.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dxf.jyoumei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kxa.guowangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://lxb.ywan-chungtsiang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gfi.jianghu66.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pyo.cqqwz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ujs.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uiq.fehbvm.com

================================================================================
来源：http://uma.sufxvd.cn

B. 流程控制
来源：http://zbf.dianchejie.cn

================================================================================
来源：http://tpf.zhoulong.xyz

[B01] 条件判断 if / else
来源：http://sji.sufxvd.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ltj.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ibx.birdmap.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gcm.shzxlz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qib.epnwcf.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://zjn.vehdjk.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dzl.zdbjq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bcc.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sfu.shuidangran.top

[B02] 多分支 else if / elif
来源：http://uyn.wangdashe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sxk.fktsv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kvo.0kj1m.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bhh.jinqigfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://exu.daria6918.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cub.svipenyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nyx.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uax.chenzaomai.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ceq.nwbrower.top

[B03] switch / match / case
来源：http://mmc.hywenlv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fry.zdbjq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jzo.hfpthk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zuu.daria6918.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://byd.svipenyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ywq.hfpthk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uoe.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tsf.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://imo.aizwys.cn

[B04] for 计数循环
来源：http://ogx.316326.xyz

Py:   for i in range(10): print(i)
来源：http://peq.wangshuangyany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vut.mhx1999.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rzk.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qlt.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rlp.guowangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pzw.yangfankeji.com

Ruby: 10.times { |i| puts i }
来源：http://zgj.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://plm.ppjwa.cn

[B05] 遍历数组 / 列表
来源：http://smv.fktsv.cn

Py:   for item in arr: print(item)
来源：http://eka.9152youxi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://muf.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jkd.jqgufenzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://axz.yonumen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ktg.iojbl.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pez.fengsongda.top

Ruby: arr.each { |item| puts item }
来源：http://twk.zhongyouzk.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xod.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://uab.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hwq.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://axc.yangfankeji.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://abh.yangfankeji.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bju.dashuyun.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cbx.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zpy.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wcr.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://awv.yanxiufei.cn

[B07] while 循环
来源：http://kms.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://emw.epnwcf.com

PHP:  while ($i < 10) { $i++; }
来源：http://ofd.yuxming.cn

JS:   while (i < 10) { i++; }
来源：http://nao.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://ewi.jyoumei.cn

Java: while (i < 10) { i++; }
来源：http://uzl.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vqt.cashguo.top

Ruby: while i < 10; i += 1; end
来源：http://xdz.ctjpmb.com

C#:   while (i < 10) { i++; }
来源：http://xpa.tanke756.top

[B08] do-while（至少执行一次）
来源：http://pyo.ivvv.top

Py:   # 无 do-while：用 while True + break
来源：http://jcp.xylfe.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jym.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://tpg.epnwcf.com

TS:   do { i++; } while (i < 10);
来源：http://ark.zhengqikj.top

Java: do { i++; } while (i < 10);
来源：http://wqa.hfpthk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ltw.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://gwc.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://kkm.feifeiyinyue.top

[B09] break 与 continue
来源：http://cfq.fanxiaobao.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bid.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://izg.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zcd.yueranfly.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fth.yfazqb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gqw.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://igq.sweek.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xgw.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hap.zhaomingkeji.xyz

[B10] 遍历同时拿索引
来源：http://plu.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iag.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xgl.yonumen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ulr.birdmap.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://olh.cdnleiting.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dxl.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bps.jlsjyb.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qyk.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dml.c1oappe.top

[B11] 生成数字序列 / 区间
来源：http://tvt.zdbjq.cn

Py:   list(range(0, 10, 2))
来源：http://ddw.jiagoushi.top

PHP:  range(0, 10, 2);
来源：http://ize.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kni.yanxiufei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jnh.aizwys.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ogs.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vgq.yonumen.top

Ruby: (0...10).step(2).to_a
来源：http://ydm.jyoumei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ukn.jiagoushi.top

[B12] 跳出多层循环
来源：http://jqr.zdbjq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ihh.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tub.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xtj.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iir.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hyg.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cqw.hesvh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aqf.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wnu.cashguo.top

[B13] 判断是否为数字
来源：http://zlx.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://fiv.pengpengdd.cyou

PHP:  is_numeric($x)
来源：http://dbx.jinqigufen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zpw.epnwcf.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://swp.tianlin.xyz

Java: x instanceof Number
来源：http://rrx.yfazqb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nrz.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://jva.uphjek.com

C#:   x is int or double or decimal
来源：http://shh.hcnkem.com

[B14] 判断值是否在集合内
来源：http://odn.zhengqikj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dok.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gbq.chenlongwang.top

JS:   [1, 2, 3].includes(x)
来源：http://gxl.yonumen.top

TS:   [1, 2, 3].includes(x)
来源：http://kih.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jvo.cdnleiting.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://obc.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ydm.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sht.nanxuanxn.top

[B15] 布尔运算与取反
来源：http://diu.ydjk.org.cn

Py:   a and b or not c
来源：http://sxc.birdmap.top

PHP:  $a && $b || !$c
来源：http://gzf.zdbjq.cn

JS:   a && b || !c
来源：http://eyv.shuidangran.top

TS:   a && b || !c
来源：http://gvo.ppjwa.cn

Java: a && b || !c
来源：http://trq.yanxiufei.cn

Go:   a && b || !c
来源：http://exs.ywan-chungtsiang.top

Ruby: a && b || !c
来源：http://dhf.yj20258.top

C#:   a && b || !c
来源：http://csa.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://ewt.c1oappe.top

Py:   if not data: return
来源：http://pui.kuanghao11.cn

PHP:  if (!$data) { return; }
来源：http://dlr.haohaochexian.top

JS:   if (!data) return;
来源：http://kii.uphjek.com

TS:   if (!data) return;
来源：http://ney.gaohongyu789.top

Java: if (data == null) return;
来源：http://blk.cheryme.top

Go:   if data == nil { return }
来源：http://ele.cqqwz.cn

Ruby: return if data.nil?
来源：http://hlp.chenzaomai.com

C#:   if (data == null) return;
来源：http://vqb.xuetiantiany.cn

================================================================================
来源：http://uva.yangfankeji.com

C. 函数与作用域
来源：http://btf.yvedp.cn

================================================================================
来源：http://bio.bbcook.cn

[C01] 定义函数
来源：http://jtu.sweek.top

Py:   def add(a, b): return a + b
来源：http://axd.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://chm.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://zbq.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uul.jinyuanbaomall.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tqq.redwolf501.top

Go:   func add(a, b int) int { return a + b }
来源：http://dgo.hnxiangtu.top

Ruby: def add(a, b); a + b; end
来源：http://ygw.andypj.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wmd.uphjek.com

[C02] 默认参数
来源：http://ezq.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://gfx.fengsongda.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xfu.jinqigufen.top

JS:   function greet(name = "World") { return name; }
来源：http://imo.yj20258.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tnu.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mlr.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://krs.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://mbd.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://hgt.aizwys.cn

[C03] 可变参数
来源：http://mqq.hesvh.cn

Py:   def total(*args): return sum(args)
来源：http://rzs.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sag.hfpthk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pfw.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zsu.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dnp.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tgw.52xcode.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wko.vqdsnc.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fct.bjfxy.top

[C04] 命名参数 / 关键字参数
来源：http://hwj.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cra.gaohongyu789.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dnl.meibo888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fcd.jinqigfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://obt.dashuyun.cn

Java: // 无：用 Builder 模式或 record
来源：http://rql.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://tln.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://gzi.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://qoi.zhiwuduotai.top

[C05] 返回多个值
来源：http://mji.ivvv.top

Py:   return a, b
来源：http://vie.dianchejie.cn

PHP:  return [$a, $b];
来源：http://kyj.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://puf.haohaochexian.top

TS:   return { a, b };
来源：http://njl.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vrt.ppjwa.cn

Go:   return a, b
来源：http://osk.fanxiaobao.xyz

Ruby: return a, b
来源：http://ial.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://bmi.shangyingyoupin.top

[C06] 匿名函数 / lambda
来源：http://tkc.hammf.cn

Py:   square = lambda x: x * x
来源：http://iys.xziqi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://okm.dianchejie.cn

JS:   const square = x => x * x;
来源：http://khl.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://rnh.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zep.hesvh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rtj.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://dka.yj202588.top

C#:   Func<int, int> square = x => x * x;
来源：http://hip.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://ezv.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vga.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cir.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qpu.fehbvm.com

TS:   arr.map(String)
来源：http://dib.andypj.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://opy.ehwqpu.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bqp.chenzaomai.com

Ruby: arr.map(&:upcase)
来源：http://tku.zycfv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://roo.sweek.top

[C08] 闭包
来源：http://wkz.dianchejie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nub.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xxs.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://omq.jqgufenzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fjd.shanyushiyangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mog.zhaomingkeji.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fkd.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lkx.hnxiangtu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qpw.andypj.xyz

[C09] 递归
来源：http://jnd.nwbrower.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://myb.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xgs.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ofe.aizwys.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://alq.shuidangran.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dnc.wangdashe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ydz.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wly.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zyf.cqqwz.cn

[C10] 变量作用域
来源：http://oom.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xwl.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yci.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fxp.ydzc1.top

TS:   同 JS
来源：http://mkh.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://yut.svipenyu.cn

Go:   花括号块级作用域
来源：http://qzv.xinyue.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://plj.birdmap.top

C#:   块级作用域
来源：http://fbi.yanxiufei.cn

[C11] 模块导入与导出
来源：http://umg.iojbl.cn

Py:   from module import func
来源：http://alt.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pud.xinyue.icu


<!-- 参考信息 -->