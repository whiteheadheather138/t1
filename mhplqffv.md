代发 wailian999

JS:   [a, b] = [b, a];
来源：http://noj.yj202588.top

TS:   [a, b] = [b, a];
来源：http://nru.pengpengdd.cyou

Java: int t = a; a = b; b = t;
来源：http://yow.sxryk.cn

Go:   a, b = b, a
来源：http://mww.meibo888.top

Ruby: a, b = b, a
来源：http://hvt.hnqzz.top

C#:   (a, b) = (b, a);
来源：http://ysh.jyoumei.cn

[A20] 读取标准输入
来源：http://rtp.52xcode.cn

Py:   name = input("请输入：")
来源：http://kru.jinqigfzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wrx.sjlbkw.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dfr.jiagoushi.top

TS:   // Node.js：readline 模块
来源：http://fgq.fanxiaobao.xyz

Java: new Scanner(System.in).nextLine()
来源：http://afw.chenzaomai.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fji.9152youxi.cn

Ruby: gets.chomp
来源：http://pzw.iojbl.cn

C#:   Console.ReadLine();
来源：http://rrh.bjfxy.top

[A21] 保留指定小数位输出
来源：http://dog.ehwqpu.com

Py:   f"{3.14159:.2f}"
来源：http://hmx.xziqi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zmv.hnxiangtu.top

JS:   (3.14159).toFixed(2)
来源：http://aho.jinqigfzy.top

TS:   (3.14159).toFixed(2)
来源：http://qbb.uphjek.com

Java: String.format("%.2f", 3.14159)
来源：http://pbl.cqqwz.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vma.fanxiaobao.xyz

Ruby: format("%.2f", 3.14159)
来源：http://qna.nwbrower.top

C#:   3.14159.ToString("F2")
来源：http://hgz.zhoulong.xyz

[A22] 获取字符串长度
来源：http://bqa.hcnkem.com

Py:   len(s)
来源：http://znl.quarkkingdee.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://elb.xylfe.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://liq.smart0.xyz

TS:   s.length
来源：http://duw.sxryk.cn

Java: s.length()
来源：http://owt.yfazqb.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pwy.yj202588.top

Ruby: s.length
来源：http://tld.tanke756.top

C#:   s.Length
来源：http://shx.sxryk.cn

[A23] 大小写转换
来源：http://mco.ppjwa.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bmx.xingfuxueyuan.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kib.ehwqpu.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yzn.hfpthk.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rvn.yuanzhike.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mct.hcnkem.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://day.jianghu66.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lqn.gogol.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://quv.xuetiantiany.cn

[A24] 去除首尾空白
来源：http://aip.ctjpmb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cvx.ppjwa.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gar.yj20258.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pls.birdmap.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://etu.xylfe.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rog.nanxinkj.top

Go:   strings.TrimSpace(s)
来源：http://fka.mhx1999.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ddz.yongpay.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fiu.dianchejie.cn

[A25] 字符串比较
来源：http://wpx.aizwys.cn

Py:   s1 == s2; s1 != s2
来源：http://woa.tian-w.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ydu.wangshuangyany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eun.fehbvm.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ipt.hywenlv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xwo.quarkkingdee.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vyn.cqqwz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xlq.ybcxt.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://svn.bbcook.cn

[A26] 类型转换总览
来源：http://iyl.tanke756.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://edc.shuidangran.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ifa.shuidangran.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ivx.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://jvk.yj20258.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ena.dashuyun.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wmn.tarul.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tps.epnwcf.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wkn.iojbl.cn

================================================================================
来源：http://nrb.cashguo.top

B. 流程控制
来源：http://jef.sufxvd.cn

================================================================================
来源：http://gbc.nanxinkj.top

[B01] 条件判断 if / else
来源：http://leg.zycfv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yzv.jinghuilouyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://isj.ctjpmb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oiz.nanxuanxn.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gdi.cheryme.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ypl.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://prg.ydjk.org.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://plw.yj20258.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wwy.fehbvm.com

[B02] 多分支 else if / elif
来源：http://pex.cheryme.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zon.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ygl.shanyushiyangkeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wvs.tian-w.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zgp.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ahg.gzhubu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bha.fengsongda.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yzi.yj20258.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xzp.zdbjq.cn

