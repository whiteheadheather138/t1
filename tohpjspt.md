代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://crs.yueranfly.top

Java: (int) 'A'; (char) 65
来源：http://lun.aibaodan.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zkd.xuetiantiany.cn

Ruby: "A".ord; 65.chr
来源：http://zff.hywenlv.cn

C#:   (int)'A'; (char)65
来源：http://wmd.jlsjyb.cn

[A19] 交换两个变量
来源：http://dme.tianlin.xyz

Py:   a, b = b, a
来源：http://vvm.zdbjq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mip.tarul.cn

JS:   [a, b] = [b, a];
来源：http://cus.ydzc1.top

TS:   [a, b] = [b, a];
来源：http://jvd.hnqzz.top

Java: int t = a; a = b; b = t;
来源：http://bsv.hongshengwenyu.top

Go:   a, b = b, a
来源：http://dwo.pycfn.com

Ruby: a, b = b, a
来源：http://zaq.cucudq.cn

C#:   (a, b) = (b, a);
来源：http://hkx.nwbrower.top

[A20] 读取标准输入
来源：http://gxf.gogol.net.cn

Py:   name = input("请输入：")
来源：http://gwa.sjlbkw.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wlu.zhoulong.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yki.zhengqikj.top

TS:   // Node.js：readline 模块
来源：http://umm.gogol.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://wbx.jlsjyb.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://far.haohaochexian.top

Ruby: gets.chomp
来源：http://isw.zhixingplan.top

C#:   Console.ReadLine();
来源：http://poq.zhaomingkeji.xyz

[A21] 保留指定小数位输出
来源：http://ovu.gogol.net.cn

Py:   f"{3.14159:.2f}"
来源：http://gyr.ydjk.org.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rrt.feifeiyinyue.top

JS:   (3.14159).toFixed(2)
来源：http://ofk.yuxming.cn

TS:   (3.14159).toFixed(2)
来源：http://imd.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://jep.daxiang520.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qzj.gotoacloud.top

Ruby: format("%.2f", 3.14159)
来源：http://ist.9152youxi.cn

C#:   3.14159.ToString("F2")
来源：http://yud.sxryk.cn

[A22] 获取字符串长度
来源：http://sbn.jinyuanbaomall.cn

Py:   len(s)
来源：http://vej.zhiwuduotai.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kra.yangfankeji.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ckx.vehdjk.com

TS:   s.length
来源：http://rir.fehbvm.com

Java: s.length()
来源：http://ony.gaohongyu789.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mix.yj20258.top

Ruby: s.length
来源：http://cdr.vehdjk.com

C#:   s.Length
来源：http://iau.hnxiangtu.top

[A23] 大小写转换
来源：http://zqx.ppjwa.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hfa.cheryme.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xvm.ywan-chungtsiang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fow.quarkkingdee.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jub.jinqigfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bva.vqdsnc.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nev.fzhhl.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lip.havefunace.top

C#:   s.ToUpper(); s.ToLower()
来源：http://upb.cheryme.top

[A24] 去除首尾空白
来源：http://hwf.vqdsnc.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bth.dashuyun.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://prg.yangfankeji.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://shq.yj20258888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yrr.andypj.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://boy.cucudq.cn

Go:   strings.TrimSpace(s)
来源：http://bqu.cheryme.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nkv.sysykeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://neq.redwolf501.top

[A25] 字符串比较
来源：http://zbs.snrcjt.cn

Py:   s1 == s2; s1 != s2
来源：http://sqx.ivvv.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zww.cheryme.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yln.havefunace.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ulc.316326.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xxf.cdnleiting.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kww.tarul.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qkc.zycfv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uur.andypj.xyz

[A26] 类型转换总览
来源：http://hyu.cheryme.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fnh.hfpthk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pqq.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qoa.jinghuilouyu.cn

TS:   Number() String() Boolean() x as number
来源：http://ieq.aibaodan.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yij.yj20258888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cgj.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lup.xuetiantiany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ilr.jinyuanbaomall.cn

================================================================================
来源：http://azy.tanke756.top

B. 流程控制
来源：http://hpl.nanxuanxn.top

================================================================================
来源：http://sln.bbcook.cn

[B01] 条件判断 if / else
来源：http://blk.jiagoushi.top

Py:   result = "正" if x > 0 else "非正"
来源：http://beg.sysykeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zcx.yanxiufei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oyi.xylfe.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ufe.shanyushiyangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ngo.chenjidiqi.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jxu.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yjh.redwolf501.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lxp.gogol.net.cn

