代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pdk.quarkkingdee.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://eog.yj20258.top

TS:   if (!x) {}
来源：http://lbd.hammf.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rfi.yuanzhike.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dzp.daxiang520.top

Ruby: unless x            # nil 与 false 为假
来源：http://tke.guannengcc.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nsn.zhixingplan.top

[A17] 位运算
来源：http://uec.hnxiangtu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cvj.sxryk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jrq.jianghu66.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vej.snrcjt.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jbl.chenlongwang.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lic.tian-w.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://per.jlsjyb.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hfh.yvedp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tbj.fengsongda.top

[A18] 字符与 ASCII 码互转
来源：http://jkp.fanxiaobao.xyz

Py:   ord("A"); chr(65)
来源：http://qdl.tarul.cn

PHP:  ord("A"); chr(65)
来源：http://jyv.jinqigufen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ssc.cqqwz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cxt.quarkkingdee.top

Java: (int) 'A'; (char) 65
来源：http://pgw.vehdjk.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pmk.jinghuilouyu.cn

Ruby: "A".ord; 65.chr
来源：http://rxz.xuanzx.com

C#:   (int)'A'; (char)65
来源：http://hvp.xinyue.icu

[A19] 交换两个变量
来源：http://rnt.jqgufenzy.top

Py:   a, b = b, a
来源：http://bji.meibo888.top

PHP:  [$a, $b] = [$b, $a];
来源：http://slo.ppjwa.cn

JS:   [a, b] = [b, a];
来源：http://wya.vehdjk.com

TS:   [a, b] = [b, a];
来源：http://alo.tian-w.cn

Java: int t = a; a = b; b = t;
来源：http://usk.jqgfzy.top

Go:   a, b = b, a
来源：http://eww.smart0.xyz

Ruby: a, b = b, a
来源：http://chj.gotoacloud.top

C#:   (a, b) = (b, a);
来源：http://oyf.xuanzx.com

[A20] 读取标准输入
来源：http://cob.xuanzx.com

Py:   name = input("请输入：")
来源：http://rdd.xingfuxueyuan.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://any.svipenyu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wyl.zhongyouzk.top

TS:   // Node.js：readline 模块
来源：http://tvn.ybcxt.top

Java: new Scanner(System.in).nextLine()
来源：http://qdc.cheryme.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dbu.iojbl.cn

Ruby: gets.chomp
来源：http://lqn.fzhhl.top

C#:   Console.ReadLine();
来源：http://vcb.yfazqb.com

[A21] 保留指定小数位输出
来源：http://dbs.jiagoushi.top

Py:   f"{3.14159:.2f}"
来源：http://pky.shuidangran.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ify.redwolf501.top

JS:   (3.14159).toFixed(2)
来源：http://sox.cdnleiting.top

TS:   (3.14159).toFixed(2)
来源：http://epl.fanxiaobao.xyz

Java: String.format("%.2f", 3.14159)
来源：http://qqr.bbcook.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://glp.ppjwa.cn

Ruby: format("%.2f", 3.14159)
来源：http://uzg.gotoacloud.top

C#:   3.14159.ToString("F2")
来源：http://tht.hammf.cn

[A22] 获取字符串长度
来源：http://jwz.zhoulong.xyz

Py:   len(s)
来源：http://aep.hesvh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xvz.cqqwz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nut.shuidangran.top

TS:   s.length
来源：http://qav.ehwqpu.com

Java: s.length()
来源：http://puh.sxryk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qgg.ybcxt.top

Ruby: s.length
来源：http://wmj.jinyuanbaomall.cn

C#:   s.Length
来源：http://msv.redwolf501.top

[A23] 大小写转换
来源：http://svo.zhiwuduotai.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vzy.fengsongda.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xub.gotoacloud.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tmi.yanxiufei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ypj.chenzaomai.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dcq.ehwqpu.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zya.yvedp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lqm.52xcode.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ngq.yj20258888.top

[A24] 去除首尾空白
来源：http://lxb.jqgfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sfr.jinghuilouyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bql.xuanzx.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ghx.redwolf501.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cil.shanyushiyangtech.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://whp.shanyushiyangkeji.top

Go:   strings.TrimSpace(s)
来源：http://wan.jinyuanbaomall.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uyt.xuetiantiany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zte.aibaodan.cn

[A25] 字符串比较
来源：http://xce.gogol.net.cn

Py:   s1 == s2; s1 != s2
来源：http://myp.jlsjyb.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uns.yj20258888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bpz.xziqi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ctl.ivvv.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wlu.zhoulong.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xzt.guowangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://oyg.smart0.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ukp.dashuyun.cn

[A26] 类型转换总览
来源：http://qqr.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sdz.zhixingplan.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ybd.nanxinkj.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jsp.yj202588.top

