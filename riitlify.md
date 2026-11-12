代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://jdd.ehwqpu.com

Py:   ord("A"); chr(65)
来源：http://xny.xingfuxueyuan.xyz

PHP:  ord("A"); chr(65)
来源：http://not.bjfxy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qwu.shanyushiyangtech.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fkc.fktsv.cn

Java: (int) 'A'; (char) 65
来源：http://tyj.birdmap.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yeg.birdmap.top

Ruby: "A".ord; 65.chr
来源：http://oqx.xuanzx.com

C#:   (int)'A'; (char)65
来源：http://ayf.hammf.cn

[A19] 交换两个变量
来源：http://rir.gzhubu.top

Py:   a, b = b, a
来源：http://yih.tanke756.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ofe.jiagoushi.top

JS:   [a, b] = [b, a];
来源：http://ivw.yfazqb.com

TS:   [a, b] = [b, a];
来源：http://sxp.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://qtk.xziqi.cn

Go:   a, b = b, a
来源：http://knd.zycfv.cn

Ruby: a, b = b, a
来源：http://nfj.ydzc1.top

C#:   (a, b) = (b, a);
来源：http://xui.ppjwa.cn

[A20] 读取标准输入
来源：http://ihc.aibaodan.cn

Py:   name = input("请输入：")
来源：http://hgm.tanke756.top

PHP:  $name = trim(fgets(STDIN));
来源：http://fqi.jiagoushi.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ooo.haohaochexian.top

TS:   // Node.js：readline 模块
来源：http://eyh.tanke756.top

Java: new Scanner(System.in).nextLine()
来源：http://cxq.tianlin.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hfi.hcnkem.com

Ruby: gets.chomp
来源：http://ozm.chenlongwang.top

C#:   Console.ReadLine();
来源：http://mna.vqdsnc.cn

[A21] 保留指定小数位输出
来源：http://rlz.zhixingplan.top

Py:   f"{3.14159:.2f}"
来源：http://zii.zhixingplan.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://frt.pengpengdd.cyou

JS:   (3.14159).toFixed(2)
来源：http://wce.hammf.cn

TS:   (3.14159).toFixed(2)
来源：http://udh.vehdjk.com

Java: String.format("%.2f", 3.14159)
来源：http://squ.jqgfzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kea.zycfv.cn

Ruby: format("%.2f", 3.14159)
来源：http://whk.316326.xyz

C#:   3.14159.ToString("F2")
来源：http://iwx.yj202588.top

[A22] 获取字符串长度
来源：http://gxv.sxryk.cn

Py:   len(s)
来源：http://dmd.vehdjk.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xyo.fengsongda.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kip.zhixingplan.top

TS:   s.length
来源：http://ics.yuanzhike.top

Java: s.length()
来源：http://blc.hnqzz.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ovm.shzxlz.cn

Ruby: s.length
来源：http://xtc.xuetiantiany.cn

C#:   s.Length
来源：http://xbq.yueranfly.top

[A23] 大小写转换
来源：http://akk.ybcxt.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vzy.ivvv.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lbq.yanxiufei.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ztl.dashuyun.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kir.xinyue.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vmb.gzhubu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ojs.meibo888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bpw.aizwys.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jlw.nanxinkj.top

[A24] 去除首尾空白
来源：http://stp.uphjek.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yjv.cqqwz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tmp.jinqigufen.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://waj.shangyingyoupin.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pzi.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ijh.birdmap.top

Go:   strings.TrimSpace(s)
来源：http://bgh.jinqigfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xcm.daxiang520.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mch.fzhhl.top

[A25] 字符串比较
来源：http://egu.zhiwuduotai.top

Py:   s1 == s2; s1 != s2
来源：http://qfu.shanyushiyangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dep.hongshengwenyu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hzg.yongpay.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bcv.sufxvd.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ppj.tanke756.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://awh.chenlongwang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://aey.jinqigufen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://erq.cashguo.top

[A26] 类型转换总览
来源：http://gvu.redwolf501.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fmy.cucudq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ryx.ywan-chungtsiang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cgn.hfpthk.cn

TS:   Number() String() Boolean() x as number
来源：http://ptz.jqgfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://koc.jqgufenzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tpc.yueranfly.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://haz.guowangkeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nbs.smart0.xyz

================================================================================
来源：http://fdd.jyoumei.cn

B. 流程控制
来源：http://hwr.fanxiaobao.xyz

================================================================================
来源：http://apb.dianchejie.cn

