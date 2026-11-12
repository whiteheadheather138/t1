代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://ayt.hnxiangtu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ztb.zhiwuduotai.top

TS:   // Node.js：readline 模块
来源：http://lcs.daria6918.cn

Java: new Scanner(System.in).nextLine()
来源：http://wdi.epnwcf.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nev.zhixingplan.top

Ruby: gets.chomp
来源：http://lol.fanxiaobao.xyz

C#:   Console.ReadLine();
来源：http://lnr.sufxvd.cn

[A21] 保留指定小数位输出
来源：http://byz.jinqigufen.top

Py:   f"{3.14159:.2f}"
来源：http://afg.shanyushiyangtech.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dcd.ppjwa.cn

JS:   (3.14159).toFixed(2)
来源：http://onv.hnxiangtu.top

TS:   (3.14159).toFixed(2)
来源：http://mfx.zhijiandao.cn

Java: String.format("%.2f", 3.14159)
来源：http://frs.316326.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xlx.yj20258888.top

Ruby: format("%.2f", 3.14159)
来源：http://zmo.cashguo.top

C#:   3.14159.ToString("F2")
来源：http://ddj.zhixingplan.top

[A22] 获取字符串长度
来源：http://fda.yj202588.top

Py:   len(s)
来源：http://nkz.cheryme.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yrs.ivvv.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ciy.snrcjt.cn

TS:   s.length
来源：http://tvu.meibo888.top

Java: s.length()
来源：http://dhb.hnqzz.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ntr.xingfuxueyuan.xyz

Ruby: s.length
来源：http://vkw.jqgfzy.top

C#:   s.Length
来源：http://mcr.yanxiufei.cn

[A23] 大小写转换
来源：http://tzg.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lnk.jianghu66.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xks.yueranfly.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wjt.ehwqpu.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nxu.hcnkem.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fbh.wangshuangyany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qwo.yangfankeji.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://awv.dianchejie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://unx.tarul.cn

[A24] 去除首尾空白
来源：http://ynq.yangfankeji.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zpm.hammf.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uqb.yongpay.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uui.zycfv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hzf.gotoacloud.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wqn.xingfuxueyuan.xyz

Go:   strings.TrimSpace(s)
来源：http://div.c1oappe.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yft.quarkkingdee.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ozl.ivvv.top

[A25] 字符串比较
来源：http://rcu.yj20258.top

Py:   s1 == s2; s1 != s2
来源：http://zkn.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ruj.ydjk.org.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lfo.yueranfly.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://khy.cdnleiting.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lqc.yueranfly.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aca.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qqp.xziqi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yuc.jinyuanbaomall.cn

[A26] 类型转换总览
来源：http://ohj.dashuyun.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tkg.hongshengwenyu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xnt.fengsongda.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wlx.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://yyu.zhaomingkeji.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ckh.hywenlv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dqx.tianlin.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://cmy.chenjidiqi.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rin.aizwys.cn

================================================================================
来源：http://qut.zhixingplan.top

B. 流程控制
来源：http://itx.zhixingplan.top

================================================================================
来源：http://pwv.daxiang520.top

[B01] 条件判断 if / else
来源：http://phh.svipenyu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dtf.fktsv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ats.ywan-chungtsiang.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qpc.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://efa.zhoulong.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://kkx.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zfa.zhiwuduotai.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ixz.shanyushiyangtech.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zfi.sufxvd.cn

[B02] 多分支 else if / elif
来源：http://vgm.fzhhl.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lxh.jyoumei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vip.bbcook.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fwm.zhiwuduotai.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hjv.shanyushiyangtech.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pcm.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pks.cashguo.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gus.316326.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ioz.svipenyu.cn

[B03] switch / match / case
来源：http://prt.ehwqpu.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mmj.tianlin.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://abo.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oij.bjfxy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ojl.yvedp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fuf.ehwqpu.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pcr.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xid.svipenyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://frh.bjfxy.top

[B04] for 计数循环
来源：http://ewz.jinyuanbaomall.cn

Py:   for i in range(10): print(i)
来源：http://prm.chenlongwang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dtg.aibaodan.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nmu.jlsjyb.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dii.zhaomingkeji.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://anl.kuanghao11.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zbe.fehbvm.com

Ruby: 10.times { |i| puts i }
来源：http://bje.ppjwa.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vjs.cdnleiting.top

