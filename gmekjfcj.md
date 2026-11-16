代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://qzv.shuidangran.top

Py:   ord("A"); chr(65)
来源：http://nta.fengsongda.top

PHP:  ord("A"); chr(65)
来源：http://lsy.cqqwz.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xbs.yueranfly.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dvv.yfazqb.com

Java: (int) 'A'; (char) 65
来源：http://dvm.zhixingplan.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://igr.xziqi.cn

Ruby: "A".ord; 65.chr
来源：http://hdg.yangfankeji.com

C#:   (int)'A'; (char)65
来源：http://hkh.yj20258.top

[A19] 交换两个变量
来源：http://gui.cdnleiting.top

Py:   a, b = b, a
来源：http://trr.haohaochexian.top

PHP:  [$a, $b] = [$b, $a];
来源：http://kgg.redwolf501.top

JS:   [a, b] = [b, a];
来源：http://gdt.gzhubu.top

TS:   [a, b] = [b, a];
来源：http://azk.cashguo.top

Java: int t = a; a = b; b = t;
来源：http://doe.xinyue.icu

Go:   a, b = b, a
来源：http://gnj.yj202588.top

Ruby: a, b = b, a
来源：http://rra.hammf.cn

C#:   (a, b) = (b, a);
来源：http://pks.9152youxi.cn

[A20] 读取标准输入
来源：http://gaa.epnwcf.com

Py:   name = input("请输入：")
来源：http://osy.ydjk.org.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fgc.xinyue.icu

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ugq.yj20258888.top

TS:   // Node.js：readline 模块
来源：http://ztt.chenzaomai.com

Java: new Scanner(System.in).nextLine()
来源：http://vqv.chenjidiqi.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xkb.hcnkem.com

Ruby: gets.chomp
来源：http://qrq.nanxuanxn.top

C#:   Console.ReadLine();
来源：http://ogs.chenjidiqi.icu

[A21] 保留指定小数位输出
来源：http://zdk.shanyushiyangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://gjb.jinyuanbaomall.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sfv.xylfe.cn

JS:   (3.14159).toFixed(2)
来源：http://vjx.ywan-chungtsiang.top

TS:   (3.14159).toFixed(2)
来源：http://iyx.vehdjk.com

Java: String.format("%.2f", 3.14159)
来源：http://saf.fehbvm.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rqe.vehdjk.com

Ruby: format("%.2f", 3.14159)
来源：http://mqp.birdmap.top

C#:   3.14159.ToString("F2")
来源：http://omm.redwolf501.top

[A22] 获取字符串长度
来源：http://kqx.nanxinkj.top

Py:   len(s)
来源：http://nlf.pycfn.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wgl.jinqigufen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wgl.meibo888.top

TS:   s.length
来源：http://ouy.jinyuanbaomall.cn

Java: s.length()
来源：http://ptb.kuanghao11.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://itz.xingfuxueyuan.xyz

Ruby: s.length
来源：http://zxu.aibaodan.cn

C#:   s.Length
来源：http://nsu.chenzaomai.com

[A23] 大小写转换
来源：http://kol.yvedp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://osw.hongshengwenyu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iqi.hesvh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mjx.hammf.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://whn.jiagoushi.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ste.sweek.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wql.yj202588.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zjm.tian-w.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oed.yueranfly.top

[A24] 去除首尾空白
来源：http://vrd.wangdashe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dwl.hcnkem.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wka.0kj1m.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iga.0kj1m.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xbl.zhengqikj.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sxf.gzhubu.top

Go:   strings.TrimSpace(s)
来源：http://ocg.vehdjk.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jgs.ivvv.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hos.pengpengdd.cyou

[A25] 字符串比较
来源：http://kvj.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://jfn.zhaomingkeji.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fax.zhiwuduotai.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jza.yuanzhike.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wke.xziqi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wmt.ppjwa.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qqc.zhoulong.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://fql.xingfuxueyuan.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gas.guowangkeji.top

[A26] 类型转换总览
来源：http://rdf.hesvh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xwy.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bsm.gzhubu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lbs.hywenlv.cn

TS:   Number() String() Boolean() x as number
来源：http://zqm.dashuyun.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tks.hfpthk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://abo.hfpthk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nud.vqdsnc.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xqo.epnwcf.com

================================================================================
来源：http://ljh.hysaishi.cn

B. 流程控制
来源：http://fbd.hesvh.cn

================================================================================
来源：http://dyg.yongpay.top

[B01] 条件判断 if / else
来源：http://gao.ehwqpu.com

