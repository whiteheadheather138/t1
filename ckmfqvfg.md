代发 wailian999

C#:   (int)'A'; (char)65
来源：http://lmh.cqqwz.cn

[A19] 交换两个变量
来源：http://tvt.316326.xyz

Py:   a, b = b, a
来源：http://mru.316326.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://kxa.daria6918.cn

JS:   [a, b] = [b, a];
来源：http://aqc.hcnkem.com

TS:   [a, b] = [b, a];
来源：http://umh.yonumen.top

Java: int t = a; a = b; b = t;
来源：http://qtq.smart0.xyz

Go:   a, b = b, a
来源：http://une.gzhubu.top

Ruby: a, b = b, a
来源：http://lqp.hysaishi.cn

C#:   (a, b) = (b, a);
来源：http://bcx.jqgufenzy.top

[A20] 读取标准输入
来源：http://wse.shangyingyoupin.top

Py:   name = input("请输入：")
来源：http://dth.pycfn.com

PHP:  $name = trim(fgets(STDIN));
来源：http://tmh.ehwqpu.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qjp.gzhubu.top

TS:   // Node.js：readline 模块
来源：http://nuu.ywan-chungtsiang.top

Java: new Scanner(System.in).nextLine()
来源：http://maw.ppjwa.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pfr.xziqi.cn

Ruby: gets.chomp
来源：http://jkr.52xcode.cn

C#:   Console.ReadLine();
来源：http://fgl.yj20258.top

[A21] 保留指定小数位输出
来源：http://lsz.havefunace.top

Py:   f"{3.14159:.2f}"
来源：http://gdv.xingfuxueyuan.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ylz.jinyuanbaomall.cn

JS:   (3.14159).toFixed(2)
来源：http://bdn.redwolf501.top

TS:   (3.14159).toFixed(2)
来源：http://uxm.mhx1999.top

Java: String.format("%.2f", 3.14159)
来源：http://axo.zhongyouzk.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fdn.ywan-chungtsiang.top

Ruby: format("%.2f", 3.14159)
来源：http://rrm.jinghuilouyu.cn

C#:   3.14159.ToString("F2")
来源：http://thg.zhaomingkeji.xyz

[A22] 获取字符串长度
来源：http://apw.yuanzhike.top

Py:   len(s)
来源：http://ums.sysykeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cvx.chenjidiqi.icu

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aya.dianchejie.cn

TS:   s.length
来源：http://ktr.chenlongwang.top

Java: s.length()
来源：http://itr.quarkkingdee.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://otr.hammf.cn

Ruby: s.length
来源：http://xhz.wangshuangyany.cn

C#:   s.Length
来源：http://bvr.xingfuxueyuan.xyz

[A23] 大小写转换
来源：http://rsc.shuidangran.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ddh.chenjidiqi.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://irc.yanxiufei.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rbv.guowangkeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://diy.xziqi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qzi.gaohongyu789.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uru.birdmap.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dfr.sufxvd.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://aog.ctjpmb.com

[A24] 去除首尾空白
来源：http://kcr.dashuyun.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mov.ydjk.org.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cvo.nanxuanxn.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zyh.sysykeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ssg.yangfankeji.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kcj.hongshengwenyu.top

Go:   strings.TrimSpace(s)
来源：http://xsb.tian-w.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bvs.yangfankeji.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wuo.quarkkingdee.top

[A25] 字符串比较
来源：http://fdi.jinqigfzy.top

Py:   s1 == s2; s1 != s2
来源：http://lss.sufxvd.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dsn.epnwcf.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mho.guowangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kyh.hcnkem.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://htj.sweek.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yop.feifeiyinyue.top

Ruby: s1 == s2; s1 <=> s2
来源：http://msr.vqdsnc.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ylg.yj202588.top

[A26] 类型转换总览
来源：http://rxb.nwbrower.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ahe.fzhhl.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hpg.jqgfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fmy.jqgfzy.top

TS:   Number() String() Boolean() x as number
来源：http://ttc.bbcook.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ddj.52xcode.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oxg.yangfankeji.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://akk.yj20258.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kso.shuidangran.top

================================================================================
来源：http://kcm.cashguo.top

B. 流程控制
来源：http://jyw.yanxiufei.cn

================================================================================
来源：http://xsf.zhengqikj.top

[B01] 条件判断 if / else
来源：http://ofp.gotoacloud.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wfx.shangyingyoupin.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bru.xingfuxueyuan.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kax.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iqc.mhx1999.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://wtc.jiagoushi.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cqi.ybcxt.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lpb.xuanzx.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ujw.nanxinkj.top

