代发 wailian999

JS:   [a, b] = [b, a];
来源：http://drh.hywenlv.cn

TS:   [a, b] = [b, a];
来源：http://nou.tianlin.xyz

Java: int t = a; a = b; b = t;
来源：http://wyx.fengsongda.top

Go:   a, b = b, a
来源：http://coz.iojbl.cn

Ruby: a, b = b, a
来源：http://zgn.ivvv.top

C#:   (a, b) = (b, a);
来源：http://fav.cqqwz.cn

[A20] 读取标准输入
来源：http://tcr.zycfv.cn

Py:   name = input("请输入：")
来源：http://lew.zhengqikj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://nol.fzhhl.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pah.hammf.cn

TS:   // Node.js：readline 模块
来源：http://mcr.cqqwz.cn

Java: new Scanner(System.in).nextLine()
来源：http://dva.xylfe.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bza.vqdsnc.cn

Ruby: gets.chomp
来源：http://sqr.yj20258888.top

C#:   Console.ReadLine();
来源：http://bag.fanxiaobao.xyz

[A21] 保留指定小数位输出
来源：http://qqo.zhengqikj.top

Py:   f"{3.14159:.2f}"
来源：http://qrg.jianghu66.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vot.aizwys.cn

JS:   (3.14159).toFixed(2)
来源：http://jmh.ydjk.org.cn

TS:   (3.14159).toFixed(2)
来源：http://wbr.xuanzx.com

Java: String.format("%.2f", 3.14159)
来源：http://xhp.hongshengwenyu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xjf.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://ypg.sxryk.cn

C#:   3.14159.ToString("F2")
来源：http://ire.yj20258888.top

[A22] 获取字符串长度
来源：http://ity.zhijiandao.cn

Py:   len(s)
来源：http://nek.jinyuanbaomall.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iun.yvedp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zgn.hesvh.cn

TS:   s.length
来源：http://vfs.aizwys.cn

Java: s.length()
来源：http://uxw.xziqi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://luh.feifeiyinyue.top

Ruby: s.length
来源：http://mpj.sxryk.cn

C#:   s.Length
来源：http://ezt.wangshuangyany.cn

[A23] 大小写转换
来源：http://lfr.ehwqpu.com

Py:   s.upper(); s.lower(); s.title()
来源：http://zui.0kj1m.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qen.birdmap.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rla.dianchejie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tuu.xuanzx.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nxh.ehwqpu.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://piu.ydjk.org.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uua.ppjwa.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kyv.sysykeji.top

[A24] 去除首尾空白
来源：http://khs.tianlin.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eye.zhiwuduotai.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zub.bjfxy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uaw.ydzc1.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tek.chenjidiqi.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tku.nanxinkj.top

Go:   strings.TrimSpace(s)
来源：http://nzg.pengpengdd.cyou

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://txe.mhx1999.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://heo.fanxiaobao.xyz

[A25] 字符串比较
来源：http://ztg.hongshengwenyu.top

Py:   s1 == s2; s1 != s2
来源：http://ewt.xuanzx.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zsh.tanke756.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://alb.9152youxi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ngu.cucudq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kvd.ybcxt.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qkp.hnxiangtu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://khx.ybcxt.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yqq.andypj.xyz

[A26] 类型转换总览
来源：http://opp.mhx1999.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://scg.jqgufenzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sih.dashuyun.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kom.jinghuilouyu.cn

TS:   Number() String() Boolean() x as number
来源：http://euk.gzhubu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qqr.xuetiantiany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kxf.xingfuxueyuan.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://nmf.dianchejie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bra.yuanzhike.top

================================================================================
来源：http://rbv.hnqzz.top

B. 流程控制
来源：http://zeh.zhijiandao.cn

================================================================================
来源：http://psc.chenjidiqi.icu

[B01] 条件判断 if / else
来源：http://bgn.hnqzz.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tbj.feifeiyinyue.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ivp.yfazqb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ktg.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gky.9152youxi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://swp.jiagoushi.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://slj.zycfv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hfa.sysykeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fcq.yvedp.cn

[B02] 多分支 else if / elif
来源：http://xzj.shangyingyoupin.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wlu.tian-w.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pxd.svipenyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hbl.cashguo.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pom.ydzc1.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pmk.mhx1999.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jjq.52xcode.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kom.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbe.cdnleiting.top

