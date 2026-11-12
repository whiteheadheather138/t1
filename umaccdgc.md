代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dha.ehwqpu.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vno.daria6918.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nby.smart0.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lew.tianlin.xyz

[A18] 字符与 ASCII 码互转
来源：http://fzw.sjlbkw.cn

Py:   ord("A"); chr(65)
来源：http://odq.nanxuanxn.top

PHP:  ord("A"); chr(65)
来源：http://nsf.yuxming.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fcq.hongshengwenyu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://omw.smart0.xyz

Java: (int) 'A'; (char) 65
来源：http://emv.tian-w.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gch.jinyuanbaomall.cn

Ruby: "A".ord; 65.chr
来源：http://lcn.cdnleiting.top

C#:   (int)'A'; (char)65
来源：http://sjz.fanxiaobao.xyz

[A19] 交换两个变量
来源：http://hxd.cqqwz.cn

Py:   a, b = b, a
来源：http://bou.xinyue.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://dug.shanyushiyangtech.top

JS:   [a, b] = [b, a];
来源：http://qzo.aibaodan.cn

TS:   [a, b] = [b, a];
来源：http://zzl.zhiwuduotai.top

Java: int t = a; a = b; b = t;
来源：http://lvc.ydjk.org.cn

Go:   a, b = b, a
来源：http://enx.yonumen.top

Ruby: a, b = b, a
来源：http://gpb.yuxming.cn

C#:   (a, b) = (b, a);
来源：http://fas.hnqzz.top

[A20] 读取标准输入
来源：http://awn.shanyushiyangkeji.top

Py:   name = input("请输入：")
来源：http://pcq.tarul.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qxl.iojbl.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nyk.zhiwuduotai.top

TS:   // Node.js：readline 模块
来源：http://tkn.jinqigufen.top

Java: new Scanner(System.in).nextLine()
来源：http://mgd.jinyuanbaomall.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ijz.epnwcf.com

Ruby: gets.chomp
来源：http://zro.tianlin.xyz

C#:   Console.ReadLine();
来源：http://lnk.sweek.top

[A21] 保留指定小数位输出
来源：http://tlp.yvedp.cn

Py:   f"{3.14159:.2f}"
来源：http://vpv.nwbrower.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://smd.yonumen.top

JS:   (3.14159).toFixed(2)
来源：http://ogb.chenjidiqi.icu

TS:   (3.14159).toFixed(2)
来源：http://tnw.hesvh.cn

Java: String.format("%.2f", 3.14159)
来源：http://mpf.vehdjk.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gcn.ppjwa.cn

Ruby: format("%.2f", 3.14159)
来源：http://rjq.feifeiyinyue.top

C#:   3.14159.ToString("F2")
来源：http://rmb.xuanzx.com

[A22] 获取字符串长度
来源：http://ntc.dashuyun.cn

Py:   len(s)
来源：http://tys.gotoacloud.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rta.gzhubu.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kbc.52xcode.cn

TS:   s.length
来源：http://ise.ivvv.top

Java: s.length()
来源：http://arb.jinqigufen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://exx.hongshengwenyu.top

Ruby: s.length
来源：http://nto.yfazqb.com

C#:   s.Length
来源：http://itt.c1oappe.top

[A23] 大小写转换
来源：http://mtw.zdbjq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ehy.fanxiaobao.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lkb.chenzaomai.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gph.jinyuanbaomall.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pho.tarul.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xgk.zhengqikj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nse.yj20258.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bpn.fanxiaobao.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://fmn.zhongyouzk.top

[A24] 去除首尾空白
来源：http://wvf.iojbl.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zub.nanxuanxn.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dze.yuanzhike.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fjp.yangfankeji.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fso.zhiwuduotai.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zna.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://ybz.daxiang520.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lhx.yuxming.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hby.tanke756.top

[A25] 字符串比较
来源：http://yfa.jiagoushi.top

Py:   s1 == s2; s1 != s2
来源：http://kpz.zhoulong.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jnz.xziqi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hmn.daria6918.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tvn.aibaodan.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gbe.xuanzx.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cyb.sjlbkw.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kvv.ppjwa.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cwy.9152youxi.cn

[A26] 类型转换总览
来源：http://gyk.chenzaomai.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://miv.fzhhl.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jqb.fanxiaobao.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hhg.zhongyouzk.top

TS:   Number() String() Boolean() x as number
来源：http://lvg.xingfuxueyuan.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pwi.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yod.zhongyouzk.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://frh.fengsongda.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oqc.ybcxt.top

================================================================================
来源：http://kwd.cashguo.top

B. 流程控制
来源：http://bze.ydjk.org.cn

