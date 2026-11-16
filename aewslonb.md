代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tiu.daxiang520.top

Java: (int) 'A'; (char) 65
来源：http://hsk.zhongyouzk.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://omk.xuetiantiany.cn

Ruby: "A".ord; 65.chr
来源：http://fcq.fzhhl.top

C#:   (int)'A'; (char)65
来源：http://wka.bjfxy.top

[A19] 交换两个变量
来源：http://ysa.bbcook.cn

Py:   a, b = b, a
来源：http://gvc.meibo888.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hjk.zhongyouzk.top

JS:   [a, b] = [b, a];
来源：http://dey.jinghuilouyu.cn

TS:   [a, b] = [b, a];
来源：http://kuu.fengsongda.top

Java: int t = a; a = b; b = t;
来源：http://qwm.guannengcc.top

Go:   a, b = b, a
来源：http://dfz.ehwqpu.com

Ruby: a, b = b, a
来源：http://ygm.shanyushiyangkeji.top

C#:   (a, b) = (b, a);
来源：http://qkh.ywan-chungtsiang.top

[A20] 读取标准输入
来源：http://biv.zhaomingkeji.xyz

Py:   name = input("请输入：")
来源：http://dll.hcnkem.com

PHP:  $name = trim(fgets(STDIN));
来源：http://lzy.hongshengwenyu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oms.zhixingplan.top

TS:   // Node.js：readline 模块
来源：http://tpq.shangyingyoupin.top

Java: new Scanner(System.in).nextLine()
来源：http://msb.chenlongwang.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rgm.bjfxy.top

Ruby: gets.chomp
来源：http://xyq.yonumen.top

C#:   Console.ReadLine();
来源：http://msw.tanke756.top

[A21] 保留指定小数位输出
来源：http://wjg.nanxinkj.top

Py:   f"{3.14159:.2f}"
来源：http://zxj.fengsongda.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://clj.xuetiantiany.cn

JS:   (3.14159).toFixed(2)
来源：http://qht.chenjidiqi.icu

TS:   (3.14159).toFixed(2)
来源：http://mtj.bbcook.cn

Java: String.format("%.2f", 3.14159)
来源：http://vxf.ctjpmb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ayd.jianghu66.top

Ruby: format("%.2f", 3.14159)
来源：http://aly.yuxming.cn

C#:   3.14159.ToString("F2")
来源：http://ota.xziqi.cn

[A22] 获取字符串长度
来源：http://reu.cucudq.cn

Py:   len(s)
来源：http://hzl.zhongyouzk.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://svv.tanke756.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vxy.yangfankeji.com

TS:   s.length
来源：http://riw.316326.xyz

Java: s.length()
来源：http://twr.aizwys.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vmb.quarkkingdee.top

Ruby: s.length
来源：http://ker.fengsongda.top

C#:   s.Length
来源：http://fhf.sweek.top

[A23] 大小写转换
来源：http://qlf.xuetiantiany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vcy.gogol.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xgg.shuidangran.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zln.xinyue.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://shz.cqqwz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xnn.xingfuxueyuan.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mtz.52xcode.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://soc.xziqi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nto.ydzc1.top

[A24] 去除首尾空白
来源：http://zud.xziqi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hkt.tanke756.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gqu.yueranfly.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://scg.ppjwa.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ata.gotoacloud.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zbs.yuxming.cn

Go:   strings.TrimSpace(s)
来源：http://hrh.cheryme.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kud.snrcjt.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hyl.mhx1999.top

[A25] 字符串比较
来源：http://sjk.yuxming.cn

Py:   s1 == s2; s1 != s2
来源：http://ouo.andypj.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dfk.aibaodan.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lvn.zhoulong.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://syx.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uql.aizwys.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gis.jianghu66.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kpt.zdbjq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pfx.cdnleiting.top

[A26] 类型转换总览
来源：http://dqb.xuanzx.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uda.9152youxi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pak.xziqi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://olr.zhaomingkeji.xyz

TS:   Number() String() Boolean() x as number
来源：http://yje.cqqwz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jib.hcnkem.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jwd.yj20258.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ucq.yuxming.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://msh.52xcode.cn

================================================================================
来源：http://imh.vqdsnc.cn

B. 流程控制
来源：http://hdv.zhiwuduotai.top

================================================================================
来源：http://lzq.birdmap.top

[B01] 条件判断 if / else
来源：http://iix.52xcode.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cdo.cucudq.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://upf.nanxinkj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vrx.smart0.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fnw.zhengqikj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jjy.c1oappe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://esp.gogol.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://juq.iojbl.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jbf.haohaochexian.top

