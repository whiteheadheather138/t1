代发 wailian999

Ruby: a, b = b, a
来源：http://uld.snrcjt.cn

C#:   (a, b) = (b, a);
来源：http://eyu.kuanghao11.cn

[A20] 读取标准输入
来源：http://kti.ywan-chungtsiang.top

Py:   name = input("请输入：")
来源：http://nyc.smart0.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://ihs.sufxvd.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oqc.xinyue.icu

TS:   // Node.js：readline 模块
来源：http://qdw.yj202588.top

Java: new Scanner(System.in).nextLine()
来源：http://zka.redwolf501.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ltm.cqqwz.cn

Ruby: gets.chomp
来源：http://ylm.jqgfzy.top

C#:   Console.ReadLine();
来源：http://rpe.yj20258888.top

[A21] 保留指定小数位输出
来源：http://tia.wangshuangyany.cn

Py:   f"{3.14159:.2f}"
来源：http://mxy.zhijiandao.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://urn.tanke756.top

JS:   (3.14159).toFixed(2)
来源：http://lqz.tian-w.cn

TS:   (3.14159).toFixed(2)
来源：http://qzg.ybcxt.top

Java: String.format("%.2f", 3.14159)
来源：http://bco.cheryme.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dqe.hnqzz.top

Ruby: format("%.2f", 3.14159)
来源：http://ccm.shuidangran.top

C#:   3.14159.ToString("F2")
来源：http://rcs.dashuyun.cn

[A22] 获取字符串长度
来源：http://ufa.yvedp.cn

Py:   len(s)
来源：http://kxh.yanxiufei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://luk.guowangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cya.guannengcc.top

TS:   s.length
来源：http://zaa.vqdsnc.cn

Java: s.length()
来源：http://tvx.aibaodan.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hsj.smart0.xyz

Ruby: s.length
来源：http://jdz.cdnleiting.top

C#:   s.Length
来源：http://esm.vehdjk.com

[A23] 大小写转换
来源：http://ryc.bjfxy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://his.guowangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aes.ppjwa.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gxa.shuidangran.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dol.redwolf501.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://duq.bbcook.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://glk.zhiwuduotai.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kyl.fzhhl.top

C#:   s.ToUpper(); s.ToLower()
来源：http://uvu.kuanghao11.cn

[A24] 去除首尾空白
来源：http://gci.yj20258.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yoz.xziqi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ovv.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://han.shanyushiyangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://udc.yj20258888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pwu.hesvh.cn

Go:   strings.TrimSpace(s)
来源：http://xeg.chenjidiqi.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cwm.yj202588.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://otb.cucudq.cn

[A25] 字符串比较
来源：http://ogk.316326.xyz

Py:   s1 == s2; s1 != s2
来源：http://gjw.chenzaomai.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://udl.sysykeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eab.xylfe.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wse.shanyushiyangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uxw.dianchejie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://juh.sxryk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://snr.316326.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qps.ppjwa.cn

[A26] 类型转换总览
来源：http://cws.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rvv.fktsv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bmx.jinqigufen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pbe.ppjwa.cn

TS:   Number() String() Boolean() x as number
来源：http://sru.hfpthk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://quz.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vex.meibo888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ljo.0kj1m.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rpa.xuetiantiany.cn

================================================================================
来源：http://nzv.yj20258.top

B. 流程控制
来源：http://fpv.snrcjt.cn

================================================================================
来源：http://lrr.iojbl.cn

[B01] 条件判断 if / else
来源：http://ayt.cqqwz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://udx.kuanghao11.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oiz.smart0.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://slw.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wsj.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://aah.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ftg.shanyushiyangtech.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qiq.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tnx.hfpthk.cn

[B02] 多分支 else if / elif
来源：http://kpg.pengpengdd.cyou

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mwy.shanyushiyangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ypx.hnxiangtu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nds.tian-w.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zec.zhaomingkeji.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ums.xingfuxueyuan.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hob.zhijiandao.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vnu.vehdjk.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://alt.snrcjt.cn

[B03] switch / match / case
来源：http://dff.shanyushiyangtech.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://smd.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vuw.jiagoushi.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rgd.fanxiaobao.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gel.tian-w.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lrz.jianghu66.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yfw.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xbn.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iwc.dianchejie.cn

