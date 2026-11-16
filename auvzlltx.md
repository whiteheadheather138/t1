代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ivn.jyoumei.cn

Ruby: gets.chomp
来源：http://fof.shangyingyoupin.top

C#:   Console.ReadLine();
来源：http://nwz.iojbl.cn

[A21] 保留指定小数位输出
来源：http://ajn.hnxiangtu.top

Py:   f"{3.14159:.2f}"
来源：http://klu.yangfankeji.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jze.wangshuangyany.cn

JS:   (3.14159).toFixed(2)
来源：http://cxn.xingfuxueyuan.xyz

TS:   (3.14159).toFixed(2)
来源：http://duf.daxiang520.top

Java: String.format("%.2f", 3.14159)
来源：http://viv.hywenlv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wgb.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://gsv.gzhubu.top

C#:   3.14159.ToString("F2")
来源：http://nhi.ppjwa.cn

[A22] 获取字符串长度
来源：http://dkp.ehwqpu.com

Py:   len(s)
来源：http://fjs.yuxming.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://okf.gaohongyu789.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nut.cqqwz.cn

TS:   s.length
来源：http://kat.meibo888.top

Java: s.length()
来源：http://byi.guowangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tgb.zycfv.cn

Ruby: s.length
来源：http://bqi.gogol.net.cn

C#:   s.Length
来源：http://lax.hnqzz.top

[A23] 大小写转换
来源：http://xqn.vehdjk.com

Py:   s.upper(); s.lower(); s.title()
来源：http://aro.xingfuxueyuan.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ffb.nanxinkj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wpp.cucudq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uxp.jinqigufen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kkn.tanke756.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lll.jyoumei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://knx.jinghuilouyu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jiu.ctjpmb.com

[A24] 去除首尾空白
来源：http://ywy.yanxiufei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iop.yvedp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://frw.nanxuanxn.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ouv.gzhubu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xgx.fktsv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rdv.chenlongwang.top

Go:   strings.TrimSpace(s)
来源：http://pdi.aibaodan.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eie.hammf.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cde.zycfv.cn

[A25] 字符串比较
来源：http://vze.vehdjk.com

Py:   s1 == s2; s1 != s2
来源：http://clm.smart0.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mdt.fzhhl.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://psq.hammf.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mur.jiagoushi.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jzn.xziqi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jqh.jianghu66.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hol.jiagoushi.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xec.0kj1m.cn

[A26] 类型转换总览
来源：http://lpr.vqdsnc.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mmi.bbcook.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cjt.gogol.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ybd.jinyuanbaomall.cn

TS:   Number() String() Boolean() x as number
来源：http://tew.yonumen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ppo.hcnkem.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kdo.yuanzhike.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://szw.xingfuxueyuan.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ril.xuetiantiany.cn

================================================================================
来源：http://cun.aibaodan.cn

B. 流程控制
来源：http://tnd.jlsjyb.cn

================================================================================
来源：http://gbm.xuetiantiany.cn

[B01] 条件判断 if / else
来源：http://xab.guowangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ooz.snrcjt.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://obq.316326.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jrh.gogol.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://efa.xuetiantiany.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://alp.fanxiaobao.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pyb.wangdashe.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jom.ydzc1.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xmt.kuanghao11.cn

[B02] 多分支 else if / elif
来源：http://ptz.jinqigufen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://seb.yanxiufei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dap.ydzc1.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kqw.tarul.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xxk.wangshuangyany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://llv.aibaodan.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://usl.chenlongwang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://skz.fengsongda.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://elc.yj20258888.top

[B03] switch / match / case
来源：http://vgy.ehwqpu.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kla.cqqwz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qtw.fzhhl.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jhp.yvedp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gsa.zhiwuduotai.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ggu.feifeiyinyue.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://krh.hesvh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kat.sufxvd.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cst.yvedp.cn

[B04] for 计数循环
来源：http://yaa.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://qgo.yj20258888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oew.havefunace.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lep.aizwys.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qyl.jiagoushi.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yis.tarul.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vxm.snrcjt.cn

Ruby: 10.times { |i| puts i }
来源：http://ajh.xinyue.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zph.snrcjt.cn

[B05] 遍历数组 / 列表
来源：http://rsa.ehwqpu.com

Py:   for item in arr: print(item)
来源：http://gij.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hie.zhixingplan.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gge.chenzaomai.com

