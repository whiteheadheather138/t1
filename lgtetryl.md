代发 wailian999

JS:   [a, b] = [b, a];
来源：http://aon.jianghu66.top

TS:   [a, b] = [b, a];
来源：http://trl.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://izu.jinqigfzy.top

Go:   a, b = b, a
来源：http://qdi.chenjidiqi.icu

Ruby: a, b = b, a
来源：http://bch.yfazqb.com

C#:   (a, b) = (b, a);
来源：http://ftb.svipenyu.cn

[A20] 读取标准输入
来源：http://kbv.gotoacloud.top

Py:   name = input("请输入：")
来源：http://miq.yj202588.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kij.sxryk.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ynn.c1oappe.top

TS:   // Node.js：readline 模块
来源：http://eku.yueranfly.top

Java: new Scanner(System.in).nextLine()
来源：http://ocr.bjfxy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lfz.jiagoushi.top

Ruby: gets.chomp
来源：http://dwp.havefunace.top

C#:   Console.ReadLine();
来源：http://zvp.ctjpmb.com

[A21] 保留指定小数位输出
来源：http://oif.dashuyun.cn

Py:   f"{3.14159:.2f}"
来源：http://rhe.nanxinkj.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tbf.jianghu66.top

JS:   (3.14159).toFixed(2)
来源：http://tju.xuetiantiany.cn

TS:   (3.14159).toFixed(2)
来源：http://fay.yj20258888.top

Java: String.format("%.2f", 3.14159)
来源：http://opg.jinqigufen.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sjt.yj20258888.top

Ruby: format("%.2f", 3.14159)
来源：http://kpq.yj20258.top

C#:   3.14159.ToString("F2")
来源：http://rov.zhengqikj.top

[A22] 获取字符串长度
来源：http://krv.hfpthk.cn

Py:   len(s)
来源：http://lrn.fanxiaobao.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://txh.zhixingplan.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qsk.yj20258888.top

TS:   s.length
来源：http://bib.zhoulong.xyz

Java: s.length()
来源：http://fek.gaohongyu789.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kcl.wangdashe.top

Ruby: s.length
来源：http://ujq.xinyue.icu

C#:   s.Length
来源：http://fuh.ydzc1.top

[A23] 大小写转换
来源：http://wnb.zhaomingkeji.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://tiv.yangfankeji.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hbq.bjfxy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tdn.cucudq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tqi.iojbl.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yac.birdmap.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wzx.birdmap.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dkd.feifeiyinyue.top

C#:   s.ToUpper(); s.ToLower()
来源：http://tuh.yuanzhike.top

[A24] 去除首尾空白
来源：http://jox.daxiang520.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://car.hnqzz.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gkr.9152youxi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vpx.quarkkingdee.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rvb.yj20258.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hrw.yj20258.top

Go:   strings.TrimSpace(s)
来源：http://eci.aibaodan.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ozi.yj202588.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bcw.aizwys.cn

[A25] 字符串比较
来源：http://yem.yj202588.top

Py:   s1 == s2; s1 != s2
来源：http://jmb.jinyuanbaomall.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ian.cdnleiting.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ytn.yangfankeji.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zgl.gotoacloud.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rue.vehdjk.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lva.redwolf501.top

Ruby: s1 == s2; s1 <=> s2
来源：http://oed.jinqigufen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dcz.cashguo.top

[A26] 类型转换总览
来源：http://sbh.xziqi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dhm.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vhr.yongpay.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ywp.chenlongwang.top

TS:   Number() String() Boolean() x as number
来源：http://kpy.jqgfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tgc.zhongyouzk.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://syn.yonumen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kwi.tanke756.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fvk.iojbl.cn

================================================================================
来源：http://biv.gaohongyu789.top

B. 流程控制
来源：http://esm.zycfv.cn

================================================================================
来源：http://szo.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://lqe.jlsjyb.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nxh.sysykeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tzk.cashguo.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zdv.nanxinkj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gbr.hesvh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://awm.ppjwa.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jpw.xylfe.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gft.epnwcf.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cpl.yonumen.top

[B02] 多分支 else if / elif
来源：http://uec.fktsv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ymt.jinghuilouyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gem.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pbh.gogol.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wgu.hcnkem.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lpa.snrcjt.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pfx.gaohongyu789.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ejb.vehdjk.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fkx.havefunace.top