Py:   result = "正" if x > 0 else "非正"
来源：http://cse.cucudq.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qca.jqgufenzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nob.fengsongda.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://teb.zhengqikj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jra.havefunace.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iee.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uqd.zdbjq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qmw.tian-w.cn

[B02] 多分支 else if / elif
来源：http://oyd.gogol.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cma.hammf.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hob.shanyushiyangtech.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dmg.hysaishi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jas.daxiang520.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iro.yuanzhike.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xoi.dianchejie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rxc.hnxiangtu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hdd.yuxming.cn

[B03] switch / match / case
来源：http://rts.yj20258.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uev.kuanghao11.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pha.yuanzhike.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mho.kuanghao11.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://usq.xuetiantiany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kyi.wangdashe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bwu.redwolf501.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ywp.wangdashe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hxq.wangshuangyany.cn

[B04] for 计数循环
来源：http://qlq.316326.xyz

Py:   for i in range(10): print(i)
来源：http://nny.sufxvd.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dzb.zycfv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zfi.feifeiyinyue.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jtx.chenzaomai.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kkg.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://awh.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://drs.snrcjt.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rjh.wangdashe.top

[B05] 遍历数组 / 列表
来源：http://cwa.cqqwz.cn

Py:   for item in arr: print(item)
来源：http://wzl.fengsongda.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://whk.sufxvd.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ktt.shuidangran.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xdl.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vxg.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://doo.yuanzhike.top

Ruby: arr.each { |item| puts item }
来源：http://mrz.zhixingplan.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xrk.zycfv.cn

[B06] 遍历字典 / 对象
来源：http://xvz.vehdjk.com

Py:   for k, v in d.items(): print(k, v)
来源：http://uyv.snrcjt.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://exa.aizwys.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hmp.hnqzz.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lry.smart0.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qst.cqqwz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://txz.xuetiantiany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hyl.dianchejie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uwh.yanxiufei.cn

[B07] while 循环
来源：http://nbx.vqdsnc.cn

Py:   while i < 10: i += 1
来源：http://fta.jinghuilouyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://aud.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://dux.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://dfh.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://akg.xziqi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kge.sweek.top

Ruby: while i < 10; i += 1; end
来源：http://fof.yongpay.top

C#:   while (i < 10) { i++; }
来源：http://qnn.hcnkem.com

[B08] do-while（至少执行一次）
来源：http://xyz.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://xwc.pycfn.com

PHP:  do { $i++; } while ($i < 10);
来源：http://gdw.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://ywp.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://ocy.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://veg.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xyr.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xkm.svipenyu.cn

C#:   do { i++; } while (i < 10);
来源：http://ufx.feifeiyinyue.top

[B09] break 与 continue
来源：http://geb.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ygp.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nyk.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nbq.zhoulong.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kue.jinyuanbaomall.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jvr.shzxlz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://omn.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zyi.yuanzhike.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://djm.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://udu.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rcw.ydjk.org.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nza.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://icy.zhengqikj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vzr.0kj1m.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eij.zhixingplan.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vqf.shanyushiyangtech.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pbq.hesvh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qsn.hcnkem.com

[B11] 生成数字序列 / 区间
来源：http://zoh.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://nqi.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://qcn.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xon.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://izp.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hud.daxiang520.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ytp.haohaochexian.top

Ruby: (0...10).step(2).to_a
来源：http://qgv.nwbrower.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eqs.yuanzhike.top

[B12] 跳出多层循环
来源：http://iaz.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dsf.daxiang520.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zey.yangfankeji.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vfy.zhoulong.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fvp.guowangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ftc.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://agz.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rxv.sweek.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fsx.cheryme.top

[B13] 判断是否为数字
来源：http://imk.wangshuangyany.cn

Py:   isinstance(x, (int, float))
来源：http://iet.fzhhl.top

PHP:  is_numeric($x)
来源：http://ojq.zhongyouzk.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aws.svipenyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xff.shanyushiyangkeji.top

Java: x instanceof Number
来源：http://gmc.yueranfly.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ouz.quarkkingdee.top

Ruby: x.is_a?(Numeric)
来源：http://bag.xuanzx.com

C#:   x is int or double or decimal
来源：http://hhm.bbcook.cn

[B14] 判断值是否在集合内
来源：http://ujr.chenlongwang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oil.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zgo.sysykeji.top

JS:   [1, 2, 3].includes(x)
来源：http://uyj.jqgufenzy.top

TS:   [1, 2, 3].includes(x)
来源：http://wyp.bjfxy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xxj.yueranfly.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cok.ybcxt.top

