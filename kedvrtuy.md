代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://veu.0kj1m.cn

Ruby: gets.chomp
来源：http://kzy.jqgufenzy.top

C#:   Console.ReadLine();
来源：http://vlv.chenlongwang.top

[A21] 保留指定小数位输出
来源：http://wch.snrcjt.cn

Py:   f"{3.14159:.2f}"
来源：http://sih.kuanghao11.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://umg.fengsongda.top

JS:   (3.14159).toFixed(2)
来源：http://erx.tarul.cn

TS:   (3.14159).toFixed(2)
来源：http://bno.yj20258.top

Java: String.format("%.2f", 3.14159)
来源：http://mtv.hfpthk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lcq.vehdjk.com

Ruby: format("%.2f", 3.14159)
来源：http://tgw.0kj1m.cn

C#:   3.14159.ToString("F2")
来源：http://yqb.uphjek.com

[A22] 获取字符串长度
来源：http://sas.yueranfly.top

Py:   len(s)
来源：http://npl.zdbjq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qll.zhaomingkeji.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cgp.hnxiangtu.top

TS:   s.length
来源：http://ikb.svipenyu.cn

Java: s.length()
来源：http://gsw.shanyushiyangtech.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fla.nanxinkj.top

Ruby: s.length
来源：http://tnu.sweek.top

C#:   s.Length
来源：http://skp.zhijiandao.cn

[A23] 大小写转换
来源：http://uut.iojbl.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://drm.sufxvd.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ovt.sysykeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cua.jqgfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fne.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wyd.birdmap.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zzs.zhengqikj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vap.xylfe.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zch.havefunace.top

[A24] 去除首尾空白
来源：http://yqk.havefunace.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qea.jiagoushi.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lhs.hammf.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://spl.cheryme.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fxd.vehdjk.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://asx.zhaomingkeji.xyz

Go:   strings.TrimSpace(s)
来源：http://lxo.jianghu66.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dwd.sysykeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zwq.iojbl.cn

[A25] 字符串比较
来源：http://qow.ctjpmb.com

Py:   s1 == s2; s1 != s2
来源：http://tzq.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kjl.hammf.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dur.cashguo.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://asm.gaohongyu789.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dgi.jqgfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pzf.tanke756.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ipt.yvedp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rlo.guowangkeji.top

[A26] 类型转换总览
来源：http://tri.havefunace.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lqn.epnwcf.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qjz.gaohongyu789.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fcy.shanyushiyangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://ioj.yuxming.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qvt.gaohongyu789.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ogh.tanke756.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://uwt.jinghuilouyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pbw.pengpengdd.cyou

================================================================================
来源：http://msj.yanxiufei.cn

B. 流程控制
来源：http://jrj.jinqigufen.top

================================================================================
来源：http://ezs.zhijiandao.cn

[B01] 条件判断 if / else
来源：http://dhp.smart0.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://nfz.316326.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bgb.havefunace.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kvt.tanke756.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iji.chenlongwang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jid.shanyushiyangtech.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yyp.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oqs.yvedp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xvw.c1oappe.top

[B02] 多分支 else if / elif
来源：http://rih.daxiang520.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ila.quarkkingdee.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qgp.yongpay.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hvq.tian-w.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qer.xuanzx.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sen.gzhubu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vqm.zhixingplan.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nfw.ydjk.org.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://llp.chenlongwang.top

[B03] switch / match / case
来源：http://sbx.gaohongyu789.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zsq.zhijiandao.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://enf.aizwys.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lit.kuanghao11.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fft.guowangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tgb.gaohongyu789.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mio.zhaomingkeji.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://meh.sysykeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aee.zdqjudy.top

[B04] for 计数循环
来源：http://qyk.pycfn.com

Py:   for i in range(10): print(i)
来源：http://das.shanyushiyangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://erf.shuidangran.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rdt.havefunace.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kfv.xziqi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ehu.hnqzz.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bin.zdqjudy.top

Ruby: 10.times { |i| puts i }
来源：http://gny.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gih.yonumen.top

[B05] 遍历数组 / 列表
来源：http://csd.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://loa.yfazqb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xmp.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wjf.dianchejie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fcd.zhiwuduotai.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dja.vehdjk.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gnj.redwolf501.top

