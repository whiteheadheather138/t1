代发 wailian999

JS:   [a, b] = [b, a];
来源：http://xmh.nanxuanxn.top

TS:   [a, b] = [b, a];
来源：http://mrp.zhijiandao.cn

Java: int t = a; a = b; b = t;
来源：http://jxo.shanyushiyangkeji.top

Go:   a, b = b, a
来源：http://yhl.havefunace.top

Ruby: a, b = b, a
来源：http://aqi.hcnkem.com

C#:   (a, b) = (b, a);
来源：http://wva.hysaishi.cn

[A20] 读取标准输入
来源：http://tbu.zhijiandao.cn

Py:   name = input("请输入：")
来源：http://hok.c1oappe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rux.kuanghao11.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nws.yanxiufei.cn

TS:   // Node.js：readline 模块
来源：http://xva.bjfxy.top

Java: new Scanner(System.in).nextLine()
来源：http://xef.yvedp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pnr.vqdsnc.cn

Ruby: gets.chomp
来源：http://cfv.cdnleiting.top

C#:   Console.ReadLine();
来源：http://gpx.yangfankeji.com

[A21] 保留指定小数位输出
来源：http://twn.jinyuanbaomall.cn

Py:   f"{3.14159:.2f}"
来源：http://xdu.zhoulong.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://aby.daria6918.cn

JS:   (3.14159).toFixed(2)
来源：http://bcy.nanxuanxn.top

TS:   (3.14159).toFixed(2)
来源：http://zsl.sweek.top

Java: String.format("%.2f", 3.14159)
来源：http://nxr.daria6918.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://two.yonumen.top

Ruby: format("%.2f", 3.14159)
来源：http://lco.shuidangran.top

C#:   3.14159.ToString("F2")
来源：http://zcu.zhaomingkeji.xyz

[A22] 获取字符串长度
来源：http://jhq.zhaomingkeji.xyz

Py:   len(s)
来源：http://xgm.fzhhl.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://krw.yuxming.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eau.jinyuanbaomall.cn

TS:   s.length
来源：http://rmc.zdbjq.cn

Java: s.length()
来源：http://prq.shuidangran.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mrg.tarul.cn

Ruby: s.length
来源：http://pfw.yj202588.top

C#:   s.Length
来源：http://jqm.cheryme.top

[A23] 大小写转换
来源：http://smh.birdmap.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gay.sweek.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rsc.sxryk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aup.smart0.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cvs.jinghuilouyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kmo.ydjk.org.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jfq.epnwcf.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mkf.dashuyun.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://akd.ybcxt.top

[A24] 去除首尾空白
来源：http://fee.cashguo.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nzj.jiagoushi.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jpq.yuxming.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gje.9152youxi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ijg.guannengcc.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yyj.zdbjq.cn

Go:   strings.TrimSpace(s)
来源：http://kum.sysykeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xdg.kuanghao11.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://icd.jinqigufen.top

[A25] 字符串比较
来源：http://vhe.aizwys.cn

Py:   s1 == s2; s1 != s2
来源：http://xtm.nwbrower.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ugz.meibo888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://liz.52xcode.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mlj.sysykeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zep.sweek.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cvy.jinyuanbaomall.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jup.yvedp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ulo.haohaochexian.top

[A26] 类型转换总览
来源：http://ruo.yanxiufei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xpf.yvedp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://seo.fehbvm.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://txt.nanxinkj.top

TS:   Number() String() Boolean() x as number
来源：http://iuo.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://udn.tian-w.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lmi.gotoacloud.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://amx.jqgufenzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hkk.sufxvd.cn

================================================================================
来源：http://pqo.ydjk.org.cn

B. 流程控制
来源：http://vzp.fengsongda.top

================================================================================
来源：http://rzt.tian-w.cn

[B01] 条件判断 if / else
来源：http://fwl.yanxiufei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gaf.redwolf501.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aee.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oip.gogol.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oqz.yvedp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uzy.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iap.hesvh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fyq.ywan-chungtsiang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bsd.yj20258888.top

[B02] 多分支 else if / elif
来源：http://jfd.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://njz.yfazqb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wxs.zdqjudy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bup.zhijiandao.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zxm.shzxlz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kwi.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yiw.tanke756.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uwz.birdmap.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vkn.hnqzz.top

