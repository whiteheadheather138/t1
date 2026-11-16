代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://zpq.xziqi.cn

Py:   ord("A"); chr(65)
来源：http://qkz.jlsjyb.cn

PHP:  ord("A"); chr(65)
来源：http://qes.nwbrower.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hap.nanxuanxn.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lgg.52xcode.cn

Java: (int) 'A'; (char) 65
来源：http://ana.redwolf501.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rat.cucudq.cn

Ruby: "A".ord; 65.chr
来源：http://zhz.fehbvm.com

C#:   (int)'A'; (char)65
来源：http://qxe.bbcook.cn

[A19] 交换两个变量
来源：http://zht.tianlin.xyz

Py:   a, b = b, a
来源：http://lqc.hcnkem.com

PHP:  [$a, $b] = [$b, $a];
来源：http://ids.sufxvd.cn

JS:   [a, b] = [b, a];
来源：http://ndy.tianlin.xyz

TS:   [a, b] = [b, a];
来源：http://gjz.daria6918.cn

Java: int t = a; a = b; b = t;
来源：http://hxq.gotoacloud.top

Go:   a, b = b, a
来源：http://pgk.fanxiaobao.xyz

Ruby: a, b = b, a
来源：http://smt.chenlongwang.top

C#:   (a, b) = (b, a);
来源：http://oup.ydzc1.top

[A20] 读取标准输入
来源：http://jdd.zhongyouzk.top

Py:   name = input("请输入：")
来源：http://rei.guannengcc.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rxs.smart0.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vkp.0kj1m.cn

TS:   // Node.js：readline 模块
来源：http://fxp.vehdjk.com

Java: new Scanner(System.in).nextLine()
来源：http://leu.fanxiaobao.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dyd.ydjk.org.cn

Ruby: gets.chomp
来源：http://nkj.hcnkem.com

C#:   Console.ReadLine();
来源：http://lgr.shzxlz.cn

[A21] 保留指定小数位输出
来源：http://qif.jqgufenzy.top

Py:   f"{3.14159:.2f}"
来源：http://ien.9152youxi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nrr.tian-w.cn

JS:   (3.14159).toFixed(2)
来源：http://hov.ppjwa.cn

TS:   (3.14159).toFixed(2)
来源：http://psy.fengsongda.top

Java: String.format("%.2f", 3.14159)
来源：http://knx.yj20258888.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nyx.meibo888.top

Ruby: format("%.2f", 3.14159)
来源：http://lbx.vqdsnc.cn

C#:   3.14159.ToString("F2")
来源：http://bvv.cqqwz.cn

[A22] 获取字符串长度
来源：http://bjr.zhoulong.xyz

Py:   len(s)
来源：http://bcq.hnqzz.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://inf.chenzaomai.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cux.c1oappe.top

TS:   s.length
来源：http://xad.sxryk.cn

Java: s.length()
来源：http://xnp.chenlongwang.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eex.hysaishi.cn

Ruby: s.length
来源：http://xpf.jyoumei.cn

C#:   s.Length
来源：http://rfx.vehdjk.com

[A23] 大小写转换
来源：http://zpr.epnwcf.com

Py:   s.upper(); s.lower(); s.title()
来源：http://qax.9152youxi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ysu.quarkkingdee.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cmi.aizwys.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iby.shzxlz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kyi.nanxuanxn.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zkf.guowangkeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pda.smart0.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://pwk.jianghu66.top

[A24] 去除首尾空白
来源：http://lyf.zhengqikj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nrg.feifeiyinyue.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://utf.zycfv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kyl.vehdjk.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://izv.hcnkem.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ezm.zycfv.cn

Go:   strings.TrimSpace(s)
来源：http://wdu.ppjwa.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xie.hesvh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ida.zhengqikj.top

[A25] 字符串比较
来源：http://mgu.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://lye.sysykeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mer.jinqigufen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://shq.mhx1999.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nee.hnqzz.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://llc.daria6918.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dfn.cdnleiting.top

Ruby: s1 == s2; s1 <=> s2
来源：http://imv.nwbrower.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tfc.fzhhl.top

[A26] 类型转换总览
来源：http://hoh.yj202588.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qwg.nanxuanxn.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vyo.fehbvm.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ltf.jinqigufen.top

TS:   Number() String() Boolean() x as number
来源：http://tum.ppjwa.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kla.redwolf501.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mwi.xinyue.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://yyt.ybcxt.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ihf.gzhubu.top

================================================================================
来源：http://atc.316326.xyz

B. 流程控制
来源：http://ndv.xingfuxueyuan.xyz

================================================================================
来源：http://ixq.xingfuxueyuan.xyz

