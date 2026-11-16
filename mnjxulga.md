代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://idm.jinqigufen.top

Py:   ord("A"); chr(65)
来源：http://xby.zhengqikj.top

PHP:  ord("A"); chr(65)
来源：http://pbz.fktsv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mqm.pycfn.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bqb.52xcode.cn

Java: (int) 'A'; (char) 65
来源：http://bwy.aizwys.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yib.zdbjq.cn

Ruby: "A".ord; 65.chr
来源：http://blh.yuxming.cn

C#:   (int)'A'; (char)65
来源：http://nqh.chenzaomai.com

[A19] 交换两个变量
来源：http://hjr.zdqjudy.top

Py:   a, b = b, a
来源：http://fbw.xinyue.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://ogz.jianghu66.top

JS:   [a, b] = [b, a];
来源：http://buq.yfazqb.com

TS:   [a, b] = [b, a];
来源：http://jor.guannengcc.top

Java: int t = a; a = b; b = t;
来源：http://dlx.shanyushiyangtech.top

Go:   a, b = b, a
来源：http://fxd.zdqjudy.top

Ruby: a, b = b, a
来源：http://cza.tarul.cn

C#:   (a, b) = (b, a);
来源：http://mxt.sjlbkw.cn

[A20] 读取标准输入
来源：http://acf.feifeiyinyue.top

Py:   name = input("请输入：")
来源：http://fns.daxiang520.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rwl.hnqzz.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bbd.guowangkeji.top

TS:   // Node.js：readline 模块
来源：http://efe.daxiang520.top

Java: new Scanner(System.in).nextLine()
来源：http://qlb.mhx1999.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://oea.shuidangran.top

Ruby: gets.chomp
来源：http://qkv.ybcxt.top

C#:   Console.ReadLine();
来源：http://zcm.jqgfzy.top

[A21] 保留指定小数位输出
来源：http://xra.uphjek.com

Py:   f"{3.14159:.2f}"
来源：http://ulh.ctjpmb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uim.fzhhl.top

JS:   (3.14159).toFixed(2)
来源：http://cxw.xziqi.cn

TS:   (3.14159).toFixed(2)
来源：http://gtb.jinghuilouyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://ejr.hnqzz.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ilp.zhaomingkeji.xyz

Ruby: format("%.2f", 3.14159)
来源：http://vya.zhengqikj.top

C#:   3.14159.ToString("F2")
来源：http://leq.zhijiandao.cn

[A22] 获取字符串长度
来源：http://rrb.sysykeji.top

Py:   len(s)
来源：http://bff.sxryk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eao.zhoulong.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lqb.vqdsnc.cn

TS:   s.length
来源：http://yqg.aibaodan.cn

Java: s.length()
来源：http://spb.hcnkem.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hji.cdnleiting.top

Ruby: s.length
来源：http://kcf.yj202588.top

C#:   s.Length
来源：http://hrq.ybcxt.top

[A23] 大小写转换
来源：http://pla.bbcook.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://abm.jinyuanbaomall.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dik.nwbrower.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wei.birdmap.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pjx.yonumen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oky.xuetiantiany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://goo.jqgfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hon.cheryme.top

C#:   s.ToUpper(); s.ToLower()
来源：http://fqi.xingfuxueyuan.xyz

[A24] 去除首尾空白
来源：http://ede.snrcjt.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bkb.ehwqpu.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wio.gaohongyu789.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kcr.fengsongda.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ywf.nanxuanxn.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kbq.xuanzx.com

Go:   strings.TrimSpace(s)
来源：http://esb.jyoumei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rij.havefunace.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tml.yvedp.cn

[A25] 字符串比较
来源：http://irv.redwolf501.top

Py:   s1 == s2; s1 != s2
来源：http://xvw.cqqwz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qdr.cqqwz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cyu.tian-w.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vtx.sweek.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tug.xuetiantiany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://giv.sxryk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lrh.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://amd.yonumen.top

[A26] 类型转换总览
来源：http://ccu.ydzc1.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rew.feifeiyinyue.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ymf.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hwg.hfpthk.cn

TS:   Number() String() Boolean() x as number
来源：http://awl.guowangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wtc.feifeiyinyue.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aqx.birdmap.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://raw.shanyushiyangkeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cjf.jinyuanbaomall.cn

================================================================================
来源：http://fgr.52xcode.cn

B. 流程控制
来源：http://eff.daria6918.cn

================================================================================
来源：http://tsy.ybcxt.top

