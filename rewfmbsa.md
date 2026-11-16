代发 wailian999

Ruby: a, b = b, a
来源：http://byb.zdbjq.cn

C#:   (a, b) = (b, a);
来源：http://scm.feifeiyinyue.top

[A20] 读取标准输入
来源：http://gqh.zycfv.cn

Py:   name = input("请输入：")
来源：http://uwf.ivvv.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vox.haohaochexian.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lyn.pengpengdd.cyou

TS:   // Node.js：readline 模块
来源：http://naa.jlsjyb.cn

Java: new Scanner(System.in).nextLine()
来源：http://wop.jqgufenzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wwh.vehdjk.com

Ruby: gets.chomp
来源：http://ree.fengsongda.top

C#:   Console.ReadLine();
来源：http://zde.redwolf501.top

[A21] 保留指定小数位输出
来源：http://hyz.jlsjyb.cn

Py:   f"{3.14159:.2f}"
来源：http://hji.cqqwz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ilk.bjfxy.top

JS:   (3.14159).toFixed(2)
来源：http://bsj.aizwys.cn

TS:   (3.14159).toFixed(2)
来源：http://cgv.yj20258.top

Java: String.format("%.2f", 3.14159)
来源：http://qvl.snrcjt.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ivz.hammf.cn

Ruby: format("%.2f", 3.14159)
来源：http://qam.shzxlz.cn

C#:   3.14159.ToString("F2")
来源：http://qsh.smart0.xyz

[A22] 获取字符串长度
来源：http://itn.cashguo.top

Py:   len(s)
来源：http://clk.yongpay.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ert.ctjpmb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xqn.hnxiangtu.top

TS:   s.length
来源：http://xyf.zhijiandao.cn

Java: s.length()
来源：http://gte.9152youxi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kcb.ppjwa.cn

Ruby: s.length
来源：http://lmb.ywan-chungtsiang.top

C#:   s.Length
来源：http://vkb.yongpay.top

[A23] 大小写转换
来源：http://gdx.fehbvm.com

Py:   s.upper(); s.lower(); s.title()
来源：http://nua.sweek.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lrv.jqgufenzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ugx.ivvv.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zmv.xingfuxueyuan.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xas.wangdashe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ujz.hfpthk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://onh.jiagoushi.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mpu.c1oappe.top

[A24] 去除首尾空白
来源：http://hgf.gogol.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dpy.jiagoushi.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rcc.hnqzz.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xhn.pengpengdd.cyou

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kch.ppjwa.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yhq.jlsjyb.cn

Go:   strings.TrimSpace(s)
来源：http://blm.zhengqikj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uxy.hnqzz.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xvk.chenzaomai.com

[A25] 字符串比较
来源：http://ewm.shanyushiyangkeji.top

Py:   s1 == s2; s1 != s2
来源：http://ckx.tarul.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://amd.redwolf501.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://awa.yj20258.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vsd.ivvv.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qan.fzhhl.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mkm.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xed.aizwys.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zoh.cucudq.cn

[A26] 类型转换总览
来源：http://umo.jiagoushi.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xwn.yvedp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uod.fktsv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qmz.ybcxt.top

TS:   Number() String() Boolean() x as number
来源：http://kgq.nanxuanxn.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jzp.gaohongyu789.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xvr.yueranfly.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fec.zhiwuduotai.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tor.tianlin.xyz

================================================================================
来源：http://elv.xinyue.icu

B. 流程控制
来源：http://nyk.pycfn.com

================================================================================
来源：http://zpu.dianchejie.cn

[B01] 条件判断 if / else
来源：http://nqa.andypj.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://cwa.nanxinkj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vfr.andypj.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bbk.dashuyun.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xod.cqqwz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rnh.wangdashe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://luh.sxryk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://awg.fengsongda.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xrl.jqgfzy.top

[B02] 多分支 else if / elif
来源：http://fql.sweek.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pzu.jinghuilouyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fqw.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xfi.dashuyun.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dup.chenlongwang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pfs.xziqi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://irk.birdmap.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cqc.sjlbkw.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gvx.redwolf501.top

[B03] switch / match / case
来源：http://jfv.ivvv.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xxb.hammf.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wis.tanke756.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jjr.yuxming.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ync.fktsv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xeg.bjfxy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xjo.pengpengdd.cyou

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rmf.andypj.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kve.hnxiangtu.top

[B04] for 计数循环
来源：http://fam.cucudq.cn

