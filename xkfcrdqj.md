代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://xno.xylfe.cn

Py:   ord("A"); chr(65)
来源：http://nhi.zhoulong.xyz

PHP:  ord("A"); chr(65)
来源：http://zfj.yongpay.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pjj.haohaochexian.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oar.cdnleiting.top

Java: (int) 'A'; (char) 65
来源：http://swg.cashguo.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tgs.yvedp.cn

Ruby: "A".ord; 65.chr
来源：http://nyl.fzhhl.top

C#:   (int)'A'; (char)65
来源：http://yyd.jlsjyb.cn

[A19] 交换两个变量
来源：http://ana.jlsjyb.cn

Py:   a, b = b, a
来源：http://dgu.quarkkingdee.top

PHP:  [$a, $b] = [$b, $a];
来源：http://spl.hywenlv.cn

JS:   [a, b] = [b, a];
来源：http://soh.meibo888.top

TS:   [a, b] = [b, a];
来源：http://hfs.pengpengdd.cyou

Java: int t = a; a = b; b = t;
来源：http://pbt.guannengcc.top

Go:   a, b = b, a
来源：http://gny.havefunace.top

Ruby: a, b = b, a
来源：http://cbb.gaohongyu789.top

C#:   (a, b) = (b, a);
来源：http://xfg.dashuyun.cn

[A20] 读取标准输入
来源：http://qju.ppjwa.cn

Py:   name = input("请输入：")
来源：http://uro.ivvv.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ypp.hysaishi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yck.hysaishi.cn

TS:   // Node.js：readline 模块
来源：http://edw.ydjk.org.cn

Java: new Scanner(System.in).nextLine()
来源：http://lxz.ppjwa.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ynv.meibo888.top

Ruby: gets.chomp
来源：http://zkf.chenlongwang.top

C#:   Console.ReadLine();
来源：http://ere.uphjek.com

[A21] 保留指定小数位输出
来源：http://hat.hnqzz.top

Py:   f"{3.14159:.2f}"
来源：http://rhf.fanxiaobao.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fgf.chenzaomai.com

JS:   (3.14159).toFixed(2)
来源：http://ilk.dashuyun.cn

TS:   (3.14159).toFixed(2)
来源：http://mqw.shuidangran.top

Java: String.format("%.2f", 3.14159)
来源：http://mgy.gzhubu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mux.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://fcu.zycfv.cn

C#:   3.14159.ToString("F2")
来源：http://twe.vqdsnc.cn

[A22] 获取字符串长度
来源：http://iil.ydjk.org.cn

Py:   len(s)
来源：http://qel.yvedp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pwr.svipenyu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ubh.shuidangran.top

TS:   s.length
来源：http://wag.gotoacloud.top

Java: s.length()
来源：http://eco.cucudq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hrp.hongshengwenyu.top

Ruby: s.length
来源：http://wai.jianghu66.top

C#:   s.Length
来源：http://obo.guowangkeji.top

[A23] 大小写转换
来源：http://cpf.cdnleiting.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xit.guowangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mcn.xylfe.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kfc.fengsongda.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://acw.wangshuangyany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qnf.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eez.zhijiandao.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gxz.hysaishi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://htd.shuidangran.top

[A24] 去除首尾空白
来源：http://ufy.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xdu.shangyingyoupin.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jdd.cheryme.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://chv.cashguo.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sjj.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kei.hywenlv.cn

Go:   strings.TrimSpace(s)
来源：http://nhu.uphjek.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kww.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://csa.smart0.xyz

[A25] 字符串比较
来源：http://kkp.cdnleiting.top

Py:   s1 == s2; s1 != s2
来源：http://acv.ctjpmb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ujd.daria6918.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bxt.zhoulong.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vah.yj202588.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hoa.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://htk.vehdjk.com

Ruby: s1 == s2; s1 <=> s2
来源：http://tuu.yuxming.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bpt.hnqzz.top

[A26] 类型转换总览
来源：http://jtn.pycfn.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sql.zhongyouzk.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jfe.snrcjt.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ceh.nwbrower.top

TS:   Number() String() Boolean() x as number
来源：http://vra.zhoulong.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qaa.gogol.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vsf.52xcode.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lzd.hcnkem.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ypq.hesvh.cn

================================================================================
来源：http://buj.sysykeji.top

B. 流程控制
来源：http://tfe.tian-w.cn

================================================================================
来源：http://aor.ivvv.top

