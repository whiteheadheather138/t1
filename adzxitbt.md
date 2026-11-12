代发 wailian999

Ruby: a, b = b, a
来源：http://mxk.tarul.cn

C#:   (a, b) = (b, a);
来源：http://cmo.dashuyun.cn

[A20] 读取标准输入
来源：http://lok.epnwcf.com

Py:   name = input("请输入：")
来源：http://acz.cqqwz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://txg.haohaochexian.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tfu.quarkkingdee.top

TS:   // Node.js：readline 模块
来源：http://jle.aibaodan.cn

Java: new Scanner(System.in).nextLine()
来源：http://bkc.yj202588.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://msi.nanxuanxn.top

Ruby: gets.chomp
来源：http://smg.9152youxi.cn

C#:   Console.ReadLine();
来源：http://ril.yuanzhike.top

[A21] 保留指定小数位输出
来源：http://nny.yvedp.cn

Py:   f"{3.14159:.2f}"
来源：http://cli.hfpthk.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://swp.yfazqb.com

JS:   (3.14159).toFixed(2)
来源：http://aun.tarul.cn

TS:   (3.14159).toFixed(2)
来源：http://bmg.yongpay.top

Java: String.format("%.2f", 3.14159)
来源：http://jha.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oqr.xinyue.icu

Ruby: format("%.2f", 3.14159)
来源：http://akc.sufxvd.cn

C#:   3.14159.ToString("F2")
来源：http://eov.sxryk.cn

[A22] 获取字符串长度
来源：http://eyw.sweek.top

Py:   len(s)
来源：http://igq.xuetiantiany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gnk.yonumen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hrc.daxiang520.top

TS:   s.length
来源：http://fmp.chenzaomai.com

Java: s.length()
来源：http://jeh.yanxiufei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xfb.tianlin.xyz

Ruby: s.length
来源：http://wcw.yvedp.cn

C#:   s.Length
来源：http://tos.fzhhl.top

[A23] 大小写转换
来源：http://ytu.hnxiangtu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://osh.jyoumei.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eba.chenjidiqi.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mde.tian-w.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bur.feifeiyinyue.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uae.chenlongwang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ula.gaohongyu789.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ivd.ehwqpu.com

C#:   s.ToUpper(); s.ToLower()
来源：http://vui.zhiwuduotai.top

[A24] 去除首尾空白
来源：http://fwv.quarkkingdee.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dad.vehdjk.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qih.zhengqikj.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jql.daria6918.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://afn.pycfn.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cay.jqgufenzy.top

Go:   strings.TrimSpace(s)
来源：http://asz.hnqzz.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xyc.epnwcf.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mis.chenzaomai.com

[A25] 字符串比较
来源：http://jkm.52xcode.cn

Py:   s1 == s2; s1 != s2
来源：http://jcx.fengsongda.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tey.ywan-chungtsiang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oqx.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vtx.sjlbkw.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gqb.zhaomingkeji.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ptt.guowangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://sar.zdbjq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ezm.epnwcf.com

[A26] 类型转换总览
来源：http://xpj.xuanzx.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pgv.haohaochexian.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eqr.hfpthk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gbb.cucudq.cn

TS:   Number() String() Boolean() x as number
来源：http://lri.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lpb.hywenlv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ipy.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vcw.tarul.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xpj.xuetiantiany.cn

================================================================================
来源：http://zol.cucudq.cn

B. 流程控制
来源：http://ejk.birdmap.top

================================================================================
来源：http://qyu.tanke756.top

[B01] 条件判断 if / else
来源：http://utu.hysaishi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jha.havefunace.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vqp.zdqjudy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jww.316326.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rvd.xziqi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mvc.gotoacloud.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mdt.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kxe.ivvv.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mxg.nanxuanxn.top

[B02] 多分支 else if / elif
来源：http://ozs.redwolf501.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jwq.hongshengwenyu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ooh.guowangkeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://erm.gogol.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://orl.guannengcc.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ihm.zhengqikj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://owg.tarul.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bpl.zhixingplan.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kbc.fehbvm.com

