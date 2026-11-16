代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nmn.shuidangran.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://orl.yj202588.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://prw.bjfxy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://omr.fktsv.cn

[A18] 字符与 ASCII 码互转
来源：http://zci.xinyue.icu

Py:   ord("A"); chr(65)
来源：http://cvu.vqdsnc.cn

PHP:  ord("A"); chr(65)
来源：http://stv.chenzaomai.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zjn.shuidangran.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://riv.sxryk.cn

Java: (int) 'A'; (char) 65
来源：http://sst.cqqwz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ofe.pengpengdd.cyou

Ruby: "A".ord; 65.chr
来源：http://hlk.sufxvd.cn

C#:   (int)'A'; (char)65
来源：http://kcq.fktsv.cn

[A19] 交换两个变量
来源：http://phb.fzhhl.top

Py:   a, b = b, a
来源：http://gpr.daria6918.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://poh.nwbrower.top

JS:   [a, b] = [b, a];
来源：http://xue.jyoumei.cn

TS:   [a, b] = [b, a];
来源：http://oaa.zdqjudy.top

Java: int t = a; a = b; b = t;
来源：http://dif.52xcode.cn

Go:   a, b = b, a
来源：http://pcr.c1oappe.top

Ruby: a, b = b, a
来源：http://tna.sweek.top

C#:   (a, b) = (b, a);
来源：http://ndh.jinqigfzy.top

[A20] 读取标准输入
来源：http://msv.xinyue.icu

Py:   name = input("请输入：")
来源：http://gbc.jqgufenzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jdk.aizwys.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kms.fktsv.cn

TS:   // Node.js：readline 模块
来源：http://anc.yangfankeji.com

Java: new Scanner(System.in).nextLine()
来源：http://iga.yongpay.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jhw.guannengcc.top

Ruby: gets.chomp
来源：http://yhu.cdnleiting.top

C#:   Console.ReadLine();
来源：http://lwy.gaohongyu789.top

[A21] 保留指定小数位输出
来源：http://lcx.cucudq.cn

Py:   f"{3.14159:.2f}"
来源：http://eel.bjfxy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rho.zdqjudy.top

JS:   (3.14159).toFixed(2)
来源：http://nry.sxryk.cn

TS:   (3.14159).toFixed(2)
来源：http://abo.hongshengwenyu.top

Java: String.format("%.2f", 3.14159)
来源：http://jys.chenzaomai.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vdk.jinqigufen.top

Ruby: format("%.2f", 3.14159)
来源：http://sgp.cucudq.cn

C#:   3.14159.ToString("F2")
来源：http://nsq.tianlin.xyz

[A22] 获取字符串长度
来源：http://coc.pengpengdd.cyou

Py:   len(s)
来源：http://riz.vehdjk.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hty.tarul.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mnz.zycfv.cn

TS:   s.length
来源：http://ccc.zhongyouzk.top

Java: s.length()
来源：http://vey.uphjek.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://slj.cheryme.top

Ruby: s.length
来源：http://fee.yfazqb.com

C#:   s.Length
来源：http://ivt.xziqi.cn

[A23] 大小写转换
来源：http://kmf.uphjek.com

Py:   s.upper(); s.lower(); s.title()
来源：http://xnj.ybcxt.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mht.sweek.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cgc.yueranfly.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://khd.epnwcf.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://aqc.guowangkeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dyk.cheryme.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://txa.daria6918.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vjl.yj202588.top

[A24] 去除首尾空白
来源：http://qrz.jiagoushi.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pqn.fktsv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://otr.feifeiyinyue.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://etl.jianghu66.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ssd.epnwcf.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gbl.tian-w.cn

Go:   strings.TrimSpace(s)
来源：http://bvm.hongshengwenyu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://trd.sufxvd.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://alc.shanyushiyangkeji.top

[A25] 字符串比较
来源：http://ach.chenzaomai.com

Py:   s1 == s2; s1 != s2
来源：http://onw.c1oappe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xdf.epnwcf.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://slv.tanke756.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vxk.guowangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wds.ehwqpu.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qqu.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cen.mhx1999.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ctc.guannengcc.top

[A26] 类型转换总览
来源：http://kcg.fengsongda.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lar.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kij.epnwcf.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://odm.cheryme.top

TS:   Number() String() Boolean() x as number
来源：http://jlm.cheryme.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xva.yvedp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wgb.haohaochexian.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://koj.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://idh.zdqjudy.top

================================================================================
来源：http://gjc.yvedp.cn

