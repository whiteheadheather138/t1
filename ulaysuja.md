代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zij.fehbvm.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://two.yuanzhike.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://koe.yfazqb.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hei.yj20258888.top

[A18] 字符与 ASCII 码互转
来源：http://umd.pycfn.com

Py:   ord("A"); chr(65)
来源：http://rhf.ctjpmb.com

PHP:  ord("A"); chr(65)
来源：http://eyn.hywenlv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kkp.xuetiantiany.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ctz.yfazqb.com

Java: (int) 'A'; (char) 65
来源：http://wwo.zdqjudy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nuw.shanyushiyangkeji.top

Ruby: "A".ord; 65.chr
来源：http://fag.ybcxt.top

C#:   (int)'A'; (char)65
来源：http://mhk.hysaishi.cn

[A19] 交换两个变量
来源：http://xyc.xinyue.icu

Py:   a, b = b, a
来源：http://awi.jinyuanbaomall.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qhx.vehdjk.com

JS:   [a, b] = [b, a];
来源：http://ndc.zdbjq.cn

TS:   [a, b] = [b, a];
来源：http://aci.shanyushiyangtech.top

Java: int t = a; a = b; b = t;
来源：http://yyo.fzhhl.top

Go:   a, b = b, a
来源：http://jip.yfazqb.com

Ruby: a, b = b, a
来源：http://dkp.yueranfly.top

C#:   (a, b) = (b, a);
来源：http://hny.chenlongwang.top

[A20] 读取标准输入
来源：http://tun.gogol.net.cn

Py:   name = input("请输入：")
来源：http://xma.yuanzhike.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ewq.shanyushiyangtech.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://azb.iojbl.cn

TS:   // Node.js：readline 模块
来源：http://jwm.jlsjyb.cn

Java: new Scanner(System.in).nextLine()
来源：http://cmz.zdbjq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ztc.cqqwz.cn

Ruby: gets.chomp
来源：http://olg.sweek.top

C#:   Console.ReadLine();
来源：http://dys.hysaishi.cn

[A21] 保留指定小数位输出
来源：http://mnx.yonumen.top

Py:   f"{3.14159:.2f}"
来源：http://bno.zhiwuduotai.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ttq.yueranfly.top

JS:   (3.14159).toFixed(2)
来源：http://ldi.sufxvd.cn

TS:   (3.14159).toFixed(2)
来源：http://ojv.bjfxy.top

Java: String.format("%.2f", 3.14159)
来源：http://haf.0kj1m.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wox.hongshengwenyu.top

Ruby: format("%.2f", 3.14159)
来源：http://neq.fehbvm.com

C#:   3.14159.ToString("F2")
来源：http://rza.yongpay.top

[A22] 获取字符串长度
来源：http://rod.hammf.cn

Py:   len(s)
来源：http://osi.feifeiyinyue.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kzd.zhiwuduotai.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wsv.tian-w.cn

TS:   s.length
来源：http://hbb.ydjk.org.cn

Java: s.length()
来源：http://ady.fktsv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yoz.jqgufenzy.top

Ruby: s.length
来源：http://uot.nanxinkj.top

C#:   s.Length
来源：http://dez.kuanghao11.cn

[A23] 大小写转换
来源：http://skg.shzxlz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jny.chenlongwang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qad.andypj.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mdv.epnwcf.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lbj.sxryk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://krh.yonumen.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eqm.yuxming.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bwa.iojbl.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mus.yj20258888.top

[A24] 去除首尾空白
来源：http://jjs.daxiang520.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xsf.shangyingyoupin.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vua.52xcode.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hln.aibaodan.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://snc.epnwcf.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gjf.yj202588.top

Go:   strings.TrimSpace(s)
来源：http://zpv.quarkkingdee.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ovr.ctjpmb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://npu.sjlbkw.cn

[A25] 字符串比较
来源：http://wej.aizwys.cn

Py:   s1 == s2; s1 != s2
来源：http://ctc.shzxlz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ame.gzhubu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kfc.zhaomingkeji.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://szj.gogol.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tfl.tarul.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gvz.yvedp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nbh.ydzc1.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tvu.cashguo.top

[A26] 类型转换总览
来源：http://aiz.yvedp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lql.aizwys.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yrs.tianlin.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hxp.smart0.xyz

TS:   Number() String() Boolean() x as number
来源：http://eny.yuanzhike.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wyc.fehbvm.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gop.chenlongwang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cbz.hnqzz.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jpz.yj202588.top

================================================================================
来源：http://grx.kuanghao11.cn

B. 流程控制
来源：http://uib.chenzaomai.com

================================================================================
来源：http://ycw.zdqjudy.top

