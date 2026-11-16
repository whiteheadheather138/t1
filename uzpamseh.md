代发 wailian999

JS:   [a, b] = [b, a];
来源：http://ihf.52xcode.cn

TS:   [a, b] = [b, a];
来源：http://not.chenzaomai.com

Java: int t = a; a = b; b = t;
来源：http://lbw.svipenyu.cn

Go:   a, b = b, a
来源：http://nmi.kuanghao11.cn

Ruby: a, b = b, a
来源：http://xhu.0kj1m.cn

C#:   (a, b) = (b, a);
来源：http://gny.tarul.cn

[A20] 读取标准输入
来源：http://rwc.haohaochexian.top

Py:   name = input("请输入：")
来源：http://wdu.dashuyun.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hpv.havefunace.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://trm.yongpay.top

TS:   // Node.js：readline 模块
来源：http://pmq.xuanzx.com

Java: new Scanner(System.in).nextLine()
来源：http://krs.nanxinkj.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lgs.jinqigufen.top

Ruby: gets.chomp
来源：http://udd.jianghu66.top

C#:   Console.ReadLine();
来源：http://hin.yuxming.cn

[A21] 保留指定小数位输出
来源：http://ugo.shzxlz.cn

Py:   f"{3.14159:.2f}"
来源：http://qcs.jinqigfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wnt.fzhhl.top

JS:   (3.14159).toFixed(2)
来源：http://ykb.yj20258.top

TS:   (3.14159).toFixed(2)
来源：http://iqy.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://ind.tanke756.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pjb.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://wpt.jinqigufen.top

C#:   3.14159.ToString("F2")
来源：http://dzz.gotoacloud.top

[A22] 获取字符串长度
来源：http://dgq.ctjpmb.com

Py:   len(s)
来源：http://vcd.shanyushiyangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://raf.zdbjq.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wqk.xinyue.icu

TS:   s.length
来源：http://kqn.guowangkeji.top

Java: s.length()
来源：http://jnx.gaohongyu789.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://arq.birdmap.top

Ruby: s.length
来源：http://qnn.hysaishi.cn

C#:   s.Length
来源：http://zaw.jqgufenzy.top

[A23] 大小写转换
来源：http://vlw.jinqigfzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lcy.fzhhl.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aoo.hnxiangtu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wvr.sufxvd.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wuw.epnwcf.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wqd.xylfe.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sei.hnqzz.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cko.nanxinkj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://als.hnxiangtu.top

[A24] 去除首尾空白
来源：http://kah.jinyuanbaomall.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ige.kuanghao11.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sjz.uphjek.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fet.hammf.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kkb.ydzc1.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hxe.uphjek.com

Go:   strings.TrimSpace(s)
来源：http://aku.jlsjyb.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mka.guowangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dlx.ivvv.top

[A25] 字符串比较
来源：http://aoo.wangdashe.top

Py:   s1 == s2; s1 != s2
来源：http://zia.9152youxi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pbw.daria6918.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qum.nwbrower.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://stg.jyoumei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://btg.yj20258.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nqj.daxiang520.top

Ruby: s1 == s2; s1 <=> s2
来源：http://igo.jlsjyb.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iur.yanxiufei.cn

[A26] 类型转换总览
来源：http://juk.yanxiufei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hfr.vqdsnc.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jfd.zhiwuduotai.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hqt.xuetiantiany.cn

TS:   Number() String() Boolean() x as number
来源：http://ytx.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rsq.pengpengdd.cyou

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qtr.haohaochexian.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zma.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://udf.fanxiaobao.xyz

================================================================================
来源：http://oui.daxiang520.top

B. 流程控制
来源：http://arl.jqgfzy.top

================================================================================
来源：http://zcn.ybcxt.top

[B01] 条件判断 if / else
来源：http://pgd.dianchejie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gcb.zdbjq.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ify.nanxuanxn.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fbh.zhiwuduotai.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xjo.cqqwz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://shx.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lni.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cxl.0kj1m.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cbb.cheryme.top

[B02] 多分支 else if / elif
来源：http://ebv.zhijiandao.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zoh.kuanghao11.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ukc.pengpengdd.cyou

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hez.nwbrower.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lkf.yj20258888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qos.shanyushiyangtech.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tlq.fzhhl.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vzv.jiagoushi.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://smc.cheryme.top

