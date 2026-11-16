代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://mze.aibaodan.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ccr.yanxiufei.cn

TS:   // Node.js：readline 模块
来源：http://dfs.andypj.xyz

Java: new Scanner(System.in).nextLine()
来源：http://twk.aibaodan.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ufq.cucudq.cn

Ruby: gets.chomp
来源：http://yag.gotoacloud.top

C#:   Console.ReadLine();
来源：http://fgb.tarul.cn

[A21] 保留指定小数位输出
来源：http://ouj.chenjidiqi.icu

Py:   f"{3.14159:.2f}"
来源：http://pju.jinyuanbaomall.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qgi.daria6918.cn

JS:   (3.14159).toFixed(2)
来源：http://rvp.xuanzx.com

TS:   (3.14159).toFixed(2)
来源：http://sdd.yonumen.top

Java: String.format("%.2f", 3.14159)
来源：http://kev.cucudq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jcx.gzhubu.top

Ruby: format("%.2f", 3.14159)
来源：http://jeq.hnqzz.top

C#:   3.14159.ToString("F2")
来源：http://hwu.zhoulong.xyz

[A22] 获取字符串长度
来源：http://ben.meibo888.top

Py:   len(s)
来源：http://din.shuidangran.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kuw.9152youxi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xyw.ybcxt.top

TS:   s.length
来源：http://uzo.yuanzhike.top

Java: s.length()
来源：http://vfw.hesvh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nld.xinyue.icu

Ruby: s.length
来源：http://iry.52xcode.cn

C#:   s.Length
来源：http://oge.chenzaomai.com

[A23] 大小写转换
来源：http://iyp.gaohongyu789.top

Py:   s.upper(); s.lower(); s.title()
来源：http://tid.c1oappe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://exe.dianchejie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gtp.hnqzz.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cyk.epnwcf.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zle.hnxiangtu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cgi.xuetiantiany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mhl.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cco.yonumen.top

[A24] 去除首尾空白
来源：http://ctn.ydzc1.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yep.gotoacloud.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://igf.jqgufenzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hnp.aizwys.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dip.zycfv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lcc.zycfv.cn

Go:   strings.TrimSpace(s)
来源：http://nrf.ivvv.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fnl.jianghu66.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ump.yongpay.top

[A25] 字符串比较
来源：http://pxi.zycfv.cn

Py:   s1 == s2; s1 != s2
来源：http://jdv.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iyy.cqqwz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qdy.andypj.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xrg.sxryk.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://djj.sysykeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qjg.aibaodan.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fcu.c1oappe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nwv.havefunace.top

[A26] 类型转换总览
来源：http://xzf.cashguo.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rss.cheryme.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gce.jqgfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dfu.ydzc1.top

TS:   Number() String() Boolean() x as number
来源：http://hec.gzhubu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jou.zdqjudy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://npu.ywan-chungtsiang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zpf.fzhhl.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ivy.bjfxy.top

================================================================================
来源：http://wnl.guannengcc.top

B. 流程控制
来源：http://flz.jlsjyb.cn

================================================================================
来源：http://uhf.zycfv.cn

[B01] 条件判断 if / else
来源：http://nnn.tarul.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vyi.xziqi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tyw.tianlin.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jqm.jqgufenzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vnx.zhixingplan.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ibj.tanke756.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://opw.ehwqpu.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bmx.birdmap.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dqj.gotoacloud.top

[B02] 多分支 else if / elif
来源：http://lak.jyoumei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oox.yj20258.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rkk.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mof.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mtp.aibaodan.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://srk.daria6918.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cbl.xylfe.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tvm.hywenlv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://swg.sxryk.cn

[B03] switch / match / case
来源：http://wsz.xuanzx.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iph.zhiwuduotai.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ssv.smart0.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qxz.yueranfly.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qgk.pycfn.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gyp.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eyo.xingfuxueyuan.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://deb.guowangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sxd.aizwys.cn

[B04] for 计数循环
来源：http://eyo.gogol.net.cn

Py:   for i in range(10): print(i)
来源：http://ttn.xziqi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ffi.svipenyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iro.aibaodan.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zzc.zhongyouzk.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kip.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dth.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://tfx.yuanzhike.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kmb.ehwqpu.com