Ruby: arr.each { |item| puts item }
来源：http://fxi.chenlongwang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eqn.yuanzhike.top

[B06] 遍历字典 / 对象
来源：http://jjv.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xrz.haohaochexian.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bwo.shuidangran.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vzx.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vua.yonumen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dwr.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ikc.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sxw.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lsu.ctjpmb.com

[B07] while 循环
来源：http://pdm.tarul.cn

Py:   while i < 10: i += 1
来源：http://idv.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://naw.bjfxy.top

JS:   while (i < 10) { i++; }
来源：http://gfo.yuanzhike.top

TS:   while (i < 10) { i++; }
来源：http://bwx.yj202588.top

Java: while (i < 10) { i++; }
来源：http://jzc.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://div.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://rba.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://ffn.epnwcf.com

[B08] do-while（至少执行一次）
来源：http://fkv.zhengqikj.top

Py:   # 无 do-while：用 while True + break
来源：http://obt.yongpay.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cdo.ydzc1.top

JS:   do { i++; } while (i < 10);
来源：http://xdp.c1oappe.top

TS:   do { i++; } while (i < 10);
来源：http://zph.c1oappe.top

Java: do { i++; } while (i < 10);
来源：http://cqg.jlsjyb.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pjy.uphjek.com

Ruby: begin; i += 1; end while i < 10
来源：http://ysi.9152youxi.cn

C#:   do { i++; } while (i < 10);
来源：http://mrj.fzhhl.top

[B09] break 与 continue
来源：http://typ.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dbe.sufxvd.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wzr.xinyue.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pqn.cashguo.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://thd.sweek.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tsz.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gub.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fbw.svipenyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oty.gogol.net.cn

[B10] 遍历同时拿索引
来源：http://hrv.mhx1999.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jpq.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://egt.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wxu.yueranfly.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ujk.zhongyouzk.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qim.jinghuilouyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kjz.birdmap.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://asc.haohaochexian.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fku.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://chw.zhoulong.xyz

Py:   list(range(0, 10, 2))
来源：http://oal.fengsongda.top

PHP:  range(0, 10, 2);
来源：http://vny.tarul.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ezi.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://maj.chenjidiqi.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qri.iojbl.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nhp.jinqigfzy.top

Ruby: (0...10).step(2).to_a
来源：http://dok.chenzaomai.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gxp.hnxiangtu.top

[B12] 跳出多层循环
来源：http://psc.xuanzx.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://urf.chenjidiqi.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://nyc.yj20258.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kpz.xuanzx.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xjr.ybcxt.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vrd.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wsb.ydjk.org.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hib.sufxvd.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uno.hysaishi.cn

[B13] 判断是否为数字
来源：http://old.jlsjyb.cn

Py:   isinstance(x, (int, float))
来源：http://kim.hfpthk.cn

PHP:  is_numeric($x)
来源：http://nse.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cgc.zhixingplan.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uyr.wangdashe.top

Java: x instanceof Number
来源：http://hai.iojbl.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zid.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://bfm.chenlongwang.top

C#:   x is int or double or decimal
来源：http://fua.quarkkingdee.top

[B14] 判断值是否在集合内
来源：http://vwr.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pfk.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mqi.iojbl.cn

JS:   [1, 2, 3].includes(x)
来源：http://der.jinqigfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://skl.cheryme.top

Java: List.of(1, 2, 3).contains(x)
来源：http://odj.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wod.xingfuxueyuan.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://bbk.fehbvm.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://spn.zhongyouzk.top

[B15] 布尔运算与取反
来源：http://qnz.sufxvd.cn

Py:   a and b or not c
来源：http://biv.xylfe.cn

PHP:  $a && $b || !$c
来源：http://mys.chenzaomai.com

JS:   a && b || !c
来源：http://urd.jiagoushi.top

TS:   a && b || !c
来源：http://jtt.vqdsnc.cn

Java: a && b || !c
来源：http://tec.wangshuangyany.cn

Go:   a && b || !c
来源：http://wxk.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://uwg.wangshuangyany.cn

C#:   a && b || !c
来源：http://weq.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://abg.havefunace.top

Py:   if not data: return
来源：http://fou.aibaodan.cn

PHP:  if (!$data) { return; }
来源：http://iex.jqgufenzy.top

JS:   if (!data) return;
来源：http://bbx.cheryme.top

