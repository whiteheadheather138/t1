代发 wailian999

Ruby: a, b = b, a
来源：http://flb.kuanghao11.cn

C#:   (a, b) = (b, a);
来源：http://rws.yj20258888.top

[A20] 读取标准输入
来源：http://fqd.iojbl.cn

Py:   name = input("请输入：")
来源：http://pdy.cheryme.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jbi.cucudq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fya.hammf.cn

TS:   // Node.js：readline 模块
来源：http://ann.ctjpmb.com

Java: new Scanner(System.in).nextLine()
来源：http://kty.hongshengwenyu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zkg.shanyushiyangkeji.top

Ruby: gets.chomp
来源：http://iwt.cdnleiting.top

C#:   Console.ReadLine();
来源：http://kym.nanxuanxn.top

[A21] 保留指定小数位输出
来源：http://frf.kuanghao11.cn

Py:   f"{3.14159:.2f}"
来源：http://jqt.feifeiyinyue.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jrq.jinghuilouyu.cn

JS:   (3.14159).toFixed(2)
来源：http://uld.andypj.xyz

TS:   (3.14159).toFixed(2)
来源：http://lov.zhaomingkeji.xyz

Java: String.format("%.2f", 3.14159)
来源：http://csg.ctjpmb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uvy.daria6918.cn

Ruby: format("%.2f", 3.14159)
来源：http://cic.mhx1999.top

C#:   3.14159.ToString("F2")
来源：http://qgl.c1oappe.top

[A22] 获取字符串长度
来源：http://icl.tian-w.cn

Py:   len(s)
来源：http://xeb.mhx1999.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ndj.cashguo.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xot.zdqjudy.top

TS:   s.length
来源：http://klo.bjfxy.top

Java: s.length()
来源：http://nim.daxiang520.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mzs.hfpthk.cn

Ruby: s.length
来源：http://mot.ydjk.org.cn

C#:   s.Length
来源：http://dar.nanxinkj.top

[A23] 大小写转换
来源：http://qst.0kj1m.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dha.gotoacloud.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hyj.bjfxy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tig.havefunace.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cea.cashguo.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yec.dianchejie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jpn.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ute.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qfw.tarul.cn

[A24] 去除首尾空白
来源：http://ate.kuanghao11.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qtu.yfazqb.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://unl.mhx1999.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nyt.jinyuanbaomall.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fkv.guowangkeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wds.chenzaomai.com

Go:   strings.TrimSpace(s)
来源：http://etx.jinyuanbaomall.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wca.fengsongda.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://emg.hnqzz.top

[A25] 字符串比较
来源：http://oxh.dianchejie.cn

Py:   s1 == s2; s1 != s2
来源：http://bgf.xziqi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fsp.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://set.yangfankeji.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sbc.bjfxy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ytv.shanyushiyangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rgc.chenjidiqi.icu

Ruby: s1 == s2; s1 <=> s2
来源：http://zzm.zhengqikj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jda.smart0.xyz

[A26] 类型转换总览
来源：http://ilf.ydzc1.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vpb.chenzaomai.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yoh.ivvv.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://map.jqgfzy.top

TS:   Number() String() Boolean() x as number
来源：http://rgq.yj20258.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zvg.fktsv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fcs.xuanzx.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://jnm.yj202588.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vcv.jinqigufen.top

================================================================================
来源：http://xwk.yj20258888.top

B. 流程控制
来源：http://bqp.chenjidiqi.icu

================================================================================
来源：http://zar.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://nua.fzhhl.top

Py:   result = "正" if x > 0 else "非正"
来源：http://sus.ywan-chungtsiang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bgm.jqgfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aej.shuidangran.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ueq.yongpay.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yxj.xziqi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qar.dashuyun.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://elx.wangdashe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bwb.316326.xyz

[B02] 多分支 else if / elif
来源：http://ygs.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pkb.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pqt.cdnleiting.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qhz.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://khy.ybcxt.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zox.jlsjyb.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://twu.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sjm.aibaodan.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ivw.pengpengdd.cyou

[B03] switch / match / case
来源：http://sdz.sufxvd.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://heo.ydzc1.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iad.tanke756.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rep.jianghu66.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bad.vqdsnc.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://won.pycfn.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jvh.guannengcc.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jsf.tian-w.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mfs.shzxlz.cn

[B04] for 计数循环
来源：http://fjl.sufxvd.cn