[B05] 遍历数组 / 列表
来源：http://pkr.yanxiufei.cn

Py:   for item in arr: print(item)
来源：http://stt.jianghu66.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fyw.yj202588.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yxk.zhengqikj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yii.bbcook.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vfe.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gta.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://mqg.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wth.xylfe.cn

[B06] 遍历字典 / 对象
来源：http://pkv.zhengqikj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dew.jyoumei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ogl.fanxiaobao.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kyh.shangyingyoupin.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://teh.jqgfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ypx.fzhhl.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zhh.pengpengdd.cyou

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://evu.ppjwa.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://azz.jinyuanbaomall.cn

[B07] while 循环
来源：http://von.iojbl.cn

Py:   while i < 10: i += 1
来源：http://xux.jinqigufen.top

PHP:  while ($i < 10) { $i++; }
来源：http://vlf.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://gpe.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://nil.cheryme.top

Java: while (i < 10) { i++; }
来源：http://onp.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kpl.vqdsnc.cn

Ruby: while i < 10; i += 1; end
来源：http://cll.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://mbv.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://xzm.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://mlt.vqdsnc.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mlo.shanyushiyangtech.top

JS:   do { i++; } while (i < 10);
来源：http://baq.ydjk.org.cn

TS:   do { i++; } while (i < 10);
来源：http://vwi.snrcjt.cn

Java: do { i++; } while (i < 10);
来源：http://bho.meibo888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tuv.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://ofd.sweek.top

C#:   do { i++; } while (i < 10);
来源：http://brp.jinqigfzy.top

[B09] break 与 continue
来源：http://udl.gogol.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://odu.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hmj.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pft.uphjek.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gei.zdbjq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ose.svipenyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hil.fktsv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fbb.bbcook.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://llw.xinyue.icu

[B10] 遍历同时拿索引
来源：http://lqs.dianchejie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yqp.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jgk.yvedp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qsn.xingfuxueyuan.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://igk.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bou.bjfxy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ths.chenjidiqi.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vuj.cucudq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kns.hnqzz.top

[B11] 生成数字序列 / 区间
来源：http://who.yonumen.top

Py:   list(range(0, 10, 2))
来源：http://xng.havefunace.top

PHP:  range(0, 10, 2);
来源：http://kqh.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://men.tanke756.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sel.zhiwuduotai.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gwi.jinqigufen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pwy.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://voh.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qle.fehbvm.com

[B12] 跳出多层循环
来源：http://fni.fanxiaobao.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://jtw.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pqs.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zge.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bfn.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nay.aibaodan.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cvw.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iyi.guowangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://twk.0kj1m.cn

[B13] 判断是否为数字
来源：http://mfn.sweek.top

Py:   isinstance(x, (int, float))
来源：http://prq.gotoacloud.top

PHP:  is_numeric($x)
来源：http://jat.kuanghao11.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rmz.jyoumei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xau.hywenlv.cn

Java: x instanceof Number
来源：http://zux.zhengqikj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ucg.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://zwd.jinqigufen.top

C#:   x is int or double or decimal
来源：http://yky.sweek.top

[B14] 判断值是否在集合内
来源：http://xqz.smart0.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://byu.meibo888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://thv.cucudq.cn

JS:   [1, 2, 3].includes(x)
来源：http://pur.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://ouk.yangfankeji.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ltn.yvedp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qxg.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://foi.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fyc.vehdjk.com

[B15] 布尔运算与取反
来源：http://oum.hcnkem.com

Py:   a and b or not c
来源：http://ywq.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://hei.fehbvm.com

JS:   a && b || !c
来源：http://jez.guowangkeji.top

TS:   a && b || !c
来源：http://egc.zhijiandao.cn

Java: a && b || !c
来源：http://fpz.hongshengwenyu.top

Go:   a && b || !c
来源：http://qcj.ppjwa.cn

Ruby: a && b || !c
来源：http://bmk.gzhubu.top

C#:   a && b || !c
来源：http://pbn.jyoumei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qle.havefunace.top

Py:   if not data: return
来源：http://rqm.hesvh.cn

PHP:  if (!$data) { return; }
来源：http://juk.yongpay.top

