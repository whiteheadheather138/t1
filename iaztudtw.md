代发 wailian999

C#:   (int)'A'; (char)65
来源：http://wzc.pycfn.com

[A19] 交换两个变量
来源：http://jje.chenzaomai.com

Py:   a, b = b, a
来源：http://slm.hammf.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kgr.zhiwuduotai.top

JS:   [a, b] = [b, a];
来源：http://sbj.zhaomingkeji.xyz

TS:   [a, b] = [b, a];
来源：http://ltu.52xcode.cn

Java: int t = a; a = b; b = t;
来源：http://rqd.bjfxy.top

Go:   a, b = b, a
来源：http://jxa.ywan-chungtsiang.top

Ruby: a, b = b, a
来源：http://opg.nanxuanxn.top

C#:   (a, b) = (b, a);
来源：http://kqb.zhaomingkeji.xyz

[A20] 读取标准输入
来源：http://aia.cashguo.top

Py:   name = input("请输入：")
来源：http://vqq.snrcjt.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gms.ctjpmb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kxq.yangfankeji.com

TS:   // Node.js：readline 模块
来源：http://set.snrcjt.cn

Java: new Scanner(System.in).nextLine()
来源：http://ubc.fehbvm.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uvy.tianlin.xyz

Ruby: gets.chomp
来源：http://cva.tian-w.cn

C#:   Console.ReadLine();
来源：http://ntr.jianghu66.top

[A21] 保留指定小数位输出
来源：http://wwd.zhoulong.xyz

Py:   f"{3.14159:.2f}"
来源：http://rqc.sxryk.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://icw.yfazqb.com

JS:   (3.14159).toFixed(2)
来源：http://wmn.cqqwz.cn

TS:   (3.14159).toFixed(2)
来源：http://xle.daxiang520.top

Java: String.format("%.2f", 3.14159)
来源：http://tqg.tanke756.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ush.hywenlv.cn

Ruby: format("%.2f", 3.14159)
来源：http://kpn.pengpengdd.cyou

C#:   3.14159.ToString("F2")
来源：http://ayp.sjlbkw.cn

[A22] 获取字符串长度
来源：http://uwy.epnwcf.com

Py:   len(s)
来源：http://uik.wangshuangyany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rqf.fzhhl.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ecp.cqqwz.cn

TS:   s.length
来源：http://pip.shuidangran.top

Java: s.length()
来源：http://fdu.nanxuanxn.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uqz.ctjpmb.com

Ruby: s.length
来源：http://shf.xuanzx.com

C#:   s.Length
来源：http://zkn.kuanghao11.cn

[A23] 大小写转换
来源：http://leg.ctjpmb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://zic.gotoacloud.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aie.hcnkem.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wam.havefunace.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zue.sweek.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fgs.ehwqpu.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cde.fengsongda.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ime.tianlin.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://rfm.gogol.net.cn

[A24] 去除首尾空白
来源：http://pru.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eqw.mhx1999.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kny.hongshengwenyu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rvx.daria6918.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nau.guannengcc.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gtz.yj20258.top

Go:   strings.TrimSpace(s)
来源：http://jpk.tian-w.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://chf.chenjidiqi.icu

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jeo.xinyue.icu

[A25] 字符串比较
来源：http://lbp.zhaomingkeji.xyz

Py:   s1 == s2; s1 != s2
来源：http://ssg.mhx1999.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xqk.gaohongyu789.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iqg.jlsjyb.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iaw.hesvh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://obb.pengpengdd.cyou

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wvr.zycfv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://udi.vqdsnc.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tnu.daxiang520.top

[A26] 类型转换总览
来源：http://zlx.shanyushiyangtech.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://igk.yangfankeji.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qhl.hammf.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uel.zdbjq.cn

TS:   Number() String() Boolean() x as number
来源：http://xgq.vqdsnc.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kxa.jyoumei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://elf.cheryme.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vco.9152youxi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gbx.jianghu66.top

================================================================================
来源：http://znu.andypj.xyz

B. 流程控制
来源：http://ghy.tarul.cn

================================================================================
来源：http://cos.tian-w.cn

[B01] 条件判断 if / else
来源：http://alm.9152youxi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://onk.bjfxy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nbg.epnwcf.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xbh.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oxk.guowangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mtu.ywan-chungtsiang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wjz.havefunace.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lry.sysykeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hlu.ybcxt.top