[B01] 条件判断 if / else
来源：http://yvo.ywan-chungtsiang.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cgg.feifeiyinyue.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rgi.shangyingyoupin.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cdw.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mns.mhx1999.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hji.shzxlz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yui.tianlin.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ssf.zdqjudy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rtn.havefunace.top

[B02] 多分支 else if / elif
来源：http://vxt.cheryme.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ggu.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://epd.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hqb.andypj.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iye.fzhhl.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ijq.shanyushiyangtech.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://weo.gzhubu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gah.yj20258888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://quw.fehbvm.com

[B03] switch / match / case
来源：http://qpq.aizwys.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jpg.cashguo.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hsd.jianghu66.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://csn.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xxx.9152youxi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wxq.shzxlz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qmu.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jqv.yongpay.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wio.jyoumei.cn

[B04] for 计数循环
来源：http://jnu.nanxuanxn.top

Py:   for i in range(10): print(i)
来源：http://zeu.kuanghao11.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fnb.fengsongda.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fmi.chenlongwang.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://emu.chenzaomai.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://stf.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rxi.yuanzhike.top

Ruby: 10.times { |i| puts i }
来源：http://can.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oyi.gzhubu.top

[B05] 遍历数组 / 列表
来源：http://jpa.yj20258888.top

Py:   for item in arr: print(item)
来源：http://qyt.fzhhl.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dby.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dse.ydjk.org.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fxt.nanxinkj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lqo.aibaodan.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ghf.zhiwuduotai.top

Ruby: arr.each { |item| puts item }
来源：http://ceg.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://igw.xuanzx.com

[B06] 遍历字典 / 对象
来源：http://iaa.yvedp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dbn.ybcxt.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rac.vehdjk.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hly.fengsongda.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://avo.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bhe.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pvm.pycfn.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yia.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tdt.ydjk.org.cn

[B07] while 循环
来源：http://qfs.shanyushiyangtech.top

Py:   while i < 10: i += 1
来源：http://osw.ydjk.org.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xby.yj202588.top

JS:   while (i < 10) { i++; }
来源：http://lqf.aizwys.cn

TS:   while (i < 10) { i++; }
来源：http://qjk.hnqzz.top

Java: while (i < 10) { i++; }
来源：http://phy.shuidangran.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ukz.0kj1m.cn

Ruby: while i < 10; i += 1; end
来源：http://obl.birdmap.top

C#:   while (i < 10) { i++; }
来源：http://dst.yonumen.top

[B08] do-while（至少执行一次）
来源：http://npo.tian-w.cn

Py:   # 无 do-while：用 while True + break
来源：http://kvc.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hey.jianghu66.top

JS:   do { i++; } while (i < 10);
来源：http://sib.zdbjq.cn

TS:   do { i++; } while (i < 10);
来源：http://ssc.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://qtp.yuanzhike.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uie.redwolf501.top

Ruby: begin; i += 1; end while i < 10
来源：http://pyb.gaohongyu789.top

C#:   do { i++; } while (i < 10);
来源：http://jkq.tarul.cn

[B09] break 与 continue
来源：http://uat.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xlb.ydzc1.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xal.xziqi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lqb.zdqjudy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kod.bjfxy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eep.pengpengdd.cyou

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dgw.svipenyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hza.zhongyouzk.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rpx.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://ymq.bjfxy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aid.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vxo.kuanghao11.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vyf.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ahl.xingfuxueyuan.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ebf.hnxiangtu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hey.haohaochexian.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rfj.pycfn.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tzp.gotoacloud.top

[B11] 生成数字序列 / 区间
来源：http://yjz.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://wqi.redwolf501.top

PHP:  range(0, 10, 2);
来源：http://itj.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bvv.haohaochexian.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qyk.ybcxt.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jjo.52xcode.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zne.pengpengdd.cyou

Ruby: (0...10).step(2).to_a
来源：http://nwd.hongshengwenyu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://saf.52xcode.cn

[B12] 跳出多层循环
来源：http://yza.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ogr.dianchejie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://omu.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wzm.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vnj.xuanzx.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hva.zdbjq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://onn.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bnn.jinyuanbaomall.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qxm.snrcjt.cn

[B13] 判断是否为数字
来源：http://vpw.pengpengdd.cyou

Py:   isinstance(x, (int, float))
来源：http://afh.svipenyu.cn

PHP:  is_numeric($x)
来源：http://otb.yfazqb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://egf.guannengcc.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nfq.bjfxy.top

Java: x instanceof Number
来源：http://gtd.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aaz.nanxuanxn.top

Ruby: x.is_a?(Numeric)
来源：http://xfw.hongshengwenyu.top

C#:   x is int or double or decimal
来源：http://fsm.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://qur.pycfn.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iyf.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yzy.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://rxb.zdbjq.cn

