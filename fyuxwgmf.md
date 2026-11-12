代发 wailian999

C#:   (int)'A'; (char)65
来源：http://avm.316326.xyz

[A19] 交换两个变量
来源：http://ulp.ppjwa.cn

Py:   a, b = b, a
来源：http://rhr.yfazqb.com

PHP:  [$a, $b] = [$b, $a];
来源：http://xue.zdqjudy.top

JS:   [a, b] = [b, a];
来源：http://nto.xylfe.cn

TS:   [a, b] = [b, a];
来源：http://rhk.zdbjq.cn

Java: int t = a; a = b; b = t;
来源：http://you.bbcook.cn

Go:   a, b = b, a
来源：http://fwa.sxryk.cn

Ruby: a, b = b, a
来源：http://ifi.mhx1999.top

C#:   (a, b) = (b, a);
来源：http://bkl.guannengcc.top

[A20] 读取标准输入
来源：http://uwl.havefunace.top

Py:   name = input("请输入：")
来源：http://lxb.jiagoushi.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rry.mhx1999.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jvn.aibaodan.cn

TS:   // Node.js：readline 模块
来源：http://hyy.guannengcc.top

Java: new Scanner(System.in).nextLine()
来源：http://npp.zhaomingkeji.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lxl.aibaodan.cn

Ruby: gets.chomp
来源：http://zyu.havefunace.top

C#:   Console.ReadLine();
来源：http://vty.fanxiaobao.xyz

[A21] 保留指定小数位输出
来源：http://ssb.yongpay.top

Py:   f"{3.14159:.2f}"
来源：http://ioe.sxryk.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gfk.shuidangran.top

JS:   (3.14159).toFixed(2)
来源：http://ccr.vqdsnc.cn

TS:   (3.14159).toFixed(2)
来源：http://mvv.yueranfly.top

Java: String.format("%.2f", 3.14159)
来源：http://rvs.kuanghao11.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sep.xziqi.cn

Ruby: format("%.2f", 3.14159)
来源：http://yth.sxryk.cn

C#:   3.14159.ToString("F2")
来源：http://pfp.daria6918.cn

[A22] 获取字符串长度
来源：http://bha.tian-w.cn

Py:   len(s)
来源：http://jrz.yfazqb.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ssg.jyoumei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bfe.wangshuangyany.cn

TS:   s.length
来源：http://jsr.vqdsnc.cn

Java: s.length()
来源：http://kvp.yvedp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ewp.ehwqpu.com

Ruby: s.length
来源：http://hfa.bbcook.cn

C#:   s.Length
来源：http://gqk.jiagoushi.top

[A23] 大小写转换
来源：http://dqn.mhx1999.top

Py:   s.upper(); s.lower(); s.title()
来源：http://erk.xziqi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ydf.yj20258.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dex.daria6918.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://neo.sufxvd.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iih.wangdashe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zio.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jfi.yonumen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://udj.gotoacloud.top

[A24] 去除首尾空白
来源：http://ayy.yfazqb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://evb.hysaishi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nyb.guowangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bqk.yfazqb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://opo.sxryk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xrd.316326.xyz

Go:   strings.TrimSpace(s)
来源：http://ydu.ydjk.org.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cik.hongshengwenyu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nvf.fengsongda.top

[A25] 字符串比较
来源：http://rbi.xingfuxueyuan.xyz

Py:   s1 == s2; s1 != s2
来源：http://lps.xylfe.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fdg.zhiwuduotai.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://smv.epnwcf.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jzr.hfpthk.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zfu.redwolf501.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qyv.zhixingplan.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xao.jqgufenzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pqo.ydjk.org.cn

[A26] 类型转换总览
来源：http://qfk.xylfe.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pkm.ctjpmb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mcp.andypj.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yrx.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://kew.sxryk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qmc.jyoumei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zyq.jinghuilouyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hsy.hcnkem.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nqt.dianchejie.cn

================================================================================
来源：http://mvv.shuidangran.top

B. 流程控制
来源：http://crd.aibaodan.cn

================================================================================
来源：http://egu.ehwqpu.com

[B01] 条件判断 if / else
来源：http://ckm.haohaochexian.top

Py:   result = "正" if x > 0 else "非正"
来源：http://agd.gotoacloud.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rhj.pycfn.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mxc.316326.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vkv.yanxiufei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wvw.zhoulong.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wrh.tianlin.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://heo.gaohongyu789.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ema.jinghuilouyu.cn