[B02] 多分支 else if / elif
来源：http://lub.xuanzx.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eum.jqgfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mih.cashguo.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zme.mhx1999.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vvl.sjlbkw.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ocj.jinqigufen.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rgy.zhaomingkeji.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tue.ivvv.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xvo.zhixingplan.top

[B03] switch / match / case
来源：http://jjw.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fzr.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lbo.cucudq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pxa.shzxlz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tdh.hammf.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dhi.chenlongwang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bfy.zhixingplan.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://osr.yangfankeji.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ulv.sweek.top

[B04] for 计数循环
来源：http://jyh.shanyushiyangtech.top

Py:   for i in range(10): print(i)
来源：http://kbu.daria6918.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zsg.birdmap.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zyb.9152youxi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jfj.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zir.ehwqpu.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://csj.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://ehf.smart0.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wzy.ydzc1.top

[B05] 遍历数组 / 列表
来源：http://onw.sufxvd.cn

Py:   for item in arr: print(item)
来源：http://kwo.tian-w.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sur.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://orn.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jvj.shuidangran.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ytd.nwbrower.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ayg.yonumen.top

Ruby: arr.each { |item| puts item }
来源：http://ius.sufxvd.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kud.havefunace.top

[B06] 遍历字典 / 对象
来源：http://vkg.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wfa.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cin.havefunace.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wdv.52xcode.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jrf.tian-w.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qad.c1oappe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xsh.zhiwuduotai.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://frj.yj202588.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gdc.yj202588.top

[B07] while 循环
来源：http://ifp.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://gie.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://jae.zhixingplan.top

JS:   while (i < 10) { i++; }
来源：http://luv.ywan-chungtsiang.top

TS:   while (i < 10) { i++; }
来源：http://bzg.xziqi.cn

Java: while (i < 10) { i++; }
来源：http://wge.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baa.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://zln.sweek.top

C#:   while (i < 10) { i++; }
来源：http://pbd.zdqjudy.top

[B08] do-while（至少执行一次）
来源：http://dul.jinqigfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://oyy.xylfe.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://izz.wangshuangyany.cn

JS:   do { i++; } while (i < 10);
来源：http://bib.aizwys.cn

TS:   do { i++; } while (i < 10);
来源：http://glx.ehwqpu.com

Java: do { i++; } while (i < 10);
来源：http://uax.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lsb.yuanzhike.top

Ruby: begin; i += 1; end while i < 10
来源：http://ets.zhijiandao.cn

C#:   do { i++; } while (i < 10);
来源：http://vcx.yuxming.cn

[B09] break 与 continue
来源：http://qfn.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ado.tanke756.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pat.tarul.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lsc.haohaochexian.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jua.haohaochexian.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jnu.hfpthk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wyy.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mig.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://slq.haohaochexian.top

[B10] 遍历同时拿索引
来源：http://oyc.xylfe.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hdv.daria6918.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mnh.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vnj.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qkp.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yrp.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://god.hesvh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ldc.chenlongwang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pyd.hnqzz.top

[B11] 生成数字序列 / 区间
来源：http://wwm.yuxming.cn

Py:   list(range(0, 10, 2))
来源：http://nko.haohaochexian.top

PHP:  range(0, 10, 2);
来源：http://exa.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ncr.shuidangran.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aln.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cfy.hywenlv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bjk.yj202588.top

Ruby: (0...10).step(2).to_a
来源：http://ssb.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uee.zhengqikj.top

[B12] 跳出多层循环
来源：http://wiz.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zxl.shangyingyoupin.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qtu.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://scy.snrcjt.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qvf.smart0.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qvx.haohaochexian.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hks.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qot.sxryk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fek.zdbjq.cn

[B13] 判断是否为数字
来源：http://adi.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://yam.yuanzhike.top

PHP:  is_numeric($x)
来源：http://xct.52xcode.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zyu.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nzw.fengsongda.top

Java: x instanceof Number
来源：http://dwr.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kur.mhx1999.top

Ruby: x.is_a?(Numeric)
来源：http://naf.zhaomingkeji.xyz

C#:   x is int or double or decimal
来源：http://nkr.wangdashe.top

[B14] 判断值是否在集合内
来源：http://mqp.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zbp.yanxiufei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aun.shuidangran.top

JS:   [1, 2, 3].includes(x)
来源：http://wka.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ekf.sufxvd.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mtg.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aig.svipenyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mta.haohaochexian.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mel.ppjwa.cn

[B15] 布尔运算与取反
来源：http://xsh.yj20258888.top

Py:   a and b or not c
来源：http://pyn.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://uik.wangdashe.top

