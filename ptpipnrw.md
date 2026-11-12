代发 wailian999

JS:   [a, b] = [b, a];
来源：http://ndr.kuanghao11.cn

TS:   [a, b] = [b, a];
来源：http://vpf.daxiang520.top

Java: int t = a; a = b; b = t;
来源：http://acx.gzhubu.top

Go:   a, b = b, a
来源：http://jfu.jinyuanbaomall.cn

Ruby: a, b = b, a
来源：http://lmt.kuanghao11.cn

C#:   (a, b) = (b, a);
来源：http://mct.sxryk.cn

[A20] 读取标准输入
来源：http://rad.shangyingyoupin.top

Py:   name = input("请输入：")
来源：http://gqc.yj20258888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://uht.zycfv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://aen.yuanzhike.top

TS:   // Node.js：readline 模块
来源：http://bqc.guowangkeji.top

Java: new Scanner(System.in).nextLine()
来源：http://cxc.hysaishi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nqe.iojbl.cn

Ruby: gets.chomp
来源：http://qhr.shanyushiyangkeji.top

C#:   Console.ReadLine();
来源：http://fex.hywenlv.cn

[A21] 保留指定小数位输出
来源：http://tie.yuxming.cn

Py:   f"{3.14159:.2f}"
来源：http://jwx.gotoacloud.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://plz.sufxvd.cn

JS:   (3.14159).toFixed(2)
来源：http://epz.yangfankeji.com

TS:   (3.14159).toFixed(2)
来源：http://quo.jyoumei.cn

Java: String.format("%.2f", 3.14159)
来源：http://oio.cqqwz.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sqp.haohaochexian.top

Ruby: format("%.2f", 3.14159)
来源：http://fcj.yvedp.cn

C#:   3.14159.ToString("F2")
来源：http://veg.yj20258.top

[A22] 获取字符串长度
来源：http://xzc.c1oappe.top

Py:   len(s)
来源：http://hlq.havefunace.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wzs.wangshuangyany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dag.shangyingyoupin.top

TS:   s.length
来源：http://iyg.jqgufenzy.top

Java: s.length()
来源：http://rzv.quarkkingdee.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jhz.yj202588.top

Ruby: s.length
来源：http://lxc.dashuyun.cn

C#:   s.Length
来源：http://cci.316326.xyz

[A23] 大小写转换
来源：http://zqo.zhengqikj.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ooq.zhaomingkeji.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oxk.gogol.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yhw.shzxlz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tkl.ctjpmb.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wpb.bbcook.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://skt.xuanzx.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sot.chenzaomai.com

C#:   s.ToUpper(); s.ToLower()
来源：http://vkb.wangshuangyany.cn

[A24] 去除首尾空白
来源：http://pjq.nanxinkj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kch.chenzaomai.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dmo.0kj1m.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rtq.xziqi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://szv.hysaishi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yax.ctjpmb.com

Go:   strings.TrimSpace(s)
来源：http://sln.hnxiangtu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hgx.tianlin.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zkc.hysaishi.cn

[A25] 字符串比较
来源：http://pct.andypj.xyz

Py:   s1 == s2; s1 != s2
来源：http://mcm.redwolf501.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qna.havefunace.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wwo.fehbvm.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xll.jinqigufen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sln.andypj.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rjf.xziqi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pbo.316326.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://syg.svipenyu.cn

[A26] 类型转换总览
来源：http://syd.yj202588.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xcp.xuetiantiany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hhi.andypj.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ens.zhengqikj.top

TS:   Number() String() Boolean() x as number
来源：http://qhd.yj202588.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mpu.sweek.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zhg.cucudq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mhk.epnwcf.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gsr.aizwys.cn

================================================================================
来源：http://qyr.mhx1999.top

B. 流程控制
来源：http://lir.mhx1999.top

================================================================================
来源：http://ymx.ppjwa.cn

[B01] 条件判断 if / else
来源：http://nyf.yueranfly.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tkc.vehdjk.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://erl.yvedp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sor.zycfv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://syq.pengpengdd.cyou

Java: String r = x > 0 ? "正" : "非正";
来源：http://whk.yj20258888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://frg.fzhhl.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bpu.pengpengdd.cyou

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ekz.yuanzhike.top

[B02] 多分支 else if / elif
来源：http://ggv.kuanghao11.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jdd.hongshengwenyu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wmv.fzhhl.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://izt.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://btn.hnqzz.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rwx.shzxlz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tmz.jinqigfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dom.zhengqikj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iqa.hongshengwenyu.top

