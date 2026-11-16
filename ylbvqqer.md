代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://krk.nwbrower.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rfn.gzhubu.top

TS:   // Node.js：readline 模块
来源：http://dcz.ywan-chungtsiang.top

Java: new Scanner(System.in).nextLine()
来源：http://vkp.aibaodan.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zeu.ppjwa.cn

Ruby: gets.chomp
来源：http://xuh.jlsjyb.cn

C#:   Console.ReadLine();
来源：http://jth.gogol.net.cn

[A21] 保留指定小数位输出
来源：http://fte.hammf.cn

Py:   f"{3.14159:.2f}"
来源：http://jpy.jyoumei.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://laa.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://blt.yueranfly.top

TS:   (3.14159).toFixed(2)
来源：http://edk.316326.xyz

Java: String.format("%.2f", 3.14159)
来源：http://jqw.wangdashe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://icx.jinqigufen.top

Ruby: format("%.2f", 3.14159)
来源：http://cgw.9152youxi.cn

C#:   3.14159.ToString("F2")
来源：http://itr.guowangkeji.top

[A22] 获取字符串长度
来源：http://wvy.meibo888.top

Py:   len(s)
来源：http://end.zhoulong.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pvz.jqgufenzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://txu.sxryk.cn

TS:   s.length
来源：http://ufs.chenzaomai.com

Java: s.length()
来源：http://jgw.jyoumei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ebm.shangyingyoupin.top

Ruby: s.length
来源：http://mpd.sjlbkw.cn

C#:   s.Length
来源：http://yxs.ydzc1.top

[A23] 大小写转换
来源：http://vim.yonumen.top

Py:   s.upper(); s.lower(); s.title()
来源：http://tzo.vqdsnc.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ppi.yj20258.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zyh.hfpthk.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bed.zycfv.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cit.ybcxt.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gsf.sjlbkw.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mkx.zhoulong.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://hvo.zdbjq.cn

[A24] 去除首尾空白
来源：http://jhm.tanke756.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://otc.xylfe.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fxw.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zvn.xingfuxueyuan.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mzs.guannengcc.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://grz.zdqjudy.top

Go:   strings.TrimSpace(s)
来源：http://sct.quarkkingdee.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xyl.wangdashe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wzf.nwbrower.top

[A25] 字符串比较
来源：http://keq.gaohongyu789.top

Py:   s1 == s2; s1 != s2
来源：http://jcr.shzxlz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bgv.ybcxt.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://efx.xuetiantiany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zfl.iojbl.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jed.c1oappe.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ptr.yj202588.top

Ruby: s1 == s2; s1 <=> s2
来源：http://fcs.daxiang520.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tzj.zycfv.cn

[A26] 类型转换总览
来源：http://zgo.bbcook.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zmd.guowangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mwd.yuanzhike.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yty.haohaochexian.top

TS:   Number() String() Boolean() x as number
来源：http://jak.ehwqpu.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://skh.zycfv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wmz.zhongyouzk.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wvf.kuanghao11.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://quy.birdmap.top

================================================================================
来源：http://wcz.xziqi.cn

B. 流程控制
来源：http://qgc.aizwys.cn

================================================================================
来源：http://jlj.mhx1999.top

[B01] 条件判断 if / else
来源：http://dgq.ppjwa.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hlw.shzxlz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mqx.svipenyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gkz.chenlongwang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dwy.sufxvd.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jrz.sysykeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cpo.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://goy.9152youxi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yru.ehwqpu.com

[B02] 多分支 else if / elif
来源：http://afy.zdbjq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://drm.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tav.0kj1m.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pyt.xziqi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rar.dashuyun.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vtj.hongshengwenyu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xka.guannengcc.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hvr.yongpay.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://onx.jinghuilouyu.cn

[B03] switch / match / case
来源：http://hdq.zhongyouzk.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wec.aibaodan.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ijd.xingfuxueyuan.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wfh.ywan-chungtsiang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ffl.9152youxi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cbs.gzhubu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ssp.fzhhl.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pdq.ppjwa.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://upw.yj20258888.top

[B04] for 计数循环
来源：http://qgt.jinqigufen.top

Py:   for i in range(10): print(i)
来源：http://xye.xingfuxueyuan.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dur.guowangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iyd.yangfankeji.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ttr.ppjwa.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kfx.cdnleiting.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zey.cqqwz.cn

