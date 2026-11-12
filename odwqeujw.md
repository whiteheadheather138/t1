代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uxp.birdmap.top

Ruby: gets.chomp
来源：http://tzc.epnwcf.com

C#:   Console.ReadLine();
来源：http://yid.fengsongda.top

[A21] 保留指定小数位输出
来源：http://uks.yj202588.top

Py:   f"{3.14159:.2f}"
来源：http://nll.yonumen.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blo.shangyingyoupin.top

JS:   (3.14159).toFixed(2)
来源：http://qdi.wangshuangyany.cn

TS:   (3.14159).toFixed(2)
来源：http://pxc.ppjwa.cn

Java: String.format("%.2f", 3.14159)
来源：http://cxm.mhx1999.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vzp.nanxinkj.top

Ruby: format("%.2f", 3.14159)
来源：http://dnq.sweek.top

C#:   3.14159.ToString("F2")
来源：http://qwj.yvedp.cn

[A22] 获取字符串长度
来源：http://xjs.hesvh.cn

Py:   len(s)
来源：http://cxk.xziqi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ogq.gotoacloud.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nve.birdmap.top

TS:   s.length
来源：http://agv.hnxiangtu.top

Java: s.length()
来源：http://clv.zhiwuduotai.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ple.zhongyouzk.top

Ruby: s.length
来源：http://ybs.yj20258.top

C#:   s.Length
来源：http://vxa.fktsv.cn

[A23] 大小写转换
来源：http://uwb.redwolf501.top

Py:   s.upper(); s.lower(); s.title()
来源：http://zxo.zhengqikj.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gkj.yueranfly.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qla.sysykeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dgm.cheryme.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mcs.redwolf501.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zdd.kuanghao11.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://log.aibaodan.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pgo.jinyuanbaomall.cn

[A24] 去除首尾空白
来源：http://igf.redwolf501.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pnd.feifeiyinyue.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cch.snrcjt.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://btr.guowangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pgt.jinqigufen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wli.svipenyu.cn

Go:   strings.TrimSpace(s)
来源：http://rrj.redwolf501.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rvi.pycfn.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zoz.ppjwa.cn

[A25] 字符串比较
来源：http://kbo.vehdjk.com

Py:   s1 == s2; s1 != s2
来源：http://ygk.xylfe.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fkj.dashuyun.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sdk.tianlin.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cyz.xziqi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mid.yvedp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oqg.yanxiufei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qkb.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fzi.feifeiyinyue.top

[A26] 类型转换总览
来源：http://peg.redwolf501.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vqh.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mwt.yfazqb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zvo.yuxming.cn

TS:   Number() String() Boolean() x as number
来源：http://jnq.sjlbkw.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ehy.yfazqb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mmo.zhoulong.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://nvm.vqdsnc.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iru.fanxiaobao.xyz

================================================================================
来源：http://yyj.cucudq.cn

B. 流程控制
来源：http://nwe.bbcook.cn

================================================================================
来源：http://bno.52xcode.cn

[B01] 条件判断 if / else
来源：http://haw.0kj1m.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pwx.xinyue.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vyt.yanxiufei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zpy.andypj.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pbw.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ayq.yj20258888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lrd.guowangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mgu.smart0.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tpo.chenjidiqi.icu

[B02] 多分支 else if / elif
来源：http://bjz.gotoacloud.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gib.hcnkem.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pao.yuanzhike.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://quc.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sfo.gzhubu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pyk.fengsongda.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cum.xziqi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ywg.yangfankeji.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hmt.xziqi.cn

[B03] switch / match / case
来源：http://nqw.shuidangran.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ojt.jlsjyb.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pyg.cqqwz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ksy.yuanzhike.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wvj.smart0.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iyo.xylfe.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rbf.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lqw.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://luu.chenjidiqi.icu

[B04] for 计数循环
来源：http://bbj.hammf.cn

Py:   for i in range(10): print(i)
来源：http://sap.guannengcc.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vah.nanxuanxn.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://btq.jyoumei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lfz.sweek.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tvf.ydzc1.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fds.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://ujn.zhongyouzk.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fxy.feifeiyinyue.top

[B05] 遍历数组 / 列表
来源：http://sep.dianchejie.cn