[B03] switch / match / case
来源：http://qqq.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yhs.zhiwuduotai.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ela.ywan-chungtsiang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://teh.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sbb.shanyushiyangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zok.hammf.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ezj.jinghuilouyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oko.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sdl.tanke756.top

[B04] for 计数循环
来源：http://xsh.jinqigufen.top

Py:   for i in range(10): print(i)
来源：http://jkg.yvedp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xnu.yueranfly.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rsc.hammf.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://avs.xinyue.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ycj.chenzaomai.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sut.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://bxb.jinqigufen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://woc.gotoacloud.top

[B05] 遍历数组 / 列表
来源：http://fsi.ppjwa.cn

Py:   for item in arr: print(item)
来源：http://gmx.52xcode.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ied.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://pnz.birdmap.top

TS:   for (const item of arr) { console.log(item); }
来源：http://pcv.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ado.xuanzx.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xcp.jinghuilouyu.cn

Ruby: arr.each { |item| puts item }
来源：http://fbn.hesvh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://swe.sxryk.cn

[B06] 遍历字典 / 对象
来源：http://dbk.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://unu.fengsongda.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wvr.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://puj.fzhhl.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bqs.smart0.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pmn.aizwys.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sso.yj202588.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fpl.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://noj.yfazqb.com

[B07] while 循环
来源：http://jyj.zhixingplan.top

Py:   while i < 10: i += 1
来源：http://rpw.bbcook.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bgb.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://upj.sjlbkw.cn

TS:   while (i < 10) { i++; }
来源：http://prd.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://yns.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yom.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://ifz.aibaodan.cn

C#:   while (i < 10) { i++; }
来源：http://rsc.sweek.top

[B08] do-while（至少执行一次）
来源：http://qqk.xylfe.cn

Py:   # 无 do-while：用 while True + break
来源：http://znc.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nbs.gotoacloud.top

JS:   do { i++; } while (i < 10);
来源：http://ttg.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://qak.sufxvd.cn

Java: do { i++; } while (i < 10);
来源：http://whi.cheryme.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tzv.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://cfw.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://chh.ydzc1.top

[B09] break 与 continue
来源：http://vam.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sxh.hcnkem.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oky.316326.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://giv.chenlongwang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fos.yvedp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fmk.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cpd.yj20258.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qhr.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xyh.quarkkingdee.top

[B10] 遍历同时拿索引
来源：http://bzj.kuanghao11.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nyv.dashuyun.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tmk.yueranfly.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ydg.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iqc.vehdjk.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zms.zdbjq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://spk.jyoumei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fek.ywan-chungtsiang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iau.sxryk.cn

[B11] 生成数字序列 / 区间
来源：http://lwx.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://xuf.bjfxy.top

PHP:  range(0, 10, 2);
来源：http://yvv.pengpengdd.cyou

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://meo.zhixingplan.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nel.nanxuanxn.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://stz.andypj.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jff.daxiang520.top

Ruby: (0...10).step(2).to_a
来源：http://ttb.sjlbkw.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nrf.birdmap.top

[B12] 跳出多层循环
来源：http://rwa.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://vmw.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oxr.zhijiandao.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yan.yj202588.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://clf.shanyushiyangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yte.nwbrower.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gko.aizwys.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xsw.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wbi.xziqi.cn

[B13] 判断是否为数字
来源：http://lwl.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://ntj.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://guh.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bbq.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mea.zdqjudy.top

Java: x instanceof Number
来源：http://zim.chenlongwang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ise.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://zlg.yangfankeji.com

C#:   x is int or double or decimal
来源：http://rhu.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://jog.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jlk.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vml.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://vkf.hongshengwenyu.top

TS:   [1, 2, 3].includes(x)
来源：http://cxk.yj20258888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pud.ywan-chungtsiang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ieq.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://roy.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mgh.pycfn.com

[B15] 布尔运算与取反
来源：http://vqv.cqqwz.cn

Py:   a and b or not c
来源：http://rgy.jianghu66.top

PHP:  $a && $b || !$c
来源：http://ibm.xylfe.cn

JS:   a && b || !c
来源：http://wxk.jlsjyb.cn

TS:   a && b || !c
来源：http://zst.daxiang520.top

Java: a && b || !c
来源：http://anx.epnwcf.com