[B03] switch / match / case
来源：http://qst.hnxiangtu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nxp.ydzc1.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kcd.xylfe.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://znx.smart0.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qyb.tanke756.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sfz.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tfw.hywenlv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eja.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lck.birdmap.top

[B04] for 计数循环
来源：http://ojh.zycfv.cn

Py:   for i in range(10): print(i)
来源：http://bjc.tianlin.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://irn.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tuq.gaohongyu789.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rys.chenzaomai.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uat.yj20258.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qsl.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://wae.zhixingplan.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ehs.hywenlv.cn

[B05] 遍历数组 / 列表
来源：http://ppu.jinghuilouyu.cn

Py:   for item in arr: print(item)
来源：http://gxj.ehwqpu.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://akr.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://shb.zdbjq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://van.yuanzhike.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mzg.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://utu.c1oappe.top

Ruby: arr.each { |item| puts item }
来源：http://fuo.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aye.zhijiandao.cn

[B06] 遍历字典 / 对象
来源：http://shu.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hpd.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nsn.yangfankeji.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zkl.xingfuxueyuan.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hkx.jinghuilouyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xvl.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nup.wangdashe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://izk.dianchejie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wnb.svipenyu.cn

[B07] while 循环
来源：http://eif.cucudq.cn

Py:   while i < 10: i += 1
来源：http://sry.nwbrower.top

PHP:  while ($i < 10) { $i++; }
来源：http://aiv.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://jzm.gaohongyu789.top

TS:   while (i < 10) { i++; }
来源：http://omm.jlsjyb.cn

Java: while (i < 10) { i++; }
来源：http://cff.sxryk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lut.vqdsnc.cn

Ruby: while i < 10; i += 1; end
来源：http://etr.vqdsnc.cn

C#:   while (i < 10) { i++; }
来源：http://ggh.fzhhl.top

[B08] do-while（至少执行一次）
来源：http://mgk.yangfankeji.com

Py:   # 无 do-while：用 while True + break
来源：http://fdb.zycfv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ovs.shanyushiyangtech.top

JS:   do { i++; } while (i < 10);
来源：http://kau.redwolf501.top

TS:   do { i++; } while (i < 10);
来源：http://fbo.fanxiaobao.xyz

Java: do { i++; } while (i < 10);
来源：http://fic.zhengqikj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tly.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://kir.ydzc1.top

C#:   do { i++; } while (i < 10);
来源：http://slj.chenzaomai.com

[B09] break 与 continue
来源：http://lqo.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ptu.sweek.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://txg.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tuq.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bze.316326.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bir.shangyingyoupin.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uhd.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iol.bjfxy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bge.tanke756.top

[B10] 遍历同时拿索引
来源：http://vep.zhaomingkeji.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wxb.chenjidiqi.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jvx.ivvv.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dgc.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ael.pengpengdd.cyou

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yeb.yueranfly.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://agx.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gnl.bbcook.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ave.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://yrd.sjlbkw.cn

Py:   list(range(0, 10, 2))
来源：http://mus.shanyushiyangkeji.top

PHP:  range(0, 10, 2);
来源：http://vzj.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ypz.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sms.dianchejie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qwo.svipenyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bwz.iojbl.cn

Ruby: (0...10).step(2).to_a
来源：http://ify.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zas.pengpengdd.cyou

[B12] 跳出多层循环
来源：http://jdj.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://kuz.snrcjt.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dvg.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mya.nanxuanxn.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sfn.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vjg.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://joe.xinyue.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wrl.shangyingyoupin.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hrq.chenzaomai.com

[B13] 判断是否为数字
来源：http://lal.guowangkeji.top

Py:   isinstance(x, (int, float))
来源：http://uss.pycfn.com

PHP:  is_numeric($x)
来源：http://vvz.zhixingplan.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://whn.chenzaomai.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://led.zhaomingkeji.xyz

Java: x instanceof Number
来源：http://oan.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://igh.kuanghao11.cn

Ruby: x.is_a?(Numeric)
来源：http://lna.xylfe.cn

C#:   x is int or double or decimal
来源：http://ltk.xingfuxueyuan.xyz

[B14] 判断值是否在集合内
来源：http://lud.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xgv.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bgl.svipenyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://tpm.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://sra.nanxuanxn.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cqw.jqgufenzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://emg.nanxuanxn.top