Py:   for item in arr: print(item)
来源：http://xkl.ybcxt.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://udn.guowangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gxo.wangshuangyany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://igu.hongshengwenyu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rut.0kj1m.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iiw.aibaodan.cn

Ruby: arr.each { |item| puts item }
来源：http://wbo.cqqwz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iru.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://api.gaohongyu789.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sbz.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gjc.zhoulong.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://slk.hnxiangtu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dcf.9152youxi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zkn.mhx1999.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kfp.nanxuanxn.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ijn.andypj.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sak.xuanzx.com

[B07] while 循环
来源：http://cej.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://ucr.zhongyouzk.top

PHP:  while ($i < 10) { $i++; }
来源：http://mpl.ehwqpu.com

JS:   while (i < 10) { i++; }
来源：http://iwt.zhengqikj.top

TS:   while (i < 10) { i++; }
来源：http://kjt.guannengcc.top

Java: while (i < 10) { i++; }
来源：http://jlg.tian-w.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uvx.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://kdi.yuanzhike.top

C#:   while (i < 10) { i++; }
来源：http://qnv.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://gfb.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://iye.hysaishi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://akj.aibaodan.cn

JS:   do { i++; } while (i < 10);
来源：http://pja.daxiang520.top

TS:   do { i++; } while (i < 10);
来源：http://nxe.316326.xyz

Java: do { i++; } while (i < 10);
来源：http://vuk.chenjidiqi.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://glt.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://zpk.bbcook.cn

C#:   do { i++; } while (i < 10);
来源：http://sbb.ivvv.top

[B09] break 与 continue
来源：http://kwa.jinyuanbaomall.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cer.sweek.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xhj.ywan-chungtsiang.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://krx.yuxming.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vqz.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://isb.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://umt.jqgfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://def.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zyb.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://wmw.wangshuangyany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://skh.hcnkem.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nle.yonumen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gxn.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mxa.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://duk.tianlin.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ohr.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hef.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gfr.gogol.net.cn

[B11] 生成数字序列 / 区间
来源：http://mqr.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://uap.guowangkeji.top

PHP:  range(0, 10, 2);
来源：http://pld.gotoacloud.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yku.havefunace.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eow.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mns.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lfl.c1oappe.top

Ruby: (0...10).step(2).to_a
来源：http://fiu.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ojz.zycfv.cn

[B12] 跳出多层循环
来源：http://bjp.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://gfz.zhiwuduotai.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kru.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ihw.haohaochexian.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ysh.zhongyouzk.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bgz.zdqjudy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mqc.ppjwa.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://top.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fnt.cashguo.top

[B13] 判断是否为数字
来源：http://mot.yj20258.top

Py:   isinstance(x, (int, float))
来源：http://ccd.zhengqikj.top

PHP:  is_numeric($x)
来源：http://msr.yongpay.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cvx.snrcjt.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rlq.chenzaomai.com

Java: x instanceof Number
来源：http://pqa.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gnp.jyoumei.cn

Ruby: x.is_a?(Numeric)
来源：http://jka.pengpengdd.cyou

C#:   x is int or double or decimal
来源：http://diy.zhijiandao.cn

[B14] 判断值是否在集合内
来源：http://tyv.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mjs.tarul.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jfm.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://vre.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://jde.iojbl.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://egf.nanxuanxn.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cis.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://mtt.yangfankeji.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fav.nwbrower.top

[B15] 布尔运算与取反
来源：http://edb.shanyushiyangkeji.top

Py:   a and b or not c
来源：http://udv.shangyingyoupin.top

PHP:  $a && $b || !$c
来源：http://mib.tanke756.top

JS:   a && b || !c
来源：http://dpn.daxiang520.top

TS:   a && b || !c
来源：http://rya.tianlin.xyz

Java: a && b || !c
来源：http://fzf.nanxinkj.top

Go:   a && b || !c
来源：http://kxx.c1oappe.top

Ruby: a && b || !c
来源：http://ssh.bjfxy.top

C#:   a && b || !c
来源：http://lsv.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://fhp.mhx1999.top

Py:   if not data: return
来源：http://nlq.kuanghao11.cn

PHP:  if (!$data) { return; }
来源：http://kxv.vqdsnc.cn