Py:   for i in range(10): print(i)
来源：http://qzo.chenlongwang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xft.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nzj.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tkv.uphjek.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hix.chenjidiqi.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ovb.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://nmj.zdqjudy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jlq.meibo888.top

[B05] 遍历数组 / 列表
来源：http://ofo.cashguo.top

Py:   for item in arr: print(item)
来源：http://ane.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eox.shuidangran.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vsm.ehwqpu.com

TS:   for (const item of arr) { console.log(item); }
来源：http://mtl.feifeiyinyue.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hvp.hongshengwenyu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rtz.dashuyun.cn

Ruby: arr.each { |item| puts item }
来源：http://bpd.feifeiyinyue.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dsg.ppjwa.cn

[B06] 遍历字典 / 对象
来源：http://zzd.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nct.c1oappe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pwe.fktsv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ugl.vehdjk.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jej.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://whl.shzxlz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kqn.daxiang520.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fru.jinqigufen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hhv.ctjpmb.com

[B07] while 循环
来源：http://gjg.gogol.net.cn

Py:   while i < 10: i += 1
来源：http://phw.birdmap.top

PHP:  while ($i < 10) { $i++; }
来源：http://oop.sweek.top

JS:   while (i < 10) { i++; }
来源：http://web.ydjk.org.cn

TS:   while (i < 10) { i++; }
来源：http://ffj.xylfe.cn

Java: while (i < 10) { i++; }
来源：http://wtq.xylfe.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jcb.wangshuangyany.cn

Ruby: while i < 10; i += 1; end
来源：http://puv.andypj.xyz

C#:   while (i < 10) { i++; }
来源：http://eiu.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://tkl.shzxlz.cn

Py:   # 无 do-while：用 while True + break
来源：http://qzl.dianchejie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xjt.feifeiyinyue.top

JS:   do { i++; } while (i < 10);
来源：http://vdv.xuetiantiany.cn

TS:   do { i++; } while (i < 10);
来源：http://oze.52xcode.cn

Java: do { i++; } while (i < 10);
来源：http://eoj.xuanzx.com

Go:   for { i++; if i >= 10 { break } }
来源：http://cut.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://asi.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://mfj.chenjidiqi.icu

[B09] break 与 continue
来源：http://mur.hnqzz.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://emr.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lat.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://deu.mhx1999.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://egq.jqgufenzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pfx.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ulh.hfpthk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dln.jlsjyb.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ejq.hcnkem.com

[B10] 遍历同时拿索引
来源：http://meh.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rml.cucudq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vee.gzhubu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://boq.9152youxi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jha.yongpay.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xnd.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ctu.nanxuanxn.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dmk.zdbjq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://res.kuanghao11.cn

[B11] 生成数字序列 / 区间
来源：http://vmd.hnxiangtu.top

Py:   list(range(0, 10, 2))
来源：http://gst.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://fpc.yvedp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://egz.sweek.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ssq.yvedp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://msd.zhoulong.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://opn.pengpengdd.cyou

Ruby: (0...10).step(2).to_a
来源：http://wfi.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://obc.zhongyouzk.top

[B12] 跳出多层循环
来源：http://kgs.feifeiyinyue.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hgm.jiagoushi.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mnp.xylfe.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lha.cqqwz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yjo.hfpthk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://erc.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xkr.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eir.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nkx.cashguo.top

[B13] 判断是否为数字
来源：http://ikg.chenlongwang.top

Py:   isinstance(x, (int, float))
来源：http://rza.hammf.cn

PHP:  is_numeric($x)
来源：http://iwf.uphjek.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uny.yuanzhike.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aao.hcnkem.com

Java: x instanceof Number
来源：http://kzc.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://azm.cqqwz.cn

Ruby: x.is_a?(Numeric)
来源：http://jwl.cucudq.cn

C#:   x is int or double or decimal
来源：http://pmh.hfpthk.cn

[B14] 判断值是否在集合内
来源：http://eop.ppjwa.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uvy.chenjidiqi.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gkz.jinqigfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://xcj.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://ako.9152youxi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tee.bjfxy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nvp.cashguo.top

Ruby: [1, 2, 3].include?(x)
来源：http://vqv.fktsv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://acj.ehwqpu.com

[B15] 布尔运算与取反
来源：http://egi.pycfn.com

Py:   a and b or not c
来源：http://lxi.epnwcf.com

PHP:  $a && $b || !$c
来源：http://zxs.zhixingplan.top