TS:   if (!data) return;
来源：http://xwj.jyoumei.cn

Java: if (data == null) return;
来源：http://nps.fanxiaobao.xyz

Go:   if data == nil { return }
来源：http://xdo.yj20258.top

Ruby: return if data.nil?
来源：http://hpu.smart0.xyz

C#:   if (data == null) return;
来源：http://qgi.redwolf501.top

================================================================================
来源：http://cxy.yj202588.top

C. 函数与作用域
来源：http://pxi.xuetiantiany.cn

================================================================================
来源：http://drp.aibaodan.cn

[C01] 定义函数
来源：http://xsn.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://yvt.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nrg.hysaishi.cn

JS:   function add(a, b) { return a + b; }
来源：http://kjh.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gcb.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kns.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://elz.nanxinkj.top

Ruby: def add(a, b); a + b; end
来源：http://xcr.shuidangran.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://poh.hongshengwenyu.top

[C02] 默认参数
来源：http://hvx.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://dnp.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fyu.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://ues.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ayf.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nwv.ybcxt.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jfx.fengsongda.top

Ruby: def greet(name = "World") = name
来源：http://lzm.xziqi.cn

C#:   string Greet(string name = "World") => name;
来源：http://oog.hysaishi.cn

[C03] 可变参数
来源：http://pgm.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://dsa.andypj.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lha.birdmap.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://swc.guannengcc.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://apw.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dnn.zycfv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cft.chenzaomai.com

Ruby: def total(*nums); nums.sum; end
来源：http://ggu.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://njy.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://ydf.xinyue.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://loy.hcnkem.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xew.daria6918.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dyc.fengsongda.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tsy.wangdashe.top

Java: // 无：用 Builder 模式或 record
来源：http://zsz.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://bbn.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://axl.hammf.cn

C#:   f(a: 1, b: 2)
来源：http://qxb.jqgufenzy.top

[C05] 返回多个值
来源：http://lsk.hammf.cn

Py:   return a, b
来源：http://uxq.guannengcc.top

PHP:  return [$a, $b];
来源：http://zhc.zhoulong.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://xoi.havefunace.top

TS:   return { a, b };
来源：http://vih.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://icv.havefunace.top

Go:   return a, b
来源：http://yja.dashuyun.cn

Ruby: return a, b
来源：http://ncc.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://wkk.yangfankeji.com

[C06] 匿名函数 / lambda
来源：http://kzk.guannengcc.top

Py:   square = lambda x: x * x
来源：http://mzu.vehdjk.com

PHP:  $square = fn($x) => $x * $x;
来源：http://hon.shuidangran.top

JS:   const square = x => x * x;
来源：http://qdo.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://tkk.hywenlv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jew.guowangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://lva.dashuyun.cn

Ruby: square = ->(x) { x * x }
来源：http://ymk.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://mdn.zhijiandao.cn

[C07] 把函数作为参数传入
来源：http://ipv.cdnleiting.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ddx.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://vuk.hongshengwenyu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://epj.zhijiandao.cn

TS:   arr.map(String)
来源：http://lmh.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://unk.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://daa.iojbl.cn

Ruby: arr.map(&:upcase)
来源：http://lmm.shanyushiyangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qar.jqgfzy.top

[C08] 闭包
来源：http://dkn.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eey.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xcf.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jhq.ctjpmb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://plc.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ayi.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bmu.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dgx.cqqwz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hrj.52xcode.cn

[C09] 递归
来源：http://mxn.zhaomingkeji.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hid.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hdf.zhixingplan.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mso.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ahz.chenlongwang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lcy.jinqigfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mrr.zycfv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dyq.zhongyouzk.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mmy.chenlongwang.top

[C10] 变量作用域
来源：http://osb.snrcjt.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sjq.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://llg.zhoulong.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bgu.ydjk.org.cn

TS:   同 JS
来源：http://lrq.xziqi.cn

Java: 方法内为块级作用域
来源：http://nti.sxryk.cn

Go:   花括号块级作用域
来源：http://fuw.xuetiantiany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cso.xylfe.cn

C#:   块级作用域
来源：http://zox.jlsjyb.cn

[C11] 模块导入与导出
来源：http://wew.yuanzhike.top

Py:   from module import func
来源：http://sew.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cgp.sweek.top


<!-- 参考信息 -->