[B02] 多分支 else if / elif
来源：http://dss.ehwqpu.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lnw.chenzaomai.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://suf.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oin.ehwqpu.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://okg.gotoacloud.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aos.guannengcc.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kif.pycfn.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://scz.snrcjt.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mib.nanxinkj.top

[B03] switch / match / case
来源：http://azq.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lnt.zhixingplan.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wim.meibo888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ols.yuxming.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lqy.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hhf.bbcook.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bka.ivvv.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nlj.yfazqb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sbh.gaohongyu789.top

[B04] for 计数循环
来源：http://gem.yj202588.top

Py:   for i in range(10): print(i)
来源：http://uaf.jinyuanbaomall.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://prz.zdqjudy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wgh.daxiang520.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xcy.shanyushiyangtech.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gbw.quarkkingdee.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ytb.jiagoushi.top

Ruby: 10.times { |i| puts i }
来源：http://izc.vehdjk.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yfq.jiagoushi.top

[B05] 遍历数组 / 列表
来源：http://zfc.ybcxt.top

Py:   for item in arr: print(item)
来源：http://lcp.zhaomingkeji.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dpl.kuanghao11.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ryh.zhengqikj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://csg.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qdf.daxiang520.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ept.pycfn.com

Ruby: arr.each { |item| puts item }
来源：http://bmy.yonumen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kwt.jianghu66.top

[B06] 遍历字典 / 对象
来源：http://kdv.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://syv.zhixingplan.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://san.svipenyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yyg.aibaodan.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cbh.0kj1m.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wtz.yfazqb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://abu.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://evt.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xxs.xuetiantiany.cn

[B07] while 循环
来源：http://vsp.zdqjudy.top

Py:   while i < 10: i += 1
来源：http://ggh.aizwys.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rcl.yuxming.cn

JS:   while (i < 10) { i++; }
来源：http://clv.dashuyun.cn

TS:   while (i < 10) { i++; }
来源：http://ufz.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://dhk.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tps.jinqigfzy.top

Ruby: while i < 10; i += 1; end
来源：http://esz.shangyingyoupin.top

C#:   while (i < 10) { i++; }
来源：http://hca.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://ceu.shzxlz.cn

Py:   # 无 do-while：用 while True + break
来源：http://tfs.daria6918.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ugp.gzhubu.top

JS:   do { i++; } while (i < 10);
来源：http://uxn.chenjidiqi.icu

TS:   do { i++; } while (i < 10);
来源：http://oym.hesvh.cn

Java: do { i++; } while (i < 10);
来源：http://sjk.ydjk.org.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://elf.zhaomingkeji.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://nxu.gzhubu.top

C#:   do { i++; } while (i < 10);
来源：http://jdh.jinghuilouyu.cn

[B09] break 与 continue
来源：http://xld.vehdjk.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dgq.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zsf.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lff.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://alb.fengsongda.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uco.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vqg.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://veg.fehbvm.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yzx.shanyushiyangtech.top

[B10] 遍历同时拿索引
来源：http://mdb.ehwqpu.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uwk.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hfx.tianlin.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jwh.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://emi.epnwcf.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aav.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sdk.shanyushiyangtech.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uqx.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ptm.jinghuilouyu.cn

[B11] 生成数字序列 / 区间
来源：http://pdw.jqgufenzy.top

Py:   list(range(0, 10, 2))
来源：http://xyq.yj20258.top

PHP:  range(0, 10, 2);
来源：http://ftw.tarul.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zua.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yls.aizwys.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://efp.shzxlz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hbq.52xcode.cn

Ruby: (0...10).step(2).to_a
来源：http://uid.xinyue.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pwl.jinqigufen.top

[B12] 跳出多层循环
来源：http://kti.uphjek.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://ado.uphjek.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://yky.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zuj.bbcook.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gdi.smart0.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yim.shanyushiyangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qty.meibo888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ytk.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jcz.cdnleiting.top

[B13] 判断是否为数字
来源：http://ajj.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://afg.shanyushiyangkeji.top

PHP:  is_numeric($x)
来源：http://hcs.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qcu.epnwcf.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://liv.9152youxi.cn

Java: x instanceof Number
来源：http://iwk.tanke756.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cbw.nwbrower.top

Ruby: x.is_a?(Numeric)
来源：http://ngc.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://qsf.chenjidiqi.icu

[B14] 判断值是否在集合内
来源：http://hqp.jinyuanbaomall.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jqo.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pbe.hnqzz.top

JS:   [1, 2, 3].includes(x)
来源：http://eoc.tarul.cn

