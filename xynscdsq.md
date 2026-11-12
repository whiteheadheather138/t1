代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://mbh.zycfv.cn

Py:   ord("A"); chr(65)
来源：http://soi.cdnleiting.top

PHP:  ord("A"); chr(65)
来源：http://zwx.fanxiaobao.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cwi.tianlin.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nar.nwbrower.top

Java: (int) 'A'; (char) 65
来源：http://jdu.cdnleiting.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lbx.nanxuanxn.top

Ruby: "A".ord; 65.chr
来源：http://fyu.redwolf501.top

C#:   (int)'A'; (char)65
来源：http://bpf.jlsjyb.cn

[A19] 交换两个变量
来源：http://dmd.zdqjudy.top

Py:   a, b = b, a
来源：http://nyx.vehdjk.com

PHP:  [$a, $b] = [$b, $a];
来源：http://bct.ppjwa.cn

JS:   [a, b] = [b, a];
来源：http://ojs.yueranfly.top

TS:   [a, b] = [b, a];
来源：http://sgg.chenjidiqi.icu

Java: int t = a; a = b; b = t;
来源：http://yhb.bbcook.cn

Go:   a, b = b, a
来源：http://yku.ydzc1.top

Ruby: a, b = b, a
来源：http://kwy.yanxiufei.cn

C#:   (a, b) = (b, a);
来源：http://dju.kuanghao11.cn

[A20] 读取标准输入
来源：http://pft.zhoulong.xyz

Py:   name = input("请输入：")
来源：http://jcx.hysaishi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sxs.yfazqb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ciy.zhengqikj.top

TS:   // Node.js：readline 模块
来源：http://xky.zhaomingkeji.xyz

Java: new Scanner(System.in).nextLine()
来源：http://let.nwbrower.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ixu.nwbrower.top

Ruby: gets.chomp
来源：http://dss.cheryme.top

C#:   Console.ReadLine();
来源：http://rwt.guannengcc.top

[A21] 保留指定小数位输出
来源：http://jqn.xuanzx.com

Py:   f"{3.14159:.2f}"
来源：http://pkd.mhx1999.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fnc.jyoumei.cn

JS:   (3.14159).toFixed(2)
来源：http://dbi.xziqi.cn

TS:   (3.14159).toFixed(2)
来源：http://gcj.shuidangran.top

Java: String.format("%.2f", 3.14159)
来源：http://tye.sysykeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eaq.ehwqpu.com

Ruby: format("%.2f", 3.14159)
来源：http://eec.hywenlv.cn

C#:   3.14159.ToString("F2")
来源：http://drn.hnqzz.top

[A22] 获取字符串长度
来源：http://esp.yonumen.top

Py:   len(s)
来源：http://wtq.wangdashe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cqs.nanxinkj.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xfz.dashuyun.cn

TS:   s.length
来源：http://zfw.xinyue.icu

Java: s.length()
来源：http://ltm.gotoacloud.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://upi.smart0.xyz

Ruby: s.length
来源：http://taz.zhengqikj.top

C#:   s.Length
来源：http://gro.yvedp.cn

[A23] 大小写转换
来源：http://mat.guowangkeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wlt.c1oappe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yin.chenjidiqi.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cbq.fktsv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dfk.shzxlz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hnb.xuetiantiany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jlh.ydjk.org.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vjn.xuanzx.com

C#:   s.ToUpper(); s.ToLower()
来源：http://sfr.dianchejie.cn

[A24] 去除首尾空白
来源：http://orc.yj202588.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pnj.chenlongwang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uud.jqgfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ypq.ydzc1.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://has.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vjd.sufxvd.cn

Go:   strings.TrimSpace(s)
来源：http://jpp.0kj1m.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rhi.nanxuanxn.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mnu.sjlbkw.cn

[A25] 字符串比较
来源：http://tat.hammf.cn

Py:   s1 == s2; s1 != s2
来源：http://vzv.xylfe.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wfn.shangyingyoupin.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cdp.birdmap.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ovx.birdmap.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ocw.shanyushiyangtech.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eaw.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xpw.ctjpmb.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zbr.fzhhl.top

[A26] 类型转换总览
来源：http://jjt.yongpay.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://coj.snrcjt.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uks.tanke756.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rlc.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://dxh.bbcook.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vwt.shuidangran.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oll.cdnleiting.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://szi.shzxlz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ohk.9152youxi.cn

================================================================================
来源：http://qsw.cqqwz.cn

B. 流程控制
来源：http://bnw.bbcook.cn

================================================================================
来源：http://vyr.jinqigfzy.top

