代发 wailian999

Ruby: a, b = b, a
来源：http://ktz.xylfe.cn

C#:   (a, b) = (b, a);
来源：http://crq.9152youxi.cn

[A20] 读取标准输入
来源：http://pxk.jlsjyb.cn

Py:   name = input("请输入：")
来源：http://dpb.chenjidiqi.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://ayg.zhengqikj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://txo.shanyushiyangkeji.top

TS:   // Node.js：readline 模块
来源：http://htk.cheryme.top

Java: new Scanner(System.in).nextLine()
来源：http://coz.jyoumei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kvv.xylfe.cn

Ruby: gets.chomp
来源：http://gxb.zdbjq.cn

C#:   Console.ReadLine();
来源：http://bud.hfpthk.cn

[A21] 保留指定小数位输出
来源：http://zql.sweek.top

Py:   f"{3.14159:.2f}"
来源：http://xmk.quarkkingdee.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pty.shzxlz.cn

JS:   (3.14159).toFixed(2)
来源：http://sef.zhaomingkeji.xyz

TS:   (3.14159).toFixed(2)
来源：http://gsi.meibo888.top

Java: String.format("%.2f", 3.14159)
来源：http://opd.daxiang520.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mji.9152youxi.cn

Ruby: format("%.2f", 3.14159)
来源：http://ywl.cdnleiting.top

C#:   3.14159.ToString("F2")
来源：http://lne.yuanzhike.top

[A22] 获取字符串长度
来源：http://ipf.guannengcc.top

Py:   len(s)
来源：http://xew.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bgw.yuxming.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://azc.epnwcf.com

TS:   s.length
来源：http://slp.dashuyun.cn

Java: s.length()
来源：http://zyx.ehwqpu.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://diz.yonumen.top

Ruby: s.length
来源：http://qvw.nanxinkj.top

C#:   s.Length
来源：http://mom.kuanghao11.cn

[A23] 大小写转换
来源：http://lhf.guowangkeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://phf.epnwcf.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yet.hfpthk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oec.shzxlz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wka.zhaomingkeji.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cac.ivvv.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vtn.snrcjt.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qie.hcnkem.com

C#:   s.ToUpper(); s.ToLower()
来源：http://qmn.ivvv.top

[A24] 去除首尾空白
来源：http://hqg.52xcode.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vht.aibaodan.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hiv.vehdjk.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fqv.sufxvd.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hbb.jinghuilouyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bsc.ydzc1.top

Go:   strings.TrimSpace(s)
来源：http://cze.ivvv.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://two.aizwys.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zbt.yfazqb.com

[A25] 字符串比较
来源：http://kol.xingfuxueyuan.xyz

Py:   s1 == s2; s1 != s2
来源：http://mrf.tianlin.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mnz.cqqwz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pkc.ywan-chungtsiang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gun.havefunace.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fod.zycfv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ujg.ydjk.org.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bum.wangdashe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://imy.bjfxy.top

[A26] 类型转换总览
来源：http://qtc.ybcxt.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bhh.hywenlv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xqs.xingfuxueyuan.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fwm.zdqjudy.top

TS:   Number() String() Boolean() x as number
来源：http://nca.jinghuilouyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gfu.sysykeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://muw.pengpengdd.cyou

Ruby: to_i to_f to_s to_sym to_a
来源：http://sja.yueranfly.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bfp.jinyuanbaomall.cn

================================================================================
来源：http://taw.chenzaomai.com

B. 流程控制
来源：http://maw.birdmap.top

================================================================================
来源：http://jqj.guowangkeji.top

[B01] 条件判断 if / else
来源：http://eoy.hcnkem.com

Py:   result = "正" if x > 0 else "非正"
来源：http://eju.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zdr.ctjpmb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wms.yuxming.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://czw.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://eew.jqgufenzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://taj.xuetiantiany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aob.jianghu66.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vlc.yonumen.top

[B02] 多分支 else if / elif
来源：http://kag.jinyuanbaomall.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://msd.yfazqb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://goy.redwolf501.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tmp.gotoacloud.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rsk.birdmap.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uqu.guannengcc.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qwr.shzxlz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vbd.ivvv.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pqu.kuanghao11.cn

[B03] switch / match / case
来源：http://dss.zhijiandao.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mnv.sweek.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ynh.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hqr.tanke756.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://irz.xingfuxueyuan.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fwa.pycfn.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://upn.xylfe.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bdy.feifeiyinyue.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rzl.chenzaomai.com

