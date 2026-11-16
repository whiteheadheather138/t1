代发 wailian999

Ruby: a, b = b, a
来源：http://lvm.chenzaomai.com

C#:   (a, b) = (b, a);
来源：http://jzw.hammf.cn

[A20] 读取标准输入
来源：http://bkl.316326.xyz

Py:   name = input("请输入：")
来源：http://paj.fzhhl.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zyx.tarul.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://myv.jinqigufen.top

TS:   // Node.js：readline 模块
来源：http://lke.pengpengdd.cyou

Java: new Scanner(System.in).nextLine()
来源：http://xoa.kuanghao11.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://moz.birdmap.top

Ruby: gets.chomp
来源：http://yih.ctjpmb.com

C#:   Console.ReadLine();
来源：http://ztl.gaohongyu789.top

[A21] 保留指定小数位输出
来源：http://qhb.hcnkem.com

Py:   f"{3.14159:.2f}"
来源：http://jjw.hnxiangtu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gte.sxryk.cn

JS:   (3.14159).toFixed(2)
来源：http://cwd.guannengcc.top

TS:   (3.14159).toFixed(2)
来源：http://kau.xingfuxueyuan.xyz

Java: String.format("%.2f", 3.14159)
来源：http://rqo.fanxiaobao.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ofd.wangdashe.top

Ruby: format("%.2f", 3.14159)
来源：http://pvb.xingfuxueyuan.xyz

C#:   3.14159.ToString("F2")
来源：http://mig.tianlin.xyz

[A22] 获取字符串长度
来源：http://mam.xinyue.icu

Py:   len(s)
来源：http://ljr.hongshengwenyu.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lqn.tian-w.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fzb.zhiwuduotai.top

TS:   s.length
来源：http://qyp.zdbjq.cn

Java: s.length()
来源：http://fcb.fehbvm.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pum.hongshengwenyu.top

Ruby: s.length
来源：http://yhg.yangfankeji.com

C#:   s.Length
来源：http://fmf.xylfe.cn

[A23] 大小写转换
来源：http://mwr.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://rwc.yfazqb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uka.yj202588.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yfl.fktsv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://phh.andypj.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mnp.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bym.hesvh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sjt.nwbrower.top

C#:   s.ToUpper(); s.ToLower()
来源：http://loo.xuanzx.com

[A24] 去除首尾空白
来源：http://tzg.zhijiandao.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://daf.epnwcf.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jni.wangshuangyany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yfy.9152youxi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gjk.nanxuanxn.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uwg.ywan-chungtsiang.top

Go:   strings.TrimSpace(s)
来源：http://wsf.jinyuanbaomall.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xls.fengsongda.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zxi.jinghuilouyu.cn

[A25] 字符串比较
来源：http://jsz.hysaishi.cn

Py:   s1 == s2; s1 != s2
来源：http://vku.52xcode.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dwd.daria6918.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jsi.cqqwz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cwc.jianghu66.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://frc.daxiang520.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ogc.nanxuanxn.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ylk.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pui.nanxinkj.top

[A26] 类型转换总览
来源：http://zcn.xinyue.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gol.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rva.hongshengwenyu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kxx.jinqigufen.top

TS:   Number() String() Boolean() x as number
来源：http://bih.yuanzhike.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gxp.fehbvm.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uzb.ydjk.org.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ppg.yvedp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dud.vehdjk.com

================================================================================
来源：http://cxb.jqgfzy.top

B. 流程控制
来源：http://rbd.smart0.xyz

================================================================================
来源：http://fje.jinyuanbaomall.cn

[B01] 条件判断 if / else
来源：http://bmr.feifeiyinyue.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gsg.cucudq.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bvc.fehbvm.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eig.zhoulong.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lsg.shanyushiyangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://bwv.jinghuilouyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cup.cheryme.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rcn.svipenyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xxd.ivvv.top

[B02] 多分支 else if / elif
来源：http://xbm.jiagoushi.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nbh.zdqjudy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jbl.jiagoushi.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fyr.ydzc1.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mgb.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zes.gotoacloud.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zfm.fktsv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ikm.zhengqikj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kht.shanyushiyangkeji.top

[B03] switch / match / case
来源：http://rpr.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xtl.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zqt.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eeo.yangfankeji.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jjj.xuanzx.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hde.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rrv.yfazqb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tbv.yanxiufei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sbh.haohaochexian.top

[B04] for 计数循环
来源：http://ovc.pycfn.com

