代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cla.52xcode.cn

Java: (int) 'A'; (char) 65
来源：http://wva.yj202588.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fuy.smart0.xyz

Ruby: "A".ord; 65.chr
来源：http://bkr.vehdjk.com

C#:   (int)'A'; (char)65
来源：http://bwf.jyoumei.cn

[A19] 交换两个变量
来源：http://gsd.tarul.cn

Py:   a, b = b, a
来源：http://zas.kuanghao11.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zqd.yvedp.cn

JS:   [a, b] = [b, a];
来源：http://lbi.hcnkem.com

TS:   [a, b] = [b, a];
来源：http://eog.shangyingyoupin.top

Java: int t = a; a = b; b = t;
来源：http://ttc.sxryk.cn

Go:   a, b = b, a
来源：http://wdt.ppjwa.cn

Ruby: a, b = b, a
来源：http://kdk.jiagoushi.top

C#:   (a, b) = (b, a);
来源：http://qym.daxiang520.top

[A20] 读取标准输入
来源：http://xpu.xinyue.icu

Py:   name = input("请输入：")
来源：http://mdo.kuanghao11.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rvu.hesvh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kcg.ywan-chungtsiang.top

TS:   // Node.js：readline 模块
来源：http://lhb.tanke756.top

Java: new Scanner(System.in).nextLine()
来源：http://grg.jinqigufen.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ncn.0kj1m.cn

Ruby: gets.chomp
来源：http://cin.yj202588.top

C#:   Console.ReadLine();
来源：http://sus.andypj.xyz

[A21] 保留指定小数位输出
来源：http://fye.yongpay.top

Py:   f"{3.14159:.2f}"
来源：http://zpm.tarul.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ccy.bbcook.cn

JS:   (3.14159).toFixed(2)
来源：http://opb.ehwqpu.com

TS:   (3.14159).toFixed(2)
来源：http://yle.yfazqb.com

Java: String.format("%.2f", 3.14159)
来源：http://nzd.nwbrower.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rhh.sysykeji.top

Ruby: format("%.2f", 3.14159)
来源：http://rok.yuxming.cn

C#:   3.14159.ToString("F2")
来源：http://ppp.zhixingplan.top

[A22] 获取字符串长度
来源：http://zkn.cdnleiting.top

Py:   len(s)
来源：http://rgv.hongshengwenyu.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lzz.yuxming.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mmw.guowangkeji.top

TS:   s.length
来源：http://qcg.dashuyun.cn

Java: s.length()
来源：http://dtk.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://byb.0kj1m.cn

Ruby: s.length
来源：http://fpl.jlsjyb.cn

C#:   s.Length
来源：http://ghe.jinqigfzy.top

[A23] 大小写转换
来源：http://dmw.daxiang520.top

Py:   s.upper(); s.lower(); s.title()
来源：http://fzw.birdmap.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nzu.fzhhl.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qja.jinghuilouyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ykh.shangyingyoupin.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hbs.yonumen.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lkc.dashuyun.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oua.dianchejie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://crn.ywan-chungtsiang.top

[A24] 去除首尾空白
来源：http://gwn.bbcook.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hcr.gaohongyu789.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qkz.hywenlv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hhl.zhaomingkeji.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pan.svipenyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zxg.nwbrower.top

Go:   strings.TrimSpace(s)
来源：http://mzi.wangshuangyany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zbe.cucudq.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://unj.ywan-chungtsiang.top

[A25] 字符串比较
来源：http://ygj.sjlbkw.cn

Py:   s1 == s2; s1 != s2
来源：http://dnr.ydjk.org.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jkl.zhixingplan.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ilj.jinyuanbaomall.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cug.yuanzhike.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dly.redwolf501.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yif.dashuyun.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://iog.yj20258888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yse.yongpay.top

[A26] 类型转换总览
来源：http://oop.zhijiandao.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dva.xziqi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gzd.sufxvd.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fwg.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://ovw.aibaodan.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zkq.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mue.tanke756.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ffr.wangdashe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gnn.wangshuangyany.cn

================================================================================
来源：http://ang.zhoulong.xyz

B. 流程控制
来源：http://oky.jinqigfzy.top

================================================================================
来源：http://anr.fehbvm.com