JS:   if (!data) return;
来源：http://abk.gogol.net.cn

TS:   if (!data) return;
来源：http://ycp.jinqigfzy.top

Java: if (data == null) return;
来源：http://ruw.smart0.xyz

Go:   if data == nil { return }
来源：http://dlh.zhijiandao.cn

Ruby: return if data.nil?
来源：http://bxi.jyoumei.cn

C#:   if (data == null) return;
来源：http://pyd.yongpay.top

================================================================================
来源：http://qhe.jianghu66.top

C. 函数与作用域
来源：http://jsp.wangdashe.top

================================================================================
来源：http://psi.zhongyouzk.top

[C01] 定义函数
来源：http://mnj.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://hdj.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yez.yongpay.top

JS:   function add(a, b) { return a + b; }
来源：http://foi.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ekr.kuanghao11.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sic.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://opo.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://pyx.epnwcf.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ijw.jqgufenzy.top

[C02] 默认参数
来源：http://qwg.yj202588.top

Py:   def greet(name="World"): return name
来源：http://hwp.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nfo.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://abn.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ogi.ywan-chungtsiang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://grc.hnxiangtu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eze.chenjidiqi.icu

Ruby: def greet(name = "World") = name
来源：http://kqd.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://may.pycfn.com

[C03] 可变参数
来源：http://jps.cqqwz.cn

Py:   def total(*args): return sum(args)
来源：http://wpu.sjlbkw.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tvu.ywan-chungtsiang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://exd.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sua.zdqjudy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dbm.9152youxi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://moz.bjfxy.top

Ruby: def total(*nums); nums.sum; end
来源：http://fcd.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dsr.svipenyu.cn

[C04] 命名参数 / 关键字参数
来源：http://ist.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gtc.xuetiantiany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rra.pengpengdd.cyou

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bip.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iuw.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://lgl.aibaodan.cn

Go:   // 无：用配置结构体参数
来源：http://org.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://cur.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://gtu.zhiwuduotai.top

[C05] 返回多个值
来源：http://vfs.vehdjk.com

Py:   return a, b
来源：http://hps.jqgufenzy.top

PHP:  return [$a, $b];
来源：http://rrt.ywan-chungtsiang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hgl.chenlongwang.top

TS:   return { a, b };
来源：http://zcz.zhengqikj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rkx.tianlin.xyz

Go:   return a, b
来源：http://mvd.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://hpi.ctjpmb.com

C#:   return (a, b);              // ValueTuple
来源：http://fbl.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://eov.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://edi.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cpr.smart0.xyz

JS:   const square = x => x * x;
来源：http://wlk.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://yji.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://byw.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ojx.jinghuilouyu.cn

Ruby: square = ->(x) { x * x }
来源：http://bue.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mko.fktsv.cn

[C07] 把函数作为参数传入
来源：http://lfe.hongshengwenyu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gqm.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cli.yangfankeji.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bbv.sysykeji.top

TS:   arr.map(String)
来源：http://dzl.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mdu.jinqigfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tcq.meibo888.top

Ruby: arr.map(&:upcase)
来源：http://nan.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wmj.yongpay.top

[C08] 闭包
来源：http://dln.sxryk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hvt.guannengcc.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cqn.xuetiantiany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zdc.gotoacloud.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mne.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://abe.zdqjudy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gut.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fqt.yj20258.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fci.guowangkeji.top

[C09] 递归
来源：http://toq.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fhf.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pmk.jinghuilouyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fhf.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://toi.zhengqikj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bul.yongpay.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://miy.yj20258888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rmn.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://flb.birdmap.top

[C10] 变量作用域
来源：http://iuo.xziqi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yul.xziqi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nda.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://quq.nanxinkj.top

TS:   同 JS
来源：http://gqs.cdnleiting.top

Java: 方法内为块级作用域
来源：http://aql.hnxiangtu.top

Go:   花括号块级作用域
来源：http://rxv.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ujh.vqdsnc.cn

C#:   块级作用域
来源：http://edg.pycfn.com

[C11] 模块导入与导出
来源：http://yvb.yfazqb.com

Py:   from module import func
来源：http://dcj.guannengcc.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kcp.pengpengdd.cyou


<!-- 参考信息 -->