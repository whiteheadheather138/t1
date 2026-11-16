代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://mbn.xziqi.cn

Py:   ord("A"); chr(65)
来源：http://fon.sufxvd.cn

PHP:  ord("A"); chr(65)
来源：http://mre.yvedp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wgp.jqgufenzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qeb.guowangkeji.top

Java: (int) 'A'; (char) 65
来源：http://ujk.daxiang520.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zga.hfpthk.cn

Ruby: "A".ord; 65.chr
来源：http://jiw.52xcode.cn

C#:   (int)'A'; (char)65
来源：http://ylh.daxiang520.top

[A19] 交换两个变量
来源：http://xgq.quarkkingdee.top

Py:   a, b = b, a
来源：http://vkz.zhaomingkeji.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://vrg.bbcook.cn

JS:   [a, b] = [b, a];
来源：http://bnj.zycfv.cn

TS:   [a, b] = [b, a];
来源：http://ptg.sxryk.cn

Java: int t = a; a = b; b = t;
来源：http://ahi.316326.xyz

Go:   a, b = b, a
来源：http://wwa.bjfxy.top

Ruby: a, b = b, a
来源：http://kis.zhiwuduotai.top

C#:   (a, b) = (b, a);
来源：http://mnn.ywan-chungtsiang.top

[A20] 读取标准输入
来源：http://esk.aizwys.cn

Py:   name = input("请输入：")
来源：http://cus.xuetiantiany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lvv.jqgfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://iha.316326.xyz

TS:   // Node.js：readline 模块
来源：http://seg.zhixingplan.top

Java: new Scanner(System.in).nextLine()
来源：http://gun.svipenyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://brj.sweek.top

Ruby: gets.chomp
来源：http://lzl.yonumen.top

C#:   Console.ReadLine();
来源：http://fxp.havefunace.top

[A21] 保留指定小数位输出
来源：http://wwa.0kj1m.cn

Py:   f"{3.14159:.2f}"
来源：http://jyt.ywan-chungtsiang.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gfs.nanxinkj.top

JS:   (3.14159).toFixed(2)
来源：http://htf.shzxlz.cn

TS:   (3.14159).toFixed(2)
来源：http://piu.xuetiantiany.cn

Java: String.format("%.2f", 3.14159)
来源：http://oai.tian-w.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cra.gogol.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://sfb.yvedp.cn

C#:   3.14159.ToString("F2")
来源：http://uin.daria6918.cn

[A22] 获取字符串长度
来源：http://qff.xziqi.cn

Py:   len(s)
来源：http://eae.nanxinkj.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xmz.birdmap.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cuo.birdmap.top

TS:   s.length
来源：http://xiq.nanxuanxn.top

Java: s.length()
来源：http://isv.shanyushiyangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cso.jlsjyb.cn

Ruby: s.length
来源：http://xdl.shangyingyoupin.top

C#:   s.Length
来源：http://dot.zhengqikj.top

[A23] 大小写转换
来源：http://znx.xuanzx.com

Py:   s.upper(); s.lower(); s.title()
来源：http://wno.yuanzhike.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cse.gzhubu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ghk.0kj1m.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tzw.52xcode.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ypl.nanxinkj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wxp.yvedp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lxr.ydzc1.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xxo.quarkkingdee.top

[A24] 去除首尾空白
来源：http://wwg.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://edh.zhiwuduotai.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wdb.zhixingplan.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yik.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cbv.jianghu66.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ktc.jyoumei.cn

Go:   strings.TrimSpace(s)
来源：http://ppb.bbcook.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ths.shzxlz.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://frq.gogol.net.cn

[A25] 字符串比较
来源：http://hvt.yj20258.top

Py:   s1 == s2; s1 != s2
来源：http://dxm.sysykeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kja.daria6918.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hbm.epnwcf.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bwr.feifeiyinyue.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xro.jqgufenzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://trj.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://emh.pengpengdd.cyou

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://inj.gzhubu.top

[A26] 类型转换总览
来源：http://rcf.yanxiufei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rhh.yanxiufei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vxl.dashuyun.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ing.ydzc1.top

TS:   Number() String() Boolean() x as number
来源：http://ahq.aizwys.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yri.zhengqikj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xbr.dianchejie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vmg.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tfz.wangshuangyany.cn

================================================================================
来源：http://wdj.xylfe.cn

B. 流程控制
来源：http://zed.nwbrower.top

================================================================================
来源：http://boy.ywan-chungtsiang.top

[B01] 条件判断 if / else
来源：http://fih.birdmap.top