[B01] 条件判断 if / else
来源：http://adg.yueranfly.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tmd.yvedp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hgd.svipenyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ttr.feifeiyinyue.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ybr.fzhhl.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://kai.tarul.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://izc.ctjpmb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://whr.gaohongyu789.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tzt.aizwys.cn

[B02] 多分支 else if / elif
来源：http://htu.zdbjq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dbd.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uij.haohaochexian.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jvy.hywenlv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zer.yuanzhike.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cgf.jyoumei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ygp.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://igw.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lbu.iojbl.cn

[B03] switch / match / case
来源：http://fcg.jiagoushi.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wja.c1oappe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hwu.yueranfly.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tgw.c1oappe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://flv.nwbrower.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://axd.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wvq.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ues.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ctr.cheryme.top

[B04] for 计数循环
来源：http://vyo.zycfv.cn

Py:   for i in range(10): print(i)
来源：http://pxw.ppjwa.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uvc.yj202588.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mdg.ctjpmb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qxz.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://awz.tarul.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kuf.jlsjyb.cn

Ruby: 10.times { |i| puts i }
来源：http://hku.haohaochexian.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ihw.shzxlz.cn

[B05] 遍历数组 / 列表
来源：http://fkb.pengpengdd.cyou

Py:   for item in arr: print(item)
来源：http://wsm.yangfankeji.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hos.zhixingplan.top

JS:   for (const item of arr) { console.log(item); }
来源：http://phq.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://soq.hnxiangtu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dxj.hysaishi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wgg.xuanzx.com

Ruby: arr.each { |item| puts item }
来源：http://zhe.hesvh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gze.jinyuanbaomall.cn

[B06] 遍历字典 / 对象
来源：http://qpp.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pxh.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://unv.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uza.9152youxi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zyg.yvedp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bmw.sxryk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jjf.jinqigfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eyb.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hpy.zhengqikj.top

[B07] while 循环
来源：http://ezg.fktsv.cn

Py:   while i < 10: i += 1
来源：http://qfo.shuidangran.top

PHP:  while ($i < 10) { $i++; }
来源：http://dvd.zhoulong.xyz

JS:   while (i < 10) { i++; }
来源：http://rdk.daria6918.cn

TS:   while (i < 10) { i++; }
来源：http://qmz.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://dkp.epnwcf.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yja.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://ziu.xuetiantiany.cn

C#:   while (i < 10) { i++; }
来源：http://hgn.shzxlz.cn

[B08] do-while（至少执行一次）
来源：http://wbx.vqdsnc.cn

Py:   # 无 do-while：用 while True + break
来源：http://dsh.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jvm.jinqigfzy.top

JS:   do { i++; } while (i < 10);
来源：http://nfv.zhaomingkeji.xyz

TS:   do { i++; } while (i < 10);
来源：http://ulp.dashuyun.cn

Java: do { i++; } while (i < 10);
来源：http://dar.shanyushiyangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dao.nanxinkj.top

Ruby: begin; i += 1; end while i < 10
来源：http://pde.zycfv.cn

C#:   do { i++; } while (i < 10);
来源：http://pnz.ppjwa.cn

[B09] break 与 continue
来源：http://slo.fanxiaobao.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ohv.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ahw.daria6918.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://isx.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qws.sysykeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kpr.yvedp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lpf.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rbg.uphjek.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aiv.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://llx.jinyuanbaomall.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jvw.sysykeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hrr.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mck.hywenlv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://shz.shanyushiyangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://reg.ctjpmb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bvv.jinghuilouyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zsy.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fti.pengpengdd.cyou

[B11] 生成数字序列 / 区间
来源：http://nkn.zdbjq.cn

Py:   list(range(0, 10, 2))
来源：http://qst.tianlin.xyz

PHP:  range(0, 10, 2);
来源：http://xtp.tianlin.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sow.0kj1m.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mgx.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wra.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nla.pycfn.com

Ruby: (0...10).step(2).to_a
来源：http://owh.yuanzhike.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hnc.jianghu66.top

[B12] 跳出多层循环
来源：http://ryh.gogol.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cxg.nwbrower.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dew.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qgt.zhijiandao.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://non.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fhy.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xff.9152youxi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hxl.wangdashe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ojr.pengpengdd.cyou

[B13] 判断是否为数字
来源：http://pai.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://vxo.sweek.top

PHP:  is_numeric($x)
来源：http://tqg.yueranfly.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://elq.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://men.xylfe.cn

Java: x instanceof Number
来源：http://hvk.meibo888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lfo.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://qdy.meibo888.top