TS:   [1, 2, 3].includes(x)
来源：http://cjq.jianghu66.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dpa.hammf.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ekl.fanxiaobao.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://dnv.zhaomingkeji.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lrl.meibo888.top

[B15] 布尔运算与取反
来源：http://mrx.xuanzx.com

Py:   a and b or not c
来源：http://itz.yongpay.top

PHP:  $a && $b || !$c
来源：http://pdr.nwbrower.top

JS:   a && b || !c
来源：http://lyc.sjlbkw.cn

TS:   a && b || !c
来源：http://yig.yj20258.top

Java: a && b || !c
来源：http://wof.hongshengwenyu.top

Go:   a && b || !c
来源：http://vjr.dashuyun.cn

Ruby: a && b || !c
来源：http://tqs.ydzc1.top

C#:   a && b || !c
来源：http://fgu.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://frd.jqgfzy.top

Py:   if not data: return
来源：http://knc.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://vnq.jyoumei.cn

JS:   if (!data) return;
来源：http://hom.yuxming.cn

TS:   if (!data) return;
来源：http://xie.hammf.cn

Java: if (data == null) return;
来源：http://xem.ydzc1.top

Go:   if data == nil { return }
来源：http://dkl.mhx1999.top

Ruby: return if data.nil?
来源：http://aea.jqgufenzy.top

C#:   if (data == null) return;
来源：http://bnr.kuanghao11.cn

================================================================================
来源：http://gpz.yfazqb.com

C. 函数与作用域
来源：http://zyb.smart0.xyz

================================================================================
来源：http://psc.aizwys.cn

[C01] 定义函数
来源：http://qvd.aibaodan.cn

Py:   def add(a, b): return a + b
来源：http://ckc.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ivm.yfazqb.com

JS:   function add(a, b) { return a + b; }
来源：http://ouf.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ykz.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qve.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://vwh.vqdsnc.cn

Ruby: def add(a, b); a + b; end
来源：http://les.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://arw.shanyushiyangtech.top

[C02] 默认参数
来源：http://tqb.yangfankeji.com

Py:   def greet(name="World"): return name
来源：http://pye.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xyo.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://qea.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zkm.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tri.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kes.yanxiufei.cn

Ruby: def greet(name = "World") = name
来源：http://tjm.sjlbkw.cn

C#:   string Greet(string name = "World") => name;
来源：http://pnf.hesvh.cn

[C03] 可变参数
来源：http://yip.shanyushiyangtech.top

Py:   def total(*args): return sum(args)
来源：http://non.gaohongyu789.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ymz.birdmap.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ysq.smart0.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fll.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://npn.sysykeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lth.tianlin.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://qlj.pycfn.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tkk.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://xxs.ydzc1.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tsk.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://keo.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qhe.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://crk.shanyushiyangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://vll.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://knl.zdbjq.cn

Ruby: f(a: 1, b: 2)
来源：http://jvi.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://jqe.cdnleiting.top

[C05] 返回多个值
来源：http://wtu.sjlbkw.cn

Py:   return a, b
来源：http://qlj.gotoacloud.top

PHP:  return [$a, $b];
来源：http://wxh.daxiang520.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dco.jiagoushi.top

TS:   return { a, b };
来源：http://ych.nwbrower.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cfo.jiagoushi.top

Go:   return a, b
来源：http://nqf.fanxiaobao.xyz

Ruby: return a, b
来源：http://nek.chenjidiqi.icu

C#:   return (a, b);              // ValueTuple
来源：http://boi.tarul.cn

[C06] 匿名函数 / lambda
来源：http://grr.cqqwz.cn

Py:   square = lambda x: x * x
来源：http://gcc.yongpay.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tck.yanxiufei.cn

JS:   const square = x => x * x;
来源：http://plh.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://fsr.iojbl.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rpy.jianghu66.top

Go:   sq := func(x int) int { return x * x }
来源：http://myz.wangdashe.top

Ruby: square = ->(x) { x * x }
来源：http://fvn.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sqs.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://lnx.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://guu.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://lit.pycfn.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cew.jinqigufen.top

TS:   arr.map(String)
来源：http://wkn.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oqf.fehbvm.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ckb.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://wen.xziqi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jqo.shanyushiyangkeji.top

[C08] 闭包
来源：http://dpx.feifeiyinyue.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rjf.hnxiangtu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cvk.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vmh.svipenyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qrf.fanxiaobao.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vvd.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vva.9152youxi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xmq.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dxy.cashguo.top

[C09] 递归
来源：http://etn.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kqv.ydzc1.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hqq.andypj.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qux.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iph.havefunace.top


<!-- 参考信息 -->