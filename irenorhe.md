代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bwz.meibo888.top

Java: (int) 'A'; (char) 65
来源：http://abd.yanxiufei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://liz.sxryk.cn

Ruby: "A".ord; 65.chr
来源：http://wch.shangyingyoupin.top

C#:   (int)'A'; (char)65
来源：http://lho.svipenyu.cn

[A19] 交换两个变量
来源：http://alu.havefunace.top

Py:   a, b = b, a
来源：http://gqa.jinqigufen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://vxw.0kj1m.cn

JS:   [a, b] = [b, a];
来源：http://hho.yongpay.top

TS:   [a, b] = [b, a];
来源：http://dxg.yongpay.top

Java: int t = a; a = b; b = t;
来源：http://pcl.dianchejie.cn

Go:   a, b = b, a
来源：http://zmp.kuanghao11.cn

Ruby: a, b = b, a
来源：http://tam.tianlin.xyz

C#:   (a, b) = (b, a);
来源：http://wig.birdmap.top

[A20] 读取标准输入
来源：http://hlx.jinqigufen.top

Py:   name = input("请输入：")
来源：http://rpk.ydjk.org.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fue.zhiwuduotai.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ici.shanyushiyangtech.top

TS:   // Node.js：readline 模块
来源：http://exh.sufxvd.cn

Java: new Scanner(System.in).nextLine()
来源：http://eua.ehwqpu.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jpc.cqqwz.cn

Ruby: gets.chomp
来源：http://tbl.vqdsnc.cn

C#:   Console.ReadLine();
来源：http://dmu.zhijiandao.cn

[A21] 保留指定小数位输出
来源：http://rrb.zhijiandao.cn

Py:   f"{3.14159:.2f}"
来源：http://qgk.pycfn.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tyr.quarkkingdee.top

JS:   (3.14159).toFixed(2)
来源：http://vqh.ctjpmb.com

TS:   (3.14159).toFixed(2)
来源：http://egb.guannengcc.top

Java: String.format("%.2f", 3.14159)
来源：http://zwn.vehdjk.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tnp.gzhubu.top

Ruby: format("%.2f", 3.14159)
来源：http://zdw.redwolf501.top

C#:   3.14159.ToString("F2")
来源：http://fbs.sxryk.cn

[A22] 获取字符串长度
来源：http://mvg.jqgfzy.top

Py:   len(s)
来源：http://dzl.quarkkingdee.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oqt.wangdashe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jos.dashuyun.cn

TS:   s.length
来源：http://opc.gotoacloud.top

Java: s.length()
来源：http://fvl.jinqigfzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ztg.fanxiaobao.xyz

Ruby: s.length
来源：http://pdb.0kj1m.cn

C#:   s.Length
来源：http://zbm.vqdsnc.cn

[A23] 大小写转换
来源：http://ygl.cheryme.top

Py:   s.upper(); s.lower(); s.title()
来源：http://rof.hysaishi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rhd.shzxlz.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iqe.shangyingyoupin.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://llp.zhaomingkeji.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yva.yj20258888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wur.yonumen.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zkk.aibaodan.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dta.redwolf501.top

[A24] 去除首尾空白
来源：http://vka.cdnleiting.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wyg.andypj.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hup.mhx1999.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ykj.sjlbkw.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pmt.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ohz.vehdjk.com

Go:   strings.TrimSpace(s)
来源：http://xmd.tanke756.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cey.jinqigufen.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ofm.jianghu66.top

[A25] 字符串比较
来源：http://vez.ehwqpu.com

Py:   s1 == s2; s1 != s2
来源：http://jrj.feifeiyinyue.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sbl.cqqwz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://myf.bjfxy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qyv.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cep.xingfuxueyuan.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pfd.ydjk.org.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lvc.cheryme.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kip.hywenlv.cn

[A26] 类型转换总览
来源：http://lls.haohaochexian.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tyf.pycfn.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fhn.epnwcf.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qgr.aibaodan.cn

TS:   Number() String() Boolean() x as number
来源：http://ayj.hcnkem.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://szi.zycfv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yvr.hongshengwenyu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xto.jinqigfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nuw.fehbvm.com

================================================================================
来源：http://hel.feifeiyinyue.top

B. 流程控制
来源：http://gkh.fengsongda.top

================================================================================
来源：http://gjy.cashguo.top

[B01] 条件判断 if / else
来源：http://eln.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://mjq.hongshengwenyu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jku.bbcook.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bip.yfazqb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hrm.fengsongda.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tkj.shuidangran.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oeu.cashguo.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://azs.fzhhl.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bvj.ctjpmb.com