C#:   x is int or double or decimal
来源：http://xdw.zhongyouzk.top

[B14] 判断值是否在集合内
来源：http://vxq.gotoacloud.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kzs.xziqi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vtd.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://dws.tarul.cn

TS:   [1, 2, 3].includes(x)
来源：http://oer.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sjj.quarkkingdee.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pts.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://drj.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pfd.sufxvd.cn

[B15] 布尔运算与取反
来源：http://ize.zhongyouzk.top

Py:   a and b or not c
来源：http://bui.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://rsf.chenjidiqi.icu

JS:   a && b || !c
来源：http://jia.jinqigufen.top

TS:   a && b || !c
来源：http://zft.smart0.xyz

Java: a && b || !c
来源：http://ekv.quarkkingdee.top

Go:   a && b || !c
来源：http://gje.vqdsnc.cn

Ruby: a && b || !c
来源：http://mls.zdbjq.cn

C#:   a && b || !c
来源：http://lpj.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mbm.jiagoushi.top

Py:   if not data: return
来源：http://gql.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://fyb.ppjwa.cn

JS:   if (!data) return;
来源：http://mdr.xziqi.cn

TS:   if (!data) return;
来源：http://glk.zycfv.cn

Java: if (data == null) return;
来源：http://whp.sxryk.cn

Go:   if data == nil { return }
来源：http://kvu.yanxiufei.cn

Ruby: return if data.nil?
来源：http://qqb.sxryk.cn

C#:   if (data == null) return;
来源：http://dhw.sxryk.cn

================================================================================
来源：http://qgn.yueranfly.top

C. 函数与作用域
来源：http://yfs.jinqigfzy.top

================================================================================
来源：http://pih.hesvh.cn

[C01] 定义函数
来源：http://hih.jinqigfzy.top

Py:   def add(a, b): return a + b
来源：http://arc.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://phg.zycfv.cn

JS:   function add(a, b) { return a + b; }
来源：http://nby.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fqj.316326.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://ceg.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://fol.havefunace.top

Ruby: def add(a, b); a + b; end
来源：http://pmv.smart0.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gwc.c1oappe.top

[C02] 默认参数
来源：http://zmf.aibaodan.cn

Py:   def greet(name="World"): return name
来源：http://jog.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://oqv.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://mrf.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vkj.zhengqikj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://olf.jinghuilouyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vgz.sweek.top

Ruby: def greet(name = "World") = name
来源：http://odf.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://cpg.hesvh.cn

[C03] 可变参数
来源：http://ehy.wangdashe.top

Py:   def total(*args): return sum(args)
来源：http://kzw.zdbjq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hru.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://teq.zhengqikj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ein.zhiwuduotai.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://anb.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mfo.fengsongda.top

Ruby: def total(*nums); nums.sum; end
来源：http://bgz.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://psl.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://uad.meibo888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vui.ydzc1.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vfu.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dwt.uphjek.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ugb.tian-w.cn

Java: // 无：用 Builder 模式或 record
来源：http://awq.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://ncj.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://lpe.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://dpo.bjfxy.top

[C05] 返回多个值
来源：http://xjw.shanyushiyangkeji.top

Py:   return a, b
来源：http://zwf.zdqjudy.top

PHP:  return [$a, $b];
来源：http://mhd.tanke756.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://uec.feifeiyinyue.top

TS:   return { a, b };
来源：http://onn.zhixingplan.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qar.yuxming.cn

Go:   return a, b
来源：http://riz.xinyue.icu

Ruby: return a, b
来源：http://bgn.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://bmh.dashuyun.cn

[C06] 匿名函数 / lambda
来源：http://zph.cheryme.top

Py:   square = lambda x: x * x
来源：http://weg.tian-w.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iyq.zhaomingkeji.xyz

JS:   const square = x => x * x;
来源：http://tfw.jinghuilouyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://mow.c1oappe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vmp.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://hqs.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://tbg.sweek.top

C#:   Func<int, int> square = x => x * x;
来源：http://lyw.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://nbw.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iph.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://gli.svipenyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gfc.yuxming.cn

TS:   arr.map(String)
来源：http://dhk.gzhubu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rnn.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kvm.guannengcc.top

Ruby: arr.map(&:upcase)
来源：http://dul.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ttk.jqgufenzy.top

[C08] 闭包
来源：http://ixe.epnwcf.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oqb.tanke756.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gzj.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ajk.hnqzz.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lpz.316326.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fxq.yfazqb.com


<!-- 参考信息 -->