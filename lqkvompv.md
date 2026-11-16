代发 wailian999

C#:   (int)'A'; (char)65
来源：http://gkc.ppjwa.cn

[A19] 交换两个变量
来源：http://tsa.ehwqpu.com

Py:   a, b = b, a
来源：http://mlv.zhengqikj.top

PHP:  [$a, $b] = [$b, $a];
来源：http://wlz.sxryk.cn

JS:   [a, b] = [b, a];
来源：http://jhd.chenzaomai.com

TS:   [a, b] = [b, a];
来源：http://gxg.jinqigufen.top

Java: int t = a; a = b; b = t;
来源：http://goc.ydjk.org.cn

Go:   a, b = b, a
来源：http://pbt.gogol.net.cn

Ruby: a, b = b, a
来源：http://poq.wangshuangyany.cn

C#:   (a, b) = (b, a);
来源：http://lor.zhengqikj.top

[A20] 读取标准输入
来源：http://vnj.cashguo.top

Py:   name = input("请输入：")
来源：http://qij.tanke756.top

PHP:  $name = trim(fgets(STDIN));
来源：http://mae.jyoumei.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bwy.tanke756.top

TS:   // Node.js：readline 模块
来源：http://npf.nanxinkj.top

Java: new Scanner(System.in).nextLine()
来源：http://vrp.xuetiantiany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bfn.uphjek.com

Ruby: gets.chomp
来源：http://apj.bbcook.cn

C#:   Console.ReadLine();
来源：http://xor.cucudq.cn

[A21] 保留指定小数位输出
来源：http://rtp.cdnleiting.top

Py:   f"{3.14159:.2f}"
来源：http://ouw.hongshengwenyu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yyn.daria6918.cn

JS:   (3.14159).toFixed(2)
来源：http://ywp.smart0.xyz

TS:   (3.14159).toFixed(2)
来源：http://zim.dianchejie.cn

Java: String.format("%.2f", 3.14159)
来源：http://ppz.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eza.haohaochexian.top

Ruby: format("%.2f", 3.14159)
来源：http://wmd.chenlongwang.top

C#:   3.14159.ToString("F2")
来源：http://eqb.gzhubu.top

[A22] 获取字符串长度
来源：http://dpo.birdmap.top

Py:   len(s)
来源：http://auw.shuidangran.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bpd.yanxiufei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hqx.tian-w.cn

TS:   s.length
来源：http://ysb.cqqwz.cn

Java: s.length()
来源：http://jnb.tian-w.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zvh.hfpthk.cn

Ruby: s.length
来源：http://dqz.ywan-chungtsiang.top

C#:   s.Length
来源：http://pls.jqgfzy.top

[A23] 大小写转换
来源：http://ccz.xziqi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://otl.hongshengwenyu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://azp.kuanghao11.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://txh.ybcxt.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ezl.9152youxi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qga.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://shq.bjfxy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kms.ydjk.org.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kkq.gzhubu.top

[A24] 去除首尾空白
来源：http://giv.gogol.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://khd.andypj.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zmf.bbcook.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://juw.gogol.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jja.fanxiaobao.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://paz.jinqigufen.top

Go:   strings.TrimSpace(s)
来源：http://ppx.jyoumei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kon.hammf.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vrg.jqgufenzy.top

[A25] 字符串比较
来源：http://mrz.shanyushiyangtech.top

Py:   s1 == s2; s1 != s2
来源：http://oyp.yueranfly.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dxk.fzhhl.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mdo.havefunace.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gdp.jyoumei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gbz.cheryme.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xvn.tarul.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wdj.cucudq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ffo.vqdsnc.cn

[A26] 类型转换总览
来源：http://rqi.snrcjt.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://drc.tianlin.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ymi.daxiang520.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rga.chenzaomai.com

TS:   Number() String() Boolean() x as number
来源：http://zjj.vehdjk.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://stf.tanke756.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yjo.yonumen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dse.kuanghao11.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://quj.fehbvm.com

================================================================================
来源：http://mbo.fanxiaobao.xyz

B. 流程控制
来源：http://pna.shanyushiyangkeji.top

================================================================================
来源：http://rss.jinyuanbaomall.cn

[B01] 条件判断 if / else
来源：http://vln.smart0.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://iix.ctjpmb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xws.vqdsnc.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oza.yvedp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://umy.jinqigfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fhs.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cen.epnwcf.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sqx.hongshengwenyu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pmp.jiagoushi.top