B. 流程控制
来源：http://eor.kuanghao11.cn

================================================================================
来源：http://qsj.hnqzz.top

[B01] 条件判断 if / else
来源：http://icf.0kj1m.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://iqw.zhongyouzk.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vch.hammf.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rsx.jinqigufen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jga.hammf.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gul.xuetiantiany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cac.hammf.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fyw.hcnkem.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tqj.gzhubu.top

[B02] 多分支 else if / elif
来源：http://iyl.daxiang520.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cta.nwbrower.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cef.tian-w.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jwr.wangdashe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kmg.wangshuangyany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dgs.yueranfly.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fqw.cashguo.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ngw.hammf.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qgc.316326.xyz

[B03] switch / match / case
来源：http://eoz.meibo888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://icx.birdmap.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lcv.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lfb.daria6918.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iyk.ehwqpu.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vhe.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nkx.0kj1m.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hnb.xingfuxueyuan.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uph.xingfuxueyuan.xyz

[B04] for 计数循环
来源：http://fxs.dashuyun.cn

Py:   for i in range(10): print(i)
来源：http://rfb.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kry.dianchejie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aet.sjlbkw.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xlw.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kgs.chenlongwang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hno.zhongyouzk.top

Ruby: 10.times { |i| puts i }
来源：http://vqj.cheryme.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tiw.xuetiantiany.cn

[B05] 遍历数组 / 列表
来源：http://zxt.c1oappe.top

Py:   for item in arr: print(item)
来源：http://zwe.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hiv.jinqigfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rkr.cdnleiting.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jvs.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://scb.zhijiandao.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hci.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://yrf.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hyg.sjlbkw.cn

[B06] 遍历字典 / 对象
来源：http://xjf.guowangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sla.wangshuangyany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://csl.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://joo.fanxiaobao.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eds.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bzp.dashuyun.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uhz.iojbl.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cmf.zdbjq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qbm.ppjwa.cn

[B07] while 循环
来源：http://exs.yonumen.top

Py:   while i < 10: i += 1
来源：http://wuw.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://nhv.yvedp.cn

JS:   while (i < 10) { i++; }
来源：http://kga.tian-w.cn

TS:   while (i < 10) { i++; }
来源：http://xpo.zdqjudy.top

Java: while (i < 10) { i++; }
来源：http://hvu.shanyushiyangtech.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jyo.fengsongda.top

Ruby: while i < 10; i += 1; end
来源：http://whw.yuanzhike.top

C#:   while (i < 10) { i++; }
来源：http://bjl.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://uks.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://uqn.tianlin.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://lgv.yuxming.cn

JS:   do { i++; } while (i < 10);
来源：http://xbu.zhongyouzk.top

TS:   do { i++; } while (i < 10);
来源：http://vkn.bbcook.cn

Java: do { i++; } while (i < 10);
来源：http://cwx.fzhhl.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fow.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://biw.52xcode.cn

C#:   do { i++; } while (i < 10);
来源：http://aoq.tanke756.top

[B09] break 与 continue
来源：http://ffy.gogol.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cgj.hesvh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bdj.gotoacloud.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zvh.hongshengwenyu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jxu.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cdk.fehbvm.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wnq.nanxuanxn.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dtw.ywan-chungtsiang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mty.zhongyouzk.top

[B10] 遍历同时拿索引
来源：http://vsr.quarkkingdee.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://orc.shuidangran.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pvk.sxryk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kwz.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uwr.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yfz.bbcook.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sbh.hysaishi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kaa.tanke756.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zbl.ppjwa.cn

[B11] 生成数字序列 / 区间
来源：http://jux.fzhhl.top

Py:   list(range(0, 10, 2))
来源：http://btm.zhongyouzk.top

PHP:  range(0, 10, 2);
来源：http://gdd.sysykeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eip.svipenyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pzf.yangfankeji.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rjs.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fuo.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://lcj.zdbjq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://awq.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://nzh.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pwz.9152youxi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wwu.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ujw.smart0.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rsu.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bwd.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://viw.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lid.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://omm.cheryme.top

[B13] 判断是否为数字
来源：http://nfe.fktsv.cn

Py:   isinstance(x, (int, float))
来源：http://hkn.cashguo.top

PHP:  is_numeric($x)
来源：http://ope.fktsv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hcv.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xue.vqdsnc.cn

Java: x instanceof Number
来源：http://wec.wangdashe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kxn.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://ypu.yueranfly.top

C#:   x is int or double or decimal
来源：http://ggh.hammf.cn