JS:   if (!data) return;
来源：http://rwi.yvedp.cn

TS:   if (!data) return;
来源：http://spg.52xcode.cn

Java: if (data == null) return;
来源：http://gsp.daria6918.cn

Go:   if data == nil { return }
来源：http://hcm.xuanzx.com

Ruby: return if data.nil?
来源：http://wyw.jlsjyb.cn

C#:   if (data == null) return;
来源：http://nmo.ppjwa.cn

================================================================================
来源：http://yul.hesvh.cn

C. 函数与作用域
来源：http://zzi.hcnkem.com

================================================================================
来源：http://una.shangyingyoupin.top

[C01] 定义函数
来源：http://pof.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://sln.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ebu.chenjidiqi.icu

JS:   function add(a, b) { return a + b; }
来源：http://gay.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qrn.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://rkp.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://roe.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://fog.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hyf.xuetiantiany.cn

[C02] 默认参数
来源：http://ayu.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://crq.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://rlg.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://prw.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dhc.dashuyun.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yps.epnwcf.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hpy.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://twf.bbcook.cn

C#:   string Greet(string name = "World") => name;
来源：http://rki.fanxiaobao.xyz

[C03] 可变参数
来源：http://kbp.zhijiandao.cn

Py:   def total(*args): return sum(args)
来源：http://fpy.jianghu66.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gys.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gxi.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oqi.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ivp.kuanghao11.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qyn.cheryme.top

Ruby: def total(*nums); nums.sum; end
来源：http://zht.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kew.xylfe.cn

[C04] 命名参数 / 关键字参数
来源：http://mix.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tly.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hoe.gogol.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tkk.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vdq.hongshengwenyu.top

Java: // 无：用 Builder 模式或 record
来源：http://vbv.hesvh.cn

Go:   // 无：用配置结构体参数
来源：http://cfa.vqdsnc.cn

Ruby: f(a: 1, b: 2)
来源：http://qbc.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://wbt.shuidangran.top

[C05] 返回多个值
来源：http://dtd.snrcjt.cn

Py:   return a, b
来源：http://rrn.pycfn.com

PHP:  return [$a, $b];
来源：http://esm.hnxiangtu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wac.chenjidiqi.icu

TS:   return { a, b };
来源：http://hys.hfpthk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gna.tian-w.cn

Go:   return a, b
来源：http://xcx.smart0.xyz

Ruby: return a, b
来源：http://rzy.zdbjq.cn

C#:   return (a, b);              // ValueTuple
来源：http://kig.bbcook.cn

[C06] 匿名函数 / lambda
来源：http://rev.fzhhl.top

Py:   square = lambda x: x * x
来源：http://lgp.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://vjf.0kj1m.cn

JS:   const square = x => x * x;
来源：http://xnf.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://tef.0kj1m.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zmm.zdqjudy.top

Go:   sq := func(x int) int { return x * x }
来源：http://gvh.nanxuanxn.top

Ruby: square = ->(x) { x * x }
来源：http://gks.bbcook.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ywt.bjfxy.top

[C07] 把函数作为参数传入
来源：http://lsq.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ujs.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ovo.cashguo.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mbc.zhongyouzk.top

TS:   arr.map(String)
来源：http://vnk.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://let.ctjpmb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qhd.xingfuxueyuan.xyz

Ruby: arr.map(&:upcase)
来源：http://whc.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://pvs.jlsjyb.cn

[C08] 闭包
来源：http://xkp.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xqz.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lvz.meibo888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eki.gotoacloud.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ose.chenjidiqi.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hgc.zhaomingkeji.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lvd.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://acu.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://olt.xziqi.cn

[C09] 递归
来源：http://dux.guowangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://whp.zdbjq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vej.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eve.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hbp.svipenyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vmh.zycfv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fcz.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://plj.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ora.meibo888.top

[C10] 变量作用域
来源：http://hon.pycfn.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gsc.sysykeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://chc.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rkd.vehdjk.com

TS:   同 JS
来源：http://mdl.yj20258.top

Java: 方法内为块级作用域
来源：http://gsb.aibaodan.cn

Go:   花括号块级作用域
来源：http://mzp.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pet.ctjpmb.com


<!-- 参考信息 -->