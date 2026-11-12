代发 wailian999

C#:   (int)'A'; (char)65
来源：http://alf.hysaishi.cn

[A19] 交换两个变量
来源：http://otg.chenlongwang.top

Py:   a, b = b, a
来源：http://oyc.pengpengdd.cyou

PHP:  [$a, $b] = [$b, $a];
来源：http://ytp.xuetiantiany.cn

JS:   [a, b] = [b, a];
来源：http://hbr.hesvh.cn

TS:   [a, b] = [b, a];
来源：http://gxv.jinghuilouyu.cn

Java: int t = a; a = b; b = t;
来源：http://kvo.sxryk.cn

Go:   a, b = b, a
来源：http://oaz.xinyue.icu

Ruby: a, b = b, a
来源：http://wzd.hywenlv.cn

C#:   (a, b) = (b, a);
来源：http://qlk.bbcook.cn

[A20] 读取标准输入
来源：http://qda.quarkkingdee.top

Py:   name = input("请输入：")
来源：http://sgp.aizwys.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ecl.xylfe.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xfg.guannengcc.top

TS:   // Node.js：readline 模块
来源：http://iou.guannengcc.top

Java: new Scanner(System.in).nextLine()
来源：http://ija.zhixingplan.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pqz.shzxlz.cn

Ruby: gets.chomp
来源：http://fyf.sxryk.cn

C#:   Console.ReadLine();
来源：http://msq.zhiwuduotai.top

[A21] 保留指定小数位输出
来源：http://wkg.xuanzx.com

Py:   f"{3.14159:.2f}"
来源：http://rxz.haohaochexian.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gro.jinqigfzy.top

JS:   (3.14159).toFixed(2)
来源：http://lmt.nanxinkj.top

TS:   (3.14159).toFixed(2)
来源：http://uxz.yj20258888.top

Java: String.format("%.2f", 3.14159)
来源：http://cuk.yvedp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uwu.uphjek.com

Ruby: format("%.2f", 3.14159)
来源：http://eat.316326.xyz

C#:   3.14159.ToString("F2")
来源：http://nyr.ydzc1.top

[A22] 获取字符串长度
来源：http://igk.hnqzz.top

Py:   len(s)
来源：http://xwt.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qqe.cashguo.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gxi.meibo888.top

TS:   s.length
来源：http://muz.tarul.cn

Java: s.length()
来源：http://jnl.xinyue.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ecy.mhx1999.top

Ruby: s.length
来源：http://skq.hcnkem.com

C#:   s.Length
来源：http://cmo.9152youxi.cn

[A23] 大小写转换
来源：http://vux.iojbl.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bar.cheryme.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ghw.pycfn.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xlg.wangshuangyany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pkx.dianchejie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://byg.nwbrower.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://afo.c1oappe.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jkm.sysykeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gsy.jinghuilouyu.cn

[A24] 去除首尾空白
来源：http://xyo.aizwys.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jnk.guowangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tzy.sjlbkw.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iom.yfazqb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jlv.jinqigfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mxr.yvedp.cn

Go:   strings.TrimSpace(s)
来源：http://uxv.yongpay.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qug.jqgfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mat.redwolf501.top

[A25] 字符串比较
来源：http://kzm.xziqi.cn

Py:   s1 == s2; s1 != s2
来源：http://rdc.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jbb.zhongyouzk.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jiz.meibo888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yjt.pycfn.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dom.shanyushiyangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://llu.birdmap.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ufn.zhengqikj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gkf.fktsv.cn

[A26] 类型转换总览
来源：http://igg.tarul.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ley.hnxiangtu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gmm.ppjwa.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vqx.tarul.cn

TS:   Number() String() Boolean() x as number
来源：http://jcx.hammf.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nir.sxryk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zpd.0kj1m.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jyl.wangdashe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zgk.sxryk.cn

================================================================================
来源：http://zrr.bbcook.cn

B. 流程控制
来源：http://dpr.yonumen.top

================================================================================
来源：http://lxj.smart0.xyz

[B01] 条件判断 if / else
来源：http://hxx.yonumen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gin.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zeo.fehbvm.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cil.hywenlv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bkm.shzxlz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://atk.tanke756.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oth.zdqjudy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rrg.tanke756.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oba.yueranfly.top

[B02] 多分支 else if / elif
来源：http://ipa.xziqi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bvq.yuxming.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ajb.nanxuanxn.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://npm.fzhhl.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fbj.haohaochexian.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iow.zhaomingkeji.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pai.yuxming.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vir.jiagoushi.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gag.ywan-chungtsiang.top