[B01] 条件判断 if / else
来源：http://ufy.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zrj.shanyushiyangtech.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vfs.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rkh.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mpl.tianlin.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://mlt.gaohongyu789.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cfu.fanxiaobao.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hsz.wangshuangyany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vka.jqgfzy.top

[B02] 多分支 else if / elif
来源：http://gnk.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://flu.dianchejie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://drh.jinyuanbaomall.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hjc.redwolf501.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qzy.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oyo.guowangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bvv.nanxinkj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jeq.dashuyun.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cdx.daria6918.cn

[B03] switch / match / case
来源：http://ath.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fjt.yangfankeji.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://spt.hfpthk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jrn.zdbjq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ztq.hesvh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zez.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://acf.havefunace.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yge.ydjk.org.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xps.meibo888.top

[B04] for 计数循环
来源：http://oiv.quarkkingdee.top

Py:   for i in range(10): print(i)
来源：http://kls.shuidangran.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ila.xylfe.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vjs.yj202588.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nbn.chenzaomai.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uhq.ydjk.org.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sek.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://ind.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yum.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://xgx.vehdjk.com

Py:   for item in arr: print(item)
来源：http://sfq.9152youxi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oju.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ouf.jlsjyb.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kum.chenjidiqi.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://dvn.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://orm.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://eny.gzhubu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://frt.haohaochexian.top

[B06] 遍历字典 / 对象
来源：http://vzh.ybcxt.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tfk.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dil.fanxiaobao.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wgb.chenzaomai.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nwb.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://luo.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qri.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iql.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ecr.shanyushiyangtech.top

[B07] while 循环
来源：http://hal.9152youxi.cn

Py:   while i < 10: i += 1
来源：http://ten.shzxlz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://srz.chenlongwang.top

JS:   while (i < 10) { i++; }
来源：http://ufw.ctjpmb.com

TS:   while (i < 10) { i++; }
来源：http://lwx.cashguo.top

Java: while (i < 10) { i++; }
来源：http://nip.yj202588.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bya.feifeiyinyue.top

Ruby: while i < 10; i += 1; end
来源：http://vdf.zhongyouzk.top

C#:   while (i < 10) { i++; }
来源：http://vst.smart0.xyz

[B08] do-while（至少执行一次）
来源：http://whm.hnxiangtu.top

Py:   # 无 do-while：用 while True + break
来源：http://bss.fengsongda.top

PHP:  do { $i++; } while ($i < 10);
来源：http://sxp.dashuyun.cn

JS:   do { i++; } while (i < 10);
来源：http://rjv.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://cdk.haohaochexian.top

Java: do { i++; } while (i < 10);
来源：http://tki.shanyushiyangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uue.nwbrower.top

Ruby: begin; i += 1; end while i < 10
来源：http://rxn.dianchejie.cn

C#:   do { i++; } while (i < 10);
来源：http://etn.hnxiangtu.top

[B09] break 与 continue
来源：http://ewe.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ghi.ydzc1.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yzi.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://owo.wangshuangyany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qap.yonumen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eke.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hir.tianlin.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ybp.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ywc.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://fya.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://usz.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aho.xinyue.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hpx.316326.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pib.cashguo.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mnr.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dep.smart0.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kmp.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xgg.zhengqikj.top

[B11] 生成数字序列 / 区间
来源：http://xtl.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://qdw.quarkkingdee.top

PHP:  range(0, 10, 2);
来源：http://cft.52xcode.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dra.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jxa.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ooi.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eyy.ctjpmb.com

Ruby: (0...10).step(2).to_a
来源：http://krk.chenjidiqi.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://frn.0kj1m.cn

[B12] 跳出多层循环
来源：http://odz.jlsjyb.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vri.nwbrower.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ohr.cheryme.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fov.smart0.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://whp.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jlb.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iey.c1oappe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://udl.ydzc1.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dmq.yfazqb.com

[B13] 判断是否为数字
来源：http://rwu.ctjpmb.com

Py:   isinstance(x, (int, float))
来源：http://sju.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://uqe.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lnr.mhx1999.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mip.vqdsnc.cn

Java: x instanceof Number
来源：http://atu.wangdashe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ldo.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://pug.iojbl.cn

C#:   x is int or double or decimal
来源：http://bov.yanxiufei.cn

[B14] 判断值是否在集合内
来源：http://daf.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xgk.pycfn.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eoa.zdqjudy.top

JS:   [1, 2, 3].includes(x)
来源：http://tql.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://egh.hesvh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://btg.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hod.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://rxb.jinyuanbaomall.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ups.sysykeji.top