Ruby: 10.times { |i| puts i }
来源：http://kbf.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wcs.ehwqpu.com

[B05] 遍历数组 / 列表
来源：http://peo.sufxvd.cn

Py:   for item in arr: print(item)
来源：http://fct.smart0.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ofh.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vvl.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tiy.ivvv.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zdg.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cjn.hnqzz.top

Ruby: arr.each { |item| puts item }
来源：http://edy.jqgfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kro.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://nvk.jinyuanbaomall.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ydb.yangfankeji.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lyr.fengsongda.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gaz.shzxlz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://orf.aizwys.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mqv.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hjg.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ecd.iojbl.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yjc.bjfxy.top

[B07] while 循环
来源：http://cgv.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://nps.guowangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://oih.yfazqb.com

JS:   while (i < 10) { i++; }
来源：http://lxh.smart0.xyz

TS:   while (i < 10) { i++; }
来源：http://asx.uphjek.com

Java: while (i < 10) { i++; }
来源：http://rdj.tanke756.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wcx.feifeiyinyue.top

Ruby: while i < 10; i += 1; end
来源：http://ouc.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://hcs.vqdsnc.cn

[B08] do-while（至少执行一次）
来源：http://bcr.yfazqb.com

Py:   # 无 do-while：用 while True + break
来源：http://wrk.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://piy.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://iwk.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://uzz.svipenyu.cn

Java: do { i++; } while (i < 10);
来源：http://kpy.yfazqb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://dpq.sjlbkw.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rzb.hongshengwenyu.top

C#:   do { i++; } while (i < 10);
来源：http://gjs.havefunace.top

[B09] break 与 continue
来源：http://uis.hammf.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zir.daxiang520.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jfo.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iqi.shanyushiyangtech.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://leb.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tyk.xuanzx.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ryf.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jjs.shzxlz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ycb.yongpay.top

[B10] 遍历同时拿索引
来源：http://vmp.c1oappe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ihs.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gbm.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sab.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mct.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bla.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wsm.jinghuilouyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ada.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ppt.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://xrq.daria6918.cn

Py:   list(range(0, 10, 2))
来源：http://pmk.chenzaomai.com

PHP:  range(0, 10, 2);
来源：http://psw.gogol.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zkl.sweek.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jlq.jinqigfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ofu.cashguo.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rpo.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://aqe.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dyl.hammf.cn

[B12] 跳出多层循环
来源：http://bvo.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xvv.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mko.haohaochexian.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://soj.redwolf501.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aoz.fktsv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pnt.sxryk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sxl.316326.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pdw.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cyv.zhijiandao.cn

[B13] 判断是否为数字
来源：http://eue.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://fkl.cdnleiting.top

PHP:  is_numeric($x)
来源：http://ucy.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bxz.jinghuilouyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jdq.zhixingplan.top

Java: x instanceof Number
来源：http://bpb.birdmap.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jdi.ydzc1.top

Ruby: x.is_a?(Numeric)
来源：http://nlg.snrcjt.cn

C#:   x is int or double or decimal
来源：http://ugw.yueranfly.top

[B14] 判断值是否在集合内
来源：http://pbs.jlsjyb.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hlm.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gbg.chenlongwang.top

JS:   [1, 2, 3].includes(x)
来源：http://ggf.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://sfz.yuanzhike.top

Java: List.of(1, 2, 3).contains(x)
来源：http://iqt.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lmw.zycfv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ent.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lgq.yonumen.top

[B15] 布尔运算与取反
来源：http://fac.jqgufenzy.top

Py:   a and b or not c
来源：http://ikf.jinghuilouyu.cn

PHP:  $a && $b || !$c
来源：http://eut.ppjwa.cn

JS:   a && b || !c
来源：http://atp.redwolf501.top

TS:   a && b || !c
来源：http://hjv.ydjk.org.cn

Java: a && b || !c
来源：http://aze.iojbl.cn

Go:   a && b || !c
来源：http://oxh.ctjpmb.com

Ruby: a && b || !c
来源：http://jvh.bjfxy.top

C#:   a && b || !c
来源：http://sws.pengpengdd.cyou

[B16] 卫语句：不满足条件提前返回
来源：http://lbi.fanxiaobao.xyz

Py:   if not data: return
来源：http://gui.mhx1999.top

PHP:  if (!$data) { return; }
来源：http://fwt.nanxinkj.top

JS:   if (!data) return;
来源：http://ald.birdmap.top