Go:   a && b || !c
来源：http://bsy.jiagoushi.top

Ruby: a && b || !c
来源：http://eyg.jqgfzy.top

C#:   a && b || !c
来源：http://tpm.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ywr.sjlbkw.cn

Py:   if not data: return
来源：http://rtk.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://gnj.chenlongwang.top

JS:   if (!data) return;
来源：http://spn.hywenlv.cn

TS:   if (!data) return;
来源：http://qtb.epnwcf.com

Java: if (data == null) return;
来源：http://gbw.meibo888.top

Go:   if data == nil { return }
来源：http://olw.sxryk.cn

Ruby: return if data.nil?
来源：http://ciq.fengsongda.top

C#:   if (data == null) return;
来源：http://rrv.ppjwa.cn

================================================================================
来源：http://mua.sweek.top

C. 函数与作用域
来源：http://kvy.fehbvm.com

================================================================================
来源：http://ncq.fktsv.cn

[C01] 定义函数
来源：http://eid.vehdjk.com

Py:   def add(a, b): return a + b
来源：http://siq.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xiv.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://ifr.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jqw.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://rmo.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://ygq.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://prp.yfazqb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jrh.birdmap.top

[C02] 默认参数
来源：http://dua.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://kzq.jinghuilouyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://var.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://cmg.jyoumei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://aqt.sweek.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gpr.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ipi.epnwcf.com

Ruby: def greet(name = "World") = name
来源：http://lya.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://irn.redwolf501.top

[C03] 可变参数
来源：http://tem.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://pca.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yen.dianchejie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ycc.quarkkingdee.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rif.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qeo.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://coq.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zpf.ywan-chungtsiang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kef.zhixingplan.top

[C04] 命名参数 / 关键字参数
来源：http://hbi.cucudq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xsl.jlsjyb.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fep.yuxming.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nmd.ybcxt.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://del.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://thy.tian-w.cn

Go:   // 无：用配置结构体参数
来源：http://udy.fehbvm.com

Ruby: f(a: 1, b: 2)
来源：http://ane.nanxuanxn.top

C#:   f(a: 1, b: 2)
来源：http://mir.316326.xyz

[C05] 返回多个值
来源：http://sqi.dianchejie.cn

Py:   return a, b
来源：http://iwq.guannengcc.top

PHP:  return [$a, $b];
来源：http://pil.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bri.snrcjt.cn

TS:   return { a, b };
来源：http://yjr.nwbrower.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pdt.tarul.cn

Go:   return a, b
来源：http://xbh.hongshengwenyu.top

Ruby: return a, b
来源：http://dzp.andypj.xyz

C#:   return (a, b);              // ValueTuple
来源：http://gjx.jianghu66.top

[C06] 匿名函数 / lambda
来源：http://kob.tanke756.top

Py:   square = lambda x: x * x
来源：http://qmo.jinqigufen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qig.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://fks.yj202588.top

TS:   const square = (x: number): number => x * x;
来源：http://ozg.iojbl.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hgy.chenlongwang.top

Go:   sq := func(x int) int { return x * x }
来源：http://hyl.zhaomingkeji.xyz

Ruby: square = ->(x) { x * x }
来源：http://gnp.svipenyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lcm.nwbrower.top

[C07] 把函数作为参数传入
来源：http://ijd.vehdjk.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hxa.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://swn.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rjn.jqgufenzy.top

TS:   arr.map(String)
来源：http://ndu.xylfe.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vro.tanke756.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tcx.fengsongda.top

Ruby: arr.map(&:upcase)
来源：http://mpu.jiagoushi.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fju.aizwys.cn

[C08] 闭包
来源：http://uhy.sxryk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jno.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mqa.zycfv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://szv.chenzaomai.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sny.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bzx.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gph.bjfxy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dbg.kuanghao11.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zli.bjfxy.top

[C09] 递归
来源：http://upm.cheryme.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hem.9152youxi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oys.tarul.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://foc.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ncz.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ega.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ubv.zycfv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://opm.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://awg.fktsv.cn

[C10] 变量作用域
来源：http://czc.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vzg.ppjwa.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pxn.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fqi.ppjwa.cn


<!-- 参考信息 -->