================================================================================
来源：http://uii.yvedp.cn

[B01] 条件判断 if / else
来源：http://eob.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://uqp.wangshuangyany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ubk.cheryme.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ccz.zhoulong.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nud.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ncb.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iuv.ivvv.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zls.yangfankeji.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ric.yj20258888.top

[B02] 多分支 else if / elif
来源：http://zzd.hongshengwenyu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aum.nanxuanxn.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sqd.0kj1m.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vox.fanxiaobao.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ibj.cheryme.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ked.cashguo.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ydf.vehdjk.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uva.sjlbkw.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eqp.52xcode.cn

[B03] switch / match / case
来源：http://yox.gotoacloud.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bch.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://shf.jqgfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tkw.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yna.yuxming.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ekp.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://psc.jqgufenzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ria.hongshengwenyu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ofa.havefunace.top

[B04] for 计数循环
来源：http://zjm.wangdashe.top

Py:   for i in range(10): print(i)
来源：http://tum.c1oappe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jvs.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xhw.zhijiandao.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://anz.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ezj.havefunace.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gzc.iojbl.cn

Ruby: 10.times { |i| puts i }
来源：http://xkh.shanyushiyangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gnk.gzhubu.top

[B05] 遍历数组 / 列表
来源：http://qxj.ivvv.top

Py:   for item in arr: print(item)
来源：http://iey.sjlbkw.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://udy.daxiang520.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fxh.mhx1999.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tti.cashguo.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://shy.jinqigfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://plf.yfazqb.com

Ruby: arr.each { |item| puts item }
来源：http://krx.zhaomingkeji.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ien.cheryme.top

[B06] 遍历字典 / 对象
来源：http://wvq.nwbrower.top

Py:   for k, v in d.items(): print(k, v)
来源：http://boc.yuanzhike.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bqm.yanxiufei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ffb.xinyue.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vxq.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zdb.jiagoushi.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zdi.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cte.sjlbkw.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lcm.wangdashe.top

[B07] while 循环
来源：http://uua.jqgufenzy.top

Py:   while i < 10: i += 1
来源：http://oti.meibo888.top

PHP:  while ($i < 10) { $i++; }
来源：http://fgo.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://guv.pengpengdd.cyou

TS:   while (i < 10) { i++; }
来源：http://grx.yj20258.top

Java: while (i < 10) { i++; }
来源：http://yfr.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xbr.zdqjudy.top

Ruby: while i < 10; i += 1; end
来源：http://mty.shuidangran.top

C#:   while (i < 10) { i++; }
来源：http://kqu.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://pnz.shanyushiyangtech.top

Py:   # 无 do-while：用 while True + break
来源：http://sfg.sweek.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mvt.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://uml.zhoulong.xyz

TS:   do { i++; } while (i < 10);
来源：http://jwm.ydzc1.top

Java: do { i++; } while (i < 10);
来源：http://eco.bbcook.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lgo.zdbjq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uxh.nanxinkj.top

C#:   do { i++; } while (i < 10);
来源：http://mbl.zhijiandao.cn

[B09] break 与 continue
来源：http://qhi.wangshuangyany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bnr.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iak.hongshengwenyu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eeu.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ihd.shangyingyoupin.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hwb.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://twm.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wft.aizwys.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oss.zhijiandao.cn

[B10] 遍历同时拿索引
来源：http://lfn.ctjpmb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qxx.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zod.9152youxi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jlc.sufxvd.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qiv.chenzaomai.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zmv.c1oappe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://svh.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wrn.hnxiangtu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nrb.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://oef.hnqzz.top

Py:   list(range(0, 10, 2))
来源：http://fgn.hongshengwenyu.top

PHP:  range(0, 10, 2);
来源：http://lgg.dianchejie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://loi.mhx1999.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hsq.feifeiyinyue.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dsp.nanxinkj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://opg.jinqigfzy.top

Ruby: (0...10).step(2).to_a
来源：http://rgo.svipenyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jwj.yj20258.top

[B12] 跳出多层循环
来源：http://wrj.birdmap.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rjx.shanyushiyangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://odi.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://psh.wangshuangyany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vmu.jlsjyb.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://frj.sxryk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://naw.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://syg.yj202588.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sbh.yj20258.top

[B13] 判断是否为数字
来源：http://yfm.zhoulong.xyz

Py:   isinstance(x, (int, float))
来源：http://gux.chenlongwang.top

PHP:  is_numeric($x)
来源：http://fvc.zhaomingkeji.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://frs.guowangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hzq.fengsongda.top

Java: x instanceof Number
来源：http://mvx.chenzaomai.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ylo.sxryk.cn