[B01] 条件判断 if / else
来源：http://oxd.gzhubu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://yee.pengpengdd.cyou

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kbi.mhx1999.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mzz.zhengqikj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://axa.guowangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://utm.cucudq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://efj.hywenlv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pdm.hfpthk.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vjl.shanyushiyangkeji.top

[B02] 多分支 else if / elif
来源：http://ymh.xuetiantiany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pbf.ywan-chungtsiang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lon.zhoulong.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mdo.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ums.chenjidiqi.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yto.sufxvd.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uvw.zhongyouzk.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jfp.yangfankeji.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ale.pycfn.com

[B03] switch / match / case
来源：http://hie.fzhhl.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ija.zycfv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mfb.xylfe.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://czj.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wmv.jinqigfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mdr.aibaodan.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sav.fzhhl.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uds.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eai.jinghuilouyu.cn

[B04] for 计数循环
来源：http://rfn.smart0.xyz

Py:   for i in range(10): print(i)
来源：http://okf.yj202588.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hto.meibo888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ksw.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pwl.gzhubu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zoy.tian-w.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lod.fehbvm.com

Ruby: 10.times { |i| puts i }
来源：http://emk.xziqi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hlv.wangdashe.top

[B05] 遍历数组 / 列表
来源：http://qnz.sweek.top

Py:   for item in arr: print(item)
来源：http://rdh.jiagoushi.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qjn.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qbi.jlsjyb.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ftp.bbcook.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ybi.cucudq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vjp.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://htk.uphjek.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zvh.yueranfly.top

[B06] 遍历字典 / 对象
来源：http://vpe.yonumen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vlo.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://buo.xuanzx.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ice.tianlin.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ups.ywan-chungtsiang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gfd.zdbjq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mtd.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hck.epnwcf.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qjx.cashguo.top

[B07] while 循环
来源：http://yqx.9152youxi.cn

Py:   while i < 10: i += 1
来源：http://iln.yj202588.top

PHP:  while ($i < 10) { $i++; }
来源：http://ucz.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://hbk.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://cfw.jinqigfzy.top

Java: while (i < 10) { i++; }
来源：http://wzl.hongshengwenyu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tyg.sysykeji.top

Ruby: while i < 10; i += 1; end
来源：http://xqs.jinghuilouyu.cn

C#:   while (i < 10) { i++; }
来源：http://ewu.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://mrx.yuxming.cn

Py:   # 无 do-while：用 while True + break
来源：http://hno.bbcook.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cva.haohaochexian.top

JS:   do { i++; } while (i < 10);
来源：http://vwr.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://fzn.zdbjq.cn

Java: do { i++; } while (i < 10);
来源：http://npc.chenjidiqi.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://hdh.chenlongwang.top

Ruby: begin; i += 1; end while i < 10
来源：http://zow.sufxvd.cn

C#:   do { i++; } while (i < 10);
来源：http://bma.uphjek.com

[B09] break 与 continue
来源：http://tpv.sxryk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fte.zhijiandao.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wye.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ayx.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tnv.ppjwa.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jgq.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://upi.birdmap.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jig.316326.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kbt.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://ags.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xup.zhengqikj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jle.xylfe.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://udq.fanxiaobao.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://voa.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qhs.yvedp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xyl.nanxinkj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ncy.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rxg.nwbrower.top

[B11] 生成数字序列 / 区间
来源：http://qiv.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://ygk.jinqigufen.top

PHP:  range(0, 10, 2);
来源：http://ylh.zhoulong.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ocd.fzhhl.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sgy.gotoacloud.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tvr.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ega.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://owx.bjfxy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jwp.zhengqikj.top

[B12] 跳出多层循环
来源：http://htn.uphjek.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://nyr.shanyushiyangtech.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lqx.hcnkem.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lte.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lpc.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://thw.hywenlv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://otq.redwolf501.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ans.chenjidiqi.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ila.yonumen.top

[B13] 判断是否为数字
来源：http://khy.daria6918.cn

Py:   isinstance(x, (int, float))
来源：http://sog.fktsv.cn

PHP:  is_numeric($x)
来源：http://vja.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uql.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ihs.zdbjq.cn

Java: x instanceof Number
来源：http://fwr.ctjpmb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iwa.yj202588.top

Ruby: x.is_a?(Numeric)
来源：http://qym.haohaochexian.top

C#:   x is int or double or decimal
来源：http://xju.zhixingplan.top

[B14] 判断值是否在集合内
来源：http://bta.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jfd.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://udk.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://iez.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://flv.meibo888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lrt.quarkkingdee.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oyf.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ctz.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aql.tarul.cn

[B15] 布尔运算与取反
来源：http://ajq.nanxinkj.top

Py:   a and b or not c
来源：http://cbs.yonumen.top