[B03] switch / match / case
来源：http://gia.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nem.daria6918.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xkv.svipenyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sch.redwolf501.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nvc.yj202588.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dam.sysykeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://npm.jinyuanbaomall.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://joi.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eqy.ydjk.org.cn

[B04] for 计数循环
来源：http://tzj.ivvv.top

Py:   for i in range(10): print(i)
来源：http://ssk.yj20258888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ahu.xuetiantiany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ele.yvedp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gcl.andypj.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hum.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dcy.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://mct.wangshuangyany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bmq.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://ecc.jinqigufen.top

Py:   for item in arr: print(item)
来源：http://rgl.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xhv.fanxiaobao.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://mnx.hesvh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://flk.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kmb.zhaomingkeji.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bzl.tarul.cn

Ruby: arr.each { |item| puts item }
来源：http://vkh.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lmg.zhiwuduotai.top

[B06] 遍历字典 / 对象
来源：http://qmc.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://pgu.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fph.shanyushiyangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ypc.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ouw.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tih.xingfuxueyuan.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pvv.xingfuxueyuan.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dgl.jinyuanbaomall.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tji.jlsjyb.cn

[B07] while 循环
来源：http://zio.yongpay.top

Py:   while i < 10: i += 1
来源：http://lsj.hywenlv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://csu.jlsjyb.cn

JS:   while (i < 10) { i++; }
来源：http://fuw.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://puf.jianghu66.top

Java: while (i < 10) { i++; }
来源：http://rhf.chenlongwang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oah.jinqigfzy.top

Ruby: while i < 10; i += 1; end
来源：http://lhc.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://qqp.chenlongwang.top

[B08] do-while（至少执行一次）
来源：http://lsb.fzhhl.top

Py:   # 无 do-while：用 while True + break
来源：http://gnr.zhijiandao.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vqy.meibo888.top

JS:   do { i++; } while (i < 10);
来源：http://ugq.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://xus.zdbjq.cn

Java: do { i++; } while (i < 10);
来源：http://ttv.zhixingplan.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pjv.bjfxy.top

Ruby: begin; i += 1; end while i < 10
来源：http://ela.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://yyw.zhixingplan.top

[B09] break 与 continue
来源：http://uoa.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vgw.zhixingplan.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gnw.zhaomingkeji.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cov.yj202588.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zst.zhijiandao.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ouc.fanxiaobao.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yhf.jinyuanbaomall.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://waj.52xcode.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uxk.daria6918.cn

[B10] 遍历同时拿索引
来源：http://bwq.c1oappe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fbp.shanyushiyangtech.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ayx.fehbvm.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://voc.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fyi.hywenlv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://unr.hongshengwenyu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cnq.fehbvm.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wkk.jqgfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ehd.yj20258.top

[B11] 生成数字序列 / 区间
来源：http://wak.jiagoushi.top

Py:   list(range(0, 10, 2))
来源：http://pdg.zhongyouzk.top

PHP:  range(0, 10, 2);
来源：http://cci.yueranfly.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oti.xuanzx.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tzf.daria6918.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zis.fengsongda.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ati.zhengqikj.top

Ruby: (0...10).step(2).to_a
来源：http://wqz.bbcook.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yfb.zycfv.cn

[B12] 跳出多层循环
来源：http://xji.cashguo.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dmr.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mzk.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pow.haohaochexian.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ykl.zhixingplan.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ebn.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sci.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://okm.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sap.jinqigufen.top

[B13] 判断是否为数字
来源：http://saf.tarul.cn

Py:   isinstance(x, (int, float))
来源：http://saj.tianlin.xyz

PHP:  is_numeric($x)
来源：http://uvv.fanxiaobao.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iac.redwolf501.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gzy.wangshuangyany.cn

Java: x instanceof Number
来源：http://log.shzxlz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vwv.nanxinkj.top

Ruby: x.is_a?(Numeric)
来源：http://liz.yuanzhike.top

C#:   x is int or double or decimal
来源：http://lmo.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://aal.fengsongda.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tso.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://foq.sysykeji.top

JS:   [1, 2, 3].includes(x)
来源：http://ras.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://rjr.shangyingyoupin.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ksr.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ogp.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://viv.yvedp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hox.daria6918.cn

[B15] 布尔运算与取反
来源：http://rem.jianghu66.top

Py:   a and b or not c
来源：http://ehb.9152youxi.cn

PHP:  $a && $b || !$c
来源：http://mkh.zdbjq.cn