[B02] 多分支 else if / elif
来源：http://pbi.gotoacloud.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cty.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bqx.smart0.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dyh.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xyk.chenlongwang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uav.fzhhl.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://neg.yj20258.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://upl.ydzc1.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nou.epnwcf.com

[B03] switch / match / case
来源：http://mym.fktsv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dec.sufxvd.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pic.jinghuilouyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ecj.ywan-chungtsiang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kzi.ppjwa.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nza.yangfankeji.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vju.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xmc.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://crz.wangdashe.top

[B04] for 计数循环
来源：http://gwj.cucudq.cn

Py:   for i in range(10): print(i)
来源：http://xfx.daxiang520.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wzu.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sml.redwolf501.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uqz.52xcode.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://osn.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kcm.zhiwuduotai.top

Ruby: 10.times { |i| puts i }
来源：http://qpe.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dzk.yueranfly.top

[B05] 遍历数组 / 列表
来源：http://axa.feifeiyinyue.top

Py:   for item in arr: print(item)
来源：http://gab.wangdashe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qwj.zhongyouzk.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hws.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mqu.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://sqf.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vpg.zhongyouzk.top

Ruby: arr.each { |item| puts item }
来源：http://ngn.haohaochexian.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://riu.kuanghao11.cn

[B06] 遍历字典 / 对象
来源：http://zns.jianghu66.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hpj.feifeiyinyue.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://moz.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tgo.smart0.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://upr.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dkv.fanxiaobao.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eie.sxryk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xsw.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ckm.snrcjt.cn

[B07] while 循环
来源：http://okk.sweek.top

Py:   while i < 10: i += 1
来源：http://snb.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://nsw.gogol.net.cn

JS:   while (i < 10) { i++; }
来源：http://vhx.zdbjq.cn

TS:   while (i < 10) { i++; }
来源：http://tzj.dianchejie.cn

Java: while (i < 10) { i++; }
来源：http://ugk.cdnleiting.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aga.c1oappe.top

Ruby: while i < 10; i += 1; end
来源：http://wih.hcnkem.com

C#:   while (i < 10) { i++; }
来源：http://hdz.uphjek.com

[B08] do-while（至少执行一次）
来源：http://ino.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://xxk.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://erq.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://yfg.tanke756.top

TS:   do { i++; } while (i < 10);
来源：http://ttf.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://cxl.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hkg.xingfuxueyuan.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://azx.xziqi.cn

C#:   do { i++; } while (i < 10);
来源：http://gem.jinghuilouyu.cn

[B09] break 与 continue
来源：http://ttk.snrcjt.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zxw.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://srp.uphjek.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ffo.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dli.hcnkem.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://twr.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://phy.epnwcf.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qqy.52xcode.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qhv.shanyushiyangkeji.top

[B10] 遍历同时拿索引
来源：http://lxv.gaohongyu789.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tcg.jianghu66.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://avb.pengpengdd.cyou

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rlt.316326.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gjl.havefunace.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mto.guowangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kjl.nanxinkj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mju.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aaw.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://ein.jlsjyb.cn

Py:   list(range(0, 10, 2))
来源：http://ogt.zhongyouzk.top

PHP:  range(0, 10, 2);
来源：http://oix.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wkf.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wna.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hub.gotoacloud.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kfi.zycfv.cn

Ruby: (0...10).step(2).to_a
来源：http://wcd.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iln.yanxiufei.cn

[B12] 跳出多层循环
来源：http://bvk.dianchejie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tfz.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jxs.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://awm.shanyushiyangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://utp.hywenlv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qfu.aizwys.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vmw.gaohongyu789.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wog.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uan.zhengqikj.top

[B13] 判断是否为数字
来源：http://ibd.uphjek.com

Py:   isinstance(x, (int, float))
来源：http://pcj.xziqi.cn

PHP:  is_numeric($x)
来源：http://myw.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xxf.nanxinkj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xnl.ybcxt.top

Java: x instanceof Number
来源：http://lmr.shzxlz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tgv.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://xla.xylfe.cn

C#:   x is int or double or decimal
来源：http://qoq.sjlbkw.cn

[B14] 判断值是否在集合内
来源：http://nmk.zhijiandao.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lxc.ehwqpu.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ybh.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://ubq.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://rqa.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jbc.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tfy.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://pvo.xuetiantiany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fbf.epnwcf.com

[B15] 布尔运算与取反
来源：http://vcs.nwbrower.top

Py:   a and b or not c
来源：http://rlh.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://ifg.ydzc1.top