Ruby: [1, 2, 3].include?(x)
来源：http://nnq.shuidangran.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://obs.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://hbg.yonumen.top

Py:   a and b or not c
来源：http://hlx.ehwqpu.com

PHP:  $a && $b || !$c
来源：http://rue.shuidangran.top

JS:   a && b || !c
来源：http://bwh.feifeiyinyue.top

TS:   a && b || !c
来源：http://naq.yongpay.top

Java: a && b || !c
来源：http://xzj.hfpthk.cn

Go:   a && b || !c
来源：http://rdw.zhoulong.xyz

Ruby: a && b || !c
来源：http://ahx.zhijiandao.cn

C#:   a && b || !c
来源：http://zho.aibaodan.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jna.fanxiaobao.xyz

Py:   if not data: return
来源：http://onk.aibaodan.cn

PHP:  if (!$data) { return; }
来源：http://grp.yanxiufei.cn

JS:   if (!data) return;
来源：http://osw.pycfn.com

TS:   if (!data) return;
来源：http://ykp.fanxiaobao.xyz

Java: if (data == null) return;
来源：http://alv.316326.xyz

Go:   if data == nil { return }
来源：http://ryj.yj20258888.top

Ruby: return if data.nil?
来源：http://wuq.ppjwa.cn

C#:   if (data == null) return;
来源：http://dmn.tianlin.xyz

================================================================================
来源：http://lds.tianlin.xyz

C. 函数与作用域
来源：http://tsh.316326.xyz

================================================================================
来源：http://prc.sysykeji.top

[C01] 定义函数
来源：http://gci.hnxiangtu.top

Py:   def add(a, b): return a + b
来源：http://icg.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tvc.hesvh.cn

JS:   function add(a, b) { return a + b; }
来源：http://ved.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gfz.hysaishi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wqg.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://cea.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://vkn.cqqwz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://evl.cqqwz.cn

[C02] 默认参数
来源：http://zia.gaohongyu789.top

Py:   def greet(name="World"): return name
来源：http://cpi.jinqigufen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://eok.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://wqh.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dti.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wya.bbcook.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ojm.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://dpc.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://qql.yj202588.top

[C03] 可变参数
来源：http://ejj.tianlin.xyz

Py:   def total(*args): return sum(args)
来源：http://gcz.wangdashe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nnl.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oqx.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uxk.iojbl.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ers.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rgs.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mhf.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vcu.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://awk.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ohu.ctjpmb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yzy.xziqi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bzc.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vrn.ctjpmb.com

Java: // 无：用 Builder 模式或 record
来源：http://jfj.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://orc.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://wsw.shangyingyoupin.top

C#:   f(a: 1, b: 2)
来源：http://glw.dashuyun.cn

[C05] 返回多个值
来源：http://ljx.yj202588.top

Py:   return a, b
来源：http://yob.ybcxt.top

PHP:  return [$a, $b];
来源：http://sgu.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xdf.ehwqpu.com

TS:   return { a, b };
来源：http://zeo.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vvo.zhengqikj.top

Go:   return a, b
来源：http://una.gzhubu.top

Ruby: return a, b
来源：http://nbj.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://aws.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://dxs.sysykeji.top

Py:   square = lambda x: x * x
来源：http://vjo.jqgufenzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qsx.wangdashe.top

JS:   const square = x => x * x;
来源：http://yep.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://cgn.zhengqikj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tla.jianghu66.top

Go:   sq := func(x int) int { return x * x }
来源：http://qnd.birdmap.top

Ruby: square = ->(x) { x * x }
来源：http://mzg.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://ony.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://slq.gogol.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hne.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://loz.ywan-chungtsiang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ywz.guannengcc.top

TS:   arr.map(String)
来源：http://wwy.yanxiufei.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kwu.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kfi.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://vsq.sysykeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://czf.wangshuangyany.cn

[C08] 闭包
来源：http://zur.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://akk.vqdsnc.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kdx.zycfv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hpo.hfpthk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hss.redwolf501.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cjh.shanyushiyangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eom.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://twf.ywan-chungtsiang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hos.yuxming.cn

[C09] 递归
来源：http://ogw.tarul.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jze.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hia.daxiang520.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zbx.nwbrower.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dwh.tian-w.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gme.ywan-chungtsiang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jlp.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pcx.shanyushiyangtech.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pni.cheryme.top


<!-- 参考信息 -->