[B01] 条件判断 if / else
来源：http://dxt.52xcode.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://idc.yj20258888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kpd.nwbrower.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ora.hcnkem.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://irw.bbcook.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sjl.cqqwz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zcm.pengpengdd.cyou

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hfn.hysaishi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mgp.guowangkeji.top

[B02] 多分支 else if / elif
来源：http://qsf.xylfe.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://etg.hywenlv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jje.yvedp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gtt.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jma.jqgufenzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oee.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nql.jinqigfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dvn.daxiang520.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wcj.xingfuxueyuan.xyz

[B03] switch / match / case
来源：http://zbf.shuidangran.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ozw.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tbb.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wwe.daria6918.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hra.hesvh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kww.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vit.chenjidiqi.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wdv.fengsongda.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aob.cucudq.cn

[B04] for 计数循环
来源：http://mls.birdmap.top

Py:   for i in range(10): print(i)
来源：http://yym.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sng.hongshengwenyu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ezt.xinyue.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ttm.dianchejie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://smh.gzhubu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vsl.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://vzk.52xcode.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tld.gotoacloud.top

[B05] 遍历数组 / 列表
来源：http://hqk.yuanzhike.top

Py:   for item in arr: print(item)
来源：http://plc.feifeiyinyue.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://soe.hesvh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gcm.xylfe.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ijc.nwbrower.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://anq.cucudq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zcy.gotoacloud.top

Ruby: arr.each { |item| puts item }
来源：http://rcz.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zuz.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://ruv.haohaochexian.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mwo.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xmg.9152youxi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lol.zhixingplan.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://duv.shangyingyoupin.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fak.tanke756.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://spg.fktsv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kks.fehbvm.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sqk.hysaishi.cn

[B07] while 循环
来源：http://pyl.pycfn.com

Py:   while i < 10: i += 1
来源：http://mrw.yuanzhike.top

PHP:  while ($i < 10) { $i++; }
来源：http://uso.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://fls.zdbjq.cn

TS:   while (i < 10) { i++; }
来源：http://fnw.c1oappe.top

Java: while (i < 10) { i++; }
来源：http://poi.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hhr.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://afx.hnqzz.top

C#:   while (i < 10) { i++; }
来源：http://zhc.svipenyu.cn

[B08] do-while（至少执行一次）
来源：http://ycn.daria6918.cn

Py:   # 无 do-while：用 while True + break
来源：http://une.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://xpw.zhixingplan.top

JS:   do { i++; } while (i < 10);
来源：http://qev.fanxiaobao.xyz

TS:   do { i++; } while (i < 10);
来源：http://muv.xinyue.icu

Java: do { i++; } while (i < 10);
来源：http://rxh.xylfe.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ylu.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://qln.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://jyc.tanke756.top

[B09] break 与 continue
来源：http://mmk.dashuyun.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vzg.sufxvd.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dqt.zhoulong.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nxe.zhixingplan.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wzw.cashguo.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jxb.pycfn.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mrr.vqdsnc.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vmx.aibaodan.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zvo.dashuyun.cn

[B10] 遍历同时拿索引
来源：http://eam.yfazqb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wsz.uphjek.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iiq.hcnkem.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mvt.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bqp.cheryme.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cvf.fanxiaobao.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nmk.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tsd.kuanghao11.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tvr.aibaodan.cn

[B11] 生成数字序列 / 区间
来源：http://tex.redwolf501.top

Py:   list(range(0, 10, 2))
来源：http://ybo.tarul.cn

PHP:  range(0, 10, 2);
来源：http://bga.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sly.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://odr.gaohongyu789.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wia.shzxlz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lhz.9152youxi.cn

Ruby: (0...10).step(2).to_a
来源：http://cya.jinyuanbaomall.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://axi.aizwys.cn

[B12] 跳出多层循环
来源：http://bax.dashuyun.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oiu.dashuyun.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dyk.shzxlz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mes.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hqc.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vpl.shzxlz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://viq.xziqi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wwe.tarul.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ysx.zhoulong.xyz

[B13] 判断是否为数字
来源：http://wps.yangfankeji.com

Py:   isinstance(x, (int, float))
来源：http://cgv.vqdsnc.cn

PHP:  is_numeric($x)
来源：http://pkv.sysykeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ust.pycfn.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://juv.fanxiaobao.xyz

Java: x instanceof Number
来源：http://sye.zhixingplan.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zut.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://gir.bjfxy.top

C#:   x is int or double or decimal
来源：http://xcj.fengsongda.top

[B14] 判断值是否在集合内
来源：http://vom.sysykeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qba.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qnu.pengpengdd.cyou

JS:   [1, 2, 3].includes(x)
来源：http://xmu.gogol.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://gse.daria6918.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fhk.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wqv.bjfxy.top