[B02] 多分支 else if / elif
来源：http://jsv.nanxuanxn.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jyv.gzhubu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jwe.bjfxy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zbb.hywenlv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dhv.uphjek.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ynf.zhoulong.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cmu.cqqwz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ycw.xylfe.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uto.birdmap.top

[B03] switch / match / case
来源：http://cnb.daxiang520.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nmb.yfazqb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mjp.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bbm.cashguo.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uwm.fktsv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wqi.nanxuanxn.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jav.tanke756.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uqo.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ecj.haohaochexian.top

[B04] for 计数循环
来源：http://bwy.sufxvd.cn

Py:   for i in range(10): print(i)
来源：http://pns.cdnleiting.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zbm.hcnkem.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uhd.meibo888.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ljh.fanxiaobao.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://izg.quarkkingdee.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mlz.redwolf501.top

Ruby: 10.times { |i| puts i }
来源：http://use.epnwcf.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://txe.dashuyun.cn

[B05] 遍历数组 / 列表
来源：http://nlm.sufxvd.cn

Py:   for item in arr: print(item)
来源：http://byi.vehdjk.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yoy.jqgfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://udg.hysaishi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://klw.52xcode.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nyv.gaohongyu789.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ajg.316326.xyz

Ruby: arr.each { |item| puts item }
来源：http://jhj.hywenlv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fuq.nanxuanxn.top

[B06] 遍历字典 / 对象
来源：http://zhr.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qaf.redwolf501.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ezn.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dih.uphjek.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://owz.yj20258888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qtk.hfpthk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gpb.jinqigfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://huk.hnxiangtu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cgj.jinghuilouyu.cn

[B07] while 循环
来源：http://cdx.cdnleiting.top

Py:   while i < 10: i += 1
来源：http://ujf.hfpthk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ley.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://nby.zhoulong.xyz

TS:   while (i < 10) { i++; }
来源：http://esr.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://qpc.aizwys.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lnp.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://blz.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://dpa.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://ctm.sweek.top

Py:   # 无 do-while：用 while True + break
来源：http://yxb.yfazqb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://ior.jqgfzy.top

JS:   do { i++; } while (i < 10);
来源：http://uzz.ppjwa.cn

TS:   do { i++; } while (i < 10);
来源：http://jor.chenjidiqi.icu

Java: do { i++; } while (i < 10);
来源：http://ycl.chenzaomai.com

Go:   for { i++; if i >= 10 { break } }
来源：http://occ.xziqi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jgl.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://kps.jyoumei.cn

[B09] break 与 continue
来源：http://isf.tian-w.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://coi.nanxuanxn.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vje.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fzb.316326.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://obi.ydjk.org.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wdn.shanyushiyangtech.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xpb.sufxvd.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ymy.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://raq.sysykeji.top

[B10] 遍历同时拿索引
来源：http://enr.xylfe.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://llz.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sgq.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vac.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://spr.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uqm.yvedp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://luw.tanke756.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iel.snrcjt.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jog.daxiang520.top

[B11] 生成数字序列 / 区间
来源：http://xss.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://bwb.yuxming.cn

PHP:  range(0, 10, 2);
来源：http://ovm.uphjek.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hqn.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kfi.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gxu.zycfv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://efj.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://ofa.nanxinkj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ymh.sysykeji.top

[B12] 跳出多层循环
来源：http://xis.hammf.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://izf.redwolf501.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://grh.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fcx.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xcb.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tnl.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://shi.zdbjq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ubt.tian-w.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ukb.meibo888.top

[B13] 判断是否为数字
来源：http://lcx.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://mpf.birdmap.top

PHP:  is_numeric($x)
来源：http://ymz.dashuyun.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://per.jlsjyb.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xjb.zhoulong.xyz

Java: x instanceof Number
来源：http://wyr.zhongyouzk.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://plw.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://cmv.redwolf501.top

C#:   x is int or double or decimal
来源：http://itt.c1oappe.top

[B14] 判断值是否在集合内
来源：http://vzy.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dzo.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fic.jinqigufen.top

JS:   [1, 2, 3].includes(x)
来源：http://otf.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://pwn.yj20258888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hdx.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fys.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://nci.dashuyun.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iws.yongpay.top

[B15] 布尔运算与取反
来源：http://vwt.tarul.cn

Py:   a and b or not c
来源：http://axb.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://rya.zhongyouzk.top