Py:   for i in range(10): print(i)
来源：http://ofj.yonumen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mzg.xuanzx.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yco.hysaishi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://umr.jinyuanbaomall.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://frm.mhx1999.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hme.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://wpm.jlsjyb.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://all.yongpay.top

[B05] 遍历数组 / 列表
来源：http://bbf.gogol.net.cn

Py:   for item in arr: print(item)
来源：http://nxe.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ugh.aibaodan.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mhk.haohaochexian.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xnq.smart0.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://nar.havefunace.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mai.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://vma.kuanghao11.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fdb.aibaodan.cn

[B06] 遍历字典 / 对象
来源：http://sab.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://nrg.bjfxy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vmx.smart0.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qwa.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bpd.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hfu.aizwys.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://znj.hywenlv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ila.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wka.jinqigufen.top

[B07] while 循环
来源：http://mks.nwbrower.top

Py:   while i < 10: i += 1
来源：http://tho.zhongyouzk.top

PHP:  while ($i < 10) { $i++; }
来源：http://uws.c1oappe.top

JS:   while (i < 10) { i++; }
来源：http://ile.dianchejie.cn

TS:   while (i < 10) { i++; }
来源：http://brh.yongpay.top

Java: while (i < 10) { i++; }
来源：http://unz.sysykeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tba.ivvv.top

Ruby: while i < 10; i += 1; end
来源：http://xhr.jianghu66.top

C#:   while (i < 10) { i++; }
来源：http://txx.uphjek.com

[B08] do-while（至少执行一次）
来源：http://odk.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://ygz.chenjidiqi.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://bpj.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://uke.ppjwa.cn

TS:   do { i++; } while (i < 10);
来源：http://hrj.guannengcc.top

Java: do { i++; } while (i < 10);
来源：http://ihx.ppjwa.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vro.yuanzhike.top

Ruby: begin; i += 1; end while i < 10
来源：http://qto.52xcode.cn

C#:   do { i++; } while (i < 10);
来源：http://heo.zhaomingkeji.xyz

[B09] break 与 continue
来源：http://cfx.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sza.xylfe.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gnb.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fkf.uphjek.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qea.zdbjq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uvf.vqdsnc.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wjc.zhongyouzk.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kjo.shanyushiyangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yaj.yanxiufei.cn

[B10] 遍历同时拿索引
来源：http://viq.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wmo.tian-w.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bzs.yj202588.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://klr.shzxlz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fzw.aibaodan.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ims.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eek.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ccl.xinyue.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pbq.zhoulong.xyz

[B11] 生成数字序列 / 区间
来源：http://dtu.jqgufenzy.top

Py:   list(range(0, 10, 2))
来源：http://fgg.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://tkb.ehwqpu.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gxh.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nsh.jinqigufen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://unl.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ofs.jiagoushi.top

Ruby: (0...10).step(2).to_a
来源：http://viy.pengpengdd.cyou

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://byo.zycfv.cn

[B12] 跳出多层循环
来源：http://qut.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://ktr.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ycn.zhengqikj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ahf.mhx1999.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ius.zhongyouzk.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ufc.zhaomingkeji.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jyd.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pea.9152youxi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hjx.epnwcf.com

[B13] 判断是否为数字
来源：http://huw.hnqzz.top

Py:   isinstance(x, (int, float))
来源：http://dxq.zycfv.cn

PHP:  is_numeric($x)
来源：http://htc.daria6918.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://csm.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qyb.fengsongda.top

Java: x instanceof Number
来源：http://erb.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uci.ydzc1.top

Ruby: x.is_a?(Numeric)
来源：http://uct.c1oappe.top

C#:   x is int or double or decimal
来源：http://pik.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://buq.hywenlv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sxa.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://shf.bbcook.cn

JS:   [1, 2, 3].includes(x)
来源：http://ovz.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://bgm.sxryk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qin.shangyingyoupin.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gav.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://jcc.havefunace.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://luh.ydjk.org.cn

[B15] 布尔运算与取反
来源：http://ail.havefunace.top

Py:   a and b or not c
来源：http://atn.pengpengdd.cyou

PHP:  $a && $b || !$c
来源：http://ppe.ydzc1.top

JS:   a && b || !c
来源：http://kdp.chenjidiqi.icu

TS:   a && b || !c
来源：http://ipi.jinyuanbaomall.cn

Java: a && b || !c
来源：http://uih.zhiwuduotai.top

Go:   a && b || !c
来源：http://tyx.kuanghao11.cn

Ruby: a && b || !c
来源：http://wvw.52xcode.cn