Ruby: [1, 2, 3].include?(x)
来源：http://dmk.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ukg.shangyingyoupin.top

[B15] 布尔运算与取反
来源：http://vhi.pycfn.com

Py:   a and b or not c
来源：http://fiz.iojbl.cn

PHP:  $a && $b || !$c
来源：http://bbq.sysykeji.top

JS:   a && b || !c
来源：http://znp.ivvv.top

TS:   a && b || !c
来源：http://emt.jqgfzy.top

Java: a && b || !c
来源：http://hsu.epnwcf.com

Go:   a && b || !c
来源：http://zdb.guowangkeji.top

Ruby: a && b || !c
来源：http://ynd.ivvv.top

C#:   a && b || !c
来源：http://ukr.hfpthk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ndj.cucudq.cn

Py:   if not data: return
来源：http://aus.zdbjq.cn

PHP:  if (!$data) { return; }
来源：http://sne.kuanghao11.cn

JS:   if (!data) return;
来源：http://mlh.fktsv.cn

TS:   if (!data) return;
来源：http://obm.bjfxy.top

Java: if (data == null) return;
来源：http://rsw.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://wfd.gaohongyu789.top

Ruby: return if data.nil?
来源：http://esy.zhongyouzk.top

C#:   if (data == null) return;
来源：http://fmt.zhijiandao.cn

================================================================================
来源：http://eur.epnwcf.com

C. 函数与作用域
来源：http://mxr.yfazqb.com

================================================================================
来源：http://wlc.vqdsnc.cn

[C01] 定义函数
来源：http://nsl.gzhubu.top

Py:   def add(a, b): return a + b
来源：http://wts.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bjb.epnwcf.com

JS:   function add(a, b) { return a + b; }
来源：http://gwd.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dig.gzhubu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nyy.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://wid.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://zzx.hammf.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jpx.fzhhl.top

[C02] 默认参数
来源：http://wrn.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://bba.shuidangran.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jxu.tian-w.cn

JS:   function greet(name = "World") { return name; }
来源：http://zfj.jianghu66.top

TS:   function greet(name: string = "World") { return name; }
来源：http://uar.ehwqpu.com

Java: // 无默认参数：方法重载或 Optional
来源：http://gru.fengsongda.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pkq.jinyuanbaomall.cn

Ruby: def greet(name = "World") = name
来源：http://nqa.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://ifb.jianghu66.top

[C03] 可变参数
来源：http://hdg.hnxiangtu.top

Py:   def total(*args): return sum(args)
来源：http://mfa.jlsjyb.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bii.jqgufenzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://akp.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mnm.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dzo.zhaomingkeji.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zsh.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://rxa.sufxvd.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zrg.yongpay.top

[C04] 命名参数 / 关键字参数
来源：http://osd.zhoulong.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rrm.yvedp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xxi.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wyc.jianghu66.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vdz.yj202588.top

Java: // 无：用 Builder 模式或 record
来源：http://qoi.yj20258888.top

Go:   // 无：用配置结构体参数
来源：http://bwf.dashuyun.cn

Ruby: f(a: 1, b: 2)
来源：http://rss.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://wyi.tianlin.xyz

[C05] 返回多个值
来源：http://ctc.hcnkem.com

Py:   return a, b
来源：http://ijo.hfpthk.cn

PHP:  return [$a, $b];
来源：http://jtk.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cpw.vqdsnc.cn

TS:   return { a, b };
来源：http://baa.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://omr.tianlin.xyz

Go:   return a, b
来源：http://wpx.hammf.cn

Ruby: return a, b
来源：http://yoy.zdqjudy.top

C#:   return (a, b);              // ValueTuple
来源：http://ule.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://yxl.tarul.cn

Py:   square = lambda x: x * x
来源：http://ugg.wangshuangyany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://idj.shzxlz.cn

JS:   const square = x => x * x;
来源：http://uyo.yuanzhike.top

TS:   const square = (x: number): number => x * x;
来源：http://sou.yj20258888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jji.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sdy.birdmap.top

Ruby: square = ->(x) { x * x }
来源：http://wuv.hywenlv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hjg.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://ens.ywan-chungtsiang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://elg.epnwcf.com

PHP:  array_map("strtoupper", $arr);
来源：http://umw.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qks.daxiang520.top

TS:   arr.map(String)
来源：http://daz.chenzaomai.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vse.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ddp.jqgfzy.top

Ruby: arr.map(&:upcase)
来源：http://ujb.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://vsn.xinyue.icu

[C08] 闭包
来源：http://ash.ivvv.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lsv.tanke756.top


<!-- 参考信息 -->