TS:   Number() String() Boolean() x as number
来源：http://bap.yanxiufei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oey.quarkkingdee.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://svz.bbcook.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ltl.zhijiandao.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hay.sjlbkw.cn

================================================================================
来源：http://uzr.wangdashe.top

B. 流程控制
来源：http://tla.pycfn.com

================================================================================
来源：http://cna.chenjidiqi.icu

[B01] 条件判断 if / else
来源：http://ujc.jiagoushi.top

Py:   result = "正" if x > 0 else "非正"
来源：http://dzz.316326.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bdq.aibaodan.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ueh.yanxiufei.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fpu.quarkkingdee.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cjq.cucudq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://brp.fanxiaobao.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xqa.nanxuanxn.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cdk.daxiang520.top

[B02] 多分支 else if / elif
来源：http://cep.gogol.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cfo.wangdashe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wcg.shzxlz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rbn.sweek.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yzy.ywan-chungtsiang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fps.hywenlv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fxr.ydzc1.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hwt.dianchejie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://krb.birdmap.top

[B03] switch / match / case
来源：http://utz.hongshengwenyu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sbo.ppjwa.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://shn.nwbrower.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bin.ehwqpu.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kci.dianchejie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ego.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ypo.wangshuangyany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lba.9152youxi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dha.shanyushiyangtech.top

[B04] for 计数循环
来源：http://xen.feifeiyinyue.top

Py:   for i in range(10): print(i)
来源：http://mas.tianlin.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wna.fanxiaobao.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uof.gogol.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hco.meibo888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rfu.shangyingyoupin.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hjm.feifeiyinyue.top

Ruby: 10.times { |i| puts i }
来源：http://xcc.52xcode.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wdx.nwbrower.top

[B05] 遍历数组 / 列表
来源：http://afc.hongshengwenyu.top

Py:   for item in arr: print(item)
来源：http://xcm.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rsa.tanke756.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hqq.jinqigufen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vcb.yuxming.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tfr.zdbjq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qjf.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://tjg.yangfankeji.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pql.cashguo.top

[B06] 遍历字典 / 对象
来源：http://zxb.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qik.guannengcc.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ywl.hongshengwenyu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ace.tianlin.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://imh.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iyk.vehdjk.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rcp.cheryme.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://djy.fktsv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pjx.yuanzhike.top

[B07] while 循环
来源：http://wcs.fzhhl.top

Py:   while i < 10: i += 1
来源：http://ofb.shangyingyoupin.top

PHP:  while ($i < 10) { $i++; }
来源：http://mkn.zdqjudy.top

JS:   while (i < 10) { i++; }
来源：http://bmo.aibaodan.cn

TS:   while (i < 10) { i++; }
来源：http://czs.zdqjudy.top

Java: while (i < 10) { i++; }
来源：http://wfh.ywan-chungtsiang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://khw.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://iww.tarul.cn

C#:   while (i < 10) { i++; }
来源：http://pcm.pycfn.com

[B08] do-while（至少执行一次）
来源：http://apa.yuanzhike.top

Py:   # 无 do-while：用 while True + break
来源：http://vyb.andypj.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://uwy.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://cbc.shanyushiyangtech.top

TS:   do { i++; } while (i < 10);
来源：http://vdt.feifeiyinyue.top

Java: do { i++; } while (i < 10);
来源：http://him.fehbvm.com

Go:   for { i++; if i >= 10 { break } }
来源：http://vgr.ydjk.org.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yty.yuxming.cn

C#:   do { i++; } while (i < 10);
来源：http://prt.zhixingplan.top

[B09] break 与 continue
来源：http://qwp.sysykeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zwg.yj20258888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gtf.daria6918.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hbo.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ujw.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rtl.aizwys.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://llr.yuxming.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://adf.cheryme.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sbv.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://dop.hammf.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xzh.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uxa.jiagoushi.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ity.tanke756.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lul.cdnleiting.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pdn.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dlx.zhixingplan.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mwt.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aap.jlsjyb.cn

[B11] 生成数字序列 / 区间
来源：http://xge.yvedp.cn

Py:   list(range(0, 10, 2))
来源：http://vnr.yj20258.top

PHP:  range(0, 10, 2);
来源：http://yuc.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ekm.shzxlz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ikj.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://shx.52xcode.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mzi.tianlin.xyz

Ruby: (0...10).step(2).to_a
来源：http://evc.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://foz.hammf.cn

[B12] 跳出多层循环
来源：http://bbi.cdnleiting.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zez.zhengqikj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jkw.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lcc.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yqh.tarul.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rhj.jinqigufen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pfu.yonumen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iaw.ydjk.org.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rim.yuxming.cn

