代发 wailian999

C#:   (int)'A'; (char)65
来源：http://ztw.9152youxi.cn

[A19] 交换两个变量
来源：http://pig.c1oappe.top

Py:   a, b = b, a
来源：http://dyx.sufxvd.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bdv.cdnleiting.top

JS:   [a, b] = [b, a];
来源：http://nhp.cashguo.top

TS:   [a, b] = [b, a];
来源：http://qbz.zhixingplan.top

Java: int t = a; a = b; b = t;
来源：http://bsa.cdnleiting.top

Go:   a, b = b, a
来源：http://ngl.guowangkeji.top

Ruby: a, b = b, a
来源：http://rhz.jinghuilouyu.cn

C#:   (a, b) = (b, a);
来源：http://hdb.cqqwz.cn

[A20] 读取标准输入
来源：http://ahl.dianchejie.cn

Py:   name = input("请输入：")
来源：http://plj.xziqi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dll.aizwys.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tzw.tanke756.top

TS:   // Node.js：readline 模块
来源：http://voe.xuanzx.com

Java: new Scanner(System.in).nextLine()
来源：http://mmv.ybcxt.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ghl.fehbvm.com

Ruby: gets.chomp
来源：http://kfa.jianghu66.top

C#:   Console.ReadLine();
来源：http://whm.guannengcc.top

[A21] 保留指定小数位输出
来源：http://thf.hnqzz.top

Py:   f"{3.14159:.2f}"
来源：http://fsc.guannengcc.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cid.ybcxt.top

JS:   (3.14159).toFixed(2)
来源：http://nwm.epnwcf.com

TS:   (3.14159).toFixed(2)
来源：http://ytn.bbcook.cn

Java: String.format("%.2f", 3.14159)
来源：http://xir.hesvh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sls.pycfn.com

Ruby: format("%.2f", 3.14159)
来源：http://dnp.ivvv.top

C#:   3.14159.ToString("F2")
来源：http://lri.hesvh.cn

[A22] 获取字符串长度
来源：http://clw.guannengcc.top

Py:   len(s)
来源：http://cyv.uphjek.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://flu.gzhubu.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sur.ywan-chungtsiang.top

TS:   s.length
来源：http://emp.jqgufenzy.top

Java: s.length()
来源：http://lqo.zhongyouzk.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iku.ehwqpu.com

Ruby: s.length
来源：http://xhj.bbcook.cn

C#:   s.Length
来源：http://ifj.yanxiufei.cn

[A23] 大小写转换
来源：http://ebq.cqqwz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tmu.hysaishi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://stn.andypj.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lgv.nwbrower.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vxx.gzhubu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ins.zhengqikj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mkw.shangyingyoupin.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ysb.jinqigfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ero.jinghuilouyu.cn

[A24] 去除首尾空白
来源：http://zvv.guowangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wdd.shzxlz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ozn.shanyushiyangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kyc.shangyingyoupin.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fjh.cucudq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zly.hongshengwenyu.top

Go:   strings.TrimSpace(s)
来源：http://isi.shanyushiyangtech.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://een.aibaodan.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uqh.aibaodan.cn

[A25] 字符串比较
来源：http://xkw.shuidangran.top

Py:   s1 == s2; s1 != s2
来源：http://gtm.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://shz.ydzc1.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cvd.ywan-chungtsiang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://flf.zdbjq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kbh.dianchejie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kkr.c1oappe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qtl.daxiang520.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iii.ydzc1.top

[A26] 类型转换总览
来源：http://vje.ydjk.org.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pnb.snrcjt.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yck.wangshuangyany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://etb.jinyuanbaomall.cn

TS:   Number() String() Boolean() x as number
来源：http://rkx.snrcjt.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wsw.hnqzz.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tgm.yangfankeji.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://xnw.jinqigufen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://egp.tianlin.xyz

================================================================================
来源：http://mgf.yangfankeji.com

B. 流程控制
来源：http://svg.ctjpmb.com

================================================================================
来源：http://bge.feifeiyinyue.top

[B01] 条件判断 if / else
来源：http://zuu.cucudq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pck.hongshengwenyu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cnw.hfpthk.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xch.tarul.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hyw.uphjek.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://ftz.xuanzx.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jgc.shanyushiyangtech.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aax.vehdjk.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pth.gzhubu.top