PHP:  $a && $b || !$c
来源：http://uaj.yonumen.top

JS:   a && b || !c
来源：http://rcv.yueranfly.top

TS:   a && b || !c
来源：http://eam.yfazqb.com

Java: a && b || !c
来源：http://wjp.yuanzhike.top

Go:   a && b || !c
来源：http://uph.xziqi.cn

Ruby: a && b || !c
来源：http://glb.xinyue.icu

C#:   a && b || !c
来源：http://muw.shuidangran.top

[B16] 卫语句：不满足条件提前返回
来源：http://ueh.shuidangran.top

Py:   if not data: return
来源：http://xie.yj202588.top

PHP:  if (!$data) { return; }
来源：http://cqu.tian-w.cn

JS:   if (!data) return;
来源：http://rjq.aibaodan.cn

TS:   if (!data) return;
来源：http://iyn.jianghu66.top

Java: if (data == null) return;
来源：http://cpf.birdmap.top

Go:   if data == nil { return }
来源：http://ico.birdmap.top

Ruby: return if data.nil?
来源：http://vcg.xingfuxueyuan.xyz

C#:   if (data == null) return;
来源：http://ozh.wangdashe.top

================================================================================
来源：http://oul.zhaomingkeji.xyz

C. 函数与作用域
来源：http://wzu.cdnleiting.top

================================================================================
来源：http://fbu.zdbjq.cn

[C01] 定义函数
来源：http://cct.yj202588.top

Py:   def add(a, b): return a + b
来源：http://hab.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zwn.shanyushiyangtech.top

JS:   function add(a, b) { return a + b; }
来源：http://vro.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://izg.chenjidiqi.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://kcz.shanyushiyangtech.top

Go:   func add(a, b int) int { return a + b }
来源：http://xet.zdqjudy.top

Ruby: def add(a, b); a + b; end
来源：http://spy.0kj1m.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://exm.meibo888.top

[C02] 默认参数
来源：http://arr.xuetiantiany.cn

Py:   def greet(name="World"): return name
来源：http://nxg.yfazqb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://hwa.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://lgn.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kpw.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nes.zhengqikj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bue.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://txr.jinyuanbaomall.cn

C#:   string Greet(string name = "World") => name;
来源：http://dzj.cdnleiting.top

[C03] 可变参数
来源：http://kja.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://nen.yongpay.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vtj.jiagoushi.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ird.dashuyun.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pgq.snrcjt.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ooa.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tca.aibaodan.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qnh.sysykeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tmh.fktsv.cn

[C04] 命名参数 / 关键字参数
来源：http://gup.bbcook.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fuy.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://myf.nanxinkj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eau.xinyue.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zio.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://owp.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://gyl.yj20258.top

Ruby: f(a: 1, b: 2)
来源：http://sby.9152youxi.cn

C#:   f(a: 1, b: 2)
来源：http://kwj.ybcxt.top

[C05] 返回多个值
来源：http://njo.yangfankeji.com

Py:   return a, b
来源：http://zwl.zdbjq.cn

PHP:  return [$a, $b];
来源：http://unp.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qfy.xingfuxueyuan.xyz

TS:   return { a, b };
来源：http://etp.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ewn.xingfuxueyuan.xyz

Go:   return a, b
来源：http://mmq.zhoulong.xyz

Ruby: return a, b
来源：http://bhv.ppjwa.cn

C#:   return (a, b);              // ValueTuple
来源：http://dhb.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://vzm.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://ysh.0kj1m.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vkp.tian-w.cn

JS:   const square = x => x * x;
来源：http://mvy.fzhhl.top

TS:   const square = (x: number): number => x * x;
来源：http://lzq.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kqr.c1oappe.top

Go:   sq := func(x int) int { return x * x }
来源：http://bxk.gaohongyu789.top

Ruby: square = ->(x) { x * x }
来源：http://oal.gzhubu.top

C#:   Func<int, int> square = x => x * x;
来源：http://exn.cucudq.cn

[C07] 把函数作为参数传入
来源：http://ncy.jinqigufen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ezh.iojbl.cn

PHP:  array_map("strtoupper", $arr);
来源：http://poq.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jtx.feifeiyinyue.top

TS:   arr.map(String)
来源：http://uzj.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://znc.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zoz.hongshengwenyu.top

Ruby: arr.map(&:upcase)
来源：http://gbo.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fyb.chenjidiqi.icu

[C08] 闭包
来源：http://bns.xylfe.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rxq.fehbvm.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dwb.fehbvm.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qco.zhongyouzk.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://okl.52xcode.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vsl.meibo888.top


<!-- 参考信息 -->