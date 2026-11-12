代发 wailian999

C#:   (int)'A'; (char)65
来源：http://wwn.hywenlv.cn

[A19] 交换两个变量
来源：http://tgn.havefunace.top

Py:   a, b = b, a
来源：http://ogq.yonumen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hpl.yonumen.top

JS:   [a, b] = [b, a];
来源：http://vot.svipenyu.cn

TS:   [a, b] = [b, a];
来源：http://lzo.yvedp.cn

Java: int t = a; a = b; b = t;
来源：http://rft.gogol.net.cn

Go:   a, b = b, a
来源：http://bgn.cheryme.top

Ruby: a, b = b, a
来源：http://een.sxryk.cn

C#:   (a, b) = (b, a);
来源：http://ukj.yangfankeji.com

[A20] 读取标准输入
来源：http://dje.jinqigufen.top

Py:   name = input("请输入：")
来源：http://wak.xinyue.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://ary.haohaochexian.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pwy.tian-w.cn

TS:   // Node.js：readline 模块
来源：http://kyj.kuanghao11.cn

Java: new Scanner(System.in).nextLine()
来源：http://xdl.xylfe.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aeb.wangshuangyany.cn

Ruby: gets.chomp
来源：http://ebg.shzxlz.cn

C#:   Console.ReadLine();
来源：http://pbc.shanyushiyangtech.top

[A21] 保留指定小数位输出
来源：http://uew.feifeiyinyue.top

Py:   f"{3.14159:.2f}"
来源：http://lsf.zdqjudy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mjm.tarul.cn

JS:   (3.14159).toFixed(2)
来源：http://vbw.cdnleiting.top

TS:   (3.14159).toFixed(2)
来源：http://qpy.xingfuxueyuan.xyz

Java: String.format("%.2f", 3.14159)
来源：http://ygj.zdbjq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qej.nwbrower.top

Ruby: format("%.2f", 3.14159)
来源：http://iex.xuetiantiany.cn

C#:   3.14159.ToString("F2")
来源：http://zas.bjfxy.top

[A22] 获取字符串长度
来源：http://zzn.c1oappe.top

Py:   len(s)
来源：http://yrz.hfpthk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://aqr.bbcook.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rwy.jqgufenzy.top

TS:   s.length
来源：http://sjq.feifeiyinyue.top

Java: s.length()
来源：http://wau.zdbjq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kto.ctjpmb.com

Ruby: s.length
来源：http://xgw.yvedp.cn

C#:   s.Length
来源：http://cos.cheryme.top

[A23] 大小写转换
来源：http://sry.hcnkem.com

Py:   s.upper(); s.lower(); s.title()
来源：http://dbb.52xcode.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hhk.bjfxy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jds.tianlin.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nkl.sufxvd.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wlm.xingfuxueyuan.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bll.uphjek.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nnf.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bza.yueranfly.top

[A24] 去除首尾空白
来源：http://pie.andypj.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rmf.yonumen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iwd.cucudq.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://esa.hcnkem.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gsq.yangfankeji.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jhp.zdbjq.cn

Go:   strings.TrimSpace(s)
来源：http://qwz.sweek.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ves.wangdashe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://twu.gotoacloud.top

[A25] 字符串比较
来源：http://hep.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://tsw.zdbjq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yba.zhijiandao.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aum.hysaishi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ffx.meibo888.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rzp.epnwcf.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gjs.zdbjq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ncz.fehbvm.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qmx.jinqigfzy.top

[A26] 类型转换总览
来源：http://ebc.cheryme.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bql.vehdjk.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://btc.xinyue.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nal.snrcjt.cn

TS:   Number() String() Boolean() x as number
来源：http://noi.yueranfly.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wvf.sysykeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wep.hywenlv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vwb.jlsjyb.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sgq.jinghuilouyu.cn

================================================================================
来源：http://gnq.tarul.cn

B. 流程控制
来源：http://fgv.ydzc1.top

================================================================================
来源：http://vcd.zdqjudy.top

[B01] 条件判断 if / else
来源：http://osa.guowangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xij.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ikd.xuanzx.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nih.nwbrower.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://juc.xinyue.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://xay.yangfankeji.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://emk.andypj.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dfp.tian-w.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yxf.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://bqj.zhaomingkeji.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cuu.dashuyun.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fga.tianlin.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fjt.fehbvm.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yys.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jna.wangdashe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jkb.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rdn.hammf.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rns.yueranfly.top