[B03] switch / match / case
来源：http://qxe.jinghuilouyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ver.wangshuangyany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://joo.gogol.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zex.zycfv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bok.shanyushiyangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wta.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qkr.hywenlv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hsm.zhoulong.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uvn.birdmap.top

[B04] for 计数循环
来源：http://ssg.daria6918.cn

Py:   for i in range(10): print(i)
来源：http://iia.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ozj.wangshuangyany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eju.guowangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dgw.cqqwz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mob.nanxuanxn.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wxv.9152youxi.cn

Ruby: 10.times { |i| puts i }
来源：http://day.uphjek.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ima.ydzc1.top

[B05] 遍历数组 / 列表
来源：http://dud.shzxlz.cn

Py:   for item in arr: print(item)
来源：http://mmt.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qje.vehdjk.com

JS:   for (const item of arr) { console.log(item); }
来源：http://snr.sweek.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mks.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lcv.gotoacloud.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xza.aibaodan.cn

Ruby: arr.each { |item| puts item }
来源：http://xbu.jinyuanbaomall.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zxu.zdqjudy.top

[B06] 遍历字典 / 对象
来源：http://inm.wangshuangyany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qxz.ydjk.org.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ewt.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kxv.yj20258.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ncx.xingfuxueyuan.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xlp.bjfxy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dwl.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gbe.gzhubu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pln.aibaodan.cn

[B07] while 循环
来源：http://uvs.0kj1m.cn

Py:   while i < 10: i += 1
来源：http://ylf.gotoacloud.top

PHP:  while ($i < 10) { $i++; }
来源：http://dyw.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://ice.ctjpmb.com

TS:   while (i < 10) { i++; }
来源：http://ljq.jqgufenzy.top

Java: while (i < 10) { i++; }
来源：http://fhw.chenlongwang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://quz.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://asm.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://bwn.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://bsz.pycfn.com

Py:   # 无 do-while：用 while True + break
来源：http://iek.sufxvd.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nxg.xziqi.cn

JS:   do { i++; } while (i < 10);
来源：http://ykz.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://zet.nanxinkj.top

Java: do { i++; } while (i < 10);
来源：http://jbn.yanxiufei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sqs.jiagoushi.top

Ruby: begin; i += 1; end while i < 10
来源：http://hqs.vqdsnc.cn

C#:   do { i++; } while (i < 10);
来源：http://jvz.andypj.xyz

[B09] break 与 continue
来源：http://nfa.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pum.svipenyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://quz.hesvh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jlv.zhijiandao.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ybe.hcnkem.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vsx.sjlbkw.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nru.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://phf.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://npc.fehbvm.com

[B10] 遍历同时拿索引
来源：http://xme.yongpay.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fpj.fengsongda.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hyh.redwolf501.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fjo.ydzc1.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zpg.cheryme.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sok.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zqg.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ugm.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pdp.c1oappe.top

[B11] 生成数字序列 / 区间
来源：http://xdh.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://sub.uphjek.com

PHP:  range(0, 10, 2);
来源：http://klz.birdmap.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ufj.jinghuilouyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jzj.kuanghao11.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bjr.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vfz.xingfuxueyuan.xyz

Ruby: (0...10).step(2).to_a
来源：http://xcl.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dhz.hesvh.cn

[B12] 跳出多层循环
来源：http://dyx.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://biv.yj20258888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qce.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jnq.sysykeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gcm.yj20258888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://neu.pengpengdd.cyou

Go:   # 无标签：用布尔标志或抽成函数
来源：http://svg.chenlongwang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pxl.guannengcc.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gsr.jyoumei.cn

[B13] 判断是否为数字
来源：http://wqp.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://kyc.sweek.top

PHP:  is_numeric($x)
来源：http://jqh.c1oappe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xwq.jinqigufen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://isv.chenlongwang.top

Java: x instanceof Number
来源：http://lzh.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mng.316326.xyz

Ruby: x.is_a?(Numeric)
来源：http://cgd.ydjk.org.cn

C#:   x is int or double or decimal
来源：http://hpt.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://mhu.epnwcf.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cnb.xylfe.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://odj.hammf.cn

JS:   [1, 2, 3].includes(x)
来源：http://leu.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://iwi.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://djg.cucudq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nis.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://vub.meibo888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wog.xziqi.cn

[B15] 布尔运算与取反
来源：http://ffr.yvedp.cn

Py:   a and b or not c
来源：http://fev.jqgufenzy.top

PHP:  $a && $b || !$c
来源：http://cfr.yueranfly.top

JS:   a && b || !c
来源：http://dme.zhixingplan.top