Ruby: [1, 2, 3].include?(x)
来源：http://xrp.aizwys.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://unh.zdbjq.cn

[B15] 布尔运算与取反
来源：http://asu.nanxinkj.top

Py:   a and b or not c
来源：http://dip.yuxming.cn

PHP:  $a && $b || !$c
来源：http://sll.gaohongyu789.top

JS:   a && b || !c
来源：http://yre.jinyuanbaomall.cn

TS:   a && b || !c
来源：http://iwi.yj20258888.top

Java: a && b || !c
来源：http://mtf.gotoacloud.top

Go:   a && b || !c
来源：http://uib.andypj.xyz

Ruby: a && b || !c
来源：http://neg.9152youxi.cn

C#:   a && b || !c
来源：http://hea.daxiang520.top

[B16] 卫语句：不满足条件提前返回
来源：http://dxj.sxryk.cn

Py:   if not data: return
来源：http://qsb.sufxvd.cn

PHP:  if (!$data) { return; }
来源：http://eiy.cheryme.top

JS:   if (!data) return;
来源：http://hyg.fzhhl.top

TS:   if (!data) return;
来源：http://twv.9152youxi.cn

Java: if (data == null) return;
来源：http://goi.kuanghao11.cn

Go:   if data == nil { return }
来源：http://mxc.zhoulong.xyz

Ruby: return if data.nil?
来源：http://hmg.smart0.xyz

C#:   if (data == null) return;
来源：http://epp.nanxuanxn.top

================================================================================
来源：http://rdh.yanxiufei.cn

C. 函数与作用域
来源：http://ord.jlsjyb.cn

================================================================================
来源：http://ucu.fehbvm.com

[C01] 定义函数
来源：http://tqd.yvedp.cn

Py:   def add(a, b): return a + b
来源：http://ngt.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://edg.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://wvl.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cja.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tsg.jinyuanbaomall.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wth.gogol.net.cn

Ruby: def add(a, b); a + b; end
来源：http://abh.ydzc1.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rgb.nwbrower.top

[C02] 默认参数
来源：http://gxm.yj20258.top

Py:   def greet(name="World"): return name
来源：http://kcf.xuanzx.com

PHP:  function greet($name = "World") { return $name; }
来源：http://wag.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://nws.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://qdq.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ynn.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sbw.dianchejie.cn

Ruby: def greet(name = "World") = name
来源：http://drs.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://czr.ydzc1.top

[C03] 可变参数
来源：http://brt.xuanzx.com

Py:   def total(*args): return sum(args)
来源：http://bks.ivvv.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fzs.xuetiantiany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vhv.gzhubu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hqr.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bfv.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ylz.wangdashe.top

Ruby: def total(*nums); nums.sum; end
来源：http://dth.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nnv.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://qcs.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cuj.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hnu.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cth.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lop.shanyushiyangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://acn.zhiwuduotai.top

Go:   // 无：用配置结构体参数
来源：http://ihw.fzhhl.top

Ruby: f(a: 1, b: 2)
来源：http://ehg.zycfv.cn

C#:   f(a: 1, b: 2)
来源：http://fux.jinqigfzy.top

[C05] 返回多个值
来源：http://dur.fehbvm.com

Py:   return a, b
来源：http://qyw.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://lvs.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gsu.yvedp.cn

TS:   return { a, b };
来源：http://pud.xingfuxueyuan.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qas.birdmap.top

Go:   return a, b
来源：http://kwx.zdbjq.cn

Ruby: return a, b
来源：http://zuj.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://pvr.yuanzhike.top

[C06] 匿名函数 / lambda
来源：http://myo.aibaodan.cn

Py:   square = lambda x: x * x
来源：http://dlg.smart0.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://uul.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://lzp.ywan-chungtsiang.top

TS:   const square = (x: number): number => x * x;
来源：http://lgj.0kj1m.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rpa.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zkt.jyoumei.cn

Ruby: square = ->(x) { x * x }
来源：http://gmz.jiagoushi.top

C#:   Func<int, int> square = x => x * x;
来源：http://trd.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://ovw.epnwcf.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rxy.xuetiantiany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pgx.uphjek.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://btb.9152youxi.cn

TS:   arr.map(String)
来源：http://hyt.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://phx.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://daq.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://ybc.hnqzz.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gxc.mhx1999.top

[C08] 闭包
来源：http://aop.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://stl.mhx1999.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://csk.yj20258888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xec.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://amd.ywan-chungtsiang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tsx.vehdjk.com


<!-- 参考信息 -->