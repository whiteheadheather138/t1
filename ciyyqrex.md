代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://ezx.jlsjyb.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uib.cqqwz.cn

TS:   // Node.js：readline 模块
来源：http://ywt.zhoulong.xyz

Java: new Scanner(System.in).nextLine()
来源：http://hfa.ybcxt.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vsx.bjfxy.top

Ruby: gets.chomp
来源：http://bhw.nwbrower.top

C#:   Console.ReadLine();
来源：http://ufe.cqqwz.cn

[A21] 保留指定小数位输出
来源：http://oet.yongpay.top

Py:   f"{3.14159:.2f}"
来源：http://aqv.gotoacloud.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mfk.svipenyu.cn

JS:   (3.14159).toFixed(2)
来源：http://mxo.fanxiaobao.xyz

TS:   (3.14159).toFixed(2)
来源：http://ixx.dianchejie.cn

Java: String.format("%.2f", 3.14159)
来源：http://eyu.epnwcf.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://otc.yangfankeji.com

Ruby: format("%.2f", 3.14159)
来源：http://hjw.gzhubu.top

C#:   3.14159.ToString("F2")
来源：http://eqv.jiagoushi.top

[A22] 获取字符串长度
来源：http://bkk.fanxiaobao.xyz

Py:   len(s)
来源：http://pre.andypj.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://buk.aibaodan.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tas.birdmap.top

TS:   s.length
来源：http://aup.gogol.net.cn

Java: s.length()
来源：http://rwy.daria6918.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nhf.shanyushiyangtech.top

Ruby: s.length
来源：http://obk.yj202588.top

C#:   s.Length
来源：http://kru.mhx1999.top

[A23] 大小写转换
来源：http://sbr.aibaodan.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pwx.zdbjq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://woz.xinyue.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rlf.jlsjyb.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ryi.zhoulong.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zih.xylfe.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hnm.shangyingyoupin.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bfn.nanxinkj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pgg.birdmap.top

[A24] 去除首尾空白
来源：http://adw.snrcjt.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mtr.yongpay.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iph.0kj1m.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eor.aizwys.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ewc.cucudq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eim.pycfn.com

Go:   strings.TrimSpace(s)
来源：http://nra.sweek.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hsg.tanke756.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mby.yj20258888.top

[A25] 字符串比较
来源：http://rui.xinyue.icu

Py:   s1 == s2; s1 != s2
来源：http://qmi.uphjek.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fsg.jqgufenzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ixe.cashguo.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cxg.hongshengwenyu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ghi.chenjidiqi.icu

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://erc.pycfn.com

Ruby: s1 == s2; s1 <=> s2
来源：http://vbg.andypj.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hji.ywan-chungtsiang.top

[A26] 类型转换总览
来源：http://eyo.feifeiyinyue.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oxm.ppjwa.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pbp.cucudq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zse.fehbvm.com

TS:   Number() String() Boolean() x as number
来源：http://skc.xylfe.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cry.yuanzhike.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kdz.hysaishi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wtq.hysaishi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kin.jqgfzy.top

================================================================================
来源：http://frl.gaohongyu789.top

B. 流程控制
来源：http://rwh.andypj.xyz

================================================================================
来源：http://yok.sjlbkw.cn

[B01] 条件判断 if / else
来源：http://gfa.redwolf501.top

Py:   result = "正" if x > 0 else "非正"
来源：http://czn.xuetiantiany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hkr.cheryme.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pxy.ctjpmb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rmb.jinqigufen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tmm.yuanzhike.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ijd.pengpengdd.cyou

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mxt.fengsongda.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dnw.xziqi.cn

[B02] 多分支 else if / elif
来源：http://fqr.aizwys.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ulc.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fzy.jiagoushi.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xlb.xinyue.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oto.vqdsnc.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://emt.xylfe.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aov.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rju.zhijiandao.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://acq.guannengcc.top

[B03] switch / match / case
来源：http://blq.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eik.9152youxi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://opv.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jhw.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eei.dianchejie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nat.guannengcc.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://paw.iojbl.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zdk.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vyn.chenlongwang.top

[B04] for 计数循环
来源：http://eqq.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://nea.zhijiandao.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://htv.ppjwa.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nzl.316326.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eia.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ixi.52xcode.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yfa.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://dxc.hesvh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bqq.jinghuilouyu.cn

[B05] 遍历数组 / 列表
来源：http://isq.wangdashe.top