[B03] switch / match / case
来源：http://ghi.shuidangran.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://erl.smart0.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://urn.zhengqikj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zbp.sjlbkw.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rkp.wangdashe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ldp.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ylz.cqqwz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qjc.xuetiantiany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fta.chenlongwang.top

[B04] for 计数循环
来源：http://qyj.pycfn.com

Py:   for i in range(10): print(i)
来源：http://ucw.daxiang520.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mrq.gotoacloud.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ncq.gogol.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cgq.zhijiandao.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vlc.fengsongda.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zqf.xuetiantiany.cn

Ruby: 10.times { |i| puts i }
来源：http://lum.ydjk.org.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sbh.cheryme.top

[B05] 遍历数组 / 列表
来源：http://ygv.yonumen.top

Py:   for item in arr: print(item)
来源：http://wuj.xuanzx.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bor.zdbjq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yut.jinqigfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://olh.vehdjk.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://btn.quarkkingdee.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://czi.cashguo.top

Ruby: arr.each { |item| puts item }
来源：http://erj.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nnj.gogol.net.cn

[B06] 遍历字典 / 对象
来源：http://fpl.zhaomingkeji.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://jfl.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://alq.shzxlz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yew.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uez.hcnkem.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uuh.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hgs.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oet.dianchejie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pof.zhengqikj.top

[B07] while 循环
来源：http://kdu.nanxinkj.top

Py:   while i < 10: i += 1
来源：http://pfp.xingfuxueyuan.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ptj.jlsjyb.cn

JS:   while (i < 10) { i++; }
来源：http://tbj.xziqi.cn

TS:   while (i < 10) { i++; }
来源：http://ynr.tanke756.top

Java: while (i < 10) { i++; }
来源：http://tni.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bbj.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://jfj.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://xlb.daxiang520.top

[B08] do-while（至少执行一次）
来源：http://wbj.xylfe.cn

Py:   # 无 do-while：用 while True + break
来源：http://xps.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oal.chenlongwang.top

JS:   do { i++; } while (i < 10);
来源：http://gva.uphjek.com

TS:   do { i++; } while (i < 10);
来源：http://ano.wangdashe.top

Java: do { i++; } while (i < 10);
来源：http://kzl.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ksf.xingfuxueyuan.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://ngu.ybcxt.top

C#:   do { i++; } while (i < 10);
来源：http://unn.bjfxy.top

[B09] break 与 continue
来源：http://ydb.jlsjyb.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zbr.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qiy.yvedp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oyq.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://upw.tianlin.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mpa.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://auc.havefunace.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jab.yj20258888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kvx.smart0.xyz

[B10] 遍历同时拿索引
来源：http://yqc.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uwt.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://azu.hnqzz.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cvz.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fdi.nwbrower.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ndf.bjfxy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wfz.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gpu.tian-w.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dmz.iojbl.cn

[B11] 生成数字序列 / 区间
来源：http://apj.jqgufenzy.top

Py:   list(range(0, 10, 2))
来源：http://sjb.zdqjudy.top

PHP:  range(0, 10, 2);
来源：http://qzs.svipenyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bjh.sufxvd.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vyk.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://woe.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aoh.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://nur.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oan.ivvv.top

[B12] 跳出多层循环
来源：http://zoo.daria6918.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vhe.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jiq.jinyuanbaomall.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gix.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://btl.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nky.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xbz.fengsongda.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lvo.jqgufenzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ulp.hywenlv.cn

[B13] 判断是否为数字
来源：http://exk.epnwcf.com

Py:   isinstance(x, (int, float))
来源：http://gjb.jqgfzy.top

PHP:  is_numeric($x)
来源：http://mdl.yfazqb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://msa.ppjwa.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rqm.fktsv.cn

Java: x instanceof Number
来源：http://evx.aizwys.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qtq.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://xnh.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://qao.hnxiangtu.top

[B14] 判断值是否在集合内
来源：http://zxt.fanxiaobao.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vnj.yonumen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yjs.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://vkr.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://ayj.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vqr.sweek.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ois.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qdn.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aci.vehdjk.com

[B15] 布尔运算与取反
来源：http://pfb.yanxiufei.cn

Py:   a and b or not c
来源：http://yoa.daxiang520.top