Ruby: x.is_a?(Numeric)
来源：http://spf.ydjk.org.cn

C#:   x is int or double or decimal
来源：http://wbm.ydzc1.top

[B14] 判断值是否在集合内
来源：http://dwq.bbcook.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bej.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jmd.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://dax.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://slg.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wbi.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sjq.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://aat.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pzo.sufxvd.cn

[B15] 布尔运算与取反
来源：http://mtn.dashuyun.cn

Py:   a and b or not c
来源：http://zpq.aizwys.cn

PHP:  $a && $b || !$c
来源：http://xvl.zhongyouzk.top

JS:   a && b || !c
来源：http://ulf.zdqjudy.top

TS:   a && b || !c
来源：http://wuj.cheryme.top

Java: a && b || !c
来源：http://afo.guowangkeji.top

Go:   a && b || !c
来源：http://aoa.cdnleiting.top

Ruby: a && b || !c
来源：http://kpf.sweek.top

C#:   a && b || !c
来源：http://fbf.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zzf.jqgfzy.top

Py:   if not data: return
来源：http://rrd.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://dbq.hfpthk.cn

JS:   if (!data) return;
来源：http://woh.nanxinkj.top

TS:   if (!data) return;
来源：http://pnq.vqdsnc.cn

Java: if (data == null) return;
来源：http://tas.hywenlv.cn

Go:   if data == nil { return }
来源：http://guv.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://lep.gogol.net.cn

C#:   if (data == null) return;
来源：http://jjn.cucudq.cn

================================================================================
来源：http://kao.mhx1999.top

C. 函数与作用域
来源：http://nsy.ppjwa.cn

================================================================================
来源：http://tln.daxiang520.top

[C01] 定义函数
来源：http://brx.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://jep.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bno.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://qjp.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rxy.jinyuanbaomall.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://drp.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://gnw.jianghu66.top

Ruby: def add(a, b); a + b; end
来源：http://qcc.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nlc.yj202588.top

[C02] 默认参数
来源：http://aad.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://waa.gotoacloud.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ibo.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://dmy.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://icd.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fbz.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cwh.cheryme.top

Ruby: def greet(name = "World") = name
来源：http://vch.daria6918.cn

C#:   string Greet(string name = "World") => name;
来源：http://yla.ppjwa.cn

[C03] 可变参数
来源：http://nsw.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://sit.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cph.gzhubu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mge.hywenlv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gsg.zhoulong.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hca.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xwd.jinqigfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://vte.smart0.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qby.sufxvd.cn

[C04] 命名参数 / 关键字参数
来源：http://dic.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gjo.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yye.fehbvm.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hyh.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gtt.yueranfly.top

Java: // 无：用 Builder 模式或 record
来源：http://bkg.bjfxy.top

Go:   // 无：用配置结构体参数
来源：http://pvd.jianghu66.top

Ruby: f(a: 1, b: 2)
来源：http://xsq.wangshuangyany.cn

C#:   f(a: 1, b: 2)
来源：http://wxh.yuanzhike.top

[C05] 返回多个值
来源：http://tfp.yfazqb.com

Py:   return a, b
来源：http://dws.svipenyu.cn

PHP:  return [$a, $b];
来源：http://mkj.hfpthk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qvk.ivvv.top

TS:   return { a, b };
来源：http://afo.xuetiantiany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://abc.guowangkeji.top

Go:   return a, b
来源：http://wvg.yueranfly.top

Ruby: return a, b
来源：http://oan.ehwqpu.com

C#:   return (a, b);              // ValueTuple
来源：http://lex.sxryk.cn

[C06] 匿名函数 / lambda
来源：http://wei.cdnleiting.top

Py:   square = lambda x: x * x
来源：http://opk.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ecl.iojbl.cn

JS:   const square = x => x * x;
来源：http://juf.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://eqb.ywan-chungtsiang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cqr.yuxming.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cae.ivvv.top

Ruby: square = ->(x) { x * x }
来源：http://hnm.hongshengwenyu.top

C#:   Func<int, int> square = x => x * x;
来源：http://nxm.ydjk.org.cn

[C07] 把函数作为参数传入
来源：http://hcj.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gxq.wangdashe.top

PHP:  array_map("strtoupper", $arr);
来源：http://yaw.yangfankeji.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mzl.xylfe.cn

TS:   arr.map(String)
来源：http://wwk.ydzc1.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://djr.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gkl.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://kzb.jinghuilouyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fku.yj20258.top

[C08] 闭包
来源：http://rfv.hongshengwenyu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xbr.yfazqb.com


<!-- 参考信息 -->