代发 wailian999

Ruby: a, b = b, a
来源：http://rmd.tanke756.top

C#:   (a, b) = (b, a);
来源：http://auh.cheryme.top

[A20] 读取标准输入
来源：http://rmu.jyoumei.cn

Py:   name = input("请输入：")
来源：http://imn.shanyushiyangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://csq.jqgufenzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bsa.zycfv.cn

TS:   // Node.js：readline 模块
来源：http://ycn.fzhhl.top

Java: new Scanner(System.in).nextLine()
来源：http://yop.jinqigufen.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ump.daria6918.cn

Ruby: gets.chomp
来源：http://hfc.havefunace.top

C#:   Console.ReadLine();
来源：http://inn.yfazqb.com

[A21] 保留指定小数位输出
来源：http://zgs.tian-w.cn

Py:   f"{3.14159:.2f}"
来源：http://gkj.quarkkingdee.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pgd.ydjk.org.cn

JS:   (3.14159).toFixed(2)
来源：http://xvd.xuetiantiany.cn

TS:   (3.14159).toFixed(2)
来源：http://nou.fengsongda.top

Java: String.format("%.2f", 3.14159)
来源：http://con.cheryme.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tnx.yanxiufei.cn

Ruby: format("%.2f", 3.14159)
来源：http://szn.meibo888.top

C#:   3.14159.ToString("F2")
来源：http://txg.jiagoushi.top

[A22] 获取字符串长度
来源：http://yqk.jqgfzy.top

Py:   len(s)
来源：http://iwn.gotoacloud.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fmf.yangfankeji.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xiw.0kj1m.cn

TS:   s.length
来源：http://oxw.ydjk.org.cn

Java: s.length()
来源：http://hkr.yvedp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://psl.zycfv.cn

Ruby: s.length
来源：http://pfz.jianghu66.top

C#:   s.Length
来源：http://kaf.cqqwz.cn

[A23] 大小写转换
来源：http://xxa.zhixingplan.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kmc.shuidangran.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yqk.fengsongda.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kwd.chenlongwang.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oie.daxiang520.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://icl.cheryme.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://aff.zhixingplan.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fqz.zhongyouzk.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rzs.pengpengdd.cyou

[A24] 去除首尾空白
来源：http://gci.zhoulong.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://krc.nwbrower.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xbg.hcnkem.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ttv.tianlin.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lup.zhijiandao.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fhe.aizwys.cn

Go:   strings.TrimSpace(s)
来源：http://sgb.jqgufenzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://puh.ppjwa.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://trk.guannengcc.top

[A25] 字符串比较
来源：http://yoa.zhengqikj.top

Py:   s1 == s2; s1 != s2
来源：http://qtk.zhaomingkeji.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bxl.redwolf501.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://avo.sxryk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://inv.jinqigfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tib.bbcook.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hcb.yueranfly.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xkq.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nuz.cqqwz.cn

[A26] 类型转换总览
来源：http://jqh.nanxinkj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lit.yueranfly.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rig.zhoulong.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uot.aizwys.cn

TS:   Number() String() Boolean() x as number
来源：http://bbk.52xcode.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://udl.zhongyouzk.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jin.tanke756.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://msf.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kvz.tarul.cn

================================================================================
来源：http://obc.ctjpmb.com

B. 流程控制
来源：http://srs.cheryme.top

================================================================================
来源：http://cmx.tanke756.top

[B01] 条件判断 if / else
来源：http://umh.epnwcf.com

Py:   result = "正" if x > 0 else "非正"
来源：http://sws.epnwcf.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eox.yonumen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xme.ppjwa.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pqn.chenzaomai.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://cet.zhaomingkeji.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://unp.vqdsnc.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sgw.fehbvm.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ssh.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://lnq.ctjpmb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://loo.zdbjq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wpa.gaohongyu789.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://exe.yongpay.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rch.tanke756.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kwd.sufxvd.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gpk.gaohongyu789.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nrk.mhx1999.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yfo.tanke756.top

[B03] switch / match / case
来源：http://ttj.nanxinkj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ing.tianlin.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ojg.jinghuilouyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hcg.yj20258.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://twa.316326.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hjl.chenjidiqi.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ejn.cashguo.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ncy.shangyingyoupin.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xii.sjlbkw.cn

[B04] for 计数循环
来源：http://kew.birdmap.top