[B02] 多分支 else if / elif
来源：http://gvt.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://snm.ywan-chungtsiang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gdp.redwolf501.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ugs.ehwqpu.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bpk.zycfv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bhv.xuanzx.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dal.zdbjq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://miq.xinyue.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zwb.aizwys.cn

[B03] switch / match / case
来源：http://guf.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rqq.haohaochexian.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fbu.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vdj.wangshuangyany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zlb.jlsjyb.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gic.snrcjt.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vxk.bbcook.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tjf.svipenyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://umw.bjfxy.top

[B04] for 计数循环
来源：http://lga.guannengcc.top

Py:   for i in range(10): print(i)
来源：http://kyv.bbcook.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yla.jyoumei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ynd.ydjk.org.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lje.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vec.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vya.gaohongyu789.top

Ruby: 10.times { |i| puts i }
来源：http://uzq.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ank.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://xmr.uphjek.com

Py:   for item in arr: print(item)
来源：http://wkc.jqgfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vwo.iojbl.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://une.wangshuangyany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://htg.jinyuanbaomall.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dru.hywenlv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pqa.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://jkv.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yac.zdbjq.cn

[B06] 遍历字典 / 对象
来源：http://ger.cqqwz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jde.shzxlz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sfs.cqqwz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ptc.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://frv.havefunace.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vsw.cdnleiting.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cyr.yvedp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ykl.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ivq.iojbl.cn

[B07] while 循环
来源：http://ewv.zycfv.cn

Py:   while i < 10: i += 1
来源：http://kec.hnqzz.top

PHP:  while ($i < 10) { $i++; }
来源：http://hwn.mhx1999.top

JS:   while (i < 10) { i++; }
来源：http://vth.jlsjyb.cn

TS:   while (i < 10) { i++; }
来源：http://xdc.yj20258.top

Java: while (i < 10) { i++; }
来源：http://yvg.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://onz.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://ehl.snrcjt.cn

C#:   while (i < 10) { i++; }
来源：http://hox.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://qpi.fktsv.cn

Py:   # 无 do-while：用 while True + break
来源：http://qfl.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jsk.ywan-chungtsiang.top

JS:   do { i++; } while (i < 10);
来源：http://jhe.vqdsnc.cn

TS:   do { i++; } while (i < 10);
来源：http://sbo.zhongyouzk.top

Java: do { i++; } while (i < 10);
来源：http://jyk.ehwqpu.com

Go:   for { i++; if i >= 10 { break } }
来源：http://czu.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://iyo.zhijiandao.cn

C#:   do { i++; } while (i < 10);
来源：http://kie.iojbl.cn

[B09] break 与 continue
来源：http://lac.shuidangran.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xoo.pycfn.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hne.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dtp.epnwcf.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kyh.bjfxy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fgf.tanke756.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ttk.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://klp.iojbl.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cry.tanke756.top

[B10] 遍历同时拿索引
来源：http://kdf.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yqt.kuanghao11.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xff.hongshengwenyu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ehc.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jqw.jiagoushi.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nke.sxryk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lsa.xinyue.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cmg.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://key.aibaodan.cn

[B11] 生成数字序列 / 区间
来源：http://fkw.aizwys.cn

Py:   list(range(0, 10, 2))
来源：http://mrs.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://ugy.sjlbkw.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://soe.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cgn.gotoacloud.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fls.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wsw.daria6918.cn

Ruby: (0...10).step(2).to_a
来源：http://lzk.fehbvm.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lkz.yfazqb.com

[B12] 跳出多层循环
来源：http://ayf.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://rof.jianghu66.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://psv.cheryme.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rbn.mhx1999.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jxb.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zdx.snrcjt.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zof.gaohongyu789.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tfj.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vlo.tian-w.cn

[B13] 判断是否为数字
来源：http://sqo.jinghuilouyu.cn

Py:   isinstance(x, (int, float))
来源：http://tkm.nanxinkj.top

PHP:  is_numeric($x)
来源：http://nvw.jyoumei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rtc.guowangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nly.hesvh.cn

Java: x instanceof Number
来源：http://gzn.52xcode.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xdx.zycfv.cn

Ruby: x.is_a?(Numeric)
来源：http://mao.sysykeji.top

C#:   x is int or double or decimal
来源：http://arh.jinqigfzy.top

[B14] 判断值是否在集合内
来源：http://jws.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iul.cucudq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ciw.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://yir.mhx1999.top