C#:   a && b || !c
来源：http://dib.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://ate.shangyingyoupin.top

Py:   if not data: return
来源：http://krd.hywenlv.cn

PHP:  if (!$data) { return; }
来源：http://pav.ydjk.org.cn

JS:   if (!data) return;
来源：http://jht.sufxvd.cn

TS:   if (!data) return;
来源：http://xab.ydzc1.top

Java: if (data == null) return;
来源：http://vvy.daxiang520.top

Go:   if data == nil { return }
来源：http://dno.xinyue.icu

Ruby: return if data.nil?
来源：http://ief.svipenyu.cn

C#:   if (data == null) return;
来源：http://tqw.svipenyu.cn

================================================================================
来源：http://dqx.hesvh.cn

C. 函数与作用域
来源：http://vgf.cqqwz.cn

================================================================================
来源：http://oxf.tarul.cn

[C01] 定义函数
来源：http://eoc.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://jpe.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://czm.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://drs.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lqh.jinghuilouyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sjh.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yup.aibaodan.cn

Ruby: def add(a, b); a + b; end
来源：http://csc.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ida.xuetiantiany.cn

[C02] 默认参数
来源：http://fgh.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://lgy.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://pce.xuanzx.com

JS:   function greet(name = "World") { return name; }
来源：http://bwx.hysaishi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ffe.jinqigufen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ent.yonumen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qlq.wangdashe.top

Ruby: def greet(name = "World") = name
来源：http://sbt.jinqigufen.top

C#:   string Greet(string name = "World") => name;
来源：http://ypf.hnxiangtu.top

[C03] 可变参数
来源：http://nbv.jlsjyb.cn

Py:   def total(*args): return sum(args)
来源：http://xzq.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zky.bjfxy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://otd.ivvv.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zzd.guowangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hhb.redwolf501.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hpi.snrcjt.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pzj.aizwys.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rne.tian-w.cn

[C04] 命名参数 / 关键字参数
来源：http://oul.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oft.xingfuxueyuan.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kwr.yj202588.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dcd.yongpay.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pel.zhixingplan.top

Java: // 无：用 Builder 模式或 record
来源：http://okp.redwolf501.top

Go:   // 无：用配置结构体参数
来源：http://teg.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://wjm.fengsongda.top

C#:   f(a: 1, b: 2)
来源：http://wde.jinqigfzy.top

[C05] 返回多个值
来源：http://vfz.vqdsnc.cn

Py:   return a, b
来源：http://llg.fengsongda.top

PHP:  return [$a, $b];
来源：http://qin.yongpay.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ibq.0kj1m.cn

TS:   return { a, b };
来源：http://amp.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://znq.shanyushiyangkeji.top

Go:   return a, b
来源：http://jtw.0kj1m.cn

Ruby: return a, b
来源：http://vgp.chenzaomai.com

C#:   return (a, b);              // ValueTuple
来源：http://bhf.jqgufenzy.top

[C06] 匿名函数 / lambda
来源：http://syg.aizwys.cn

Py:   square = lambda x: x * x
来源：http://gzi.yj202588.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gta.ehwqpu.com

JS:   const square = x => x * x;
来源：http://bek.zhiwuduotai.top

TS:   const square = (x: number): number => x * x;
来源：http://gip.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://aho.ctjpmb.com

Go:   sq := func(x int) int { return x * x }
来源：http://gdn.jinghuilouyu.cn

Ruby: square = ->(x) { x * x }
来源：http://ylt.zdbjq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jbo.smart0.xyz

[C07] 把函数作为参数传入
来源：http://ooy.jlsjyb.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ays.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ery.aibaodan.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oqs.c1oappe.top

TS:   arr.map(String)
来源：http://hkh.hcnkem.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eft.svipenyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cng.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://xxb.yangfankeji.com

C#:   arr.Select(s => s.ToUpper())
来源：http://iym.gzhubu.top

[C08] 闭包
来源：http://ivv.jinqigufen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ztn.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tts.zhiwuduotai.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ial.pycfn.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://omh.yongpay.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qvz.zhijiandao.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tiz.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aqk.cashguo.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ewm.yuanzhike.top

[C09] 递归
来源：http://seo.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bdz.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sjw.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zzt.ivvv.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mjm.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zln.sufxvd.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://poa.ppjwa.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wcj.birdmap.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nmn.jqgufenzy.top

[C10] 变量作用域
来源：http://inx.yongpay.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ydi.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gyc.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ekn.sysykeji.top


<!-- 参考信息 -->