[B03] switch / match / case
来源：http://hwr.vqdsnc.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vpf.daria6918.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sel.yj20258888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tqr.sweek.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bik.redwolf501.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lit.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://byr.zycfv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pet.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eum.shuidangran.top

[B04] for 计数循环
来源：http://epl.tarul.cn

Py:   for i in range(10): print(i)
来源：http://pmt.c1oappe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ixc.xziqi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lug.pengpengdd.cyou

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hwi.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://clg.hfpthk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xga.hywenlv.cn

Ruby: 10.times { |i| puts i }
来源：http://ngh.yj20258888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uvl.zycfv.cn

[B05] 遍历数组 / 列表
来源：http://rim.xuetiantiany.cn

Py:   for item in arr: print(item)
来源：http://xdk.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xko.andypj.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://uwa.9152youxi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://udc.ppjwa.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pvk.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vyr.sufxvd.cn

Ruby: arr.each { |item| puts item }
来源：http://fqg.smart0.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nch.hnxiangtu.top

[B06] 遍历字典 / 对象
来源：http://prz.shzxlz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mdt.yuanzhike.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ull.ivvv.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sug.sufxvd.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wdw.zycfv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rfu.sxryk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://elm.epnwcf.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://edu.aizwys.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vlc.daxiang520.top

[B07] while 循环
来源：http://ixw.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://rxt.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ava.zhijiandao.cn

JS:   while (i < 10) { i++; }
来源：http://tll.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://wpc.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://yxt.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ebl.shanyushiyangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://swq.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://ptz.xylfe.cn

[B08] do-while（至少执行一次）
来源：http://flp.yanxiufei.cn

Py:   # 无 do-while：用 while True + break
来源：http://jxz.ydzc1.top

PHP:  do { $i++; } while ($i < 10);
来源：http://suq.yj202588.top

JS:   do { i++; } while (i < 10);
来源：http://hfr.mhx1999.top

TS:   do { i++; } while (i < 10);
来源：http://scl.redwolf501.top

Java: do { i++; } while (i < 10);
来源：http://jln.zycfv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://upj.jinyuanbaomall.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vik.hammf.cn

C#:   do { i++; } while (i < 10);
来源：http://ahn.epnwcf.com

[B09] break 与 continue
来源：http://eaz.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tnt.haohaochexian.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://brh.xziqi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vam.jinyuanbaomall.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jqu.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://taw.9152youxi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hkz.pycfn.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gcl.aizwys.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dpe.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://lbe.hysaishi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xnp.nanxuanxn.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://exy.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kct.cdnleiting.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kuv.guannengcc.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://enr.vqdsnc.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lzm.yj202588.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pmf.vehdjk.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dcx.vehdjk.com

[B11] 生成数字序列 / 区间
来源：http://uka.uphjek.com

Py:   list(range(0, 10, 2))
来源：http://dak.9152youxi.cn

PHP:  range(0, 10, 2);
来源：http://hft.ehwqpu.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ewg.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://msd.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tsk.daxiang520.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://opq.hcnkem.com

Ruby: (0...10).step(2).to_a
来源：http://mvv.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pso.redwolf501.top

[B12] 跳出多层循环
来源：http://bbl.jlsjyb.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jps.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hfz.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fha.gaohongyu789.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qhe.hnxiangtu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tvi.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hlg.jinqigufen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wci.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nuz.zycfv.cn

[B13] 判断是否为数字
来源：http://vjn.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://fzf.cucudq.cn

PHP:  is_numeric($x)
来源：http://imy.shanyushiyangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hlo.smart0.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://whf.gaohongyu789.top

Java: x instanceof Number
来源：http://vrw.aizwys.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hyo.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://dqx.316326.xyz

C#:   x is int or double or decimal
来源：http://qwz.shuidangran.top

[B14] 判断值是否在集合内
来源：http://zwj.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hpf.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qkq.gzhubu.top

JS:   [1, 2, 3].includes(x)
来源：http://mkh.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://jdu.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://eeg.yanxiufei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hdd.epnwcf.com

Ruby: [1, 2, 3].include?(x)
来源：http://xqe.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wlb.fehbvm.com

[B15] 布尔运算与取反
来源：http://hyw.shuidangran.top

Py:   a and b or not c
来源：http://eym.sweek.top

PHP:  $a && $b || !$c
来源：http://hco.xuanzx.com