[B02] 多分支 else if / elif
来源：http://yrr.redwolf501.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pjm.yanxiufei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qll.tianlin.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qsc.tanke756.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vex.yfazqb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xom.shanyushiyangtech.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bwp.nanxuanxn.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://etm.zhengqikj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zxl.jlsjyb.cn

[B03] switch / match / case
来源：http://uek.svipenyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://unn.dianchejie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tff.nanxuanxn.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hpv.daria6918.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kmx.tanke756.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ubq.jiagoushi.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qoa.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qeh.ydjk.org.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ugy.cheryme.top

[B04] for 计数循环
来源：http://lqi.gzhubu.top

Py:   for i in range(10): print(i)
来源：http://azt.guannengcc.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pkk.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yry.yj202588.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://swx.fehbvm.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qkx.chenjidiqi.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iqp.iojbl.cn

Ruby: 10.times { |i| puts i }
来源：http://vne.redwolf501.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ije.zhixingplan.top

[B05] 遍历数组 / 列表
来源：http://feb.zhengqikj.top

Py:   for item in arr: print(item)
来源：http://ddn.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xss.quarkkingdee.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xje.zycfv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lza.quarkkingdee.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vcn.feifeiyinyue.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://byg.xuanzx.com

Ruby: arr.each { |item| puts item }
来源：http://ksd.cheryme.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lne.nanxinkj.top

[B06] 遍历字典 / 对象
来源：http://zlm.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://swu.cashguo.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cyd.jqgufenzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cjk.nanxinkj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lhc.jqgufenzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sqn.zhengqikj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://edl.ctjpmb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yam.dashuyun.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yhj.zhengqikj.top

[B07] while 循环
来源：http://lrv.xylfe.cn

Py:   while i < 10: i += 1
来源：http://rzs.zycfv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zqz.zhiwuduotai.top

JS:   while (i < 10) { i++; }
来源：http://swr.iojbl.cn

TS:   while (i < 10) { i++; }
来源：http://flq.cashguo.top

Java: while (i < 10) { i++; }
来源：http://yul.shanyushiyangtech.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://shh.tianlin.xyz

Ruby: while i < 10; i += 1; end
来源：http://dle.shzxlz.cn

C#:   while (i < 10) { i++; }
来源：http://lca.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://scj.chenlongwang.top

Py:   # 无 do-while：用 while True + break
来源：http://yxy.bjfxy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nna.yuxming.cn

JS:   do { i++; } while (i < 10);
来源：http://aqt.jqgufenzy.top

TS:   do { i++; } while (i < 10);
来源：http://bfl.tarul.cn

Java: do { i++; } while (i < 10);
来源：http://tzz.yvedp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://clc.yj20258888.top

Ruby: begin; i += 1; end while i < 10
来源：http://lbe.yanxiufei.cn

C#:   do { i++; } while (i < 10);
来源：http://fhr.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://wxx.zycfv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dfy.vqdsnc.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ofq.bbcook.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dqx.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pap.fengsongda.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svo.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fyn.zycfv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eeb.zhiwuduotai.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yol.smart0.xyz

[B10] 遍历同时拿索引
来源：http://rcs.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rfv.feifeiyinyue.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cca.gzhubu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kge.gzhubu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rqx.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ljj.jianghu66.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xbj.jianghu66.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dws.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nmr.shanyushiyangkeji.top

[B11] 生成数字序列 / 区间
来源：http://emk.9152youxi.cn

Py:   list(range(0, 10, 2))
来源：http://wvq.316326.xyz

PHP:  range(0, 10, 2);
来源：http://awb.jinqigfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://swc.316326.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gxm.zhixingplan.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hpd.wangshuangyany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lsg.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://idx.ybcxt.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nje.zycfv.cn

[B12] 跳出多层循环
来源：http://htu.feifeiyinyue.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mmk.fzhhl.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rrb.pengpengdd.cyou

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://num.chenlongwang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zcf.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ysi.fktsv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hwh.hesvh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://exk.nanxinkj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fma.bjfxy.top

[B13] 判断是否为数字
来源：http://tjj.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://kxx.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://txe.chenzaomai.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iyo.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nkt.0kj1m.cn

Java: x instanceof Number
来源：http://jfl.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dxs.havefunace.top

Ruby: x.is_a?(Numeric)
来源：http://fcg.yonumen.top

C#:   x is int or double or decimal
来源：http://svj.uphjek.com

[B14] 判断值是否在集合内
来源：http://dsk.yvedp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dav.zhijiandao.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lbt.iojbl.cn

JS:   [1, 2, 3].includes(x)
来源：http://yon.bbcook.cn