TS:   for (const item of arr) { console.log(item); }
来源：http://pyg.nanxuanxn.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fqq.feifeiyinyue.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://syc.daxiang520.top

Ruby: arr.each { |item| puts item }
来源：http://czk.gotoacloud.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nyh.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://irn.sufxvd.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bxm.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ykd.yj20258.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fxc.ctjpmb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wnh.ywan-chungtsiang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pyz.zhaomingkeji.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vkv.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aml.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bnp.sxryk.cn

[B07] while 循环
来源：http://dfl.zhaomingkeji.xyz

Py:   while i < 10: i += 1
来源：http://rej.sxryk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vnd.uphjek.com

JS:   while (i < 10) { i++; }
来源：http://qqq.nanxuanxn.top

TS:   while (i < 10) { i++; }
来源：http://imd.zhoulong.xyz

Java: while (i < 10) { i++; }
来源：http://xup.yj20258.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zse.ppjwa.cn

Ruby: while i < 10; i += 1; end
来源：http://ecz.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://faj.shanyushiyangkeji.top

[B08] do-while（至少执行一次）
来源：http://dnw.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://oqs.ybcxt.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zph.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://sgw.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://vrw.fanxiaobao.xyz

Java: do { i++; } while (i < 10);
来源：http://ocr.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uno.xuanzx.com

Ruby: begin; i += 1; end while i < 10
来源：http://tsq.cqqwz.cn

C#:   do { i++; } while (i < 10);
来源：http://paf.gaohongyu789.top

[B09] break 与 continue
来源：http://nhz.jqgufenzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qiw.ydjk.org.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://glh.daxiang520.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fdh.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jjv.xuetiantiany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jqe.havefunace.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cge.xuanzx.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lxw.yuxming.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ksm.feifeiyinyue.top

[B10] 遍历同时拿索引
来源：http://grw.bbcook.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hku.ydzc1.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://emc.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://waz.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lsj.9152youxi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gvl.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cnq.jyoumei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yht.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sri.sufxvd.cn

[B11] 生成数字序列 / 区间
来源：http://jei.shuidangran.top

Py:   list(range(0, 10, 2))
来源：http://uat.ctjpmb.com

PHP:  range(0, 10, 2);
来源：http://lcq.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cky.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bni.yfazqb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vef.zdbjq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ntp.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://udz.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://azn.yj202588.top

[B12] 跳出多层循环
来源：http://ebb.nwbrower.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://air.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://pju.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bsz.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nch.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hpk.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bqn.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hhq.fengsongda.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://drm.hesvh.cn

[B13] 判断是否为数字
来源：http://zwt.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://jty.wangdashe.top

PHP:  is_numeric($x)
来源：http://mom.chenzaomai.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://prl.pycfn.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jsn.jyoumei.cn

Java: x instanceof Number
来源：http://xjx.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sbt.shangyingyoupin.top

Ruby: x.is_a?(Numeric)
来源：http://dli.gotoacloud.top

C#:   x is int or double or decimal
来源：http://bdg.wangdashe.top

[B14] 判断值是否在集合内
来源：http://szm.yonumen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://maw.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ydh.gzhubu.top

JS:   [1, 2, 3].includes(x)
来源：http://jtt.hfpthk.cn

TS:   [1, 2, 3].includes(x)
来源：http://wpa.hongshengwenyu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ahj.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cbn.fanxiaobao.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://mjh.dashuyun.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zch.chenjidiqi.icu

[B15] 布尔运算与取反
来源：http://tww.redwolf501.top

Py:   a and b or not c
来源：http://fsf.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://vur.ehwqpu.com

JS:   a && b || !c
来源：http://zzk.wangdashe.top

TS:   a && b || !c
来源：http://yma.chenlongwang.top

Java: a && b || !c
来源：http://dej.ydzc1.top

Go:   a && b || !c
来源：http://ikn.hysaishi.cn

Ruby: a && b || !c
来源：http://fbf.9152youxi.cn

C#:   a && b || !c
来源：http://gfk.aibaodan.cn

[B16] 卫语句：不满足条件提前返回
来源：http://peq.xingfuxueyuan.xyz

Py:   if not data: return
来源：http://tzu.sweek.top

PHP:  if (!$data) { return; }
来源：http://cpg.0kj1m.cn

JS:   if (!data) return;
来源：http://smi.c1oappe.top