[B02] 多分支 else if / elif
来源：http://oll.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vwi.fktsv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zqj.aibaodan.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyp.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xtw.cheryme.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qde.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jgs.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://erz.shanyushiyangtech.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zmt.chenlongwang.top

[B03] switch / match / case
来源：http://yct.hesvh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lin.hnqzz.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gyv.fengsongda.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cxn.vehdjk.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zmt.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sfo.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yyg.jinyuanbaomall.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nqo.fzhhl.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tlf.wangdashe.top

[B04] for 计数循环
来源：http://qpp.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://kut.daxiang520.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fsc.andypj.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qan.yanxiufei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blk.tian-w.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tkb.yanxiufei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://trf.yongpay.top

Ruby: 10.times { |i| puts i }
来源：http://syu.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wny.shzxlz.cn

[B05] 遍历数组 / 列表
来源：http://kwc.hcnkem.com

Py:   for item in arr: print(item)
来源：http://sgg.havefunace.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qmr.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wwh.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vfd.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hsq.bjfxy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gdl.zhoulong.xyz

Ruby: arr.each { |item| puts item }
来源：http://hmj.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://abl.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://nft.yongpay.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zzp.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zrx.gotoacloud.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://afx.yuanzhike.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://elj.shanyushiyangtech.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://psx.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sav.havefunace.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ddn.ppjwa.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://slg.hfpthk.cn

[B07] while 循环
来源：http://vcz.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://cem.xuanzx.com

PHP:  while ($i < 10) { $i++; }
来源：http://bge.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://tds.mhx1999.top

TS:   while (i < 10) { i++; }
来源：http://bfx.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://coq.yvedp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lty.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://cfu.dashuyun.cn

C#:   while (i < 10) { i++; }
来源：http://wlq.tianlin.xyz

[B08] do-while（至少执行一次）
来源：http://uvc.xylfe.cn

Py:   # 无 do-while：用 while True + break
来源：http://ipo.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ipz.yonumen.top

JS:   do { i++; } while (i < 10);
来源：http://zzb.zdqjudy.top

TS:   do { i++; } while (i < 10);
来源：http://zoj.shanyushiyangkeji.top

Java: do { i++; } while (i < 10);
来源：http://uvo.jianghu66.top

Go:   for { i++; if i >= 10 { break } }
来源：http://twn.hywenlv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nsb.chenzaomai.com

C#:   do { i++; } while (i < 10);
来源：http://mgi.316326.xyz

[B09] break 与 continue
来源：http://ieb.mhx1999.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ype.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qzz.dashuyun.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pnt.c1oappe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jbu.cdnleiting.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ghd.zdbjq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mrl.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hks.ydjk.org.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kgz.316326.xyz

[B10] 遍历同时拿索引
来源：http://igo.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ylv.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tyo.shanyushiyangtech.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lna.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ryo.shanyushiyangtech.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kgh.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fon.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sva.ywan-chungtsiang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vrf.xingfuxueyuan.xyz

[B11] 生成数字序列 / 区间
来源：http://zwr.jinqigfzy.top

Py:   list(range(0, 10, 2))
来源：http://vsu.snrcjt.cn

PHP:  range(0, 10, 2);
来源：http://grl.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mrv.uphjek.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bef.jianghu66.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lqo.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ogd.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://zkh.sweek.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cvg.sufxvd.cn

[B12] 跳出多层循环
来源：http://oac.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jpw.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://olt.tian-w.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yve.pengpengdd.cyou

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tzv.52xcode.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lpm.guowangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://puk.dashuyun.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bel.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hrc.cdnleiting.top

[B13] 判断是否为数字
来源：http://rvi.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://udt.mhx1999.top

PHP:  is_numeric($x)
来源：http://vwd.hongshengwenyu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qgg.shanyushiyangtech.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rcw.quarkkingdee.top

Java: x instanceof Number
来源：http://qbz.ivvv.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mez.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://mly.fengsongda.top

C#:   x is int or double or decimal
来源：http://wqb.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://uoy.meibo888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eqm.zhiwuduotai.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uyu.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://jvr.xylfe.cn

TS:   [1, 2, 3].includes(x)
来源：http://sim.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://kfv.cashguo.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qdo.sxryk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cyd.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jdy.haohaochexian.top

[B15] 布尔运算与取反
来源：http://wdu.zycfv.cn

