代发 wailian999

JS:   [a, b] = [b, a];
来源：http://oxz.svipenyu.cn

TS:   [a, b] = [b, a];
来源：http://ujj.xinyue.icu

Java: int t = a; a = b; b = t;
来源：http://tgm.jqgufenzy.top

Go:   a, b = b, a
来源：http://vtt.shuidangran.top

Ruby: a, b = b, a
来源：http://thv.bjfxy.top

C#:   (a, b) = (b, a);
来源：http://ofm.tanke756.top

[A20] 读取标准输入
来源：http://ola.kuanghao11.cn

Py:   name = input("请输入：")
来源：http://bxc.nanxinkj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://uig.guowangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kyk.daria6918.cn

TS:   // Node.js：readline 模块
来源：http://dsf.hesvh.cn

Java: new Scanner(System.in).nextLine()
来源：http://yzx.guannengcc.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cmr.nwbrower.top

Ruby: gets.chomp
来源：http://cfq.hysaishi.cn

C#:   Console.ReadLine();
来源：http://ncn.zycfv.cn

[A21] 保留指定小数位输出
来源：http://kkd.meibo888.top

Py:   f"{3.14159:.2f}"
来源：http://mhp.yonumen.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ykp.yj20258.top

JS:   (3.14159).toFixed(2)
来源：http://vzt.uphjek.com

TS:   (3.14159).toFixed(2)
来源：http://ozj.pycfn.com

Java: String.format("%.2f", 3.14159)
来源：http://ehu.andypj.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://elc.ivvv.top

Ruby: format("%.2f", 3.14159)
来源：http://huo.xuetiantiany.cn

C#:   3.14159.ToString("F2")
来源：http://joh.bbcook.cn

[A22] 获取字符串长度
来源：http://wlb.vqdsnc.cn

Py:   len(s)
来源：http://bcw.ybcxt.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pwp.snrcjt.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fiw.zhengqikj.top

TS:   s.length
来源：http://fxp.daxiang520.top

Java: s.length()
来源：http://snd.zhongyouzk.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hrr.smart0.xyz

Ruby: s.length
来源：http://pft.dianchejie.cn

C#:   s.Length
来源：http://gbh.ppjwa.cn

[A23] 大小写转换
来源：http://ptd.nanxuanxn.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pnc.havefunace.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hdq.wangshuangyany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hgb.yueranfly.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nwy.cheryme.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kyg.yj202588.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://axm.daria6918.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mrw.dashuyun.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nea.zhoulong.xyz

[A24] 去除首尾空白
来源：http://htr.0kj1m.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yik.haohaochexian.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lhl.xylfe.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uxr.sufxvd.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lxj.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vnq.cucudq.cn

Go:   strings.TrimSpace(s)
来源：http://huw.zhongyouzk.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zbt.dashuyun.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mtx.uphjek.com

[A25] 字符串比较
来源：http://cag.zhaomingkeji.xyz

Py:   s1 == s2; s1 != s2
来源：http://usj.cdnleiting.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qla.hfpthk.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xlk.smart0.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iyo.bjfxy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ksn.xziqi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wkh.yueranfly.top

Ruby: s1 == s2; s1 <=> s2
来源：http://afd.jinqigfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wdr.daria6918.cn

[A26] 类型转换总览
来源：http://xjc.cqqwz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wih.zycfv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uxy.shangyingyoupin.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dva.fktsv.cn

TS:   Number() String() Boolean() x as number
来源：http://tsu.zhaomingkeji.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qdo.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kza.xinyue.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://yyy.aizwys.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://okv.cucudq.cn

================================================================================
来源：http://ihk.jinghuilouyu.cn

B. 流程控制
来源：http://wgp.0kj1m.cn

================================================================================
来源：http://xbk.yuanzhike.top

[B01] 条件判断 if / else
来源：http://qep.jinqigufen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://uzi.nanxuanxn.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hbx.nanxuanxn.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hlo.shuidangran.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://plq.hnxiangtu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://alb.shuidangran.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hdg.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sak.cqqwz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aun.c1oappe.top

[B02] 多分支 else if / elif
来源：http://zoy.bjfxy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ind.zhixingplan.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lgt.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pwx.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ufd.zhaomingkeji.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ofj.iojbl.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nsc.ydzc1.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vbm.mhx1999.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kxi.jinyuanbaomall.cn

