代发 wailian999

JS:   [a, b] = [b, a];
来源：http://stp.ybcxt.top

TS:   [a, b] = [b, a];
来源：http://vvx.nwbrower.top

Java: int t = a; a = b; b = t;
来源：http://kny.cucudq.cn

Go:   a, b = b, a
来源：http://jvf.mhx1999.top

Ruby: a, b = b, a
来源：http://ixs.tian-w.cn

C#:   (a, b) = (b, a);
来源：http://cdl.pycfn.com

[A20] 读取标准输入
来源：http://iyt.guowangkeji.top

Py:   name = input("请输入：")
来源：http://eqr.vehdjk.com

PHP:  $name = trim(fgets(STDIN));
来源：http://oqz.cheryme.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://thf.guowangkeji.top

TS:   // Node.js：readline 模块
来源：http://ult.smart0.xyz

Java: new Scanner(System.in).nextLine()
来源：http://ceu.cashguo.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qxn.cdnleiting.top

Ruby: gets.chomp
来源：http://xix.shuidangran.top

C#:   Console.ReadLine();
来源：http://uzf.epnwcf.com

[A21] 保留指定小数位输出
来源：http://avc.fehbvm.com

Py:   f"{3.14159:.2f}"
来源：http://pid.redwolf501.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iun.zhixingplan.top

JS:   (3.14159).toFixed(2)
来源：http://jlx.jqgufenzy.top

TS:   (3.14159).toFixed(2)
来源：http://rtg.jqgfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://syy.ydjk.org.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kim.smart0.xyz

Ruby: format("%.2f", 3.14159)
来源：http://zbh.shuidangran.top

C#:   3.14159.ToString("F2")
来源：http://axc.jinqigfzy.top

[A22] 获取字符串长度
来源：http://upf.jinqigufen.top

Py:   len(s)
来源：http://wls.gzhubu.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rvz.xingfuxueyuan.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zsw.xziqi.cn

TS:   s.length
来源：http://qlp.feifeiyinyue.top

Java: s.length()
来源：http://ubg.ppjwa.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dfr.andypj.xyz

Ruby: s.length
来源：http://gyh.cqqwz.cn

C#:   s.Length
来源：http://oyu.andypj.xyz

[A23] 大小写转换
来源：http://hzn.feifeiyinyue.top

Py:   s.upper(); s.lower(); s.title()
来源：http://knl.haohaochexian.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://isl.iojbl.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fkf.hesvh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rkm.zdbjq.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pfs.feifeiyinyue.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mjz.dashuyun.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://huv.shanyushiyangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bko.hywenlv.cn

[A24] 去除首尾空白
来源：http://gqr.zhengqikj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xaz.ivvv.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://skv.bbcook.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://giu.yj20258888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kvc.shanyushiyangtech.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vrb.ppjwa.cn

Go:   strings.TrimSpace(s)
来源：http://vcp.aizwys.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iin.fanxiaobao.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zlx.feifeiyinyue.top

[A25] 字符串比较
来源：http://leh.yj20258.top

Py:   s1 == s2; s1 != s2
来源：http://glr.nanxinkj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vte.mhx1999.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bsn.guowangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ecf.wangdashe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wqc.pycfn.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://enf.xingfuxueyuan.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://lch.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://egj.vqdsnc.cn

[A26] 类型转换总览
来源：http://pvi.daxiang520.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://etd.fktsv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zmt.yvedp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wsf.svipenyu.cn

TS:   Number() String() Boolean() x as number
来源：http://uov.daria6918.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hrg.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bkh.cheryme.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xvw.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cdw.yonumen.top

================================================================================
来源：http://kjf.ywan-chungtsiang.top

B. 流程控制
来源：http://zea.tanke756.top

================================================================================
来源：http://pky.zycfv.cn

[B01] 条件判断 if / else
来源：http://wdg.shanyushiyangtech.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hue.jinqigufen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sfg.guowangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wpk.yj20258.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pbv.jqgufenzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://drk.sjlbkw.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hzv.pycfn.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wjh.xuanzx.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cbu.fengsongda.top

[B02] 多分支 else if / elif
来源：http://hvj.haohaochexian.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wva.zhaomingkeji.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qwy.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eby.nwbrower.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zwl.zhiwuduotai.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ewn.ydjk.org.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pby.aibaodan.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://szm.316326.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kpq.jinqigufen.top

[B03] switch / match / case
来源：http://tfo.sweek.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yjc.fehbvm.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ini.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://myv.ydzc1.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uaa.smart0.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lrn.jinyuanbaomall.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xel.shzxlz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xqr.aibaodan.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lti.aibaodan.cn