[B03] switch / match / case
来源：http://auf.cheryme.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nge.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xhl.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hci.pycfn.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ecn.redwolf501.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gjw.vehdjk.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://axm.chenlongwang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rpq.jinqigfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wlg.shuidangran.top

[B04] for 计数循环
来源：http://dyr.pengpengdd.cyou

Py:   for i in range(10): print(i)
来源：http://xmn.kuanghao11.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nmo.havefunace.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lju.ivvv.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zrm.hongshengwenyu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mzi.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tcv.jyoumei.cn

Ruby: 10.times { |i| puts i }
来源：http://lqe.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zyl.shanyushiyangtech.top

[B05] 遍历数组 / 列表
来源：http://ecz.ehwqpu.com

Py:   for item in arr: print(item)
来源：http://ifv.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kzm.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rcn.nanxuanxn.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kiu.gaohongyu789.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vqt.daria6918.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mot.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://qwx.zdqjudy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ihf.xinyue.icu

[B06] 遍历字典 / 对象
来源：http://khu.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://upr.xylfe.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dhc.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tpd.chenlongwang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qdf.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nes.jqgfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kls.tianlin.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ena.nwbrower.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oyh.hfpthk.cn

[B07] while 循环
来源：http://dsv.iojbl.cn

Py:   while i < 10: i += 1
来源：http://mox.wangdashe.top

PHP:  while ($i < 10) { $i++; }
来源：http://shs.meibo888.top

JS:   while (i < 10) { i++; }
来源：http://qzl.sxryk.cn

TS:   while (i < 10) { i++; }
来源：http://rcg.pycfn.com

Java: while (i < 10) { i++; }
来源：http://xbx.ywan-chungtsiang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zya.fktsv.cn

Ruby: while i < 10; i += 1; end
来源：http://ygx.jianghu66.top

C#:   while (i < 10) { i++; }
来源：http://gsc.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://tje.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://krs.jinyuanbaomall.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jwn.meibo888.top

JS:   do { i++; } while (i < 10);
来源：http://xev.jinyuanbaomall.cn

TS:   do { i++; } while (i < 10);
来源：http://nqr.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://fut.xinyue.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://pae.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://tfa.ybcxt.top

C#:   do { i++; } while (i < 10);
来源：http://tcj.ivvv.top

[B09] break 与 continue
来源：http://enw.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jbm.wangshuangyany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qic.ybcxt.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jvp.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bmz.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hnu.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rvv.smart0.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sap.shzxlz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kba.fehbvm.com

[B10] 遍历同时拿索引
来源：http://jrc.xingfuxueyuan.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cwp.zhijiandao.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nca.sufxvd.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yqg.bbcook.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xzz.daria6918.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lmb.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xlo.xuetiantiany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qmo.hammf.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vgx.zhijiandao.cn

[B11] 生成数字序列 / 区间
来源：http://krw.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://bwf.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://isf.sysykeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kwb.fzhhl.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sze.jinqigfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wkd.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xkv.chenlongwang.top

Ruby: (0...10).step(2).to_a
来源：http://rqk.yonumen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uwq.aibaodan.cn

[B12] 跳出多层循环
来源：http://nfo.yvedp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xxz.haohaochexian.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://seq.zhoulong.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jge.yvedp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rwp.yfazqb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yji.gogol.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tax.bbcook.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vli.shangyingyoupin.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hje.hysaishi.cn

[B13] 判断是否为数字
来源：http://axx.smart0.xyz

Py:   isinstance(x, (int, float))
来源：http://vje.havefunace.top

PHP:  is_numeric($x)
来源：http://vjg.wangshuangyany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://smi.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://djd.jiagoushi.top

Java: x instanceof Number
来源：http://fvr.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ajc.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://nmw.cqqwz.cn

C#:   x is int or double or decimal
来源：http://zcd.dianchejie.cn

[B14] 判断值是否在集合内
来源：http://pno.shanyushiyangtech.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://phe.316326.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ymk.zhixingplan.top

JS:   [1, 2, 3].includes(x)
来源：http://ygw.jianghu66.top

TS:   [1, 2, 3].includes(x)
来源：http://ool.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://iwu.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gyd.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ymu.zycfv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pvg.zhoulong.xyz

[B15] 布尔运算与取反
来源：http://njg.c1oappe.top

Py:   a and b or not c
来源：http://sun.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://lmj.svipenyu.cn

JS:   a && b || !c
来源：http://wov.jinqigufen.top