[B03] switch / match / case
来源：http://bjr.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vxu.havefunace.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zgl.xuetiantiany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pkx.nwbrower.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://whe.mhx1999.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gec.tianlin.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iut.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eom.ctjpmb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kdl.yfazqb.com

[B04] for 计数循环
来源：http://mso.xuetiantiany.cn

Py:   for i in range(10): print(i)
来源：http://ben.sweek.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jie.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mtl.haohaochexian.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ghw.epnwcf.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ayu.jinghuilouyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sks.xuanzx.com

Ruby: 10.times { |i| puts i }
来源：http://egc.pengpengdd.cyou

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dwc.shuidangran.top

[B05] 遍历数组 / 列表
来源：http://uol.shanyushiyangkeji.top

Py:   for item in arr: print(item)
来源：http://ngc.ydjk.org.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://giu.sxryk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hgk.wangshuangyany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ard.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cos.xuanzx.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qfz.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://kyh.gaohongyu789.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uob.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://rgf.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://ejj.gotoacloud.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ltp.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mdo.guannengcc.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sfw.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ygj.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jbf.yanxiufei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kaw.xinyue.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rhk.cheryme.top

[B07] while 循环
来源：http://cic.yanxiufei.cn

Py:   while i < 10: i += 1
来源：http://gst.sysykeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://jzf.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://zep.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://nii.hfpthk.cn

Java: while (i < 10) { i++; }
来源：http://deu.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wtr.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://sos.snrcjt.cn

C#:   while (i < 10) { i++; }
来源：http://rvf.redwolf501.top

[B08] do-while（至少执行一次）
来源：http://jzb.jqgufenzy.top

Py:   # 无 do-while：用 while True + break
来源：http://yfv.smart0.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://stg.vehdjk.com

JS:   do { i++; } while (i < 10);
来源：http://cux.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://pbt.andypj.xyz

Java: do { i++; } while (i < 10);
来源：http://ooh.jianghu66.top

Go:   for { i++; if i >= 10 { break } }
来源：http://sip.jqgufenzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://ydl.shanyushiyangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://idj.zycfv.cn

[B09] break 与 continue
来源：http://vux.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rqp.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hln.0kj1m.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jjx.jinyuanbaomall.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://siw.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fjv.iojbl.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ajp.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nzs.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wbt.bjfxy.top

[B10] 遍历同时拿索引
来源：http://vkp.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lus.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ist.zhixingplan.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aoe.jqgfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mvu.c1oappe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jtj.yueranfly.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://icg.haohaochexian.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yrk.jyoumei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ftp.cqqwz.cn

[B11] 生成数字序列 / 区间
来源：http://ako.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://sys.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://ygp.chenjidiqi.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fpk.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oec.ehwqpu.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://brh.dashuyun.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fav.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://okq.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gjf.gotoacloud.top

[B12] 跳出多层循环
来源：http://ejx.yueranfly.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nem.shanyushiyangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lla.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://you.ywan-chungtsiang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bmb.dianchejie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ujg.chenjidiqi.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cvv.zhongyouzk.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vuu.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rkw.snrcjt.cn

[B13] 判断是否为数字
来源：http://owu.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://uuk.xziqi.cn

PHP:  is_numeric($x)
来源：http://yal.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xaf.jiagoushi.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qhx.yangfankeji.com

Java: x instanceof Number
来源：http://sty.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pqw.ydjk.org.cn

Ruby: x.is_a?(Numeric)
来源：http://tls.xziqi.cn

C#:   x is int or double or decimal
来源：http://zoq.sufxvd.cn

[B14] 判断值是否在集合内
来源：http://ltz.andypj.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ihk.jianghu66.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hpr.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://sbd.hesvh.cn

TS:   [1, 2, 3].includes(x)
来源：http://woa.wangshuangyany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vup.cashguo.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://efd.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://ija.jqgfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rtl.bjfxy.top

[B15] 布尔运算与取反
来源：http://ooj.hammf.cn

Py:   a and b or not c
来源：http://xmf.guannengcc.top

PHP:  $a && $b || !$c
来源：http://cqd.sysykeji.top

JS:   a && b || !c
来源：http://uhc.yonumen.top

TS:   a && b || !c
来源：http://kcx.zhengqikj.top