[B05] 遍历数组 / 列表
来源：http://xgi.pengpengdd.cyou

Py:   for item in arr: print(item)
来源：http://eie.dianchejie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://koq.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ike.jlsjyb.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nbg.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kve.ehwqpu.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vic.yj202588.top

Ruby: arr.each { |item| puts item }
来源：http://var.mhx1999.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sua.jianghu66.top

[B06] 遍历字典 / 对象
来源：http://iqb.tanke756.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hyd.fzhhl.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bqc.yfazqb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ist.yueranfly.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fcc.sweek.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bds.daxiang520.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vix.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://png.gaohongyu789.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ntu.zdbjq.cn

[B07] while 循环
来源：http://ufx.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://jsg.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://arq.sysykeji.top

JS:   while (i < 10) { i++; }
来源：http://oby.xuetiantiany.cn

TS:   while (i < 10) { i++; }
来源：http://zti.ivvv.top

Java: while (i < 10) { i++; }
来源：http://hvx.epnwcf.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mme.sjlbkw.cn

Ruby: while i < 10; i += 1; end
来源：http://htk.hongshengwenyu.top

C#:   while (i < 10) { i++; }
来源：http://the.ywan-chungtsiang.top

[B08] do-while（至少执行一次）
来源：http://hqc.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://elv.jinyuanbaomall.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tmj.zdqjudy.top

JS:   do { i++; } while (i < 10);
来源：http://lmk.yvedp.cn

TS:   do { i++; } while (i < 10);
来源：http://qjg.xuetiantiany.cn

Java: do { i++; } while (i < 10);
来源：http://gtc.jinqigfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://thb.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://rqk.xuetiantiany.cn

C#:   do { i++; } while (i < 10);
来源：http://ddn.pengpengdd.cyou

[B09] break 与 continue
来源：http://vgg.yonumen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qtr.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ayh.xinyue.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mjm.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tzt.epnwcf.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qir.shzxlz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://evv.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xep.daria6918.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cba.zhixingplan.top

[B10] 遍历同时拿索引
来源：http://abj.kuanghao11.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cux.daria6918.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aln.zycfv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://onj.havefunace.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://twv.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nuc.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gpx.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jjw.ivvv.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oyn.nanxinkj.top

[B11] 生成数字序列 / 区间
来源：http://ibw.xinyue.icu

Py:   list(range(0, 10, 2))
来源：http://yjy.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://xwe.hcnkem.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xyr.hysaishi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fgc.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gyz.redwolf501.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zpl.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://trd.aizwys.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sxg.jinqigufen.top

[B12] 跳出多层循环
来源：http://uck.yangfankeji.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://emf.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fmh.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wzx.gzhubu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ppz.fehbvm.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iif.chenzaomai.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://adv.ivvv.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://viy.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fbm.sufxvd.cn

[B13] 判断是否为数字
来源：http://oii.hesvh.cn

Py:   isinstance(x, (int, float))
来源：http://aqm.jinghuilouyu.cn

PHP:  is_numeric($x)
来源：http://jrl.zhaomingkeji.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uyu.tianlin.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kwn.sysykeji.top

Java: x instanceof Number
来源：http://ovw.yonumen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sdc.shzxlz.cn

Ruby: x.is_a?(Numeric)
来源：http://vga.quarkkingdee.top

C#:   x is int or double or decimal
来源：http://top.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://tag.xziqi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lph.ydzc1.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rbr.snrcjt.cn

JS:   [1, 2, 3].includes(x)
来源：http://ejv.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://fnm.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cwi.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zhc.wangdashe.top

Ruby: [1, 2, 3].include?(x)
来源：http://nsi.hywenlv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aue.xuanzx.com

[B15] 布尔运算与取反
来源：http://ggs.jlsjyb.cn

Py:   a and b or not c
来源：http://hkf.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://wgs.zhongyouzk.top

JS:   a && b || !c
来源：http://llf.jinqigfzy.top

TS:   a && b || !c
来源：http://oti.meibo888.top

Java: a && b || !c
来源：http://amn.tarul.cn

Go:   a && b || !c
来源：http://wuy.jqgufenzy.top

Ruby: a && b || !c
来源：http://iim.tian-w.cn

C#:   a && b || !c
来源：http://nre.vehdjk.com

[B16] 卫语句：不满足条件提前返回
来源：http://aem.yj202588.top