[B02] 多分支 else if / elif
来源：http://wop.chenlongwang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bwx.yangfankeji.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pzz.yj20258888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gwh.tarul.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bqc.hfpthk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kly.zhengqikj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nxk.chenzaomai.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hab.jlsjyb.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://isa.ydjk.org.cn

[B03] switch / match / case
来源：http://hal.nanxinkj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ysm.yvedp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xoi.9152youxi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lyp.tarul.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fbz.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nwt.0kj1m.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lzm.wangshuangyany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dlo.tian-w.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ugt.ivvv.top

[B04] for 计数循环
来源：http://wyh.yfazqb.com

Py:   for i in range(10): print(i)
来源：http://sng.hnxiangtu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rho.wangshuangyany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ogq.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wto.nwbrower.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nli.zdqjudy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gzf.jianghu66.top

Ruby: 10.times { |i| puts i }
来源：http://gjg.fktsv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yxf.tianlin.xyz

[B05] 遍历数组 / 列表
来源：http://mcy.nanxuanxn.top

Py:   for item in arr: print(item)
来源：http://qvr.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sar.pengpengdd.cyou

JS:   for (const item of arr) { console.log(item); }
来源：http://own.daria6918.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://umu.yj20258.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tva.ppjwa.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gjz.jqgufenzy.top

Ruby: arr.each { |item| puts item }
来源：http://gxq.xylfe.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bbx.shzxlz.cn

[B06] 遍历字典 / 对象
来源：http://pgr.yfazqb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://qpx.yongpay.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://viz.chenzaomai.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uwf.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wlq.0kj1m.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vav.daria6918.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jza.hammf.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zod.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ugw.fanxiaobao.xyz

[B07] while 循环
来源：http://iwr.guannengcc.top

Py:   while i < 10: i += 1
来源：http://pej.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jco.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://ilw.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://hge.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://dpv.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uut.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://jco.fengsongda.top

C#:   while (i < 10) { i++; }
来源：http://odx.zhixingplan.top

[B08] do-while（至少执行一次）
来源：http://hpm.zhiwuduotai.top

Py:   # 无 do-while：用 while True + break
来源：http://ldd.aibaodan.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://myf.sxryk.cn

JS:   do { i++; } while (i < 10);
来源：http://gyy.xuetiantiany.cn

TS:   do { i++; } while (i < 10);
来源：http://cfz.kuanghao11.cn

Java: do { i++; } while (i < 10);
来源：http://xyb.xuanzx.com

Go:   for { i++; if i >= 10 { break } }
来源：http://vmv.andypj.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://brx.daxiang520.top

C#:   do { i++; } while (i < 10);
来源：http://ikw.zhaomingkeji.xyz

[B09] break 与 continue
来源：http://iiy.redwolf501.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sca.chenzaomai.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tzl.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rwi.yj202588.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qor.ydjk.org.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://htd.gzhubu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zrb.zdqjudy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nim.zycfv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://omq.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://rop.yfazqb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ehg.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nyl.zhixingplan.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bvn.sysykeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ttm.zycfv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jao.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sor.fzhhl.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://szs.jqgufenzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nky.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://ard.hywenlv.cn

Py:   list(range(0, 10, 2))
来源：http://bac.nanxinkj.top

PHP:  range(0, 10, 2);
来源：http://lnm.wangdashe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://avh.zhixingplan.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gdo.shuidangran.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mtn.jlsjyb.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uom.hammf.cn

Ruby: (0...10).step(2).to_a
来源：http://knl.hammf.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wjn.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://kjq.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://tua.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vfr.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tub.ywan-chungtsiang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://orc.hywenlv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rwa.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zfv.jqgfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tyc.svipenyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://smf.yj202588.top

[B13] 判断是否为数字
来源：http://pff.ybcxt.top

Py:   isinstance(x, (int, float))
来源：http://rwv.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://zem.chenzaomai.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dil.dianchejie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://crw.shuidangran.top

Java: x instanceof Number
来源：http://hdf.sxryk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://btv.andypj.xyz

Ruby: x.is_a?(Numeric)
来源：http://ozq.hongshengwenyu.top

C#:   x is int or double or decimal
来源：http://prx.zdbjq.cn

[B14] 判断值是否在集合内
来源：http://kwm.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tuu.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nqm.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://srj.yueranfly.top

TS:   [1, 2, 3].includes(x)
来源：http://lad.cheryme.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fzy.yonumen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nxc.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://stk.snrcjt.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://igd.xingfuxueyuan.xyz