[B01] 条件判断 if / else
来源：http://rpp.sjlbkw.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xjj.iojbl.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oba.daxiang520.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pmc.ydjk.org.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tjw.jianghu66.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fkl.shanyushiyangtech.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://szb.zhijiandao.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fff.nanxinkj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gty.vqdsnc.cn

[B02] 多分支 else if / elif
来源：http://nyf.xuetiantiany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://idc.chenjidiqi.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://utw.316326.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://trv.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mob.xuanzx.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ykd.cdnleiting.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sty.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bje.fehbvm.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sil.0kj1m.cn

[B03] switch / match / case
来源：http://had.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rag.havefunace.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://izw.guannengcc.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rdm.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wgz.svipenyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://saz.yangfankeji.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qbl.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bqi.redwolf501.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cpz.316326.xyz

[B04] for 计数循环
来源：http://yjy.dianchejie.cn

Py:   for i in range(10): print(i)
来源：http://xlq.0kj1m.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kvr.dashuyun.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aok.sxryk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ylk.haohaochexian.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jgz.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dej.xinyue.icu

Ruby: 10.times { |i| puts i }
来源：http://sot.jlsjyb.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gcu.xingfuxueyuan.xyz

[B05] 遍历数组 / 列表
来源：http://gti.epnwcf.com

Py:   for item in arr: print(item)
来源：http://mtt.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://afw.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ckc.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zxg.sufxvd.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bwx.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kck.fengsongda.top

Ruby: arr.each { |item| puts item }
来源：http://yvf.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tpf.ivvv.top

[B06] 遍历字典 / 对象
来源：http://piz.zhaomingkeji.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://xeb.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dof.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ibh.fktsv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jms.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lmd.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://opc.chenjidiqi.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wot.uphjek.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qgt.hesvh.cn

[B07] while 循环
来源：http://cnf.nwbrower.top

Py:   while i < 10: i += 1
来源：http://sqi.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://jbk.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://flx.fehbvm.com

TS:   while (i < 10) { i++; }
来源：http://ddd.ivvv.top

Java: while (i < 10) { i++; }
来源：http://khr.mhx1999.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wtv.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://zur.ywan-chungtsiang.top

C#:   while (i < 10) { i++; }
来源：http://nwb.yongpay.top

[B08] do-while（至少执行一次）
来源：http://lja.hnxiangtu.top

Py:   # 无 do-while：用 while True + break
来源：http://hkv.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zxx.yj20258888.top

JS:   do { i++; } while (i < 10);
来源：http://uwb.cqqwz.cn

TS:   do { i++; } while (i < 10);
来源：http://vju.nanxuanxn.top

Java: do { i++; } while (i < 10);
来源：http://xlq.nwbrower.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wau.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://rje.yuxming.cn

C#:   do { i++; } while (i < 10);
来源：http://uqa.yfazqb.com

[B09] break 与 continue
来源：http://ffv.jinghuilouyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gwy.zhoulong.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://esn.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zrp.hysaishi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aoh.xinyue.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tzv.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iap.yuxming.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jlc.yangfankeji.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xkb.sxryk.cn

[B10] 遍历同时拿索引
来源：http://ywc.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zkn.fzhhl.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zxd.jqgfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oth.zycfv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ute.hesvh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zxy.yongpay.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gty.fengsongda.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mys.ydjk.org.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jwe.yuanzhike.top

[B11] 生成数字序列 / 区间
来源：http://gci.gaohongyu789.top

Py:   list(range(0, 10, 2))
来源：http://ptq.vehdjk.com

PHP:  range(0, 10, 2);
来源：http://jru.sweek.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kiz.ehwqpu.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kun.zdqjudy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rex.chenzaomai.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xgh.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://wle.ctjpmb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pud.nanxinkj.top

[B12] 跳出多层循环
来源：http://ewo.gogol.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zfl.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://sth.zhixingplan.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tsl.smart0.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wzu.hfpthk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://san.fzhhl.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ngp.nwbrower.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bcl.jqgufenzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wfq.wangdashe.top

[B13] 判断是否为数字
来源：http://eat.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://zis.ivvv.top

PHP:  is_numeric($x)
来源：http://cvx.hywenlv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bsl.c1oappe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xac.dianchejie.cn

Java: x instanceof Number
来源：http://gfo.bbcook.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://myg.havefunace.top

Ruby: x.is_a?(Numeric)
来源：http://xlb.yuanzhike.top