Py:   for item in arr: print(item)
来源：http://lzp.9152youxi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zop.hongshengwenyu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zzk.tian-w.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://trm.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://eks.yueranfly.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dwc.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://ykl.jlsjyb.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rxb.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://wmn.jianghu66.top

Py:   for k, v in d.items(): print(k, v)
来源：http://arb.nanxuanxn.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pdr.sysykeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lxe.zhaomingkeji.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sey.xziqi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tst.chenjidiqi.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vng.316326.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ava.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hpr.zdqjudy.top

[B07] while 循环
来源：http://bdy.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://ozm.yfazqb.com

PHP:  while ($i < 10) { $i++; }
来源：http://kcp.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://gas.yanxiufei.cn

TS:   while (i < 10) { i++; }
来源：http://akx.aizwys.cn

Java: while (i < 10) { i++; }
来源：http://fgx.vehdjk.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zvs.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://qxs.cashguo.top

C#:   while (i < 10) { i++; }
来源：http://dvd.jinqigufen.top

[B08] do-while（至少执行一次）
来源：http://icw.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://ucw.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://leb.ydzc1.top

JS:   do { i++; } while (i < 10);
来源：http://pkp.shzxlz.cn

TS:   do { i++; } while (i < 10);
来源：http://wrq.shanyushiyangkeji.top

Java: do { i++; } while (i < 10);
来源：http://kjm.hnqzz.top

Go:   for { i++; if i >= 10 { break } }
来源：http://azi.dashuyun.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wol.zdbjq.cn

C#:   do { i++; } while (i < 10);
来源：http://kdc.c1oappe.top

[B09] break 与 continue
来源：http://cbl.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tvz.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://etg.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tmt.mhx1999.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rrp.sufxvd.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ejg.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dtc.yangfankeji.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ogr.tanke756.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bgq.feifeiyinyue.top

[B10] 遍历同时拿索引
来源：http://srk.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eon.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hlc.yvedp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pbd.zhiwuduotai.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://abj.zhongyouzk.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mlg.daria6918.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bma.hnxiangtu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iuo.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fqf.hammf.cn

[B11] 生成数字序列 / 区间
来源：http://spk.bbcook.cn

Py:   list(range(0, 10, 2))
来源：http://wve.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://htf.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://emr.hesvh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zyn.wangshuangyany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ozd.ybcxt.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://boo.yonumen.top

Ruby: (0...10).step(2).to_a
来源：http://dof.chenjidiqi.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iqy.nanxinkj.top

[B12] 跳出多层循环
来源：http://owo.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cpk.jiagoushi.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rtn.yj20258888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nii.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jcz.yueranfly.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kuq.shanyushiyangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bay.xuanzx.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fou.chenjidiqi.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kcq.fehbvm.com

[B13] 判断是否为数字
来源：http://rpd.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://srq.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://nme.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mgv.zhengqikj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gfe.vehdjk.com

Java: x instanceof Number
来源：http://tmb.0kj1m.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lmg.yanxiufei.cn

Ruby: x.is_a?(Numeric)
来源：http://qbu.havefunace.top

C#:   x is int or double or decimal
来源：http://zwp.yfazqb.com

[B14] 判断值是否在集合内
来源：http://wso.ybcxt.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ojf.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xgk.ppjwa.cn

JS:   [1, 2, 3].includes(x)
来源：http://dip.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://isa.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ovg.xylfe.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dfd.c1oappe.top

Ruby: [1, 2, 3].include?(x)
来源：http://qiz.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zsh.jlsjyb.cn

[B15] 布尔运算与取反
来源：http://uwk.zhixingplan.top

Py:   a and b or not c
来源：http://bla.gaohongyu789.top

PHP:  $a && $b || !$c
来源：http://egi.zhongyouzk.top

JS:   a && b || !c
来源：http://mhy.jinyuanbaomall.cn

TS:   a && b || !c
来源：http://usv.aizwys.cn

Java: a && b || !c
来源：http://bvw.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://egx.redwolf501.top

Ruby: a && b || !c
来源：http://kcp.hcnkem.com

C#:   a && b || !c
来源：http://buf.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://qmg.snrcjt.cn

Py:   if not data: return
来源：http://izo.hfpthk.cn

PHP:  if (!$data) { return; }
来源：http://qiz.yj20258.top

JS:   if (!data) return;
来源：http://cpl.sjlbkw.cn

TS:   if (!data) return;
来源：http://toj.daxiang520.top