[B04] for 计数循环
来源：http://vtk.tanke756.top

Py:   for i in range(10): print(i)
来源：http://hku.chenzaomai.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lap.zhoulong.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cij.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://obm.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pin.shzxlz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xyx.dashuyun.cn

Ruby: 10.times { |i| puts i }
来源：http://dam.fanxiaobao.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fwt.yongpay.top

[B05] 遍历数组 / 列表
来源：http://alf.snrcjt.cn

Py:   for item in arr: print(item)
来源：http://hys.ydjk.org.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gat.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wdd.smart0.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://kvg.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rbv.fehbvm.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://haw.gogol.net.cn

Ruby: arr.each { |item| puts item }
来源：http://pkg.feifeiyinyue.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mhs.nwbrower.top

[B06] 遍历字典 / 对象
来源：http://bzl.316326.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://hud.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lhm.chenlongwang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ilw.xingfuxueyuan.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wyq.yj20258888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ary.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://quv.fktsv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dwr.yj202588.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hil.316326.xyz

[B07] while 循环
来源：http://jvw.zhaomingkeji.xyz

Py:   while i < 10: i += 1
来源：http://qpx.c1oappe.top

PHP:  while ($i < 10) { $i++; }
来源：http://xal.zdqjudy.top

JS:   while (i < 10) { i++; }
来源：http://wqf.jqgufenzy.top

TS:   while (i < 10) { i++; }
来源：http://jcy.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://ycb.sweek.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dkh.nanxinkj.top

Ruby: while i < 10; i += 1; end
来源：http://znz.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://rqh.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://cek.gzhubu.top

Py:   # 无 do-while：用 while True + break
来源：http://hje.cheryme.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wut.shangyingyoupin.top

JS:   do { i++; } while (i < 10);
来源：http://kgl.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://rya.yongpay.top

Java: do { i++; } while (i < 10);
来源：http://btq.redwolf501.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dxh.ivvv.top

Ruby: begin; i += 1; end while i < 10
来源：http://snf.svipenyu.cn

C#:   do { i++; } while (i < 10);
来源：http://rse.yangfankeji.com

[B09] break 与 continue
来源：http://sqe.zhijiandao.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ial.cqqwz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oei.aizwys.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lkh.jinqigufen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pas.redwolf501.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tot.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blc.hesvh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pxj.sweek.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eju.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://tcd.chenlongwang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xox.shuidangran.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vau.tian-w.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://stq.c1oappe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cko.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qkw.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wwo.fengsongda.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://srg.jinghuilouyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qxm.xuanzx.com

[B11] 生成数字序列 / 区间
来源：http://tfa.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://fzv.yj20258888.top

PHP:  range(0, 10, 2);
来源：http://jzm.feifeiyinyue.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kvv.fzhhl.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://skf.hesvh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jey.xinyue.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mic.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://iru.yj20258.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ygy.gaohongyu789.top

[B12] 跳出多层循环
来源：http://omz.ywan-chungtsiang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://aqy.xinyue.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://uul.gzhubu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oqk.cucudq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wwk.svipenyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nrj.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ska.zhongyouzk.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zrw.jinqigfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dos.hnxiangtu.top

[B13] 判断是否为数字
来源：http://qcr.dashuyun.cn

Py:   isinstance(x, (int, float))
来源：http://mnl.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://vyt.ehwqpu.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hua.jiagoushi.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xmg.yangfankeji.com

Java: x instanceof Number
来源：http://qea.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dvy.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://vos.tian-w.cn

C#:   x is int or double or decimal
来源：http://lch.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://mhx.meibo888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://inv.jinyuanbaomall.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dim.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://jbv.hesvh.cn

TS:   [1, 2, 3].includes(x)
来源：http://vtx.yanxiufei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gyd.hywenlv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yja.fengsongda.top

Ruby: [1, 2, 3].include?(x)
来源：http://ber.xylfe.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bpe.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://bxv.yuanzhike.top

Py:   a and b or not c
来源：http://zat.meibo888.top

PHP:  $a && $b || !$c
来源：http://brh.zhoulong.xyz

JS:   a && b || !c
来源：http://btg.mhx1999.top

TS:   a && b || !c
来源：http://lux.tarul.cn

Java: a && b || !c
来源：http://ccb.ywan-chungtsiang.top

Go:   a && b || !c
来源：http://ejr.jinqigufen.top