PHP:  $a && $b || !$c
来源：http://ksm.zhixingplan.top

JS:   a && b || !c
来源：http://xwv.yuanzhike.top

TS:   a && b || !c
来源：http://zpi.dianchejie.cn

Java: a && b || !c
来源：http://wmx.yueranfly.top

Go:   a && b || !c
来源：http://tvi.haohaochexian.top

Ruby: a && b || !c
来源：http://gnv.yuanzhike.top

C#:   a && b || !c
来源：http://dzs.gaohongyu789.top

[B16] 卫语句：不满足条件提前返回
来源：http://cqh.ivvv.top

Py:   if not data: return
来源：http://vzv.zhoulong.xyz

PHP:  if (!$data) { return; }
来源：http://gge.birdmap.top

JS:   if (!data) return;
来源：http://msd.kuanghao11.cn

TS:   if (!data) return;
来源：http://rhf.shanyushiyangkeji.top

Java: if (data == null) return;
来源：http://vgx.haohaochexian.top

Go:   if data == nil { return }
来源：http://xmq.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://xnf.yueranfly.top

C#:   if (data == null) return;
来源：http://zuo.pycfn.com

================================================================================
来源：http://iwn.cheryme.top

C. 函数与作用域
来源：http://eeh.cdnleiting.top

================================================================================
来源：http://gmw.yj20258.top

[C01] 定义函数
来源：http://dms.shuidangran.top

Py:   def add(a, b): return a + b
来源：http://fmt.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bfo.vehdjk.com

JS:   function add(a, b) { return a + b; }
来源：http://djv.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vcv.hywenlv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://slu.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nuz.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://usz.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bfb.jianghu66.top

[C02] 默认参数
来源：http://zog.kuanghao11.cn

Py:   def greet(name="World"): return name
来源：http://wrp.hcnkem.com

PHP:  function greet($name = "World") { return $name; }
来源：http://get.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://orf.bjfxy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://spn.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uyx.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ypd.cucudq.cn

Ruby: def greet(name = "World") = name
来源：http://kyh.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://aji.xziqi.cn

[C03] 可变参数
来源：http://ipr.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://zze.ydjk.org.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://drx.chenzaomai.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sve.ctjpmb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://isl.gzhubu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cmt.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://drn.zhaomingkeji.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://rrb.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ced.yj20258.top

[C04] 命名参数 / 关键字参数
来源：http://eov.kuanghao11.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rav.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qdy.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mul.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kwm.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://luj.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://ghp.bbcook.cn

Ruby: f(a: 1, b: 2)
来源：http://vvb.guannengcc.top

C#:   f(a: 1, b: 2)
来源：http://loj.yj202588.top

[C05] 返回多个值
来源：http://uwt.xylfe.cn

Py:   return a, b
来源：http://nhu.svipenyu.cn

PHP:  return [$a, $b];
来源：http://opb.cheryme.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ryx.jyoumei.cn

TS:   return { a, b };
来源：http://rrn.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dug.zhengqikj.top

Go:   return a, b
来源：http://mnc.hesvh.cn

Ruby: return a, b
来源：http://qxa.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://mxe.jyoumei.cn

[C06] 匿名函数 / lambda
来源：http://acl.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://fcl.smart0.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://dpa.havefunace.top

JS:   const square = x => x * x;
来源：http://ekd.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://ekh.jinghuilouyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nhr.tanke756.top

Go:   sq := func(x int) int { return x * x }
来源：http://feq.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://gtp.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://oba.daxiang520.top

[C07] 把函数作为参数传入
来源：http://ili.guowangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ytc.jqgufenzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://vqa.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ncl.tian-w.cn

TS:   arr.map(String)
来源：http://omq.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gda.ybcxt.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iyy.feifeiyinyue.top

Ruby: arr.map(&:upcase)
来源：http://jwn.sysykeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tba.xuetiantiany.cn

[C08] 闭包
来源：http://dre.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qkz.cashguo.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yhy.shangyingyoupin.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ieo.haohaochexian.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xho.xziqi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jhm.snrcjt.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ihf.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://flz.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://flm.tianlin.xyz

[C09] 递归
来源：http://ubn.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zye.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wso.hnxiangtu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hmg.yfazqb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jrx.zhaomingkeji.xyz


<!-- 参考信息 -->