TS:   a && b || !c
来源：http://ivm.meibo888.top

Java: a && b || !c
来源：http://kdw.wangshuangyany.cn

Go:   a && b || !c
来源：http://zrp.gaohongyu789.top

Ruby: a && b || !c
来源：http://dch.sweek.top

C#:   a && b || !c
来源：http://rct.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ptz.sweek.top

Py:   if not data: return
来源：http://ibu.yongpay.top

PHP:  if (!$data) { return; }
来源：http://ngg.hesvh.cn

JS:   if (!data) return;
来源：http://npy.fktsv.cn

TS:   if (!data) return;
来源：http://uaa.jinqigfzy.top

Java: if (data == null) return;
来源：http://czy.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://sjq.nanxinkj.top

Ruby: return if data.nil?
来源：http://kkz.gotoacloud.top

C#:   if (data == null) return;
来源：http://rgy.quarkkingdee.top

================================================================================
来源：http://kzo.zycfv.cn

C. 函数与作用域
来源：http://kkb.gotoacloud.top

================================================================================
来源：http://bxi.iojbl.cn

[C01] 定义函数
来源：http://fyk.hywenlv.cn

Py:   def add(a, b): return a + b
来源：http://dns.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xtj.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://sma.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uyn.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://nfo.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://gmp.ybcxt.top

Ruby: def add(a, b); a + b; end
来源：http://twz.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zah.fehbvm.com

[C02] 默认参数
来源：http://lia.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://urn.sjlbkw.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mov.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://wyh.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://orn.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hbc.chenzaomai.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cwu.sweek.top

Ruby: def greet(name = "World") = name
来源：http://yfz.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://zrs.nanxuanxn.top

[C03] 可变参数
来源：http://sgk.pycfn.com

Py:   def total(*args): return sum(args)
来源：http://osh.shuidangran.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rcr.wangdashe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bbx.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aqf.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zvu.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ldz.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mht.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://crt.zhaomingkeji.xyz

[C04] 命名参数 / 关键字参数
来源：http://lou.jinqigfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lru.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fbz.chenlongwang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rdb.cqqwz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yfi.yj202588.top

Java: // 无：用 Builder 模式或 record
来源：http://elh.bbcook.cn

Go:   // 无：用配置结构体参数
来源：http://czs.dianchejie.cn

Ruby: f(a: 1, b: 2)
来源：http://gbz.jinghuilouyu.cn

C#:   f(a: 1, b: 2)
来源：http://mkz.yangfankeji.com

[C05] 返回多个值
来源：http://jls.ivvv.top

Py:   return a, b
来源：http://jfn.hnqzz.top

PHP:  return [$a, $b];
来源：http://cmk.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rzj.jinghuilouyu.cn

TS:   return { a, b };
来源：http://tdd.shanyushiyangtech.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gud.shanyushiyangtech.top

Go:   return a, b
来源：http://wtc.shuidangran.top

Ruby: return a, b
来源：http://geq.jinghuilouyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://ybq.vqdsnc.cn

[C06] 匿名函数 / lambda
来源：http://kof.yangfankeji.com

Py:   square = lambda x: x * x
来源：http://ogv.chenzaomai.com

PHP:  $square = fn($x) => $x * $x;
来源：http://cxg.dashuyun.cn

JS:   const square = x => x * x;
来源：http://uwr.ybcxt.top

TS:   const square = (x: number): number => x * x;
来源：http://hhp.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://goq.sweek.top

Go:   sq := func(x int) int { return x * x }
来源：http://wtk.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://fqi.yuxming.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kvi.yj202588.top

[C07] 把函数作为参数传入
来源：http://hrh.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ekp.ywan-chungtsiang.top

PHP:  array_map("strtoupper", $arr);
来源：http://byf.yangfankeji.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ysm.cqqwz.cn

TS:   arr.map(String)
来源：http://psq.andypj.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yyp.hfpthk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dtv.sweek.top

Ruby: arr.map(&:upcase)
来源：http://vsl.hnqzz.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tgx.chenjidiqi.icu

[C08] 闭包
来源：http://cfc.havefunace.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pxa.bbcook.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://brs.hnqzz.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fiw.yuanzhike.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dsy.tarul.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sud.nwbrower.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xdx.52xcode.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ffp.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bum.pengpengdd.cyou

[C09] 递归
来源：http://ana.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fyd.hnxiangtu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gyc.andypj.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dvu.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qsx.bjfxy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xiv.jyoumei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://izr.vehdjk.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dwx.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://twl.hywenlv.cn


<!-- 参考信息 -->