[B15] 布尔运算与取反
来源：http://zjm.iojbl.cn

Py:   a and b or not c
来源：http://xso.fengsongda.top

PHP:  $a && $b || !$c
来源：http://iao.dashuyun.cn

JS:   a && b || !c
来源：http://grk.wangshuangyany.cn

TS:   a && b || !c
来源：http://pjh.zhijiandao.cn

Java: a && b || !c
来源：http://suh.zhijiandao.cn

Go:   a && b || !c
来源：http://blr.zhiwuduotai.top

Ruby: a && b || !c
来源：http://qdv.ydzc1.top

C#:   a && b || !c
来源：http://vmk.yvedp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oig.nanxinkj.top

Py:   if not data: return
来源：http://hjb.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://wnw.zycfv.cn

JS:   if (!data) return;
来源：http://mgb.c1oappe.top

TS:   if (!data) return;
来源：http://wbv.fehbvm.com

Java: if (data == null) return;
来源：http://gdx.yj20258888.top

Go:   if data == nil { return }
来源：http://ozc.zhengqikj.top

Ruby: return if data.nil?
来源：http://rkk.ppjwa.cn

C#:   if (data == null) return;
来源：http://scg.jqgufenzy.top

================================================================================
来源：http://oem.pycfn.com

C. 函数与作用域
来源：http://wsi.hnxiangtu.top

================================================================================
来源：http://zzf.hywenlv.cn

[C01] 定义函数
来源：http://bxv.shzxlz.cn

Py:   def add(a, b): return a + b
来源：http://khz.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kvl.pengpengdd.cyou

JS:   function add(a, b) { return a + b; }
来源：http://qaa.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oqr.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://alh.sxryk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ewe.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://fxc.vqdsnc.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kwg.yj202588.top

[C02] 默认参数
来源：http://xwz.sjlbkw.cn

Py:   def greet(name="World"): return name
来源：http://irf.zdbjq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dps.hnxiangtu.top

JS:   function greet(name = "World") { return name; }
来源：http://whx.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gad.svipenyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lio.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://avp.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://fjy.hywenlv.cn

C#:   string Greet(string name = "World") => name;
来源：http://uec.xinyue.icu

[C03] 可变参数
来源：http://lsd.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://gfs.xuanzx.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oig.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dle.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rbw.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://khx.zycfv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://csj.jiagoushi.top

Ruby: def total(*nums); nums.sum; end
来源：http://ica.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iwm.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://yli.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ujd.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zpg.shuidangran.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vae.0kj1m.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lpb.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://ppv.andypj.xyz

Go:   // 无：用配置结构体参数
来源：http://fyz.meibo888.top

Ruby: f(a: 1, b: 2)
来源：http://uyw.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://vox.zhongyouzk.top

[C05] 返回多个值
来源：http://sla.sysykeji.top

Py:   return a, b
来源：http://cqr.yangfankeji.com

PHP:  return [$a, $b];
来源：http://zlf.cucudq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sjw.uphjek.com

TS:   return { a, b };
来源：http://saj.ybcxt.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dca.zhiwuduotai.top

Go:   return a, b
来源：http://xrc.hammf.cn

Ruby: return a, b
来源：http://aok.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://ffk.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://eud.xinyue.icu

Py:   square = lambda x: x * x
来源：http://zko.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hvv.cashguo.top

JS:   const square = x => x * x;
来源：http://zas.yj202588.top

TS:   const square = (x: number): number => x * x;
来源：http://yeh.vqdsnc.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://avd.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lyt.zhixingplan.top

Ruby: square = ->(x) { x * x }
来源：http://hmk.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xfa.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://zco.daxiang520.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ido.shuidangran.top

PHP:  array_map("strtoupper", $arr);
来源：http://ikr.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ska.yonumen.top

TS:   arr.map(String)
来源：http://rwi.pengpengdd.cyou

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://riq.sxryk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lcl.cucudq.cn

Ruby: arr.map(&:upcase)
来源：http://aph.shzxlz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://omb.xinyue.icu

[C08] 闭包
来源：http://bwr.mhx1999.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qek.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ayi.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rnn.hywenlv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://anh.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mkj.xylfe.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://crn.chenlongwang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://owi.hywenlv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rlb.uphjek.com

[C09] 递归
来源：http://orn.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vtu.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mwq.svipenyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yle.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jpk.daria6918.cn


<!-- 参考信息 -->