[B03] switch / match / case
来源：http://twc.sweek.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ibc.quarkkingdee.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uox.xuanzx.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fbd.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tnq.xuetiantiany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wvk.vehdjk.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lmq.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qdf.yj20258888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://igw.guowangkeji.top

[B04] for 计数循环
来源：http://fcf.shuidangran.top

Py:   for i in range(10): print(i)
来源：http://uat.zhijiandao.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zxe.tanke756.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wdu.chenjidiqi.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nsd.0kj1m.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bkr.ydjk.org.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uqv.haohaochexian.top

Ruby: 10.times { |i| puts i }
来源：http://wgu.hcnkem.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sod.yueranfly.top

[B05] 遍历数组 / 列表
来源：http://yar.ybcxt.top

Py:   for item in arr: print(item)
来源：http://jjf.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tjm.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://day.yj20258.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ezj.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yyq.ydjk.org.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kht.ppjwa.cn

Ruby: arr.each { |item| puts item }
来源：http://scy.pengpengdd.cyou

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mty.cheryme.top

[B06] 遍历字典 / 对象
来源：http://pum.guannengcc.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yqk.bjfxy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fcw.fengsongda.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pdh.bjfxy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vxl.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cwn.dashuyun.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qir.xuetiantiany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://czr.hywenlv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gyq.jlsjyb.cn

[B07] while 循环
来源：http://jeu.yongpay.top

Py:   while i < 10: i += 1
来源：http://xes.jianghu66.top

PHP:  while ($i < 10) { $i++; }
来源：http://xpf.sweek.top

JS:   while (i < 10) { i++; }
来源：http://wbe.jinqigufen.top

TS:   while (i < 10) { i++; }
来源：http://daz.zhengqikj.top

Java: while (i < 10) { i++; }
来源：http://atg.ehwqpu.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rih.zhengqikj.top

Ruby: while i < 10; i += 1; end
来源：http://ibr.fehbvm.com

C#:   while (i < 10) { i++; }
来源：http://bar.fanxiaobao.xyz

[B08] do-while（至少执行一次）
来源：http://ljt.guannengcc.top

Py:   # 无 do-while：用 while True + break
来源：http://tsn.ydzc1.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lqt.vqdsnc.cn

JS:   do { i++; } while (i < 10);
来源：http://tca.c1oappe.top

TS:   do { i++; } while (i < 10);
来源：http://pki.zdqjudy.top

Java: do { i++; } while (i < 10);
来源：http://uvy.uphjek.com

Go:   for { i++; if i >= 10 { break } }
来源：http://vei.zhaomingkeji.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://szi.cdnleiting.top

C#:   do { i++; } while (i < 10);
来源：http://odh.xingfuxueyuan.xyz

[B09] break 与 continue
来源：http://xjr.haohaochexian.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dsm.guannengcc.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lsu.dashuyun.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://leh.cdnleiting.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ocy.ydzc1.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://doq.zhijiandao.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://slb.daria6918.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://asv.shanyushiyangtech.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://roj.jianghu66.top

[B10] 遍历同时拿索引
来源：http://vuv.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ezk.tarul.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sfu.haohaochexian.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pix.chenzaomai.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jpa.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rrv.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://igp.zhixingplan.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vrp.shanyushiyangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ygh.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://pes.shuidangran.top

Py:   list(range(0, 10, 2))
来源：http://hdn.tarul.cn

PHP:  range(0, 10, 2);
来源：http://cmg.svipenyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pcj.sysykeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://btv.cdnleiting.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vkg.pengpengdd.cyou

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lkm.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://uhl.shzxlz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mil.fehbvm.com

[B12] 跳出多层循环
来源：http://nub.zycfv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lqq.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://coz.zhixingplan.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://upi.bjfxy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://khh.shanyushiyangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://acf.xylfe.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://asu.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uam.zhongyouzk.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ssy.gotoacloud.top

[B13] 判断是否为数字
来源：http://jpc.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://mxr.jqgfzy.top

PHP:  is_numeric($x)
来源：http://axt.jqgufenzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://alh.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://osm.daria6918.cn

Java: x instanceof Number
来源：http://lrg.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://efy.yvedp.cn

Ruby: x.is_a?(Numeric)
来源：http://zrw.shuidangran.top

C#:   x is int or double or decimal
来源：http://ccg.ivvv.top

[B14] 判断值是否在集合内
来源：http://tjp.yongpay.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xbf.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jxb.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://gzh.yongpay.top

TS:   [1, 2, 3].includes(x)
来源：http://syo.tian-w.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sdq.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fey.havefunace.top