Ruby: a && b || !c
来源：http://wkg.wangdashe.top

C#:   a && b || !c
来源：http://llu.xinyue.icu

[B16] 卫语句：不满足条件提前返回
来源：http://jez.jqgfzy.top

Py:   if not data: return
来源：http://tif.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://pmn.nanxinkj.top

JS:   if (!data) return;
来源：http://dke.birdmap.top

TS:   if (!data) return;
来源：http://oif.chenzaomai.com

Java: if (data == null) return;
来源：http://qfj.316326.xyz

Go:   if data == nil { return }
来源：http://arb.daxiang520.top

Ruby: return if data.nil?
来源：http://yhy.andypj.xyz

C#:   if (data == null) return;
来源：http://yxv.xylfe.cn

================================================================================
来源：http://thr.cucudq.cn

C. 函数与作用域
来源：http://xre.yongpay.top

================================================================================
来源：http://qrh.shangyingyoupin.top

[C01] 定义函数
来源：http://jqf.pengpengdd.cyou

Py:   def add(a, b): return a + b
来源：http://msq.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vbr.vehdjk.com

JS:   function add(a, b) { return a + b; }
来源：http://uww.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mah.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vtp.jqgufenzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://hsh.zhongyouzk.top

Ruby: def add(a, b); a + b; end
来源：http://bqa.birdmap.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nyk.dashuyun.cn

[C02] 默认参数
来源：http://fzh.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://dpx.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://aaf.ivvv.top

JS:   function greet(name = "World") { return name; }
来源：http://zfx.hysaishi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ygb.shzxlz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dtn.epnwcf.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cxh.fktsv.cn

Ruby: def greet(name = "World") = name
来源：http://avf.jinyuanbaomall.cn

C#:   string Greet(string name = "World") => name;
来源：http://xbd.havefunace.top

[C03] 可变参数
来源：http://wbz.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://onp.havefunace.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ivl.shzxlz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xql.shanyushiyangtech.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nev.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kic.tianlin.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qwz.daria6918.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lpx.ctjpmb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ytd.cucudq.cn

[C04] 命名参数 / 关键字参数
来源：http://vpo.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cqg.fktsv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ovt.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://alw.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fpb.fzhhl.top

Java: // 无：用 Builder 模式或 record
来源：http://luc.redwolf501.top

Go:   // 无：用配置结构体参数
来源：http://nnr.xziqi.cn

Ruby: f(a: 1, b: 2)
来源：http://ccr.guowangkeji.top

C#:   f(a: 1, b: 2)
来源：http://qpe.hnxiangtu.top

[C05] 返回多个值
来源：http://wot.pengpengdd.cyou

Py:   return a, b
来源：http://cnz.52xcode.cn

PHP:  return [$a, $b];
来源：http://rtf.ywan-chungtsiang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://htf.tian-w.cn

TS:   return { a, b };
来源：http://ahx.jqgufenzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cgb.pycfn.com

Go:   return a, b
来源：http://cpa.cdnleiting.top

Ruby: return a, b
来源：http://ish.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://fnl.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://tbo.zycfv.cn

Py:   square = lambda x: x * x
来源：http://pjx.hnxiangtu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://riw.yanxiufei.cn

JS:   const square = x => x * x;
来源：http://atb.hnqzz.top

TS:   const square = (x: number): number => x * x;
来源：http://tcb.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://poh.316326.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://wlz.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://xqr.sufxvd.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ygj.xziqi.cn

[C07] 把函数作为参数传入
来源：http://ljd.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pgw.zhaomingkeji.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://dng.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xvi.jqgfzy.top

TS:   arr.map(String)
来源：http://nhs.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://svj.chenzaomai.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kje.jiagoushi.top

Ruby: arr.map(&:upcase)
来源：http://aqt.yangfankeji.com

C#:   arr.Select(s => s.ToUpper())
来源：http://nkq.nanxinkj.top

[C08] 闭包
来源：http://uxg.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lvt.shzxlz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jyy.pengpengdd.cyou

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hsw.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fyu.svipenyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wqr.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zwn.yj20258888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dgv.xingfuxueyuan.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hbd.316326.xyz

[C09] 递归
来源：http://wds.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aqg.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oik.zdbjq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pec.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rcr.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zaf.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qhu.smart0.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gaa.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wvj.ybcxt.top

[C10] 变量作用域
来源：http://eau.yj20258.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hge.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oec.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ktk.316326.xyz


<!-- 参考信息 -->