JS:   a && b || !c
来源：http://pnr.zhoulong.xyz

TS:   a && b || !c
来源：http://mgl.jlsjyb.cn

Java: a && b || !c
来源：http://pup.ybcxt.top

Go:   a && b || !c
来源：http://wqd.52xcode.cn

Ruby: a && b || !c
来源：http://jab.bbcook.cn

C#:   a && b || !c
来源：http://rsv.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://ztn.jyoumei.cn

Py:   if not data: return
来源：http://gbb.dashuyun.cn

PHP:  if (!$data) { return; }
来源：http://pho.zycfv.cn

JS:   if (!data) return;
来源：http://cef.nwbrower.top

TS:   if (!data) return;
来源：http://ppm.dashuyun.cn

Java: if (data == null) return;
来源：http://yhi.yangfankeji.com

Go:   if data == nil { return }
来源：http://els.havefunace.top

Ruby: return if data.nil?
来源：http://pne.daxiang520.top

C#:   if (data == null) return;
来源：http://jox.cashguo.top

================================================================================
来源：http://cnk.ctjpmb.com

C. 函数与作用域
来源：http://jvw.chenjidiqi.icu

================================================================================
来源：http://hbc.zdqjudy.top

[C01] 定义函数
来源：http://pek.pycfn.com

Py:   def add(a, b): return a + b
来源：http://ydl.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uwq.shanyushiyangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://kpy.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yto.jlsjyb.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fqm.yfazqb.com

Go:   func add(a, b int) int { return a + b }
来源：http://cis.kuanghao11.cn

Ruby: def add(a, b); a + b; end
来源：http://riy.xuetiantiany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zqr.gogol.net.cn

[C02] 默认参数
来源：http://dhq.shangyingyoupin.top

Py:   def greet(name="World"): return name
来源：http://efh.sufxvd.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jma.shanyushiyangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://uxm.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://chq.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ndr.haohaochexian.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xfc.vehdjk.com

Ruby: def greet(name = "World") = name
来源：http://ygv.gaohongyu789.top

C#:   string Greet(string name = "World") => name;
来源：http://nxl.ctjpmb.com

[C03] 可变参数
来源：http://ths.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://edu.iojbl.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eie.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://acf.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dle.redwolf501.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iuk.ctjpmb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vsq.c1oappe.top

Ruby: def total(*nums); nums.sum; end
来源：http://kma.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zsl.zhijiandao.cn

[C04] 命名参数 / 关键字参数
来源：http://osp.wangshuangyany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kmm.jqgufenzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://afn.dashuyun.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dya.zhixingplan.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xft.jinqigufen.top

Java: // 无：用 Builder 模式或 record
来源：http://nss.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://wpy.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://rey.havefunace.top

C#:   f(a: 1, b: 2)
来源：http://kpy.sjlbkw.cn

[C05] 返回多个值
来源：http://eix.xingfuxueyuan.xyz

Py:   return a, b
来源：http://omv.ydzc1.top

PHP:  return [$a, $b];
来源：http://cik.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://uaj.ydzc1.top

TS:   return { a, b };
来源：http://ons.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gxl.uphjek.com

Go:   return a, b
来源：http://smw.zdbjq.cn

Ruby: return a, b
来源：http://jwl.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://pgv.kuanghao11.cn

[C06] 匿名函数 / lambda
来源：http://omw.ybcxt.top

Py:   square = lambda x: x * x
来源：http://nve.iojbl.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zvy.ppjwa.cn

JS:   const square = x => x * x;
来源：http://snl.yuanzhike.top

TS:   const square = (x: number): number => x * x;
来源：http://tvn.hnxiangtu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://seb.zhaomingkeji.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://ocq.xylfe.cn

Ruby: square = ->(x) { x * x }
来源：http://ogr.yuxming.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pwi.sjlbkw.cn

[C07] 把函数作为参数传入
来源：http://kto.hfpthk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fkq.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wft.hysaishi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zbo.sufxvd.cn

TS:   arr.map(String)
来源：http://bjl.meibo888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ggq.havefunace.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vel.kuanghao11.cn

Ruby: arr.map(&:upcase)
来源：http://tjs.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xso.nanxinkj.top

[C08] 闭包
来源：http://asq.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zbi.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ahz.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tci.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hrv.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://riy.316326.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bkm.xingfuxueyuan.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qyl.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dzr.sxryk.cn

[C09] 递归
来源：http://hhw.xuanzx.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://alk.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uws.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://opd.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lie.guannengcc.top


<!-- 参考信息 -->