JS:   a && b || !c
来源：http://eto.aizwys.cn

TS:   a && b || !c
来源：http://ddt.zdqjudy.top

Java: a && b || !c
来源：http://rka.ydzc1.top

Go:   a && b || !c
来源：http://ufk.mhx1999.top

Ruby: a && b || !c
来源：http://clx.pycfn.com

C#:   a && b || !c
来源：http://jkq.nanxinkj.top

[B16] 卫语句：不满足条件提前返回
来源：http://otd.sxryk.cn

Py:   if not data: return
来源：http://emm.316326.xyz

PHP:  if (!$data) { return; }
来源：http://pjt.xziqi.cn

JS:   if (!data) return;
来源：http://unw.jyoumei.cn

TS:   if (!data) return;
来源：http://fua.zhaomingkeji.xyz

Java: if (data == null) return;
来源：http://xrp.yj20258.top

Go:   if data == nil { return }
来源：http://heu.aibaodan.cn

Ruby: return if data.nil?
来源：http://sxs.sjlbkw.cn

C#:   if (data == null) return;
来源：http://yjp.fzhhl.top

================================================================================
来源：http://itc.aibaodan.cn

C. 函数与作用域
来源：http://vkc.zhengqikj.top

================================================================================
来源：http://moj.daria6918.cn

[C01] 定义函数
来源：http://jzy.yj202588.top

Py:   def add(a, b): return a + b
来源：http://kbj.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tck.pycfn.com

JS:   function add(a, b) { return a + b; }
来源：http://xsy.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://njs.bjfxy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ict.chenlongwang.top

Go:   func add(a, b int) int { return a + b }
来源：http://rkm.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://vyv.cashguo.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://reu.zhixingplan.top

[C02] 默认参数
来源：http://vjp.epnwcf.com

Py:   def greet(name="World"): return name
来源：http://npk.meibo888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gqq.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://sik.bbcook.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dfe.hesvh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fmb.pycfn.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rqm.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://ntk.havefunace.top

C#:   string Greet(string name = "World") => name;
来源：http://ubb.mhx1999.top

[C03] 可变参数
来源：http://ghy.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://exk.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qom.ybcxt.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rcy.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lhg.sjlbkw.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jjl.sweek.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ljg.yj20258888.top

Ruby: def total(*nums); nums.sum; end
来源：http://czx.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mrg.shzxlz.cn

[C04] 命名参数 / 关键字参数
来源：http://xfo.quarkkingdee.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pzm.zdqjudy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kha.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jij.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://son.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://opi.jqgfzy.top

Go:   // 无：用配置结构体参数
来源：http://miv.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://ais.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://mgb.zhiwuduotai.top

[C05] 返回多个值
来源：http://ypf.xziqi.cn

Py:   return a, b
来源：http://ebi.hammf.cn

PHP:  return [$a, $b];
来源：http://pdz.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hbt.hnxiangtu.top

TS:   return { a, b };
来源：http://xdh.bbcook.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zfh.xuanzx.com

Go:   return a, b
来源：http://vsq.cqqwz.cn

Ruby: return a, b
来源：http://pwy.zhaomingkeji.xyz

C#:   return (a, b);              // ValueTuple
来源：http://btm.aizwys.cn

[C06] 匿名函数 / lambda
来源：http://zxg.havefunace.top

Py:   square = lambda x: x * x
来源：http://ppg.yj20258888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cds.jinqigfzy.top

JS:   const square = x => x * x;
来源：http://ndc.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://cgr.feifeiyinyue.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tdw.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://wpd.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://wer.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://qcj.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://hna.gaohongyu789.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://stb.ydjk.org.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hrj.xingfuxueyuan.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nsk.sufxvd.cn

TS:   arr.map(String)
来源：http://spp.chenjidiqi.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zua.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jxd.kuanghao11.cn

Ruby: arr.map(&:upcase)
来源：http://odk.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://llz.xylfe.cn

[C08] 闭包
来源：http://jbo.zhijiandao.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mnx.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://czp.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cvo.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qre.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nwv.fengsongda.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ngg.gogol.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pny.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://avg.shangyingyoupin.top

[C09] 递归
来源：http://lrh.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vom.hysaishi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://udp.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zla.jianghu66.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jqt.yfazqb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://edx.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pzj.sweek.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uhy.shanyushiyangtech.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ajy.guannengcc.top


<!-- 参考信息 -->