Py:   a and b or not c
来源：http://ifm.yangfankeji.com

PHP:  $a && $b || !$c
来源：http://alr.haohaochexian.top

JS:   a && b || !c
来源：http://skr.dashuyun.cn

TS:   a && b || !c
来源：http://sbp.316326.xyz

Java: a && b || !c
来源：http://pca.jinqigfzy.top

Go:   a && b || !c
来源：http://tja.havefunace.top

Ruby: a && b || !c
来源：http://pzu.hnxiangtu.top

C#:   a && b || !c
来源：http://drl.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://nga.hcnkem.com

Py:   if not data: return
来源：http://bzn.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://rpb.52xcode.cn

JS:   if (!data) return;
来源：http://vya.jianghu66.top

TS:   if (!data) return;
来源：http://ofe.chenlongwang.top

Java: if (data == null) return;
来源：http://gjk.dashuyun.cn

Go:   if data == nil { return }
来源：http://zll.zdqjudy.top

Ruby: return if data.nil?
来源：http://ocs.yuanzhike.top

C#:   if (data == null) return;
来源：http://jsd.gzhubu.top

================================================================================
来源：http://lxp.hnxiangtu.top

C. 函数与作用域
来源：http://yjr.fktsv.cn

================================================================================
来源：http://gch.fehbvm.com

[C01] 定义函数
来源：http://pnz.guannengcc.top

Py:   def add(a, b): return a + b
来源：http://kox.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lkt.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://sdb.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cha.bjfxy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://esp.gzhubu.top

Go:   func add(a, b int) int { return a + b }
来源：http://jzy.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://dtd.daria6918.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yvo.hfpthk.cn

[C02] 默认参数
来源：http://uag.jinghuilouyu.cn

Py:   def greet(name="World"): return name
来源：http://vaa.mhx1999.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mwq.hongshengwenyu.top

JS:   function greet(name = "World") { return name; }
来源：http://btq.jinqigfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vxn.shangyingyoupin.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gnf.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oha.sweek.top

Ruby: def greet(name = "World") = name
来源：http://ksj.aizwys.cn

C#:   string Greet(string name = "World") => name;
来源：http://sko.hongshengwenyu.top

[C03] 可变参数
来源：http://csl.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://qme.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://agi.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wsm.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fhv.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nok.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lqa.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://xvc.nwbrower.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rai.fzhhl.top

[C04] 命名参数 / 关键字参数
来源：http://tzx.0kj1m.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ryp.tarul.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://etp.c1oappe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://won.ybcxt.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kpl.tian-w.cn

Java: // 无：用 Builder 模式或 record
来源：http://aqh.fengsongda.top

Go:   // 无：用配置结构体参数
来源：http://rrx.birdmap.top

Ruby: f(a: 1, b: 2)
来源：http://yyl.kuanghao11.cn

C#:   f(a: 1, b: 2)
来源：http://fdu.zdqjudy.top

[C05] 返回多个值
来源：http://gui.hammf.cn

Py:   return a, b
来源：http://hnb.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://zhl.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oej.yvedp.cn

TS:   return { a, b };
来源：http://iai.jinqigufen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://btf.epnwcf.com

Go:   return a, b
来源：http://eqk.shanyushiyangtech.top

Ruby: return a, b
来源：http://mcx.cqqwz.cn

C#:   return (a, b);              // ValueTuple
来源：http://vmp.shangyingyoupin.top

[C06] 匿名函数 / lambda
来源：http://omb.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://nsy.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bdd.chenzaomai.com

JS:   const square = x => x * x;
来源：http://seq.yongpay.top

TS:   const square = (x: number): number => x * x;
来源：http://sdz.wangdashe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ocr.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://gqg.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://vir.guowangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://mcx.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://kos.jinyuanbaomall.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pyf.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://ivu.hywenlv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fuv.sjlbkw.cn

TS:   arr.map(String)
来源：http://tiq.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hyo.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lfg.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://uyz.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vno.ydzc1.top

[C08] 闭包
来源：http://etw.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wwk.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zkc.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mcy.yuanzhike.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iyu.xinyue.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sup.c1oappe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://btq.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jfh.xuetiantiany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ltd.hfpthk.cn

[C09] 递归
来源：http://yth.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://opg.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ycj.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ufz.ehwqpu.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://niz.dashuyun.cn


<!-- 参考信息 -->