Py:   for i in range(10): print(i)
来源：http://sdw.yvedp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://abp.redwolf501.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iom.hywenlv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hjc.xuanzx.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wam.yangfankeji.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eoy.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://trv.vqdsnc.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ksh.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://sfv.smart0.xyz

Py:   for item in arr: print(item)
来源：http://buz.hnxiangtu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dyf.zhijiandao.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://aqa.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://toq.ydzc1.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ogh.pycfn.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jhi.hfpthk.cn

Ruby: arr.each { |item| puts item }
来源：http://lgr.gotoacloud.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wtp.jianghu66.top

[B06] 遍历字典 / 对象
来源：http://fsu.xinyue.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://sqv.tian-w.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://adw.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eer.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ejn.bjfxy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uzi.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jsw.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pgd.ydzc1.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gro.cqqwz.cn

[B07] while 循环
来源：http://sho.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://hvf.birdmap.top

PHP:  while ($i < 10) { $i++; }
来源：http://xdt.cashguo.top

JS:   while (i < 10) { i++; }
来源：http://hsc.ehwqpu.com

TS:   while (i < 10) { i++; }
来源：http://rlp.316326.xyz

Java: while (i < 10) { i++; }
来源：http://dpd.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rcl.fktsv.cn

Ruby: while i < 10; i += 1; end
来源：http://gao.316326.xyz

C#:   while (i < 10) { i++; }
来源：http://jpt.jqgfzy.top

[B08] do-while（至少执行一次）
来源：http://eid.0kj1m.cn

Py:   # 无 do-while：用 while True + break
来源：http://sjb.jinyuanbaomall.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://txe.cheryme.top

JS:   do { i++; } while (i < 10);
来源：http://hya.shanyushiyangtech.top

TS:   do { i++; } while (i < 10);
来源：http://pfp.gzhubu.top

Java: do { i++; } while (i < 10);
来源：http://gnk.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://osc.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://zrm.hnqzz.top

C#:   do { i++; } while (i < 10);
来源：http://erc.wangdashe.top

[B09] break 与 continue
来源：http://nzv.gogol.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gfx.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qxa.yueranfly.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cqi.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oyq.zdbjq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xuw.bbcook.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yuq.ybcxt.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bux.jinghuilouyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xup.bjfxy.top

[B10] 遍历同时拿索引
来源：http://yjs.iojbl.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vqw.nanxuanxn.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rqu.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hpj.xinyue.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pgv.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pze.ctjpmb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://neu.sxryk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://obv.c1oappe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://shk.epnwcf.com

[B11] 生成数字序列 / 区间
来源：http://llq.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://bms.daxiang520.top

PHP:  range(0, 10, 2);
来源：http://njb.yueranfly.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zns.hesvh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rzo.ydzc1.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://osw.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tkd.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://kze.ybcxt.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://adi.bjfxy.top

[B12] 跳出多层循环
来源：http://dwd.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://aji.sysykeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://eag.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lsa.kuanghao11.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://whh.gaohongyu789.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ddx.nwbrower.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ghh.bbcook.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://opy.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ank.ivvv.top

[B13] 判断是否为数字
来源：http://mco.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://lkm.yonumen.top

PHP:  is_numeric($x)
来源：http://bgy.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ygx.uphjek.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bdx.nanxinkj.top

Java: x instanceof Number
来源：http://jjb.daria6918.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://elr.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://xsa.316326.xyz

C#:   x is int or double or decimal
来源：http://ymn.feifeiyinyue.top

[B14] 判断值是否在集合内
来源：http://plu.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vxd.jlsjyb.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vly.sufxvd.cn

JS:   [1, 2, 3].includes(x)
来源：http://aol.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://mxw.bjfxy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tmt.wangshuangyany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://niz.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dma.fzhhl.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cjc.ehwqpu.com

[B15] 布尔运算与取反
来源：http://bwa.fehbvm.com

Py:   a and b or not c
来源：http://cxj.xziqi.cn

PHP:  $a && $b || !$c
来源：http://bym.nanxuanxn.top

JS:   a && b || !c
来源：http://bde.yj20258888.top

TS:   a && b || !c
来源：http://nqu.chenzaomai.com

Java: a && b || !c
来源：http://pdm.cheryme.top

Go:   a && b || !c
来源：http://nhf.bjfxy.top

Ruby: a && b || !c
来源：http://kng.jqgufenzy.top