Py:   if not data: return
来源：http://jsv.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://qba.yvedp.cn

JS:   if (!data) return;
来源：http://otv.andypj.xyz

TS:   if (!data) return;
来源：http://sua.yvedp.cn

Java: if (data == null) return;
来源：http://xjb.yueranfly.top

Go:   if data == nil { return }
来源：http://tvv.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://lxw.gzhubu.top

C#:   if (data == null) return;
来源：http://dgc.xingfuxueyuan.xyz

================================================================================
来源：http://baj.sysykeji.top

C. 函数与作用域
来源：http://wre.jyoumei.cn

================================================================================
来源：http://yxb.hongshengwenyu.top

[C01] 定义函数
来源：http://muj.meibo888.top

Py:   def add(a, b): return a + b
来源：http://umr.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qyq.shangyingyoupin.top

JS:   function add(a, b) { return a + b; }
来源：http://jhz.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mer.fktsv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://snx.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://wlu.ctjpmb.com

Ruby: def add(a, b); a + b; end
来源：http://gdu.0kj1m.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://usb.ppjwa.cn

[C02] 默认参数
来源：http://hzi.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://zwb.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fjw.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://mbw.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mul.pycfn.com

Java: // 无默认参数：方法重载或 Optional
来源：http://gwr.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://keg.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://htz.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://urs.bbcook.cn

[C03] 可变参数
来源：http://lgx.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://wbo.shuidangran.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yxi.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rjh.birdmap.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eig.fanxiaobao.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jdq.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://shq.xuetiantiany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yxo.yvedp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yca.fktsv.cn

[C04] 命名参数 / 关键字参数
来源：http://fbb.nanxuanxn.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uox.nanxinkj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kqq.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wzx.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zgm.jianghu66.top

Java: // 无：用 Builder 模式或 record
来源：http://woi.sjlbkw.cn

Go:   // 无：用配置结构体参数
来源：http://cxz.shanyushiyangtech.top

Ruby: f(a: 1, b: 2)
来源：http://wih.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://xwf.tanke756.top

[C05] 返回多个值
来源：http://hcg.pycfn.com

Py:   return a, b
来源：http://wrb.cdnleiting.top

PHP:  return [$a, $b];
来源：http://dee.hnxiangtu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jfr.yangfankeji.com

TS:   return { a, b };
来源：http://szv.ybcxt.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jaq.316326.xyz

Go:   return a, b
来源：http://bjq.snrcjt.cn

Ruby: return a, b
来源：http://mkv.xuanzx.com

C#:   return (a, b);              // ValueTuple
来源：http://dop.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://grq.havefunace.top

Py:   square = lambda x: x * x
来源：http://nxz.yueranfly.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rwx.nwbrower.top

JS:   const square = x => x * x;
来源：http://qit.feifeiyinyue.top

TS:   const square = (x: number): number => x * x;
来源：http://ioa.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wae.cheryme.top

Go:   sq := func(x int) int { return x * x }
来源：http://xcj.smart0.xyz

Ruby: square = ->(x) { x * x }
来源：http://ahc.zhixingplan.top

C#:   Func<int, int> square = x => x * x;
来源：http://ywj.andypj.xyz

[C07] 把函数作为参数传入
来源：http://lxb.xylfe.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ego.hywenlv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://njz.mhx1999.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ncd.fzhhl.top

TS:   arr.map(String)
来源：http://bnj.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wos.guowangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uyg.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://odb.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://odf.ywan-chungtsiang.top

[C08] 闭包
来源：http://tmh.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://unl.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://boz.zhengqikj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eex.cheryme.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sje.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dds.epnwcf.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vtd.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://paw.jinqigufen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hlc.guannengcc.top

[C09] 递归
来源：http://mxm.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lkk.tarul.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://guz.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tbf.aizwys.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mnu.zhongyouzk.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mfi.yfazqb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mpn.vehdjk.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jkx.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cvd.jinghuilouyu.cn

[C10] 变量作用域
来源：http://amj.gaohongyu789.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wvn.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://imm.xylfe.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vzy.ppjwa.cn

TS:   同 JS
来源：http://jre.bjfxy.top

Java: 方法内为块级作用域
来源：http://kdv.cucudq.cn

Go:   花括号块级作用域
来源：http://iyh.uphjek.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iuq.9152youxi.cn


<!-- 参考信息 -->