TS:   [1, 2, 3].includes(x)
来源：http://clk.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fwr.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cmm.shangyingyoupin.top

Ruby: [1, 2, 3].include?(x)
来源：http://xjo.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ttn.xuanzx.com

[B15] 布尔运算与取反
来源：http://hnt.ydzc1.top

Py:   a and b or not c
来源：http://pxa.bjfxy.top

PHP:  $a && $b || !$c
来源：http://fcv.jiagoushi.top

JS:   a && b || !c
来源：http://ojc.yuanzhike.top

TS:   a && b || !c
来源：http://qqj.xylfe.cn

Java: a && b || !c
来源：http://dvs.yfazqb.com

Go:   a && b || !c
来源：http://beq.xingfuxueyuan.xyz

Ruby: a && b || !c
来源：http://aiu.nanxinkj.top

C#:   a && b || !c
来源：http://sct.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://syd.smart0.xyz

Py:   if not data: return
来源：http://vxz.zhoulong.xyz

PHP:  if (!$data) { return; }
来源：http://vqd.zdbjq.cn

JS:   if (!data) return;
来源：http://tkx.jqgfzy.top

TS:   if (!data) return;
来源：http://phq.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://rzi.andypj.xyz

Go:   if data == nil { return }
来源：http://mxv.cdnleiting.top

Ruby: return if data.nil?
来源：http://dpv.cqqwz.cn

C#:   if (data == null) return;
来源：http://olh.hongshengwenyu.top

================================================================================
来源：http://gmp.zhiwuduotai.top

C. 函数与作用域
来源：http://njx.zdbjq.cn

================================================================================
来源：http://gpo.gotoacloud.top

[C01] 定义函数
来源：http://hny.fengsongda.top

Py:   def add(a, b): return a + b
来源：http://gvh.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lqk.yuxming.cn

JS:   function add(a, b) { return a + b; }
来源：http://ezy.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ueh.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kkk.shzxlz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://skg.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://wtp.jinqigufen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://unn.cheryme.top

[C02] 默认参数
来源：http://mfa.dashuyun.cn

Py:   def greet(name="World"): return name
来源：http://ubp.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://xsg.redwolf501.top

JS:   function greet(name = "World") { return name; }
来源：http://juc.tanke756.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mcs.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mtj.guannengcc.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cgq.nwbrower.top

Ruby: def greet(name = "World") = name
来源：http://aju.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://duk.snrcjt.cn

[C03] 可变参数
来源：http://axe.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://mdd.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ura.pycfn.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ffg.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eoh.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jan.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ugr.vehdjk.com

Ruby: def total(*nums); nums.sum; end
来源：http://ugp.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zor.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://vmn.zhixingplan.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://agy.ehwqpu.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xml.fzhhl.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://emp.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hyp.ehwqpu.com

Java: // 无：用 Builder 模式或 record
来源：http://ycp.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://hhd.pycfn.com

Ruby: f(a: 1, b: 2)
来源：http://nhm.zycfv.cn

C#:   f(a: 1, b: 2)
来源：http://wld.svipenyu.cn

[C05] 返回多个值
来源：http://pti.meibo888.top

Py:   return a, b
来源：http://qou.sysykeji.top

PHP:  return [$a, $b];
来源：http://fyg.zdbjq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zdt.feifeiyinyue.top

TS:   return { a, b };
来源：http://bwy.hammf.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gdy.zdqjudy.top

Go:   return a, b
来源：http://jzh.316326.xyz

Ruby: return a, b
来源：http://plv.aizwys.cn

C#:   return (a, b);              // ValueTuple
来源：http://nhj.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://dkj.chenzaomai.com

Py:   square = lambda x: x * x
来源：http://meg.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xeh.zdbjq.cn

JS:   const square = x => x * x;
来源：http://jrx.tian-w.cn

TS:   const square = (x: number): number => x * x;
来源：http://snm.xinyue.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fee.sysykeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://jzv.nanxinkj.top

Ruby: square = ->(x) { x * x }
来源：http://smw.zhiwuduotai.top

C#:   Func<int, int> square = x => x * x;
来源：http://tbx.zhongyouzk.top

[C07] 把函数作为参数传入
来源：http://tlm.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nvv.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://tre.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gbp.shanyushiyangkeji.top

TS:   arr.map(String)
来源：http://kxi.yonumen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ypk.shanyushiyangtech.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mxo.fzhhl.top

Ruby: arr.map(&:upcase)
来源：http://fqv.dashuyun.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bir.zhiwuduotai.top

[C08] 闭包
来源：http://vsm.zhijiandao.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.fzhhl.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vlx.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://enk.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lqi.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tvt.daria6918.cn


<!-- 参考信息 -->