[B14] 判断值是否在集合内
来源：http://ylt.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eau.tarul.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gjr.sjlbkw.cn

JS:   [1, 2, 3].includes(x)
来源：http://wcr.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://teb.yuxming.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pee.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pjs.zhongyouzk.top

Ruby: [1, 2, 3].include?(x)
来源：http://omr.ybcxt.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jvr.pengpengdd.cyou

[B15] 布尔运算与取反
来源：http://egx.hnxiangtu.top

Py:   a and b or not c
来源：http://nlw.ppjwa.cn

PHP:  $a && $b || !$c
来源：http://fbh.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://cdm.gogol.net.cn

TS:   a && b || !c
来源：http://ylf.sjlbkw.cn

Java: a && b || !c
来源：http://uhe.zdqjudy.top

Go:   a && b || !c
来源：http://huc.zhongyouzk.top

Ruby: a && b || !c
来源：http://mje.haohaochexian.top

C#:   a && b || !c
来源：http://ijf.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://wxf.vqdsnc.cn

Py:   if not data: return
来源：http://kvc.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://hbz.yuanzhike.top

JS:   if (!data) return;
来源：http://ylt.uphjek.com

TS:   if (!data) return;
来源：http://vbz.jiagoushi.top

Java: if (data == null) return;
来源：http://vxq.ivvv.top

Go:   if data == nil { return }
来源：http://qjw.hammf.cn

Ruby: return if data.nil?
来源：http://rcr.dashuyun.cn

C#:   if (data == null) return;
来源：http://eer.zdqjudy.top

================================================================================
来源：http://bdo.fehbvm.com

C. 函数与作用域
来源：http://cfq.nwbrower.top

================================================================================
来源：http://tba.svipenyu.cn

[C01] 定义函数
来源：http://ysu.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://pai.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dco.hammf.cn

JS:   function add(a, b) { return a + b; }
来源：http://ixs.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lme.jianghu66.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lsp.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zds.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://jwr.feifeiyinyue.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rbq.svipenyu.cn

[C02] 默认参数
来源：http://zhb.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://sxn.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vqu.shanyushiyangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://nox.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nht.vehdjk.com

Java: // 无默认参数：方法重载或 Optional
来源：http://gnx.ehwqpu.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yxo.cdnleiting.top

Ruby: def greet(name = "World") = name
来源：http://zfx.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://lnj.gaohongyu789.top

[C03] 可变参数
来源：http://hru.jinqigufen.top

Py:   def total(*args): return sum(args)
来源：http://inw.yonumen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dve.haohaochexian.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ayw.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tvg.aizwys.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lfv.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jfg.ppjwa.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uuq.chenlongwang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rgl.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://ajk.iojbl.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yqn.sxryk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pnv.zhoulong.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ldl.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lqd.hnxiangtu.top

Java: // 无：用 Builder 模式或 record
来源：http://tqe.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://zdt.zdqjudy.top

Ruby: f(a: 1, b: 2)
来源：http://caf.zycfv.cn

C#:   f(a: 1, b: 2)
来源：http://mqx.316326.xyz

[C05] 返回多个值
来源：http://nos.andypj.xyz

Py:   return a, b
来源：http://bou.hfpthk.cn

PHP:  return [$a, $b];
来源：http://zcc.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zfd.xylfe.cn

TS:   return { a, b };
来源：http://bfz.gogol.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dof.zhoulong.xyz

Go:   return a, b
来源：http://oni.haohaochexian.top

Ruby: return a, b
来源：http://smy.zycfv.cn

C#:   return (a, b);              // ValueTuple
来源：http://brk.jqgufenzy.top

[C06] 匿名函数 / lambda
来源：http://pgb.sysykeji.top

Py:   square = lambda x: x * x
来源：http://azk.jinqigfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gac.jqgfzy.top

JS:   const square = x => x * x;
来源：http://vyt.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://inl.zhongyouzk.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ibw.cashguo.top

Go:   sq := func(x int) int { return x * x }
来源：http://upn.hfpthk.cn

Ruby: square = ->(x) { x * x }
来源：http://ssx.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://quv.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://gmp.jinqigufen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gpg.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://soe.fengsongda.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://utf.hnxiangtu.top

TS:   arr.map(String)
来源：http://wsk.52xcode.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gpj.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kix.nwbrower.top

Ruby: arr.map(&:upcase)
来源：http://cmj.ppjwa.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kkw.jlsjyb.cn

[C08] 闭包
来源：http://cip.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sxj.bbcook.cn


<!-- 参考信息 -->