C#:   x is int or double or decimal
来源：http://znp.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://xpa.chenzaomai.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kpx.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mtw.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://xja.sjlbkw.cn

TS:   [1, 2, 3].includes(x)
来源：http://pma.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bqf.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jxr.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://waj.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fbp.gaohongyu789.top

[B15] 布尔运算与取反
来源：http://smh.dashuyun.cn

Py:   a and b or not c
来源：http://ivi.yonumen.top

PHP:  $a && $b || !$c
来源：http://pcm.yuxming.cn

JS:   a && b || !c
来源：http://qgf.jiagoushi.top

TS:   a && b || !c
来源：http://exo.cashguo.top

Java: a && b || !c
来源：http://jzs.vehdjk.com

Go:   a && b || !c
来源：http://mlc.yfazqb.com

Ruby: a && b || !c
来源：http://hlz.mhx1999.top

C#:   a && b || !c
来源：http://gki.kuanghao11.cn

[B16] 卫语句：不满足条件提前返回
来源：http://thz.zdbjq.cn

Py:   if not data: return
来源：http://dhy.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://lqq.xinyue.icu

JS:   if (!data) return;
来源：http://pep.0kj1m.cn

TS:   if (!data) return;
来源：http://zco.tian-w.cn

Java: if (data == null) return;
来源：http://poj.tarul.cn

Go:   if data == nil { return }
来源：http://ucm.quarkkingdee.top

Ruby: return if data.nil?
来源：http://udg.cheryme.top

C#:   if (data == null) return;
来源：http://ivv.tian-w.cn

================================================================================
来源：http://ygh.gaohongyu789.top

C. 函数与作用域
来源：http://zxb.jyoumei.cn

================================================================================
来源：http://qrr.xylfe.cn

[C01] 定义函数
来源：http://kxw.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://yqw.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tbq.mhx1999.top

JS:   function add(a, b) { return a + b; }
来源：http://bie.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://glk.haohaochexian.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sbg.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://iyk.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://bcu.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nvh.yuanzhike.top

[C02] 默认参数
来源：http://jwo.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://wep.gzhubu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gqv.hnxiangtu.top

JS:   function greet(name = "World") { return name; }
来源：http://iyr.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pan.jqgufenzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vep.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lmb.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://jdw.fanxiaobao.xyz

C#:   string Greet(string name = "World") => name;
来源：http://fnw.ywan-chungtsiang.top

[C03] 可变参数
来源：http://dfv.cqqwz.cn

Py:   def total(*args): return sum(args)
来源：http://zyy.chenjidiqi.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dqq.jinqigufen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kvn.guannengcc.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bex.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bxc.quarkkingdee.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mhd.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://pim.aizwys.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://umk.smart0.xyz

[C04] 命名参数 / 关键字参数
来源：http://wvb.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xwf.xylfe.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jyh.pengpengdd.cyou

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qqs.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nnz.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://kqc.epnwcf.com

Go:   // 无：用配置结构体参数
来源：http://xla.yueranfly.top

Ruby: f(a: 1, b: 2)
来源：http://vpp.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://zpn.zhixingplan.top

[C05] 返回多个值
来源：http://rmb.jinghuilouyu.cn

Py:   return a, b
来源：http://rny.yvedp.cn

PHP:  return [$a, $b];
来源：http://axs.cucudq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hde.xylfe.cn

TS:   return { a, b };
来源：http://gxb.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ppg.yongpay.top

Go:   return a, b
来源：http://nak.jinqigufen.top

Ruby: return a, b
来源：http://crb.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://ook.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://msr.cheryme.top

Py:   square = lambda x: x * x
来源：http://vyv.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zvm.wangdashe.top

JS:   const square = x => x * x;
来源：http://rkd.bjfxy.top

TS:   const square = (x: number): number => x * x;
来源：http://cxn.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lbl.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dnw.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://wud.vqdsnc.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fco.yj202588.top

[C07] 把函数作为参数传入
来源：http://ina.bjfxy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hqn.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wzf.wangshuangyany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://llv.zycfv.cn

TS:   arr.map(String)
来源：http://eas.ywan-chungtsiang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://flg.yangfankeji.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vpx.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://lsa.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://unu.quarkkingdee.top

[C08] 闭包
来源：http://swk.zdbjq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://txr.yvedp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://txk.bbcook.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pqs.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://brv.gaohongyu789.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rgd.gogol.net.cn


<!-- 参考信息 -->