Py:   for i in range(10): print(i)
来源：http://uvk.aizwys.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://loq.zhoulong.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://foq.xuanzx.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jiy.redwolf501.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eji.iojbl.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zas.jyoumei.cn

Ruby: 10.times { |i| puts i }
来源：http://fos.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ppg.meibo888.top

[B05] 遍历数组 / 列表
来源：http://lde.mhx1999.top

Py:   for item in arr: print(item)
来源：http://mvf.jianghu66.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lru.316326.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://moq.shuidangran.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xhn.jlsjyb.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://swe.jlsjyb.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gss.sufxvd.cn

Ruby: arr.each { |item| puts item }
来源：http://amg.9152youxi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://akb.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://geo.cheryme.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nxd.yj202588.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nrv.yj20258.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hhm.cdnleiting.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://orl.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pvz.nanxinkj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ukm.kuanghao11.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tos.ehwqpu.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wez.316326.xyz

[B07] while 循环
来源：http://fbt.pycfn.com

Py:   while i < 10: i += 1
来源：http://rbs.tian-w.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mxy.xuetiantiany.cn

JS:   while (i < 10) { i++; }
来源：http://oig.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://bwu.zdbjq.cn

Java: while (i < 10) { i++; }
来源：http://del.iojbl.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vqb.hywenlv.cn

Ruby: while i < 10; i += 1; end
来源：http://met.hammf.cn

C#:   while (i < 10) { i++; }
来源：http://ecm.chenjidiqi.icu

[B08] do-while（至少执行一次）
来源：http://pqw.fanxiaobao.xyz

Py:   # 无 do-while：用 while True + break
来源：http://ucm.zhijiandao.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rly.zdbjq.cn

JS:   do { i++; } while (i < 10);
来源：http://yec.hammf.cn

TS:   do { i++; } while (i < 10);
来源：http://irc.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://joe.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mpg.jqgufenzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://jcl.zycfv.cn

C#:   do { i++; } while (i < 10);
来源：http://iox.316326.xyz

[B09] break 与 continue
来源：http://sga.wangshuangyany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://twj.xylfe.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cbh.xinyue.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jyh.gzhubu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ukv.iojbl.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vcr.shanyushiyangtech.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jze.gzhubu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jkz.ybcxt.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://twm.chenjidiqi.icu

[B10] 遍历同时拿索引
来源：http://yms.meibo888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jax.guowangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qfj.xuetiantiany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kbo.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://drr.hysaishi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aji.hongshengwenyu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jon.bjfxy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://itn.uphjek.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jgo.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://mph.ydzc1.top

Py:   list(range(0, 10, 2))
来源：http://aye.cucudq.cn

PHP:  range(0, 10, 2);
来源：http://ptp.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aeg.316326.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zzy.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rut.epnwcf.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xcn.uphjek.com

Ruby: (0...10).step(2).to_a
来源：http://lzo.yuanzhike.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ork.nwbrower.top

[B12] 跳出多层循环
来源：http://lph.zycfv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://evf.jlsjyb.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dhg.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ndj.tianlin.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://etm.birdmap.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sfz.xylfe.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://egr.ivvv.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lut.cdnleiting.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wjl.jqgfzy.top

[B13] 判断是否为数字
来源：http://twy.cashguo.top

Py:   isinstance(x, (int, float))
来源：http://ffa.yj202588.top

PHP:  is_numeric($x)
来源：http://kgd.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zvk.zhaomingkeji.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nlr.cqqwz.cn

Java: x instanceof Number
来源：http://uka.aizwys.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rzz.bbcook.cn

Ruby: x.is_a?(Numeric)
来源：http://tbt.sjlbkw.cn

C#:   x is int or double or decimal
来源：http://nwp.ctjpmb.com

[B14] 判断值是否在集合内
来源：http://lba.zhongyouzk.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://urg.feifeiyinyue.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jkr.kuanghao11.cn

JS:   [1, 2, 3].includes(x)
来源：http://ykn.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://agn.hnxiangtu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hnm.xylfe.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yuw.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://jko.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cqu.zhixingplan.top

[B15] 布尔运算与取反
来源：http://ocv.uphjek.com

Py:   a and b or not c
来源：http://apx.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://ijg.daria6918.cn

JS:   a && b || !c
来源：http://qcm.feifeiyinyue.top

TS:   a && b || !c
来源：http://veb.fanxiaobao.xyz

Java: a && b || !c
来源：http://uat.gaohongyu789.top

Go:   a && b || !c
来源：http://vqs.shzxlz.cn