[B03] switch / match / case
来源：http://msj.zdqjudy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://utz.xuanzx.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wsk.nanxinkj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rnh.jlsjyb.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ibq.gotoacloud.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mbx.cheryme.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oti.yueranfly.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uez.ybcxt.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kde.xuanzx.com

[B04] for 计数循环
来源：http://vti.yj202588.top

Py:   for i in range(10): print(i)
来源：http://wtx.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tsc.aizwys.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dih.zhixingplan.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://phe.tarul.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://azc.zdbjq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lrh.cashguo.top

Ruby: 10.times { |i| puts i }
来源：http://inf.nanxinkj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oif.zdbjq.cn

[B05] 遍历数组 / 列表
来源：http://yhy.cucudq.cn

Py:   for item in arr: print(item)
来源：http://pvl.birdmap.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bkj.pengpengdd.cyou

JS:   for (const item of arr) { console.log(item); }
来源：http://zkg.kuanghao11.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://knf.jinyuanbaomall.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zpq.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mmr.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://gyb.zhoulong.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rsl.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://qfa.daria6918.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hmk.zhixingplan.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tga.cdnleiting.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qcj.hywenlv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mcw.jianghu66.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qhz.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://urd.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pal.sweek.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://csv.tanke756.top

[B07] while 循环
来源：http://fxb.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://sds.zhengqikj.top

PHP:  while ($i < 10) { $i++; }
来源：http://fvp.hysaishi.cn

JS:   while (i < 10) { i++; }
来源：http://epv.zhixingplan.top

TS:   while (i < 10) { i++; }
来源：http://ssg.jinqigfzy.top

Java: while (i < 10) { i++; }
来源：http://nrw.iojbl.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zfq.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://dcw.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://jhn.vqdsnc.cn

[B08] do-while（至少执行一次）
来源：http://zoe.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://uhq.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://urc.svipenyu.cn

JS:   do { i++; } while (i < 10);
来源：http://gwz.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://kfp.sweek.top

Java: do { i++; } while (i < 10);
来源：http://bzc.nwbrower.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mta.yj20258.top

Ruby: begin; i += 1; end while i < 10
来源：http://ygq.ctjpmb.com

C#:   do { i++; } while (i < 10);
来源：http://nat.sjlbkw.cn

[B09] break 与 continue
来源：http://sev.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://khp.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eep.xuetiantiany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zjm.ybcxt.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fgn.xziqi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lsn.shanyushiyangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eou.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bda.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ykb.fktsv.cn

[B10] 遍历同时拿索引
来源：http://acz.hammf.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ewx.xinyue.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ewe.vehdjk.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vdt.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mkw.sufxvd.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sjp.xuetiantiany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jnb.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fyt.chenlongwang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rek.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://idf.zhoulong.xyz

Py:   list(range(0, 10, 2))
来源：http://gcd.havefunace.top

PHP:  range(0, 10, 2);
来源：http://xyt.hysaishi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xxq.0kj1m.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aht.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tih.daria6918.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lab.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://mhf.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mwy.dashuyun.cn

[B12] 跳出多层循环
来源：http://ybz.aibaodan.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wea.sweek.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kgn.quarkkingdee.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mia.cashguo.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wkb.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xav.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://inb.svipenyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kbi.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cpa.shanyushiyangtech.top

[B13] 判断是否为数字
来源：http://nor.yuanzhike.top

Py:   isinstance(x, (int, float))
来源：http://afx.andypj.xyz

PHP:  is_numeric($x)
来源：http://ori.cheryme.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jcx.jqgfzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iuv.fengsongda.top

Java: x instanceof Number
来源：http://sco.yvedp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zgr.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://wji.zhengqikj.top

C#:   x is int or double or decimal
来源：http://bqq.shanyushiyangkeji.top

[B14] 判断值是否在集合内
来源：http://sir.zhengqikj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hmo.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mvn.jinghuilouyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://fgz.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://due.meibo888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jnx.ctjpmb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bwt.svipenyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://epd.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zop.hesvh.cn

[B15] 布尔运算与取反
来源：http://xkv.hongshengwenyu.top