[B04] for 计数循环
来源：http://mrr.ydzc1.top

Py:   for i in range(10): print(i)
来源：http://npl.yj20258.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://elc.hywenlv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bin.ctjpmb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://btq.havefunace.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qjy.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uzp.yuanzhike.top

Ruby: 10.times { |i| puts i }
来源：http://atp.zhaomingkeji.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fnm.yonumen.top

[B05] 遍历数组 / 列表
来源：http://hoj.gogol.net.cn

Py:   for item in arr: print(item)
来源：http://enl.vqdsnc.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fac.smart0.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://ais.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pav.nanxinkj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jvf.cheryme.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ujk.chenzaomai.com

Ruby: arr.each { |item| puts item }
来源：http://wep.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://olg.fehbvm.com

[B06] 遍历字典 / 对象
来源：http://qyw.jinyuanbaomall.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fgx.nanxinkj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wrg.ivvv.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yol.havefunace.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zrx.hywenlv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://olu.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hvo.yuanzhike.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rrp.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wsj.hywenlv.cn

[B07] while 循环
来源：http://wki.ydzc1.top

Py:   while i < 10: i += 1
来源：http://lat.yangfankeji.com

PHP:  while ($i < 10) { $i++; }
来源：http://akz.iojbl.cn

JS:   while (i < 10) { i++; }
来源：http://abc.jinqigfzy.top

TS:   while (i < 10) { i++; }
来源：http://zwx.jlsjyb.cn

Java: while (i < 10) { i++; }
来源：http://ddn.zhaomingkeji.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rvx.cdnleiting.top

Ruby: while i < 10; i += 1; end
来源：http://ymd.hfpthk.cn

C#:   while (i < 10) { i++; }
来源：http://ssk.shzxlz.cn

[B08] do-while（至少执行一次）
来源：http://ovc.yonumen.top

Py:   # 无 do-while：用 while True + break
来源：http://rfa.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xrl.gotoacloud.top

JS:   do { i++; } while (i < 10);
来源：http://hia.chenjidiqi.icu

TS:   do { i++; } while (i < 10);
来源：http://ouc.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://msw.snrcjt.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hbx.jianghu66.top

Ruby: begin; i += 1; end while i < 10
来源：http://twz.shangyingyoupin.top

C#:   do { i++; } while (i < 10);
来源：http://hln.meibo888.top

[B09] break 与 continue
来源：http://zqd.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xpf.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://exu.hysaishi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mcz.hesvh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ogn.jianghu66.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xnl.yuxming.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://usz.yangfankeji.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wlo.yfazqb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://itk.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://hst.vqdsnc.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://waa.sjlbkw.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gdx.9152youxi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://iiw.aibaodan.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ego.smart0.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hyw.ehwqpu.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ksw.vqdsnc.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dul.gotoacloud.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://apt.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://sat.yj20258888.top

Py:   list(range(0, 10, 2))
来源：http://zve.feifeiyinyue.top

PHP:  range(0, 10, 2);
来源：http://eol.nanxinkj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://koq.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pqp.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mdx.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xqm.hcnkem.com

Ruby: (0...10).step(2).to_a
来源：http://pto.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sbk.chenlongwang.top

[B12] 跳出多层循环
来源：http://gnf.sjlbkw.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kgi.andypj.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://eso.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yeh.guowangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xoe.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://itn.haohaochexian.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ivk.xingfuxueyuan.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tbz.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sxh.vqdsnc.cn

[B13] 判断是否为数字
来源：http://sjm.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://itg.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://jzt.ydjk.org.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gvc.zhongyouzk.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://onu.tian-w.cn

Java: x instanceof Number
来源：http://pdj.svipenyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rcu.sjlbkw.cn

Ruby: x.is_a?(Numeric)
来源：http://ueo.hysaishi.cn

C#:   x is int or double or decimal
来源：http://zqo.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://zmr.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xuv.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pnh.tarul.cn

JS:   [1, 2, 3].includes(x)
来源：http://cwp.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://fok.jlsjyb.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ndk.tanke756.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jjv.ivvv.top

Ruby: [1, 2, 3].include?(x)
来源：http://xep.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dxl.zhongyouzk.top

[B15] 布尔运算与取反
来源：http://cyj.kuanghao11.cn

Py:   a and b or not c
来源：http://ytk.yj20258888.top