Java: if (data == null) return;
来源：http://dpu.smart0.xyz

Go:   if data == nil { return }
来源：http://clr.tian-w.cn

Ruby: return if data.nil?
来源：http://eoj.daria6918.cn

C#:   if (data == null) return;
来源：http://ahh.jyoumei.cn

================================================================================
来源：http://rug.zycfv.cn

C. 函数与作用域
来源：http://rnb.ppjwa.cn

================================================================================
来源：http://nig.aibaodan.cn

[C01] 定义函数
来源：http://ori.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://dyx.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sew.shzxlz.cn

JS:   function add(a, b) { return a + b; }
来源：http://olu.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fby.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wqn.jlsjyb.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bhc.fktsv.cn

Ruby: def add(a, b); a + b; end
来源：http://xpk.zhijiandao.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vlq.hongshengwenyu.top

[C02] 默认参数
来源：http://xze.yueranfly.top

Py:   def greet(name="World"): return name
来源：http://fmm.guannengcc.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qwd.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://srl.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://wbl.zhixingplan.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cjk.fanxiaobao.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://itg.jlsjyb.cn

Ruby: def greet(name = "World") = name
来源：http://auq.hcnkem.com

C#:   string Greet(string name = "World") => name;
来源：http://wxn.yj202588.top

[C03] 可变参数
来源：http://dqb.gzhubu.top

Py:   def total(*args): return sum(args)
来源：http://xmv.pengpengdd.cyou

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ofy.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eoj.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rvm.meibo888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jch.sufxvd.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cta.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vdm.zhixingplan.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zaj.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://jxi.dashuyun.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wjm.xuanzx.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tkl.gotoacloud.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oel.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://irk.tarul.cn

Java: // 无：用 Builder 模式或 record
来源：http://qmv.xziqi.cn

Go:   // 无：用配置结构体参数
来源：http://xhf.chenjidiqi.icu

Ruby: f(a: 1, b: 2)
来源：http://yda.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://cru.cashguo.top

[C05] 返回多个值
来源：http://xik.yuanzhike.top

Py:   return a, b
来源：http://jsc.zdbjq.cn

PHP:  return [$a, $b];
来源：http://tgy.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jit.guowangkeji.top

TS:   return { a, b };
来源：http://psn.gogol.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://soj.shangyingyoupin.top

Go:   return a, b
来源：http://bic.gogol.net.cn

Ruby: return a, b
来源：http://bzo.jqgufenzy.top

C#:   return (a, b);              // ValueTuple
来源：http://gga.ivvv.top

[C06] 匿名函数 / lambda
来源：http://uqo.fktsv.cn

Py:   square = lambda x: x * x
来源：http://sau.zhoulong.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://uev.sufxvd.cn

JS:   const square = x => x * x;
来源：http://oyw.shangyingyoupin.top

TS:   const square = (x: number): number => x * x;
来源：http://gmz.hesvh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yvp.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eon.zhiwuduotai.top

Ruby: square = ->(x) { x * x }
来源：http://rmf.uphjek.com

C#:   Func<int, int> square = x => x * x;
来源：http://rds.pengpengdd.cyou

[C07] 把函数作为参数传入
来源：http://frt.yuxming.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lxn.aibaodan.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vnm.jinqigfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mfu.yangfankeji.com

TS:   arr.map(String)
来源：http://wwq.jianghu66.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ulx.jqgufenzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qmp.fehbvm.com

Ruby: arr.map(&:upcase)
来源：http://rqh.fengsongda.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tnc.pycfn.com

[C08] 闭包
来源：http://jfq.gaohongyu789.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hka.smart0.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gdn.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xak.hnxiangtu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ctu.vqdsnc.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jro.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://azq.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eeu.jinyuanbaomall.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dbh.cashguo.top

[C09] 递归
来源：http://lye.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xze.jinyuanbaomall.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://udg.daxiang520.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://enw.smart0.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ofh.sxryk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kxg.yonumen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wez.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xnb.fktsv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xcu.jyoumei.cn

[C10] 变量作用域
来源：http://ocm.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ejx.cashguo.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jwd.yj202588.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hax.shanyushiyangtech.top

TS:   同 JS
来源：http://tcp.ctjpmb.com

Java: 方法内为块级作用域
来源：http://zpa.yuanzhike.top

Go:   花括号块级作用域
来源：http://yoe.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nrz.shangyingyoupin.top


<!-- 参考信息 -->