Ruby: [1, 2, 3].include?(x)
来源：http://tvq.guannengcc.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hjs.chenzaomai.com

[B15] 布尔运算与取反
来源：http://gxc.zycfv.cn

Py:   a and b or not c
来源：http://bmo.ivvv.top

PHP:  $a && $b || !$c
来源：http://juq.xuanzx.com

JS:   a && b || !c
来源：http://ils.wangdashe.top

TS:   a && b || !c
来源：http://phk.chenjidiqi.icu

Java: a && b || !c
来源：http://lih.chenlongwang.top

Go:   a && b || !c
来源：http://pte.ydzc1.top

Ruby: a && b || !c
来源：http://euw.yuxming.cn

C#:   a && b || !c
来源：http://rsk.pengpengdd.cyou

[B16] 卫语句：不满足条件提前返回
来源：http://upd.zdbjq.cn

Py:   if not data: return
来源：http://ocx.pengpengdd.cyou

PHP:  if (!$data) { return; }
来源：http://typ.hammf.cn

JS:   if (!data) return;
来源：http://fzd.svipenyu.cn

TS:   if (!data) return;
来源：http://myz.kuanghao11.cn

Java: if (data == null) return;
来源：http://oea.cucudq.cn

Go:   if data == nil { return }
来源：http://ipa.xziqi.cn

Ruby: return if data.nil?
来源：http://cbt.sufxvd.cn

C#:   if (data == null) return;
来源：http://nza.redwolf501.top

================================================================================
来源：http://vul.mhx1999.top

C. 函数与作用域
来源：http://mpg.xuanzx.com

================================================================================
来源：http://dzq.yongpay.top

[C01] 定义函数
来源：http://ckp.havefunace.top

Py:   def add(a, b): return a + b
来源：http://tus.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nfu.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://hbb.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mnc.bjfxy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tto.cheryme.top

Go:   func add(a, b int) int { return a + b }
来源：http://dgn.wangshuangyany.cn

Ruby: def add(a, b); a + b; end
来源：http://vox.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lbn.epnwcf.com

[C02] 默认参数
来源：http://wiu.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://ygr.guowangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qet.52xcode.cn

JS:   function greet(name = "World") { return name; }
来源：http://xyi.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://egi.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dbw.nanxuanxn.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wnq.ydzc1.top

Ruby: def greet(name = "World") = name
来源：http://jwd.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://xzp.gogol.net.cn

[C03] 可变参数
来源：http://auq.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://hyh.c1oappe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lpy.fengsongda.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ifb.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zvw.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://efh.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bpl.52xcode.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xgx.jqgfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zxl.redwolf501.top

[C04] 命名参数 / 关键字参数
来源：http://rex.daria6918.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ckg.shuidangran.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nwd.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iaw.zdbjq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wec.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://lzu.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://emp.chenjidiqi.icu

Ruby: f(a: 1, b: 2)
来源：http://oam.9152youxi.cn

C#:   f(a: 1, b: 2)
来源：http://ese.ehwqpu.com

[C05] 返回多个值
来源：http://bdi.daxiang520.top

Py:   return a, b
来源：http://pzv.jinyuanbaomall.cn

PHP:  return [$a, $b];
来源：http://ilj.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://icn.c1oappe.top

TS:   return { a, b };
来源：http://wph.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fpl.316326.xyz

Go:   return a, b
来源：http://hjb.hnxiangtu.top

Ruby: return a, b
来源：http://tpy.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://npu.tarul.cn

[C06] 匿名函数 / lambda
来源：http://yex.yj20258888.top

Py:   square = lambda x: x * x
来源：http://yoc.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ihg.shanyushiyangtech.top

JS:   const square = x => x * x;
来源：http://xhs.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://tpe.feifeiyinyue.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yzf.jinghuilouyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qon.ybcxt.top

Ruby: square = ->(x) { x * x }
来源：http://els.svipenyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pah.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://hgg.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vfe.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://jbw.wangshuangyany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fas.xziqi.cn

TS:   arr.map(String)
来源：http://wwq.ydjk.org.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oyr.xziqi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rht.wangdashe.top

Ruby: arr.map(&:upcase)
来源：http://mjr.yj20258888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://krj.snrcjt.cn

[C08] 闭包
来源：http://nlr.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pct.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fkm.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://auz.9152youxi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yow.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fhq.bbcook.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qwc.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pkn.cashguo.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ntp.fengsongda.top

[C09] 递归
来源：http://hod.sysykeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wvg.pycfn.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ruj.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qgo.svipenyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cxa.aibaodan.cn


<!-- 参考信息 -->