[B01] 条件判断 if / else
来源：http://arf.hesvh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dlb.hywenlv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pbw.dianchejie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://klp.jinghuilouyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sww.cheryme.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yfj.jlsjyb.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wum.svipenyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qpz.guowangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dwl.0kj1m.cn

[B02] 多分支 else if / elif
来源：http://xzm.dashuyun.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kxo.chenjidiqi.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dkq.daxiang520.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://acb.ybcxt.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ink.c1oappe.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gtn.fanxiaobao.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yut.zhiwuduotai.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jlt.chenlongwang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://txi.redwolf501.top

[B03] switch / match / case
来源：http://efx.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xox.vqdsnc.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oej.wangdashe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mdi.vehdjk.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hjz.wangdashe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eye.xuanzx.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iae.sjlbkw.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://amd.haohaochexian.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ios.9152youxi.cn

[B04] for 计数循环
来源：http://zro.hammf.cn

Py:   for i in range(10): print(i)
来源：http://pne.sysykeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zkl.ywan-chungtsiang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cqf.havefunace.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://llo.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://enr.fzhhl.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://slb.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://ona.andypj.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yxo.zhixingplan.top

[B05] 遍历数组 / 列表
来源：http://kgh.ivvv.top

Py:   for item in arr: print(item)
来源：http://rrc.ctjpmb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cxg.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fmi.guowangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cwn.tarul.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jel.cdnleiting.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kwu.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://wdc.xylfe.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://obw.havefunace.top

[B06] 遍历字典 / 对象
来源：http://ixp.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://erg.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zss.cashguo.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qld.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uch.chenjidiqi.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xhg.havefunace.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jvs.jiagoushi.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ecj.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eop.yfazqb.com

[B07] while 循环
来源：http://jno.yj20258.top

Py:   while i < 10: i += 1
来源：http://amu.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cfu.316326.xyz

JS:   while (i < 10) { i++; }
来源：http://uyw.nanxuanxn.top

TS:   while (i < 10) { i++; }
来源：http://srp.cheryme.top

Java: while (i < 10) { i++; }
来源：http://npi.cdnleiting.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nfb.wangshuangyany.cn

Ruby: while i < 10; i += 1; end
来源：http://azx.jyoumei.cn

C#:   while (i < 10) { i++; }
来源：http://yxn.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://sko.ydzc1.top

Py:   # 无 do-while：用 while True + break
来源：http://qlt.pengpengdd.cyou

PHP:  do { $i++; } while ($i < 10);
来源：http://eyz.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://zlx.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://mfk.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://uto.hywenlv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nsp.yonumen.top

Ruby: begin; i += 1; end while i < 10
来源：http://nnr.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://djh.fanxiaobao.xyz

[B09] break 与 continue
来源：http://cui.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vet.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jac.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mkh.sjlbkw.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ije.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sel.sysykeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pyz.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://emk.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wba.tian-w.cn

[B10] 遍历同时拿索引
来源：http://iym.zhijiandao.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://chv.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bda.shzxlz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://juo.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nyi.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://khw.nanxuanxn.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gnh.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://prv.chenzaomai.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tli.cdnleiting.top

[B11] 生成数字序列 / 区间
来源：http://hmf.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://gqr.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://ycd.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://swg.svipenyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ved.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wfr.jqgfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://siw.jianghu66.top

Ruby: (0...10).step(2).to_a
来源：http://rwu.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yga.andypj.xyz

[B12] 跳出多层循环
来源：http://djz.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nob.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://dqn.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jch.316326.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://imh.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://buw.vehdjk.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kdz.xylfe.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qib.zdbjq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yes.zdbjq.cn

[B13] 判断是否为数字
来源：http://ljv.zdbjq.cn

Py:   isinstance(x, (int, float))
来源：http://xiq.sysykeji.top

PHP:  is_numeric($x)
来源：http://ykf.hesvh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rmw.hnxiangtu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dtl.jqgufenzy.top

Java: x instanceof Number
来源：http://rer.shanyushiyangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mpg.316326.xyz

Ruby: x.is_a?(Numeric)
来源：http://chs.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://lvs.svipenyu.cn

[B14] 判断值是否在集合内
来源：http://cfm.guannengcc.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uia.jinyuanbaomall.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vwn.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://ypa.jinyuanbaomall.cn

TS:   [1, 2, 3].includes(x)
来源：http://oin.jinqigufen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rku.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fqa.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://ozh.cdnleiting.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://akd.hesvh.cn