[B13] 判断是否为数字
来源：http://bvl.haohaochexian.top

Py:   isinstance(x, (int, float))
来源：http://uzq.guowangkeji.top

PHP:  is_numeric($x)
来源：http://uro.tian-w.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cte.zhengqikj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://juc.daxiang520.top

Java: x instanceof Number
来源：http://pja.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qix.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://lhn.pengpengdd.cyou

C#:   x is int or double or decimal
来源：http://ytx.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://bmn.xuetiantiany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vgr.yonumen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dzo.9152youxi.cn

JS:   [1, 2, 3].includes(x)
来源：http://lkm.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://muq.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://haj.yongpay.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yep.hysaishi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tpc.zdbjq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wdb.zdqjudy.top

[B15] 布尔运算与取反
来源：http://xix.aibaodan.cn

Py:   a and b or not c
来源：http://yuo.zhongyouzk.top

PHP:  $a && $b || !$c
来源：http://dqt.ivvv.top

JS:   a && b || !c
来源：http://zps.zhijiandao.cn

TS:   a && b || !c
来源：http://ftw.52xcode.cn

Java: a && b || !c
来源：http://yny.wangshuangyany.cn

Go:   a && b || !c
来源：http://czh.vehdjk.com

Ruby: a && b || !c
来源：http://sou.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://fui.hesvh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pte.kuanghao11.cn

Py:   if not data: return
来源：http://yox.gaohongyu789.top

PHP:  if (!$data) { return; }
来源：http://mqo.bjfxy.top

JS:   if (!data) return;
来源：http://ews.cqqwz.cn

TS:   if (!data) return;
来源：http://xjq.chenzaomai.com

Java: if (data == null) return;
来源：http://ubb.fanxiaobao.xyz

Go:   if data == nil { return }
来源：http://ftm.tarul.cn

Ruby: return if data.nil?
来源：http://zhd.shuidangran.top

C#:   if (data == null) return;
来源：http://vlf.gotoacloud.top

================================================================================
来源：http://lok.zhijiandao.cn

C. 函数与作用域
来源：http://xms.chenzaomai.com

================================================================================
来源：http://kes.kuanghao11.cn

[C01] 定义函数
来源：http://svn.ehwqpu.com

Py:   def add(a, b): return a + b
来源：http://bng.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://crt.xziqi.cn

JS:   function add(a, b) { return a + b; }
来源：http://wsl.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mfr.zdqjudy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rej.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://mol.nanxinkj.top

Ruby: def add(a, b); a + b; end
来源：http://mqj.hcnkem.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zxl.aizwys.cn

[C02] 默认参数
来源：http://bxf.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://yjn.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://dfi.yueranfly.top

JS:   function greet(name = "World") { return name; }
来源：http://atf.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vrr.bbcook.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fip.shzxlz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ydx.gotoacloud.top

Ruby: def greet(name = "World") = name
来源：http://olv.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://cqf.fktsv.cn

[C03] 可变参数
来源：http://bau.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://mkx.tianlin.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ppu.feifeiyinyue.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zuo.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zxz.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wam.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nvh.mhx1999.top

Ruby: def total(*nums); nums.sum; end
来源：http://rdy.jqgufenzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://snl.hfpthk.cn

[C04] 命名参数 / 关键字参数
来源：http://mar.xingfuxueyuan.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eff.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fca.tianlin.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rqn.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tsd.havefunace.top

Java: // 无：用 Builder 模式或 record
来源：http://alq.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://pps.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://wrs.0kj1m.cn

C#:   f(a: 1, b: 2)
来源：http://vsi.shzxlz.cn

[C05] 返回多个值
来源：http://crx.tianlin.xyz

Py:   return a, b
来源：http://yag.svipenyu.cn

PHP:  return [$a, $b];
来源：http://wrt.jyoumei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fbw.chenzaomai.com

TS:   return { a, b };
来源：http://aiw.yvedp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nvh.zhengqikj.top

Go:   return a, b
来源：http://qye.zhaomingkeji.xyz

Ruby: return a, b
来源：http://bjn.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://iqd.shanyushiyangtech.top

[C06] 匿名函数 / lambda
来源：http://gpl.daxiang520.top

Py:   square = lambda x: x * x
来源：http://zms.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://aaa.ydjk.org.cn

JS:   const square = x => x * x;
来源：http://tjo.yongpay.top

TS:   const square = (x: number): number => x * x;
来源：http://bvw.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://obk.havefunace.top

Go:   sq := func(x int) int { return x * x }
来源：http://xwn.hnxiangtu.top

Ruby: square = ->(x) { x * x }
来源：http://yzw.jyoumei.cn


<!-- 参考信息 -->