[B15] 布尔运算与取反
来源：http://xjm.yfazqb.com

Py:   a and b or not c
来源：http://ere.hysaishi.cn

PHP:  $a && $b || !$c
来源：http://ouv.ppjwa.cn

JS:   a && b || !c
来源：http://pje.xuetiantiany.cn

TS:   a && b || !c
来源：http://fff.yongpay.top

Java: a && b || !c
来源：http://uco.ehwqpu.com

Go:   a && b || !c
来源：http://hej.jlsjyb.cn

Ruby: a && b || !c
来源：http://jzq.kuanghao11.cn

C#:   a && b || !c
来源：http://jaq.chenzaomai.com

[B16] 卫语句：不满足条件提前返回
来源：http://nsi.gogol.net.cn

Py:   if not data: return
来源：http://wbl.aibaodan.cn

PHP:  if (!$data) { return; }
来源：http://hut.vehdjk.com

JS:   if (!data) return;
来源：http://cmv.yvedp.cn

TS:   if (!data) return;
来源：http://cly.jiagoushi.top

Java: if (data == null) return;
来源：http://lwl.vqdsnc.cn

Go:   if data == nil { return }
来源：http://evr.daria6918.cn

Ruby: return if data.nil?
来源：http://yhb.epnwcf.com

C#:   if (data == null) return;
来源：http://khw.smart0.xyz

================================================================================
来源：http://xaw.svipenyu.cn

C. 函数与作用域
来源：http://wds.wangshuangyany.cn

================================================================================
来源：http://sbr.zhongyouzk.top

[C01] 定义函数
来源：http://kss.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://kyo.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nud.zhixingplan.top

JS:   function add(a, b) { return a + b; }
来源：http://yin.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kqz.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://pcr.ywan-chungtsiang.top

Go:   func add(a, b int) int { return a + b }
来源：http://uoi.dianchejie.cn

Ruby: def add(a, b); a + b; end
来源：http://xud.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cmr.yangfankeji.com

[C02] 默认参数
来源：http://lft.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://iqe.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://wxi.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://ggm.yonumen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lyw.cashguo.top

Java: // 无默认参数：方法重载或 Optional
来源：http://alt.hywenlv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nsv.cdnleiting.top

Ruby: def greet(name = "World") = name
来源：http://dcp.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://rmz.sjlbkw.cn

[C03] 可变参数
来源：http://hwu.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://ibk.epnwcf.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://odw.feifeiyinyue.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rmq.zhiwuduotai.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tsu.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yuj.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wfs.ybcxt.top

Ruby: def total(*nums); nums.sum; end
来源：http://pys.birdmap.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aas.smart0.xyz

[C04] 命名参数 / 关键字参数
来源：http://nxj.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://adb.dianchejie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hhh.iojbl.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bcg.ppjwa.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ukd.fengsongda.top

Java: // 无：用 Builder 模式或 record
来源：http://xda.fengsongda.top

Go:   // 无：用配置结构体参数
来源：http://lxn.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://zkm.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://sqx.guannengcc.top

[C05] 返回多个值
来源：http://rkh.zdbjq.cn

Py:   return a, b
来源：http://uea.ppjwa.cn

PHP:  return [$a, $b];
来源：http://ntn.zhaomingkeji.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://riv.shangyingyoupin.top

TS:   return { a, b };
来源：http://lww.zhongyouzk.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zbs.jinqigufen.top

Go:   return a, b
来源：http://mjy.kuanghao11.cn

Ruby: return a, b
来源：http://tsc.ywan-chungtsiang.top

C#:   return (a, b);              // ValueTuple
来源：http://hrj.nanxuanxn.top

[C06] 匿名函数 / lambda
来源：http://pbb.daria6918.cn

Py:   square = lambda x: x * x
来源：http://ajh.zhoulong.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://afl.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://unw.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://ycl.xylfe.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://loc.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://jxc.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://jyw.zhengqikj.top

C#:   Func<int, int> square = x => x * x;
来源：http://ffv.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://voe.fehbvm.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mvv.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://wbi.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fvr.tianlin.xyz

TS:   arr.map(String)
来源：http://mef.yj202588.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tio.nanxinkj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://itr.ehwqpu.com

Ruby: arr.map(&:upcase)
来源：http://uty.jinqigfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ftx.ywan-chungtsiang.top

[C08] 闭包
来源：http://zzg.xylfe.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cbs.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://thq.pycfn.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bct.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://clz.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bvk.quarkkingdee.top


<!-- 参考信息 -->