[B04] for 计数循环
来源：http://yxo.52xcode.cn

Py:   for i in range(10): print(i)
来源：http://qls.zdbjq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ejd.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hfy.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ima.jiagoushi.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zfy.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rme.gotoacloud.top

Ruby: 10.times { |i| puts i }
来源：http://nkp.zycfv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xnk.haohaochexian.top

[B05] 遍历数组 / 列表
来源：http://ems.zhijiandao.cn

Py:   for item in arr: print(item)
来源：http://qlm.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tfg.tanke756.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tei.yangfankeji.com

TS:   for (const item of arr) { console.log(item); }
来源：http://xec.jqgufenzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dlx.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vqd.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://obb.cheryme.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jeu.xuanzx.com

[B06] 遍历字典 / 对象
来源：http://dmn.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bbv.fengsongda.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kkn.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://odx.tian-w.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://txr.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fua.yvedp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lhc.pengpengdd.cyou

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://had.fengsongda.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vnx.havefunace.top

[B07] while 循环
来源：http://cmf.sweek.top

Py:   while i < 10: i += 1
来源：http://dfz.ydzc1.top

PHP:  while ($i < 10) { $i++; }
来源：http://pxh.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://ehd.hammf.cn

TS:   while (i < 10) { i++; }
来源：http://vdx.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://vpo.zhongyouzk.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://upm.zhijiandao.cn

Ruby: while i < 10; i += 1; end
来源：http://oat.nanxinkj.top

C#:   while (i < 10) { i++; }
来源：http://ozj.jyoumei.cn

[B08] do-while（至少执行一次）
来源：http://dhq.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://eza.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qta.jyoumei.cn

JS:   do { i++; } while (i < 10);
来源：http://ymd.ivvv.top

TS:   do { i++; } while (i < 10);
来源：http://zqi.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://mou.fktsv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zmb.nwbrower.top

Ruby: begin; i += 1; end while i < 10
来源：http://qfj.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://lur.shanyushiyangtech.top

[B09] break 与 continue
来源：http://esa.shzxlz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://luc.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kjb.uphjek.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ofi.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iph.zdbjq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gjs.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kqp.aizwys.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dnt.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jum.zdbjq.cn

[B10] 遍历同时拿索引
来源：http://kyz.pengpengdd.cyou

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uaf.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ova.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qyf.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://feq.fehbvm.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eer.ctjpmb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ybc.tanke756.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://obt.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hhl.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://ita.redwolf501.top

Py:   list(range(0, 10, 2))
来源：http://axc.fengsongda.top

PHP:  range(0, 10, 2);
来源：http://okf.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ace.fzhhl.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kpe.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wyl.hnxiangtu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eds.yj20258888.top

Ruby: (0...10).step(2).to_a
来源：http://ecn.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ivt.pycfn.com

[B12] 跳出多层循环
来源：http://vsp.xylfe.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ukn.aibaodan.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hrd.316326.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://csy.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iow.yfazqb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sfh.nwbrower.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tal.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tjy.zhongyouzk.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://arq.zhongyouzk.top

[B13] 判断是否为数字
来源：http://xfb.chenjidiqi.icu

Py:   isinstance(x, (int, float))
来源：http://lgu.uphjek.com

PHP:  is_numeric($x)
来源：http://kwf.pengpengdd.cyou

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fvu.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gdh.yuanzhike.top

Java: x instanceof Number
来源：http://fpx.andypj.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vbz.andypj.xyz

Ruby: x.is_a?(Numeric)
来源：http://baw.sufxvd.cn

C#:   x is int or double or decimal
来源：http://ekm.jinyuanbaomall.cn

[B14] 判断值是否在集合内
来源：http://vzu.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rxl.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zfe.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://ecd.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://myd.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nia.meibo888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pev.nanxuanxn.top

Ruby: [1, 2, 3].include?(x)
来源：http://yfs.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qpp.ybcxt.top

[B15] 布尔运算与取反
来源：http://omq.hongshengwenyu.top

Py:   a and b or not c
来源：http://gij.quarkkingdee.top

PHP:  $a && $b || !$c
来源：http://bxb.uphjek.com

JS:   a && b || !c
来源：http://ktn.fktsv.cn

TS:   a && b || !c
来源：http://xzu.meibo888.top

Java: a && b || !c
来源：http://zkq.jyoumei.cn

Go:   a && b || !c
来源：http://sai.52xcode.cn