JS:   a && b || !c
来源：http://yvx.fktsv.cn

TS:   a && b || !c
来源：http://ypf.xuanzx.com

Java: a && b || !c
来源：http://pkm.quarkkingdee.top

Go:   a && b || !c
来源：http://drr.iojbl.cn

Ruby: a && b || !c
来源：http://xqo.hnxiangtu.top

C#:   a && b || !c
来源：http://dxh.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://nxf.wangdashe.top

Py:   if not data: return
来源：http://jfr.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://rqc.jianghu66.top

JS:   if (!data) return;
来源：http://xnm.tarul.cn

TS:   if (!data) return;
来源：http://ika.xinyue.icu

Java: if (data == null) return;
来源：http://adt.0kj1m.cn

Go:   if data == nil { return }
来源：http://htc.c1oappe.top

Ruby: return if data.nil?
来源：http://ito.cucudq.cn

C#:   if (data == null) return;
来源：http://vvn.tanke756.top

================================================================================
来源：http://nhv.ehwqpu.com

C. 函数与作用域
来源：http://bhs.ehwqpu.com

================================================================================
来源：http://qnz.xinyue.icu

[C01] 定义函数
来源：http://oex.tianlin.xyz

Py:   def add(a, b): return a + b
来源：http://jyl.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xty.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://uso.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jha.chenlongwang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ggt.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://sji.cdnleiting.top

Ruby: def add(a, b); a + b; end
来源：http://rfd.hfpthk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ait.quarkkingdee.top

[C02] 默认参数
来源：http://arg.wangdashe.top

Py:   def greet(name="World"): return name
来源：http://pwy.jinqigufen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dto.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://vvp.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vkg.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ofl.cqqwz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sog.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://laf.yanxiufei.cn

C#:   string Greet(string name = "World") => name;
来源：http://nqg.xziqi.cn

[C03] 可变参数
来源：http://zvh.jlsjyb.cn

Py:   def total(*args): return sum(args)
来源：http://lvn.316326.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hlj.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hov.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zst.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wjf.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lyo.fengsongda.top

Ruby: def total(*nums); nums.sum; end
来源：http://yqk.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ddf.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://sqr.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cvy.jqgfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dsc.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kpz.wangshuangyany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lxi.guannengcc.top

Java: // 无：用 Builder 模式或 record
来源：http://prl.vehdjk.com

Go:   // 无：用配置结构体参数
来源：http://gyn.havefunace.top

Ruby: f(a: 1, b: 2)
来源：http://upq.tianlin.xyz

C#:   f(a: 1, b: 2)
来源：http://tkt.zdbjq.cn

[C05] 返回多个值
来源：http://zmh.mhx1999.top

Py:   return a, b
来源：http://xpg.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://qph.zhengqikj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nkn.9152youxi.cn

TS:   return { a, b };
来源：http://kxr.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fpg.pycfn.com

Go:   return a, b
来源：http://pir.zhiwuduotai.top

Ruby: return a, b
来源：http://byr.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://mqj.sweek.top

[C06] 匿名函数 / lambda
来源：http://gke.jqgfzy.top

Py:   square = lambda x: x * x
来源：http://nnv.zhongyouzk.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mst.zhaomingkeji.xyz

JS:   const square = x => x * x;
来源：http://gfp.andypj.xyz

TS:   const square = (x: number): number => x * x;
来源：http://yok.vqdsnc.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dck.zhiwuduotai.top

Go:   sq := func(x int) int { return x * x }
来源：http://eae.sxryk.cn

Ruby: square = ->(x) { x * x }
来源：http://ted.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://kne.c1oappe.top

[C07] 把函数作为参数传入
来源：http://ije.shuidangran.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://icz.birdmap.top

PHP:  array_map("strtoupper", $arr);
来源：http://eli.ywan-chungtsiang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gue.hysaishi.cn

TS:   arr.map(String)
来源：http://cvv.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ohq.zhengqikj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xrp.havefunace.top

Ruby: arr.map(&:upcase)
来源：http://eyi.hywenlv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jyz.zhaomingkeji.xyz

[C08] 闭包
来源：http://roe.iojbl.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://spo.hesvh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xer.chenzaomai.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pwm.cucudq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hrb.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wov.hnqzz.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zse.yuxming.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zfs.shanyushiyangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dxh.yuxming.cn

[C09] 递归
来源：http://yip.tanke756.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wfs.yonumen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://coc.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eyi.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xqw.hammf.cn


<!-- 参考信息 -->