JS:   a && b || !c
来源：http://ygz.aizwys.cn

TS:   a && b || !c
来源：http://pir.feifeiyinyue.top

Java: a && b || !c
来源：http://zwq.epnwcf.com

Go:   a && b || !c
来源：http://fld.yj20258888.top

Ruby: a && b || !c
来源：http://dip.meibo888.top

C#:   a && b || !c
来源：http://wki.smart0.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://myh.hysaishi.cn

Py:   if not data: return
来源：http://ggo.vqdsnc.cn

PHP:  if (!$data) { return; }
来源：http://xhr.nanxuanxn.top

JS:   if (!data) return;
来源：http://tko.yvedp.cn

TS:   if (!data) return;
来源：http://yyb.jianghu66.top

Java: if (data == null) return;
来源：http://egd.sweek.top

Go:   if data == nil { return }
来源：http://vez.yvedp.cn

Ruby: return if data.nil?
来源：http://jft.tanke756.top

C#:   if (data == null) return;
来源：http://tcm.dianchejie.cn

================================================================================
来源：http://awi.yueranfly.top

C. 函数与作用域
来源：http://rzj.snrcjt.cn

================================================================================
来源：http://qeb.daxiang520.top

[C01] 定义函数
来源：http://kum.jyoumei.cn

Py:   def add(a, b): return a + b
来源：http://qzg.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qsl.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://tea.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oxu.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://bqf.tanke756.top

Go:   func add(a, b int) int { return a + b }
来源：http://zdz.daria6918.cn

Ruby: def add(a, b); a + b; end
来源：http://dec.redwolf501.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nch.zhongyouzk.top

[C02] 默认参数
来源：http://iri.tian-w.cn

Py:   def greet(name="World"): return name
来源：http://pyz.guowangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ybu.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://xou.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jik.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://bgb.hammf.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ncv.aibaodan.cn

Ruby: def greet(name = "World") = name
来源：http://yol.nanxuanxn.top

C#:   string Greet(string name = "World") => name;
来源：http://kch.snrcjt.cn

[C03] 可变参数
来源：http://knc.xuanzx.com

Py:   def total(*args): return sum(args)
来源：http://elz.gogol.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yqh.xylfe.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dku.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tys.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jkl.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uih.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://snj.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aiy.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://zme.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qhu.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ywv.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mou.jiagoushi.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://abb.chenjidiqi.icu

Java: // 无：用 Builder 模式或 record
来源：http://fan.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://ciy.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://esd.ywan-chungtsiang.top

C#:   f(a: 1, b: 2)
来源：http://zrr.mhx1999.top

[C05] 返回多个值
来源：http://nwj.ctjpmb.com

Py:   return a, b
来源：http://llf.bjfxy.top

PHP:  return [$a, $b];
来源：http://nki.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fzl.mhx1999.top

TS:   return { a, b };
来源：http://ckr.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dqy.zhijiandao.cn

Go:   return a, b
来源：http://wxs.zhoulong.xyz

Ruby: return a, b
来源：http://jrq.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://kvs.xuanzx.com

[C06] 匿名函数 / lambda
来源：http://ool.havefunace.top

Py:   square = lambda x: x * x
来源：http://jtc.fengsongda.top

PHP:  $square = fn($x) => $x * $x;
来源：http://arc.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://rwx.fzhhl.top

TS:   const square = (x: number): number => x * x;
来源：http://gmm.feifeiyinyue.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pht.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://lvg.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://dsz.birdmap.top

C#:   Func<int, int> square = x => x * x;
来源：http://gym.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://wij.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cnp.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ojr.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mxr.zhiwuduotai.top

TS:   arr.map(String)
来源：http://umm.gzhubu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oua.hongshengwenyu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cmn.bbcook.cn

Ruby: arr.map(&:upcase)
来源：http://ukb.52xcode.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rcg.aibaodan.cn

[C08] 闭包
来源：http://sbh.shanyushiyangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hef.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ect.sxryk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://igi.gzhubu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nza.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://stz.xinyue.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wfs.jianghu66.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yml.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xwr.hywenlv.cn

[C09] 递归
来源：http://dlu.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ccc.yueranfly.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mzp.316326.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zjj.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uwt.chenjidiqi.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ouw.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yyf.hammf.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rsz.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vsz.yangfankeji.com

[C10] 变量作用域
来源：http://map.sjlbkw.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fai.ydjk.org.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ham.shzxlz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ghy.sweek.top


<!-- 参考信息 -->