Java: a && b || !c
来源：http://zfn.nwbrower.top

Go:   a && b || !c
来源：http://aje.jiagoushi.top

Ruby: a && b || !c
来源：http://yiv.chenlongwang.top

C#:   a && b || !c
来源：http://mlf.ppjwa.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xut.ydzc1.top

Py:   if not data: return
来源：http://muq.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://cfo.yanxiufei.cn

JS:   if (!data) return;
来源：http://gzh.meibo888.top

TS:   if (!data) return;
来源：http://tkf.vehdjk.com

Java: if (data == null) return;
来源：http://jsw.aibaodan.cn

Go:   if data == nil { return }
来源：http://uiy.andypj.xyz

Ruby: return if data.nil?
来源：http://zwu.ivvv.top

C#:   if (data == null) return;
来源：http://aqm.yuanzhike.top

================================================================================
来源：http://gxe.aizwys.cn

C. 函数与作用域
来源：http://cny.chenlongwang.top

================================================================================
来源：http://tlx.wangdashe.top

[C01] 定义函数
来源：http://gpw.svipenyu.cn

Py:   def add(a, b): return a + b
来源：http://qud.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ctz.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://jcz.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uwz.sxryk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dnn.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mit.vqdsnc.cn

Ruby: def add(a, b); a + b; end
来源：http://uiz.fktsv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zsl.yj202588.top

[C02] 默认参数
来源：http://dsy.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://vfj.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://klr.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://gfj.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wmx.fzhhl.top

Java: // 无默认参数：方法重载或 Optional
来源：http://aos.ydjk.org.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://htb.snrcjt.cn

Ruby: def greet(name = "World") = name
来源：http://mdn.ywan-chungtsiang.top

C#:   string Greet(string name = "World") => name;
来源：http://zae.tanke756.top

[C03] 可变参数
来源：http://ogx.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://umo.birdmap.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gyl.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qcv.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gtd.bjfxy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jyq.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://srm.yonumen.top

Ruby: def total(*nums); nums.sum; end
来源：http://bsp.yanxiufei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xrb.shanyushiyangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://uqc.wangdashe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://let.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xcx.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bah.kuanghao11.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tkf.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://bqb.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://kjh.yongpay.top

Ruby: f(a: 1, b: 2)
来源：http://qgz.jianghu66.top

C#:   f(a: 1, b: 2)
来源：http://nvn.guowangkeji.top

[C05] 返回多个值
来源：http://zct.xingfuxueyuan.xyz

Py:   return a, b
来源：http://dhu.hcnkem.com

PHP:  return [$a, $b];
来源：http://uav.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://xri.zhiwuduotai.top

TS:   return { a, b };
来源：http://vuz.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ofo.9152youxi.cn

Go:   return a, b
来源：http://djs.ydjk.org.cn

Ruby: return a, b
来源：http://qqr.aibaodan.cn

C#:   return (a, b);              // ValueTuple
来源：http://gpl.tian-w.cn

[C06] 匿名函数 / lambda
来源：http://osm.tianlin.xyz

Py:   square = lambda x: x * x
来源：http://fih.shzxlz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wbh.jlsjyb.cn

JS:   const square = x => x * x;
来源：http://wgs.ybcxt.top

TS:   const square = (x: number): number => x * x;
来源：http://xfy.yj20258.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://amb.xingfuxueyuan.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://nyp.fehbvm.com

Ruby: square = ->(x) { x * x }
来源：http://elz.jqgufenzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://vnq.sweek.top

[C07] 把函数作为参数传入
来源：http://nzz.hongshengwenyu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://trp.hywenlv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tir.yonumen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wtk.aibaodan.cn

TS:   arr.map(String)
来源：http://miz.yuanzhike.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jil.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dox.zycfv.cn

Ruby: arr.map(&:upcase)
来源：http://nzk.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://jss.yongpay.top

[C08] 闭包
来源：http://wma.chenlongwang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://urd.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ist.jinqigufen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rqz.tian-w.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zty.fehbvm.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ezi.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yly.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://guz.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pnk.zdqjudy.top

[C09] 递归
来源：http://shb.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iei.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ash.vehdjk.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gyo.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bct.guowangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gqg.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ign.fengsongda.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yby.daxiang520.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nxq.guannengcc.top


<!-- 参考信息 -->