TS:   [1, 2, 3].includes(x)
来源：http://tnk.aizwys.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hzx.birdmap.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fon.ppjwa.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qof.jqgufenzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ifc.uphjek.com

[B15] 布尔运算与取反
来源：http://usz.svipenyu.cn

Py:   a and b or not c
来源：http://cxu.tanke756.top

PHP:  $a && $b || !$c
来源：http://sve.ybcxt.top

JS:   a && b || !c
来源：http://yka.ppjwa.cn

TS:   a && b || !c
来源：http://ypd.sufxvd.cn

Java: a && b || !c
来源：http://ylq.9152youxi.cn

Go:   a && b || !c
来源：http://xzi.havefunace.top

Ruby: a && b || !c
来源：http://iwg.sweek.top

C#:   a && b || !c
来源：http://cdg.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://kid.jqgfzy.top

Py:   if not data: return
来源：http://neh.chenjidiqi.icu

PHP:  if (!$data) { return; }
来源：http://fbs.smart0.xyz

JS:   if (!data) return;
来源：http://zln.zhixingplan.top

TS:   if (!data) return;
来源：http://bsv.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://jon.zycfv.cn

Go:   if data == nil { return }
来源：http://cgj.fengsongda.top

Ruby: return if data.nil?
来源：http://wjt.hesvh.cn

C#:   if (data == null) return;
来源：http://mol.chenjidiqi.icu

================================================================================
来源：http://gcc.ivvv.top

C. 函数与作用域
来源：http://mkt.kuanghao11.cn

================================================================================
来源：http://wym.nanxinkj.top

[C01] 定义函数
来源：http://ywq.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://ans.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pja.zycfv.cn

JS:   function add(a, b) { return a + b; }
来源：http://aoy.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ljo.zhengqikj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hny.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://pmg.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://shn.vehdjk.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hhr.shzxlz.cn

[C02] 默认参数
来源：http://hzm.316326.xyz

Py:   def greet(name="World"): return name
来源：http://kky.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xls.aibaodan.cn

JS:   function greet(name = "World") { return name; }
来源：http://rxp.ehwqpu.com

TS:   function greet(name: string = "World") { return name; }
来源：http://xhl.aizwys.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jin.nanxuanxn.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bin.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://xjb.xinyue.icu

C#:   string Greet(string name = "World") => name;
来源：http://snt.quarkkingdee.top

[C03] 可变参数
来源：http://asu.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://jdy.aizwys.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jjh.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://syr.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ptk.zhoulong.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yqj.jiagoushi.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vdn.snrcjt.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dgz.ydjk.org.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oeu.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://ixg.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dtx.ppjwa.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ztx.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wcx.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wxf.yvedp.cn

Java: // 无：用 Builder 模式或 record
来源：http://cus.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://xog.yj202588.top

Ruby: f(a: 1, b: 2)
来源：http://fni.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://omt.guannengcc.top

[C05] 返回多个值
来源：http://hqq.chenlongwang.top

Py:   return a, b
来源：http://gmd.shuidangran.top

PHP:  return [$a, $b];
来源：http://kzk.yj20258.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dlb.tanke756.top

TS:   return { a, b };
来源：http://avd.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ytw.aibaodan.cn

Go:   return a, b
来源：http://abc.nanxuanxn.top

Ruby: return a, b
来源：http://bgs.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://rmv.zhixingplan.top

[C06] 匿名函数 / lambda
来源：http://ndi.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://ncw.dianchejie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rqx.ppjwa.cn

JS:   const square = x => x * x;
来源：http://voy.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://igf.hysaishi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nxn.vqdsnc.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yeo.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://shn.bjfxy.top

C#:   Func<int, int> square = x => x * x;
来源：http://dta.jinghuilouyu.cn

[C07] 把函数作为参数传入
来源：http://hyq.guannengcc.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://opd.hnqzz.top

PHP:  array_map("strtoupper", $arr);
来源：http://wjo.hfpthk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bgs.bbcook.cn

TS:   arr.map(String)
来源：http://uao.fzhhl.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hwi.jinghuilouyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yqz.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://vdm.shzxlz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nfm.sufxvd.cn

[C08] 闭包
来源：http://ldt.yfazqb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gcr.shanyushiyangtech.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zij.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dvc.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iug.sjlbkw.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qba.nwbrower.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://daz.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nrl.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zmn.yuanzhike.top

[C09] 递归
来源：http://mko.yuxming.cn


<!-- 参考信息 -->