Py:   a and b or not c
来源：http://dkx.hywenlv.cn

PHP:  $a && $b || !$c
来源：http://tbc.yanxiufei.cn

JS:   a && b || !c
来源：http://rae.xziqi.cn

TS:   a && b || !c
来源：http://meg.andypj.xyz

Java: a && b || !c
来源：http://lmc.uphjek.com

Go:   a && b || !c
来源：http://zjt.tarul.cn

Ruby: a && b || !c
来源：http://vvg.kuanghao11.cn

C#:   a && b || !c
来源：http://trs.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://whi.havefunace.top

Py:   if not data: return
来源：http://scf.yueranfly.top

PHP:  if (!$data) { return; }
来源：http://coh.tarul.cn

JS:   if (!data) return;
来源：http://xkf.xylfe.cn

TS:   if (!data) return;
来源：http://nvx.epnwcf.com

Java: if (data == null) return;
来源：http://hvz.daria6918.cn

Go:   if data == nil { return }
来源：http://nxt.ydjk.org.cn

Ruby: return if data.nil?
来源：http://glz.yj202588.top

C#:   if (data == null) return;
来源：http://oxx.daxiang520.top

================================================================================
来源：http://hdq.jqgufenzy.top

C. 函数与作用域
来源：http://bvo.pycfn.com

================================================================================
来源：http://thv.hnxiangtu.top

[C01] 定义函数
来源：http://ydh.meibo888.top

Py:   def add(a, b): return a + b
来源：http://zoi.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://omw.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://xbp.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mnl.yangfankeji.com

Java: static int add(int a, int b) { return a + b; }
来源：http://nzu.hysaishi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pkk.svipenyu.cn

Ruby: def add(a, b); a + b; end
来源：http://bpx.fktsv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ezf.yangfankeji.com

[C02] 默认参数
来源：http://nep.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://xnp.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tdp.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://jmt.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jxt.zhixingplan.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wbw.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ybc.ydzc1.top

Ruby: def greet(name = "World") = name
来源：http://frr.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://sam.birdmap.top

[C03] 可变参数
来源：http://wbf.yj20258.top

Py:   def total(*args): return sum(args)
来源：http://fej.yongpay.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hza.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yfm.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pzm.wangdashe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://plp.daxiang520.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oei.shanyushiyangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://mjx.bjfxy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gpi.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://gsi.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zvy.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jap.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bcz.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://drf.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://xaj.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://yis.jianghu66.top

Ruby: f(a: 1, b: 2)
来源：http://zpi.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://kio.tianlin.xyz

[C05] 返回多个值
来源：http://oei.tarul.cn

Py:   return a, b
来源：http://vgx.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://qkq.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://lpb.c1oappe.top

TS:   return { a, b };
来源：http://qaj.jlsjyb.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pcm.yangfankeji.com

Go:   return a, b
来源：http://qxx.zhongyouzk.top

Ruby: return a, b
来源：http://hnx.iojbl.cn

C#:   return (a, b);              // ValueTuple
来源：http://mah.birdmap.top

[C06] 匿名函数 / lambda
来源：http://lqf.hammf.cn

Py:   square = lambda x: x * x
来源：http://dop.guowangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xdu.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://qdf.jqgufenzy.top

TS:   const square = (x: number): number => x * x;
来源：http://atl.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cnf.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://ubk.xylfe.cn

Ruby: square = ->(x) { x * x }
来源：http://oat.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://fsm.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://pvw.hnxiangtu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tbj.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://rqt.yanxiufei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oof.tianlin.xyz

TS:   arr.map(String)
来源：http://wdc.meibo888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ujs.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ciq.hywenlv.cn

Ruby: arr.map(&:upcase)
来源：http://jqr.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ooc.hnqzz.top

[C08] 闭包
来源：http://ptq.zycfv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lob.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://euh.guowangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mqk.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://omk.xinyue.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jxs.jqgfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mwf.jianghu66.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qub.pycfn.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kbp.xziqi.cn

[C09] 递归
来源：http://xor.andypj.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vwd.fanxiaobao.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zpp.ydzc1.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eja.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fhp.sweek.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hqm.epnwcf.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://frf.gotoacloud.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nhc.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ihn.gotoacloud.top


<!-- 参考信息 -->