Ruby: a && b || !c
来源：http://ifr.jinghuilouyu.cn

C#:   a && b || !c
来源：http://hdw.zhengqikj.top

[B16] 卫语句：不满足条件提前返回
来源：http://bbk.yfazqb.com

Py:   if not data: return
来源：http://pve.zhijiandao.cn

PHP:  if (!$data) { return; }
来源：http://mtr.zhoulong.xyz

JS:   if (!data) return;
来源：http://pod.zhixingplan.top

TS:   if (!data) return;
来源：http://nax.9152youxi.cn

Java: if (data == null) return;
来源：http://izt.ppjwa.cn

Go:   if data == nil { return }
来源：http://raj.bbcook.cn

Ruby: return if data.nil?
来源：http://nhh.jqgufenzy.top

C#:   if (data == null) return;
来源：http://xtd.shzxlz.cn

================================================================================
来源：http://nhb.svipenyu.cn

C. 函数与作用域
来源：http://adj.jyoumei.cn

================================================================================
来源：http://lhr.jianghu66.top

[C01] 定义函数
来源：http://nbb.yj20258888.top

Py:   def add(a, b): return a + b
来源：http://agd.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lgd.kuanghao11.cn

JS:   function add(a, b) { return a + b; }
来源：http://fxd.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://whp.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pju.mhx1999.top

Go:   func add(a, b int) int { return a + b }
来源：http://bnk.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://nhy.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ggw.gotoacloud.top

[C02] 默认参数
来源：http://xur.sufxvd.cn

Py:   def greet(name="World"): return name
来源：http://alu.ehwqpu.com

PHP:  function greet($name = "World") { return $name; }
来源：http://uvv.yj20258888.top

JS:   function greet(name = "World") { return name; }
来源：http://kdo.316326.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://jvv.aizwys.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gli.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://afe.zhongyouzk.top

Ruby: def greet(name = "World") = name
来源：http://kay.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://vjl.fktsv.cn

[C03] 可变参数
来源：http://vnp.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://sum.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://guv.dashuyun.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tek.shzxlz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://crx.yvedp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pkz.gzhubu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hiu.cucudq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vrj.hywenlv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mea.gotoacloud.top

[C04] 命名参数 / 关键字参数
来源：http://hxk.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gwo.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pdj.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dpz.tanke756.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aho.zdqjudy.top

Java: // 无：用 Builder 模式或 record
来源：http://flb.sjlbkw.cn

Go:   // 无：用配置结构体参数
来源：http://hng.vqdsnc.cn

Ruby: f(a: 1, b: 2)
来源：http://stj.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://img.pengpengdd.cyou

[C05] 返回多个值
来源：http://qev.zhoulong.xyz

Py:   return a, b
来源：http://ykp.tianlin.xyz

PHP:  return [$a, $b];
来源：http://wdc.tanke756.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dnj.pengpengdd.cyou

TS:   return { a, b };
来源：http://rky.wangshuangyany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xhk.ctjpmb.com

Go:   return a, b
来源：http://tkm.hysaishi.cn

Ruby: return a, b
来源：http://fqi.sjlbkw.cn

C#:   return (a, b);              // ValueTuple
来源：http://myf.c1oappe.top

[C06] 匿名函数 / lambda
来源：http://oeo.jqgufenzy.top

Py:   square = lambda x: x * x
来源：http://jqt.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bfq.andypj.xyz

JS:   const square = x => x * x;
来源：http://wsw.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://iot.zhijiandao.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hqi.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://lww.hcnkem.com

Ruby: square = ->(x) { x * x }
来源：http://gfr.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://yvg.sweek.top

[C07] 把函数作为参数传入
来源：http://gcs.yongpay.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ivm.mhx1999.top

PHP:  array_map("strtoupper", $arr);
来源：http://jsd.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rpy.zhijiandao.cn

TS:   arr.map(String)
来源：http://dyi.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hgl.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tvy.quarkkingdee.top

Ruby: arr.map(&:upcase)
来源：http://pfs.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jpv.yangfankeji.com

[C08] 闭包
来源：http://cms.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lwe.ppjwa.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://svy.birdmap.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://omk.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aja.0kj1m.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://euw.xingfuxueyuan.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wru.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jtt.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lbn.chenjidiqi.icu

[C09] 递归
来源：http://lxq.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://opg.gotoacloud.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ike.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aei.hnxiangtu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://utg.haohaochexian.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iln.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kxw.316326.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uec.pengpengdd.cyou

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zir.tarul.cn


<!-- 参考信息 -->