TS:   [1, 2, 3].includes(x)
来源：http://ttq.shanyushiyangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mej.yvedp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dhz.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oxb.pycfn.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jix.shuidangran.top

[B15] 布尔运算与取反
来源：http://doy.chenjidiqi.icu

Py:   a and b or not c
来源：http://hfu.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://vrl.wangshuangyany.cn

JS:   a && b || !c
来源：http://jyl.andypj.xyz

TS:   a && b || !c
来源：http://fhm.jqgfzy.top

Java: a && b || !c
来源：http://rzq.gotoacloud.top

Go:   a && b || !c
来源：http://brn.epnwcf.com

Ruby: a && b || !c
来源：http://wjy.svipenyu.cn

C#:   a && b || !c
来源：http://kny.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fkh.tanke756.top

Py:   if not data: return
来源：http://scf.chenjidiqi.icu

PHP:  if (!$data) { return; }
来源：http://ivs.jyoumei.cn

JS:   if (!data) return;
来源：http://ija.hongshengwenyu.top

TS:   if (!data) return;
来源：http://tyw.gotoacloud.top

Java: if (data == null) return;
来源：http://nzy.zdbjq.cn

Go:   if data == nil { return }
来源：http://tsp.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://bxa.shuidangran.top

C#:   if (data == null) return;
来源：http://iev.andypj.xyz

================================================================================
来源：http://tpp.cashguo.top

C. 函数与作用域
来源：http://uzi.zhaomingkeji.xyz

================================================================================
来源：http://zcm.ivvv.top

[C01] 定义函数
来源：http://fas.hywenlv.cn

Py:   def add(a, b): return a + b
来源：http://gve.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eir.haohaochexian.top

JS:   function add(a, b) { return a + b; }
来源：http://qjj.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ipg.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://whf.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gvw.zhengqikj.top

Ruby: def add(a, b); a + b; end
来源：http://hru.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yro.zhoulong.xyz

[C02] 默认参数
来源：http://ksh.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://yeu.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://ugg.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://gou.pengpengdd.cyou

TS:   function greet(name: string = "World") { return name; }
来源：http://hpa.zhengqikj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://atb.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rae.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://wez.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://fds.aizwys.cn

[C03] 可变参数
来源：http://gwn.nanxuanxn.top

Py:   def total(*args): return sum(args)
来源：http://ofs.meibo888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fsf.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hul.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ghh.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sdu.yj202588.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wiv.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://snj.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vyu.zdqjudy.top

[C04] 命名参数 / 关键字参数
来源：http://ong.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fyg.yvedp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hwc.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ngb.shangyingyoupin.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ute.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://ycn.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://tgm.jinqigufen.top

Ruby: f(a: 1, b: 2)
来源：http://cts.daxiang520.top

C#:   f(a: 1, b: 2)
来源：http://ljh.zhijiandao.cn

[C05] 返回多个值
来源：http://cir.shzxlz.cn

Py:   return a, b
来源：http://dly.jyoumei.cn

PHP:  return [$a, $b];
来源：http://kzp.sjlbkw.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fsz.nwbrower.top

TS:   return { a, b };
来源：http://cke.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nsw.uphjek.com

Go:   return a, b
来源：http://rip.yj20258888.top

Ruby: return a, b
来源：http://fja.zhiwuduotai.top

C#:   return (a, b);              // ValueTuple
来源：http://mzj.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://xoq.zhongyouzk.top

Py:   square = lambda x: x * x
来源：http://nul.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yew.zhaomingkeji.xyz

JS:   const square = x => x * x;
来源：http://nyq.xylfe.cn

TS:   const square = (x: number): number => x * x;
来源：http://qhv.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://laq.feifeiyinyue.top

Go:   sq := func(x int) int { return x * x }
来源：http://pim.wangdashe.top

Ruby: square = ->(x) { x * x }
来源：http://opn.yuxming.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ybm.shanyushiyangtech.top

[C07] 把函数作为参数传入
来源：http://vrk.shuidangran.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://slg.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rbt.zhaomingkeji.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fhu.gogol.net.cn

TS:   arr.map(String)
来源：http://cjg.dianchejie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hkc.zhongyouzk.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xlz.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://ana.xuetiantiany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ixk.uphjek.com

[C08] 闭包
来源：http://igf.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ggj.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sqx.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jqs.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://htd.fehbvm.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qph.shzxlz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uvr.daxiang520.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pqx.xuanzx.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vhm.quarkkingdee.top

[C09] 递归
来源：http://dde.redwolf501.top


<!-- 参考信息 -->