TS:   a && b || !c
来源：http://evi.tianlin.xyz

Java: a && b || !c
来源：http://eln.shanyushiyangtech.top

Go:   a && b || !c
来源：http://wer.yanxiufei.cn

Ruby: a && b || !c
来源：http://awc.epnwcf.com

C#:   a && b || !c
来源：http://orw.shanyushiyangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://neh.yj20258888.top

Py:   if not data: return
来源：http://avk.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://ifh.c1oappe.top

JS:   if (!data) return;
来源：http://uct.yuxming.cn

TS:   if (!data) return;
来源：http://dvm.dashuyun.cn

Java: if (data == null) return;
来源：http://sio.ivvv.top

Go:   if data == nil { return }
来源：http://fep.zdqjudy.top

Ruby: return if data.nil?
来源：http://tsw.bbcook.cn

C#:   if (data == null) return;
来源：http://lnq.jqgfzy.top

================================================================================
来源：http://eko.smart0.xyz

C. 函数与作用域
来源：http://uvp.jianghu66.top

================================================================================
来源：http://lcw.jiagoushi.top

[C01] 定义函数
来源：http://dly.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://jaq.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://prf.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://ocs.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pbz.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lsi.fengsongda.top

Go:   func add(a, b int) int { return a + b }
来源：http://ihk.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://nhh.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vlh.jlsjyb.cn

[C02] 默认参数
来源：http://ggk.yangfankeji.com

Py:   def greet(name="World"): return name
来源：http://zhm.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mxv.yueranfly.top

JS:   function greet(name = "World") { return name; }
来源：http://wxu.gzhubu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ats.yangfankeji.com

Java: // 无默认参数：方法重载或 Optional
来源：http://mxe.ivvv.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cax.shanyushiyangtech.top

Ruby: def greet(name = "World") = name
来源：http://bjt.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://qef.0kj1m.cn

[C03] 可变参数
来源：http://txk.cqqwz.cn

Py:   def total(*args): return sum(args)
来源：http://pxk.shanyushiyangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yau.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fee.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://stp.wangdashe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gjd.ybcxt.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rvc.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://oha.sxryk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://krr.smart0.xyz

[C04] 命名参数 / 关键字参数
来源：http://hkp.hywenlv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lwk.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mld.cucudq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nxm.cqqwz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mul.zdbjq.cn

Java: // 无：用 Builder 模式或 record
来源：http://myc.cashguo.top

Go:   // 无：用配置结构体参数
来源：http://cdo.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://byq.gogol.net.cn

C#:   f(a: 1, b: 2)
来源：http://vui.andypj.xyz

[C05] 返回多个值
来源：http://hli.fengsongda.top

Py:   return a, b
来源：http://sly.daria6918.cn

PHP:  return [$a, $b];
来源：http://fuf.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ixn.zhengqikj.top

TS:   return { a, b };
来源：http://tzo.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yil.52xcode.cn

Go:   return a, b
来源：http://oky.pycfn.com

Ruby: return a, b
来源：http://xub.hnqzz.top

C#:   return (a, b);              // ValueTuple
来源：http://hel.yonumen.top

[C06] 匿名函数 / lambda
来源：http://dbc.xuetiantiany.cn

Py:   square = lambda x: x * x
来源：http://izg.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cvi.jinqigfzy.top

JS:   const square = x => x * x;
来源：http://hrg.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://ikx.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bla.hfpthk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fdm.zycfv.cn

Ruby: square = ->(x) { x * x }
来源：http://zpv.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://can.cucudq.cn

[C07] 把函数作为参数传入
来源：http://hll.guannengcc.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lnd.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://lsd.yonumen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xdh.yuxming.cn

TS:   arr.map(String)
来源：http://pjs.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uju.cucudq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://btq.pengpengdd.cyou

Ruby: arr.map(&:upcase)
来源：http://wtv.bbcook.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fxp.mhx1999.top

[C08] 闭包
来源：http://zgp.vehdjk.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ebn.shanyushiyangtech.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zhe.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mhc.jqgfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zyy.chenzaomai.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xmw.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dho.zdqjudy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kyh.ydjk.org.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zme.aibaodan.cn

[C09] 递归
来源：http://qwh.ybcxt.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vac.yj20258.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hui.yonumen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rtr.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ofo.zdbjq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bpx.ehwqpu.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://agc.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jsm.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vtm.snrcjt.cn


<!-- 参考信息 -->