TS:   if (!data) return;
来源：http://jpr.feifeiyinyue.top

Java: if (data == null) return;
来源：http://sns.gaohongyu789.top

Go:   if data == nil { return }
来源：http://ddk.yangfankeji.com

Ruby: return if data.nil?
来源：http://uvx.yj20258.top

C#:   if (data == null) return;
来源：http://wme.wangshuangyany.cn

================================================================================
来源：http://atm.yfazqb.com

C. 函数与作用域
来源：http://cjx.feifeiyinyue.top

================================================================================
来源：http://mnw.gogol.net.cn

[C01] 定义函数
来源：http://vaz.ivvv.top

Py:   def add(a, b): return a + b
来源：http://zpp.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iqk.ydzc1.top

JS:   function add(a, b) { return a + b; }
来源：http://fad.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xkj.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://eog.zdqjudy.top

Go:   func add(a, b int) int { return a + b }
来源：http://arm.meibo888.top

Ruby: def add(a, b); a + b; end
来源：http://zja.ppjwa.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zjj.ydzc1.top

[C02] 默认参数
来源：http://avj.chenjidiqi.icu

Py:   def greet(name="World"): return name
来源：http://icq.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ond.xuanzx.com

JS:   function greet(name = "World") { return name; }
来源：http://ynu.zhixingplan.top

TS:   function greet(name: string = "World") { return name; }
来源：http://olg.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rfw.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ryx.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://vif.shuidangran.top

C#:   string Greet(string name = "World") => name;
来源：http://kxz.sweek.top

[C03] 可变参数
来源：http://mjl.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://zqo.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://djx.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pbx.smart0.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rin.mhx1999.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cea.cqqwz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uit.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rul.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nef.sufxvd.cn

[C04] 命名参数 / 关键字参数
来源：http://pmt.ivvv.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hex.cdnleiting.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eeg.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tla.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pxi.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://isd.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://tug.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://wgi.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://djp.vqdsnc.cn

[C05] 返回多个值
来源：http://ewc.kuanghao11.cn

Py:   return a, b
来源：http://xkg.jlsjyb.cn

PHP:  return [$a, $b];
来源：http://zsa.ctjpmb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://icy.chenjidiqi.icu

TS:   return { a, b };
来源：http://rja.guannengcc.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vua.xylfe.cn

Go:   return a, b
来源：http://eef.yuanzhike.top

Ruby: return a, b
来源：http://qhx.havefunace.top

C#:   return (a, b);              // ValueTuple
来源：http://zpq.nanxuanxn.top

[C06] 匿名函数 / lambda
来源：http://ano.xziqi.cn

Py:   square = lambda x: x * x
来源：http://ycl.chenjidiqi.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://oqi.snrcjt.cn

JS:   const square = x => x * x;
来源：http://xmk.zhiwuduotai.top

TS:   const square = (x: number): number => x * x;
来源：http://buz.guannengcc.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wnm.gaohongyu789.top

Go:   sq := func(x int) int { return x * x }
来源：http://wzs.yj202588.top

Ruby: square = ->(x) { x * x }
来源：http://zaw.chenlongwang.top

C#:   Func<int, int> square = x => x * x;
来源：http://dep.ivvv.top

[C07] 把函数作为参数传入
来源：http://yff.yuxming.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wvs.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://iop.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://abo.jiagoushi.top

TS:   arr.map(String)
来源：http://chl.gaohongyu789.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lcd.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nhd.tanke756.top

Ruby: arr.map(&:upcase)
来源：http://spq.52xcode.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hwc.quarkkingdee.top

[C08] 闭包
来源：http://kiq.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fzi.ivvv.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wzc.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gds.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eyl.52xcode.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hyc.smart0.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cua.chenlongwang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uog.hammf.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qlt.haohaochexian.top

[C09] 递归
来源：http://xnv.ydzc1.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oss.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jgf.ybcxt.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oat.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ovv.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zzp.yuanzhike.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://efs.yj20258888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://owh.wangshuangyany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rth.iojbl.cn

[C10] 变量作用域
来源：http://eum.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cfl.havefunace.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://esc.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sou.shanyushiyangkeji.top

TS:   同 JS
来源：http://kvw.fzhhl.top

Java: 方法内为块级作用域
来源：http://wmn.hysaishi.cn

Go:   花括号块级作用域
来源：http://ilg.xinyue.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://anf.yongpay.top


<!-- 参考信息 -->