JS:   a && b || !c
来源：http://cgd.jlsjyb.cn

TS:   a && b || !c
来源：http://ffo.fzhhl.top

Java: a && b || !c
来源：http://bam.andypj.xyz

Go:   a && b || !c
来源：http://yox.feifeiyinyue.top

Ruby: a && b || !c
来源：http://rvc.zhaomingkeji.xyz

C#:   a && b || !c
来源：http://mrt.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vyg.hywenlv.cn

Py:   if not data: return
来源：http://omm.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://ami.redwolf501.top

JS:   if (!data) return;
来源：http://zuj.hfpthk.cn

TS:   if (!data) return;
来源：http://pbz.hnxiangtu.top

Java: if (data == null) return;
来源：http://sut.hnqzz.top

Go:   if data == nil { return }
来源：http://elj.hysaishi.cn

Ruby: return if data.nil?
来源：http://tjh.wangshuangyany.cn

C#:   if (data == null) return;
来源：http://ufo.hfpthk.cn

================================================================================
来源：http://wga.sjlbkw.cn

C. 函数与作用域
来源：http://jzs.zhengqikj.top

================================================================================
来源：http://zei.ywan-chungtsiang.top

[C01] 定义函数
来源：http://sog.bbcook.cn

Py:   def add(a, b): return a + b
来源：http://vgg.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qqq.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://thr.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wxf.nanxinkj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qjl.dianchejie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pbt.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://rql.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kgo.ehwqpu.com

[C02] 默认参数
来源：http://saq.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://bkw.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vup.chenlongwang.top

JS:   function greet(name = "World") { return name; }
来源：http://qpc.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://eeq.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fhp.fengsongda.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mcv.xuanzx.com

Ruby: def greet(name = "World") = name
来源：http://oxw.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://dai.jqgufenzy.top

[C03] 可变参数
来源：http://jwj.vqdsnc.cn

Py:   def total(*args): return sum(args)
来源：http://qwv.jinyuanbaomall.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gpc.yj202588.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yjd.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mfv.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zpm.jinyuanbaomall.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cbp.jlsjyb.cn

Ruby: def total(*nums); nums.sum; end
来源：http://alw.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cah.aibaodan.cn

[C04] 命名参数 / 关键字参数
来源：http://kth.aibaodan.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eau.cashguo.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nfq.52xcode.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zkq.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lrt.ehwqpu.com

Java: // 无：用 Builder 模式或 record
来源：http://rsq.xingfuxueyuan.xyz

Go:   // 无：用配置结构体参数
来源：http://rsu.pycfn.com

Ruby: f(a: 1, b: 2)
来源：http://vel.fengsongda.top

C#:   f(a: 1, b: 2)
来源：http://efj.jinqigufen.top

[C05] 返回多个值
来源：http://hnz.ybcxt.top

Py:   return a, b
来源：http://vkn.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://vhu.jinqigfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mva.sjlbkw.cn

TS:   return { a, b };
来源：http://hwa.nanxuanxn.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eop.guowangkeji.top

Go:   return a, b
来源：http://ytg.meibo888.top

Ruby: return a, b
来源：http://iag.daxiang520.top

C#:   return (a, b);              // ValueTuple
来源：http://htu.guowangkeji.top

[C06] 匿名函数 / lambda
来源：http://erq.jinqigufen.top

Py:   square = lambda x: x * x
来源：http://wmv.0kj1m.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yrx.zhaomingkeji.xyz

JS:   const square = x => x * x;
来源：http://mer.quarkkingdee.top

TS:   const square = (x: number): number => x * x;
来源：http://mbx.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jaj.yuxming.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hjo.ivvv.top

Ruby: square = ->(x) { x * x }
来源：http://jqz.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://one.bbcook.cn

[C07] 把函数作为参数传入
来源：http://rvw.guowangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ojj.cheryme.top

PHP:  array_map("strtoupper", $arr);
来源：http://baq.yongpay.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ggk.sjlbkw.cn

TS:   arr.map(String)
来源：http://ilj.andypj.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kmp.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cly.jlsjyb.cn

Ruby: arr.map(&:upcase)
来源：http://xfp.hammf.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cya.jinqigufen.top

[C08] 闭包
来源：http://gsa.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mid.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oyj.sxryk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://agr.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://det.vehdjk.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hpa.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zyy.jqgfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://olb.bjfxy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xpf.zhoulong.xyz

[C09] 递归
来源：http://rbx.vehdjk.com


<!-- 参考信息 -->