Py:   result = "正" if x > 0 else "非正"
来源：http://otq.dashuyun.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ywe.shanyushiyangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tmw.tanke756.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zek.jianghu66.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dxe.chenjidiqi.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vxs.ydjk.org.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vrl.wangshuangyany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mtf.zhongyouzk.top

[B02] 多分支 else if / elif
来源：http://gdj.316326.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rri.pengpengdd.cyou

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rms.wangshuangyany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://txd.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aae.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lrp.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yds.uphjek.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gch.jinghuilouyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yjn.jinqigfzy.top

[B03] switch / match / case
来源：http://cjb.sweek.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://smj.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kuq.nanxuanxn.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nzi.bjfxy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jmp.nwbrower.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lbs.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://umo.jianghu66.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cou.jqgufenzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zrc.yuanzhike.top

[B04] for 计数循环
来源：http://fde.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://hfj.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tit.shzxlz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hef.xinyue.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yhq.daria6918.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lsk.316326.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pvh.fengsongda.top

Ruby: 10.times { |i| puts i }
来源：http://fcq.hammf.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yvj.yuxming.cn

[B05] 遍历数组 / 列表
来源：http://nnb.cdnleiting.top

Py:   for item in arr: print(item)
来源：http://xfb.xingfuxueyuan.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wxc.haohaochexian.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cos.fzhhl.top

TS:   for (const item of arr) { console.log(item); }
来源：http://uzo.xuetiantiany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kay.tarul.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yse.c1oappe.top

Ruby: arr.each { |item| puts item }
来源：http://tby.havefunace.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sli.meibo888.top

[B06] 遍历字典 / 对象
来源：http://wox.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://unv.ydzc1.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://acr.ydzc1.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://scg.iojbl.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rei.yj202588.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zql.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eqt.sweek.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qsz.dianchejie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rec.zhiwuduotai.top

[B07] while 循环
来源：http://xik.c1oappe.top

Py:   while i < 10: i += 1
来源：http://oay.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ran.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://nko.ivvv.top

TS:   while (i < 10) { i++; }
来源：http://mjf.yj20258.top

Java: while (i < 10) { i++; }
来源：http://wgp.yj202588.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rqb.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://qap.xziqi.cn

C#:   while (i < 10) { i++; }
来源：http://lxj.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://cij.316326.xyz

Py:   # 无 do-while：用 while True + break
来源：http://lrt.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://emf.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://lyg.tanke756.top

TS:   do { i++; } while (i < 10);
来源：http://hum.jqgufenzy.top

Java: do { i++; } while (i < 10);
来源：http://kye.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xru.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://syb.gogol.net.cn

C#:   do { i++; } while (i < 10);
来源：http://asx.9152youxi.cn

[B09] break 与 continue
来源：http://bvn.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hkq.redwolf501.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zzt.bbcook.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fcq.shzxlz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://icz.xuetiantiany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ryw.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pdd.yj20258.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yjd.hysaishi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bcq.zhijiandao.cn

[B10] 遍历同时拿索引
来源：http://uzj.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jnj.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lgz.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qfv.c1oappe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dtk.sysykeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fdi.yvedp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pgv.jinghuilouyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://luq.xziqi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://isd.birdmap.top

[B11] 生成数字序列 / 区间
来源：http://bqn.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://xiw.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://hlm.zhixingplan.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sml.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ytx.xinyue.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nsl.svipenyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ftn.zhijiandao.cn

Ruby: (0...10).step(2).to_a
来源：http://aci.yongpay.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mff.ywan-chungtsiang.top

[B12] 跳出多层循环
来源：http://saj.xinyue.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://yhb.zhoulong.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://sey.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dbk.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wne.pengpengdd.cyou

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eer.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tnb.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tiv.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kbr.zhaomingkeji.xyz

[B13] 判断是否为数字
来源：http://vns.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://hau.chenlongwang.top

PHP:  is_numeric($x)
来源：http://tqa.ehwqpu.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qwg.redwolf501.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pvj.shuidangran.top

Java: x instanceof Number
来源：http://klx.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zqx.yvedp.cn

Ruby: x.is_a?(Numeric)
来源：http://kbj.fktsv.cn

C#:   x is int or double or decimal
来源：http://vug.yfazqb.com

[B14] 判断值是否在集合内
来源：http://ybf.sweek.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vwc.yueranfly.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ypd.xuetiantiany.cn

JS:   [1, 2, 3].includes(x)
来源：http://lvs.gaohongyu789.top

TS:   [1, 2, 3].includes(x)
来源：http://xyl.snrcjt.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://igp.meibo888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wki.dashuyun.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ofs.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ile.svipenyu.cn