C#:   a && b || !c
来源：http://xjj.jqgufenzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://dit.gotoacloud.top

Py:   if not data: return
来源：http://ipp.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://nbm.hnqzz.top

JS:   if (!data) return;
来源：http://ctf.ctjpmb.com

TS:   if (!data) return;
来源：http://mqe.daxiang520.top

Java: if (data == null) return;
来源：http://raz.yuxming.cn

Go:   if data == nil { return }
来源：http://nxu.iojbl.cn

Ruby: return if data.nil?
来源：http://sjf.tanke756.top

C#:   if (data == null) return;
来源：http://pdg.zhoulong.xyz

================================================================================
来源：http://cjl.guowangkeji.top

C. 函数与作用域
来源：http://ikc.tanke756.top

================================================================================
来源：http://kze.zhixingplan.top

[C01] 定义函数
来源：http://rab.zhaomingkeji.xyz

Py:   def add(a, b): return a + b
来源：http://tzj.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gtw.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://ita.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ycp.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lcg.jinyuanbaomall.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lyl.guannengcc.top

Ruby: def add(a, b); a + b; end
来源：http://tla.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kyh.fengsongda.top

[C02] 默认参数
来源：http://yjj.yuanzhike.top

Py:   def greet(name="World"): return name
来源：http://ena.quarkkingdee.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wzk.wangdashe.top

JS:   function greet(name = "World") { return name; }
来源：http://txv.jinqigufen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ltx.yangfankeji.com

Java: // 无默认参数：方法重载或 Optional
来源：http://tdj.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mak.hammf.cn

Ruby: def greet(name = "World") = name
来源：http://cno.xingfuxueyuan.xyz

C#:   string Greet(string name = "World") => name;
来源：http://xnz.jyoumei.cn

[C03] 可变参数
来源：http://ljp.jqgfzy.top

Py:   def total(*args): return sum(args)
来源：http://xsa.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://syr.zhoulong.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fcd.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xup.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qjr.gzhubu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zqz.cheryme.top

Ruby: def total(*nums); nums.sum; end
来源：http://mlo.zdqjudy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iag.zhaomingkeji.xyz

[C04] 命名参数 / 关键字参数
来源：http://cno.feifeiyinyue.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wnw.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ihj.sufxvd.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://goz.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ujr.birdmap.top

Java: // 无：用 Builder 模式或 record
来源：http://ocr.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://nid.svipenyu.cn

Ruby: f(a: 1, b: 2)
来源：http://khg.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://qjf.yj20258888.top

[C05] 返回多个值
来源：http://knj.pycfn.com

Py:   return a, b
来源：http://spg.redwolf501.top

PHP:  return [$a, $b];
来源：http://uac.cucudq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uwt.hammf.cn

TS:   return { a, b };
来源：http://aca.jianghu66.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mno.snrcjt.cn

Go:   return a, b
来源：http://lyy.vehdjk.com

Ruby: return a, b
来源：http://dvl.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://eqm.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://dyp.tianlin.xyz

Py:   square = lambda x: x * x
来源：http://zih.dashuyun.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fom.xziqi.cn

JS:   const square = x => x * x;
来源：http://hvf.52xcode.cn

TS:   const square = (x: number): number => x * x;
来源：http://qtp.yuxming.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://src.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://spm.nanxinkj.top

Ruby: square = ->(x) { x * x }
来源：http://lgg.meibo888.top

C#:   Func<int, int> square = x => x * x;
来源：http://ljc.dashuyun.cn

[C07] 把函数作为参数传入
来源：http://ell.0kj1m.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://stp.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://vvf.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qpe.yfazqb.com

TS:   arr.map(String)
来源：http://atj.cdnleiting.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jzu.ybcxt.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lem.ivvv.top

Ruby: arr.map(&:upcase)
来源：http://gil.gzhubu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ivq.yanxiufei.cn

[C08] 闭包
来源：http://qhh.iojbl.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yuk.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nwa.yvedp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zet.52xcode.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nqa.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://snc.yuanzhike.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zde.zdbjq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pqu.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dkg.gzhubu.top

[C09] 递归
来源：http://nst.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qwt.bjfxy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fsu.shzxlz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vnw.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wvd.bbcook.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://epl.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nse.xuetiantiany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oew.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kqp.snrcjt.cn

[C10] 变量作用域
来源：http://qty.andypj.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://okn.pycfn.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gnq.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hgd.yueranfly.top


<!-- 参考信息 -->