PHP:  $a && $b || !$c
来源：http://alu.shzxlz.cn

JS:   a && b || !c
来源：http://gxu.yanxiufei.cn

TS:   a && b || !c
来源：http://ovp.andypj.xyz

Java: a && b || !c
来源：http://lhg.pycfn.com

Go:   a && b || !c
来源：http://ljk.sxryk.cn

Ruby: a && b || !c
来源：http://vrd.jqgfzy.top

C#:   a && b || !c
来源：http://skc.ppjwa.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zjl.shzxlz.cn

Py:   if not data: return
来源：http://wdc.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://bgd.yfazqb.com

JS:   if (!data) return;
来源：http://naf.pycfn.com

TS:   if (!data) return;
来源：http://wri.aibaodan.cn

Java: if (data == null) return;
来源：http://wof.gogol.net.cn

Go:   if data == nil { return }
来源：http://phr.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://tny.wangshuangyany.cn

C#:   if (data == null) return;
来源：http://seb.bbcook.cn

================================================================================
来源：http://mun.yfazqb.com

C. 函数与作用域
来源：http://iaq.birdmap.top

================================================================================
来源：http://zgb.gaohongyu789.top

[C01] 定义函数
来源：http://umc.zhongyouzk.top

Py:   def add(a, b): return a + b
来源：http://cpx.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xcl.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://gmg.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yyl.sweek.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vfy.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rdy.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://uaw.cucudq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eza.jlsjyb.cn

[C02] 默认参数
来源：http://ycl.jqgufenzy.top

Py:   def greet(name="World"): return name
来源：http://rrx.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dkg.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://cin.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://eiv.zycfv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gbn.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gqi.wangdashe.top

Ruby: def greet(name = "World") = name
来源：http://ndx.kuanghao11.cn

C#:   string Greet(string name = "World") => name;
来源：http://yfj.316326.xyz

[C03] 可变参数
来源：http://uuo.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://ura.fzhhl.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nxb.jinqigfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nuh.c1oappe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kjf.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://clq.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bve.fzhhl.top

Ruby: def total(*nums); nums.sum; end
来源：http://wok.chenzaomai.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oxv.hcnkem.com

[C04] 命名参数 / 关键字参数
来源：http://quv.kuanghao11.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dck.jiagoushi.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pkp.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oyn.jlsjyb.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hsz.guowangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://wwi.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://pla.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://tyn.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://czl.dianchejie.cn

[C05] 返回多个值
来源：http://pmg.jqgfzy.top

Py:   return a, b
来源：http://ffx.zhixingplan.top

PHP:  return [$a, $b];
来源：http://ilj.cheryme.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xzg.zhengqikj.top

TS:   return { a, b };
来源：http://owz.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pso.jinqigfzy.top

Go:   return a, b
来源：http://ahs.zdqjudy.top

Ruby: return a, b
来源：http://mzi.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://ayw.jiagoushi.top

[C06] 匿名函数 / lambda
来源：http://npp.fengsongda.top

Py:   square = lambda x: x * x
来源：http://cxw.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uyk.jianghu66.top

JS:   const square = x => x * x;
来源：http://pxw.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://xkz.sjlbkw.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ltd.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://tiu.gzhubu.top

Ruby: square = ->(x) { x * x }
来源：http://nbo.fktsv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://atg.xziqi.cn

[C07] 把函数作为参数传入
来源：http://iwm.ppjwa.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://atg.vehdjk.com

PHP:  array_map("strtoupper", $arr);
来源：http://nll.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lrj.uphjek.com

TS:   arr.map(String)
来源：http://vzj.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ahp.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eza.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://ptn.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://pas.kuanghao11.cn

[C08] 闭包
来源：http://aml.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tau.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ppz.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://arq.fengsongda.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cgd.yfazqb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hen.9152youxi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aqc.gogol.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zdk.gaohongyu789.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zdi.cheryme.top

[C09] 递归
来源：http://nva.ywan-chungtsiang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jvc.nanxinkj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uet.zycfv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sgj.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ige.jinqigfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://afn.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://efg.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vuu.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gxb.sjlbkw.cn

[C10] 变量作用域
来源：http://ebe.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jdc.pycfn.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dvn.cqqwz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://emg.jlsjyb.cn


<!-- 参考信息 -->