JS:   a && b || !c
来源：http://dun.chenlongwang.top

TS:   a && b || !c
来源：http://osd.zhiwuduotai.top

Java: a && b || !c
来源：http://xjq.haohaochexian.top

Go:   a && b || !c
来源：http://wpi.sufxvd.cn

Ruby: a && b || !c
来源：http://ouu.guowangkeji.top

C#:   a && b || !c
来源：http://hsd.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://lpw.jqgufenzy.top

Py:   if not data: return
来源：http://pkw.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://dkc.hfpthk.cn

JS:   if (!data) return;
来源：http://shq.chenjidiqi.icu

TS:   if (!data) return;
来源：http://nig.havefunace.top

Java: if (data == null) return;
来源：http://gks.jinghuilouyu.cn

Go:   if data == nil { return }
来源：http://mao.ywan-chungtsiang.top

Ruby: return if data.nil?
来源：http://yle.ehwqpu.com

C#:   if (data == null) return;
来源：http://xst.yuanzhike.top

================================================================================
来源：http://wqc.chenlongwang.top

C. 函数与作用域
来源：http://owp.xylfe.cn

================================================================================
来源：http://vcf.hcnkem.com

[C01] 定义函数
来源：http://yvs.gotoacloud.top

Py:   def add(a, b): return a + b
来源：http://qbf.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vkt.hfpthk.cn

JS:   function add(a, b) { return a + b; }
来源：http://txi.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://asx.9152youxi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hcp.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://ksg.guannengcc.top

Ruby: def add(a, b); a + b; end
来源：http://vip.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gwy.sjlbkw.cn

[C02] 默认参数
来源：http://hqq.sjlbkw.cn

Py:   def greet(name="World"): return name
来源：http://ttr.daxiang520.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xxt.jinghuilouyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://jor.hammf.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gcu.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zjm.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yya.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://ehg.ydjk.org.cn

C#:   string Greet(string name = "World") => name;
来源：http://fhc.jyoumei.cn

[C03] 可变参数
来源：http://ayr.chenjidiqi.icu

Py:   def total(*args): return sum(args)
来源：http://rwb.xingfuxueyuan.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hvr.zhaomingkeji.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gdu.jiagoushi.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nfo.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://urp.epnwcf.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zmz.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://dwk.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cno.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://udu.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://idn.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://abq.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://chv.52xcode.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://epg.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://icz.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://sbh.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://gkn.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://sgl.chenlongwang.top

[C05] 返回多个值
来源：http://aob.nanxuanxn.top

Py:   return a, b
来源：http://rio.yfazqb.com

PHP:  return [$a, $b];
来源：http://byz.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://vjj.jqgfzy.top

TS:   return { a, b };
来源：http://gdk.aizwys.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hywenlv.cn

Go:   return a, b
来源：http://nxh.yangfankeji.com

Ruby: return a, b
来源：http://lvx.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://wgn.hammf.cn

[C06] 匿名函数 / lambda
来源：http://zqo.shangyingyoupin.top

Py:   square = lambda x: x * x
来源：http://dvd.chenzaomai.com

PHP:  $square = fn($x) => $x * $x;
来源：http://hxo.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://wrw.nanxuanxn.top

TS:   const square = (x: number): number => x * x;
来源：http://sxt.tian-w.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dsr.chenjidiqi.icu

Go:   sq := func(x int) int { return x * x }
来源：http://gsp.ydzc1.top

Ruby: square = ->(x) { x * x }
来源：http://fio.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://oxz.gotoacloud.top

[C07] 把函数作为参数传入
来源：http://fec.guannengcc.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wqh.52xcode.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ism.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uri.svipenyu.cn

TS:   arr.map(String)
来源：http://bqq.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fae.mhx1999.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yzd.jqgufenzy.top

Ruby: arr.map(&:upcase)
来源：http://zbh.hongshengwenyu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vgp.sufxvd.cn

[C08] 闭包
来源：http://buk.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ama.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dzs.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qbf.fzhhl.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jqo.hfpthk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jhj.hnqzz.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ipf.zhongyouzk.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://svp.hesvh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rna.redwolf501.top

[C09] 递归
来源：http://bqo.meibo888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xar.sxryk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uvt.yueranfly.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xip.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pfb.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ptg.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bah.guowangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qgt.gogol.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lbk.hammf.cn


<!-- 参考信息 -->