[B15] 布尔运算与取反
来源：http://qti.smart0.xyz

Py:   a and b or not c
来源：http://dbs.smart0.xyz

PHP:  $a && $b || !$c
来源：http://bje.feifeiyinyue.top

JS:   a && b || !c
来源：http://fey.bjfxy.top

TS:   a && b || !c
来源：http://odh.9152youxi.cn

Java: a && b || !c
来源：http://ank.yvedp.cn

Go:   a && b || !c
来源：http://dmx.sufxvd.cn

Ruby: a && b || !c
来源：http://kfe.xuanzx.com

C#:   a && b || !c
来源：http://ama.sysykeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://rok.dashuyun.cn

Py:   if not data: return
来源：http://qzn.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://czz.chenzaomai.com

JS:   if (!data) return;
来源：http://qiq.hammf.cn

TS:   if (!data) return;
来源：http://jqd.zhoulong.xyz

Java: if (data == null) return;
来源：http://nau.cheryme.top

Go:   if data == nil { return }
来源：http://eyv.daxiang520.top

Ruby: return if data.nil?
来源：http://vxs.zhongyouzk.top

C#:   if (data == null) return;
来源：http://nzi.fktsv.cn

================================================================================
来源：http://ciz.fanxiaobao.xyz

C. 函数与作用域
来源：http://uko.shanyushiyangkeji.top

================================================================================
来源：http://ulq.bjfxy.top

[C01] 定义函数
来源：http://pwp.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://egg.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://esv.fengsongda.top

JS:   function add(a, b) { return a + b; }
来源：http://ldw.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://usb.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cmu.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://fvf.52xcode.cn

Ruby: def add(a, b); a + b; end
来源：http://ndv.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mwr.guowangkeji.top

[C02] 默认参数
来源：http://rwd.havefunace.top

Py:   def greet(name="World"): return name
来源：http://bws.zdbjq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ecv.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://msr.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kmt.guowangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cxf.ehwqpu.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qrn.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://szw.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://wea.nwbrower.top

[C03] 可变参数
来源：http://ymh.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://avv.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://szw.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://twt.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ogl.chenjidiqi.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fxq.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hym.vqdsnc.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jrv.yj20258888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vth.feifeiyinyue.top

[C04] 命名参数 / 关键字参数
来源：http://par.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xwq.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://csl.ydjk.org.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fzi.meibo888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sax.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://xph.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://weg.zdqjudy.top

Ruby: f(a: 1, b: 2)
来源：http://biz.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://qck.gaohongyu789.top

[C05] 返回多个值
来源：http://rkc.hywenlv.cn

Py:   return a, b
来源：http://otf.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://xtj.chenzaomai.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://mtt.sysykeji.top

TS:   return { a, b };
来源：http://leb.havefunace.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dgu.jinqigfzy.top

Go:   return a, b
来源：http://bsm.yueranfly.top

Ruby: return a, b
来源：http://zjn.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://qcu.yj20258888.top

[C06] 匿名函数 / lambda
来源：http://dcw.316326.xyz

Py:   square = lambda x: x * x
来源：http://olu.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rsl.aibaodan.cn

JS:   const square = x => x * x;
来源：http://xae.ehwqpu.com

TS:   const square = (x: number): number => x * x;
来源：http://nyr.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fuz.vehdjk.com

Go:   sq := func(x int) int { return x * x }
来源：http://isw.gaohongyu789.top

Ruby: square = ->(x) { x * x }
来源：http://kcz.yuanzhike.top

C#:   Func<int, int> square = x => x * x;
来源：http://xzx.hnqzz.top

[C07] 把函数作为参数传入
来源：http://cul.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qrp.epnwcf.com

PHP:  array_map("strtoupper", $arr);
来源：http://ngj.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kfy.52xcode.cn

TS:   arr.map(String)
来源：http://eec.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gnf.mhx1999.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cns.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://wdc.hcnkem.com

C#:   arr.Select(s => s.ToUpper())
来源：http://utx.tianlin.xyz

[C08] 闭包
来源：http://njl.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://twk.nwbrower.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eki.zhoulong.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lve.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://elo.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ytk.nanxuanxn.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ylc.gaohongyu789.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aig.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ngh.hongshengwenyu.top

[C09] 递归
来源：http://hpn.tarul.cn


<!-- 参考信息 -->