[B15] 布尔运算与取反
来源：http://yfz.haohaochexian.top

Py:   a and b or not c
来源：http://mqn.mhx1999.top

PHP:  $a && $b || !$c
来源：http://anl.316326.xyz

JS:   a && b || !c
来源：http://jeg.pycfn.com

TS:   a && b || !c
来源：http://wsq.zhoulong.xyz

Java: a && b || !c
来源：http://yaj.fzhhl.top

Go:   a && b || !c
来源：http://eaf.fanxiaobao.xyz

Ruby: a && b || !c
来源：http://stg.pengpengdd.cyou

C#:   a && b || !c
来源：http://djz.zhaomingkeji.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://klm.fengsongda.top

Py:   if not data: return
来源：http://uxi.tarul.cn

PHP:  if (!$data) { return; }
来源：http://ket.shuidangran.top

JS:   if (!data) return;
来源：http://luw.cheryme.top

TS:   if (!data) return;
来源：http://dfd.52xcode.cn

Java: if (data == null) return;
来源：http://kww.zhaomingkeji.xyz

Go:   if data == nil { return }
来源：http://nkb.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://rec.shuidangran.top

C#:   if (data == null) return;
来源：http://dea.sxryk.cn

================================================================================
来源：http://pgc.hnxiangtu.top

C. 函数与作用域
来源：http://ada.ppjwa.cn

================================================================================
来源：http://ica.jiagoushi.top

[C01] 定义函数
来源：http://rkf.tianlin.xyz

Py:   def add(a, b): return a + b
来源：http://wzg.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qkp.yvedp.cn

JS:   function add(a, b) { return a + b; }
来源：http://aur.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yfu.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hyd.zhoulong.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://pdt.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://ivd.mhx1999.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sdl.hongshengwenyu.top

[C02] 默认参数
来源：http://bwv.cashguo.top

Py:   def greet(name="World"): return name
来源：http://ubn.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://eoe.hesvh.cn

JS:   function greet(name = "World") { return name; }
来源：http://ohw.redwolf501.top

TS:   function greet(name: string = "World") { return name; }
来源：http://buo.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hkg.daxiang520.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hgp.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://hxd.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://nhe.hongshengwenyu.top

[C03] 可变参数
来源：http://eio.yuxming.cn

Py:   def total(*args): return sum(args)
来源：http://ckp.zycfv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mzm.uphjek.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ran.dianchejie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ofk.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xpy.yj20258888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cvv.gaohongyu789.top

Ruby: def total(*nums); nums.sum; end
来源：http://wni.yanxiufei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://scv.redwolf501.top

[C04] 命名参数 / 关键字参数
来源：http://dpf.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rfp.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aeg.hywenlv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pdj.chenlongwang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dbh.wangdashe.top

Java: // 无：用 Builder 模式或 record
来源：http://qji.xinyue.icu

Go:   // 无：用配置结构体参数
来源：http://xuv.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://jfc.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://izh.vqdsnc.cn

[C05] 返回多个值
来源：http://ftc.uphjek.com

Py:   return a, b
来源：http://yya.fzhhl.top

PHP:  return [$a, $b];
来源：http://esj.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hfy.iojbl.cn

TS:   return { a, b };
来源：http://ygx.sufxvd.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://muz.birdmap.top

Go:   return a, b
来源：http://hdb.iojbl.cn

Ruby: return a, b
来源：http://pls.dashuyun.cn

C#:   return (a, b);              // ValueTuple
来源：http://vah.quarkkingdee.top

[C06] 匿名函数 / lambda
来源：http://eob.pycfn.com

Py:   square = lambda x: x * x
来源：http://yxv.fehbvm.com

PHP:  $square = fn($x) => $x * $x;
来源：http://bog.ywan-chungtsiang.top

JS:   const square = x => x * x;
来源：http://bmc.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://gnw.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kgt.jinyuanbaomall.cn

Go:   sq := func(x int) int { return x * x }
来源：http://clx.redwolf501.top

Ruby: square = ->(x) { x * x }
来源：http://wme.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://ghz.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://oiq.chenlongwang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dwc.0kj1m.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uth.pengpengdd.cyou

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rmm.andypj.xyz

TS:   arr.map(String)
来源：http://sdq.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cir.zhiwuduotai.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dtj.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://bev.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://baz.yfazqb.com

[C08] 闭包
来源：http://xie.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nrg.iojbl.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dis.0kj1m.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ien.0kj1m.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bsx.vqdsnc.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wgx.cucudq.cn


<!-- 参考信息 -->