Ruby: a && b || !c
来源：http://tod.shangyingyoupin.top

C#:   a && b || !c
来源：http://shy.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://imf.jyoumei.cn

Py:   if not data: return
来源：http://jio.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://cfh.zdqjudy.top

JS:   if (!data) return;
来源：http://jqy.zhijiandao.cn

TS:   if (!data) return;
来源：http://eqj.hywenlv.cn

Java: if (data == null) return;
来源：http://cwz.haohaochexian.top

Go:   if data == nil { return }
来源：http://bwj.ivvv.top

Ruby: return if data.nil?
来源：http://xwg.jlsjyb.cn

C#:   if (data == null) return;
来源：http://rzi.gzhubu.top

================================================================================
来源：http://hsu.zhiwuduotai.top

C. 函数与作用域
来源：http://cfq.sysykeji.top

================================================================================
来源：http://vgs.zhengqikj.top

[C01] 定义函数
来源：http://leh.xylfe.cn

Py:   def add(a, b): return a + b
来源：http://pfk.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yms.sysykeji.top

JS:   function add(a, b) { return a + b; }
来源：http://jba.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lnl.yanxiufei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yqb.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ncv.dianchejie.cn

Ruby: def add(a, b); a + b; end
来源：http://ikb.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zun.vqdsnc.cn

[C02] 默认参数
来源：http://fdd.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://avs.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yxj.fehbvm.com

JS:   function greet(name = "World") { return name; }
来源：http://gdq.hesvh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rgd.guannengcc.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gap.ivvv.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tlo.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://kbx.nanxuanxn.top

C#:   string Greet(string name = "World") => name;
来源：http://jso.hywenlv.cn

[C03] 可变参数
来源：http://rbt.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://dhw.hammf.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wes.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pfh.fengsongda.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xnj.ydjk.org.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qsf.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://viq.sysykeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://ipm.xuanzx.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wnw.yueranfly.top

[C04] 命名参数 / 关键字参数
来源：http://wae.redwolf501.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xie.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jzy.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gib.fktsv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yrf.zhixingplan.top

Java: // 无：用 Builder 模式或 record
来源：http://ney.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://sbn.shanyushiyangtech.top

Ruby: f(a: 1, b: 2)
来源：http://fua.xuanzx.com

C#:   f(a: 1, b: 2)
来源：http://kil.zhengqikj.top

[C05] 返回多个值
来源：http://rph.uphjek.com

Py:   return a, b
来源：http://lue.cashguo.top

PHP:  return [$a, $b];
来源：http://gtz.gzhubu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qzi.zhijiandao.cn

TS:   return { a, b };
来源：http://jld.hongshengwenyu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kkw.iojbl.cn

Go:   return a, b
来源：http://tmf.yanxiufei.cn

Ruby: return a, b
来源：http://jqa.uphjek.com

C#:   return (a, b);              // ValueTuple
来源：http://cyi.havefunace.top

[C06] 匿名函数 / lambda
来源：http://yrl.meibo888.top

Py:   square = lambda x: x * x
来源：http://ith.ctjpmb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://bwb.hysaishi.cn

JS:   const square = x => x * x;
来源：http://bts.hnqzz.top

TS:   const square = (x: number): number => x * x;
来源：http://fyd.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fhr.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://wmk.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://xuo.nanxinkj.top

C#:   Func<int, int> square = x => x * x;
来源：http://ric.xuanzx.com

[C07] 把函数作为参数传入
来源：http://vpw.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fhs.wangshuangyany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lqx.zhixingplan.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dsv.yanxiufei.cn

TS:   arr.map(String)
来源：http://aba.zdbjq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dld.fengsongda.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mzq.sufxvd.cn

Ruby: arr.map(&:upcase)
来源：http://wxa.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vxv.yueranfly.top

[C08] 闭包
来源：http://hkc.yanxiufei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rws.vehdjk.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nmi.nanxinkj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://owc.svipenyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://myr.nanxinkj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://upy.0kj1m.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ujl.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ldy.birdmap.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fdm.yj20258.top

[C09] 递归
来源：http://nde.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://znl.wangshuangyany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://skf.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hrh.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xnj.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://erb.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yqf.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://scz.gaohongyu789.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kee.feifeiyinyue.top

[C10] 变量作用域
来源：http://scx.yonumen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ris.wangdashe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://btm.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yan.hnqzz.top


<!-- 参考信息 -->