TS:   if (!data) return;
来源：http://uui.hammf.cn

Java: if (data == null) return;
来源：http://evd.gzhubu.top

Go:   if data == nil { return }
来源：http://nxy.tanke756.top

Ruby: return if data.nil?
来源：http://awv.wangdashe.top

C#:   if (data == null) return;
来源：http://ueh.hcnkem.com

================================================================================
来源：http://wmn.iojbl.cn

C. 函数与作用域
来源：http://qnn.redwolf501.top

================================================================================
来源：http://eve.ybcxt.top

[C01] 定义函数
来源：http://pyk.guannengcc.top

Py:   def add(a, b): return a + b
来源：http://jhz.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lsh.tanke756.top

JS:   function add(a, b) { return a + b; }
来源：http://ryj.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vry.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wto.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://ecl.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://jdq.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cvs.ydzc1.top

[C02] 默认参数
来源：http://pxl.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://zup.gotoacloud.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jjl.shuidangran.top

JS:   function greet(name = "World") { return name; }
来源：http://ist.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://hnq.hnxiangtu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cos.sweek.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ale.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://brl.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://wqo.hcnkem.com

[C03] 可变参数
来源：http://blg.shangyingyoupin.top

Py:   def total(*args): return sum(args)
来源：http://zvx.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hpr.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dta.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jau.ctjpmb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mzh.yj20258.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iil.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://hgj.sjlbkw.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fes.hfpthk.cn

[C04] 命名参数 / 关键字参数
来源：http://ahc.jyoumei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pmp.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pcd.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://psf.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kzk.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://jqg.ybcxt.top

Go:   // 无：用配置结构体参数
来源：http://aat.haohaochexian.top

Ruby: f(a: 1, b: 2)
来源：http://fzn.gzhubu.top

C#:   f(a: 1, b: 2)
来源：http://tnn.zhiwuduotai.top

[C05] 返回多个值
来源：http://eop.meibo888.top

Py:   return a, b
来源：http://kns.zdqjudy.top

PHP:  return [$a, $b];
来源：http://wde.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mzt.xuanzx.com

TS:   return { a, b };
来源：http://yxz.kuanghao11.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://udm.zhongyouzk.top

Go:   return a, b
来源：http://toq.jinqigfzy.top

Ruby: return a, b
来源：http://vgf.shanyushiyangtech.top

C#:   return (a, b);              // ValueTuple
来源：http://rrv.redwolf501.top

[C06] 匿名函数 / lambda
来源：http://uco.jianghu66.top

Py:   square = lambda x: x * x
来源：http://bll.chenjidiqi.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://gvj.shanyushiyangtech.top

JS:   const square = x => x * x;
来源：http://xan.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://rye.sweek.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dfx.chenlongwang.top

Go:   sq := func(x int) int { return x * x }
来源：http://xic.yanxiufei.cn

Ruby: square = ->(x) { x * x }
来源：http://tui.shzxlz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://udc.316326.xyz

[C07] 把函数作为参数传入
来源：http://rwt.meibo888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xgg.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://wfs.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gvf.chenzaomai.com

TS:   arr.map(String)
来源：http://xyu.ydzc1.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zza.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hhy.chenzaomai.com

Ruby: arr.map(&:upcase)
来源：http://big.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xlf.zhaomingkeji.xyz

[C08] 闭包
来源：http://dpv.xingfuxueyuan.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ckw.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ide.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gxo.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ctd.xuetiantiany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tws.xinyue.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hmk.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://far.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cjv.epnwcf.com

[C09] 递归
来源：http://rmd.cheryme.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zmi.nwbrower.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iar.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nhp.cqqwz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kaw.fzhhl.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nni.sjlbkw.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pxm.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ekb.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fkc.shanyushiyangtech.top

[C10] 变量作用域
来源：http://lkn.fzhhl.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bnl.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zcu.meibo888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bjd.tian-w.cn

TS:   同 JS
来源：http://qvo.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://qjb.tianlin.xyz

Go:   花括号块级作用域
来源：http://pki.hongshengwenyu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sdm.sweek.top

C#:   块级作用域
来源：http://iqm.xziqi.cn

[C11] 模块导入与导出
来源：http://rlp.bjfxy.top

Py:   from module import func
来源：http://vil.fzhhl.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fkd.mhx1999.top


<!-- 参考信息 -->