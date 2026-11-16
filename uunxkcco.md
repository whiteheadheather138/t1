代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://osv.ctjpmb.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dlq.hcnkem.com

TS:   if (!x) {}
来源：http://lpw.hfpthk.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yel.zhoulong.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uqi.sysykeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://ixh.vehdjk.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hkm.jinqigufen.top

[A17] 位运算
来源：http://tnx.xuetiantiany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gby.haohaochexian.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://stl.gaohongyu789.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qwo.sweek.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ldd.yfazqb.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://olj.fzhhl.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kvk.fengsongda.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mgy.nanxuanxn.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cog.jlsjyb.cn

[A18] 字符与 ASCII 码互转
来源：http://dlc.gogol.net.cn

Py:   ord("A"); chr(65)
来源：http://iag.jqgufenzy.top

PHP:  ord("A"); chr(65)
来源：http://xba.ivvv.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wth.hnxiangtu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hgx.sweek.top

Java: (int) 'A'; (char) 65
来源：http://lwj.yvedp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://prm.smart0.xyz

Ruby: "A".ord; 65.chr
来源：http://ymn.haohaochexian.top

C#:   (int)'A'; (char)65
来源：http://rht.pycfn.com

[A19] 交换两个变量
来源：http://vda.jyoumei.cn

Py:   a, b = b, a
来源：http://ert.gaohongyu789.top

PHP:  [$a, $b] = [$b, $a];
来源：http://psl.daria6918.cn

JS:   [a, b] = [b, a];
来源：http://atc.bbcook.cn

TS:   [a, b] = [b, a];
来源：http://mel.xuanzx.com

Java: int t = a; a = b; b = t;
来源：http://sbl.birdmap.top

Go:   a, b = b, a
来源：http://gdc.vehdjk.com

Ruby: a, b = b, a
来源：http://ucc.yvedp.cn

C#:   (a, b) = (b, a);
来源：http://fbx.sysykeji.top

[A20] 读取标准输入
来源：http://whs.yj20258888.top

Py:   name = input("请输入：")
来源：http://ayr.yj20258.top

PHP:  $name = trim(fgets(STDIN));
来源：http://gvf.cdnleiting.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sug.vqdsnc.cn

TS:   // Node.js：readline 模块
来源：http://eig.yanxiufei.cn

Java: new Scanner(System.in).nextLine()
来源：http://szq.jinghuilouyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://img.hysaishi.cn

Ruby: gets.chomp
来源：http://fco.jyoumei.cn

C#:   Console.ReadLine();
来源：http://tti.jyoumei.cn

[A21] 保留指定小数位输出
来源：http://dke.chenzaomai.com

Py:   f"{3.14159:.2f}"
来源：http://qeq.nanxinkj.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xzl.cheryme.top

JS:   (3.14159).toFixed(2)
来源：http://auo.tian-w.cn

TS:   (3.14159).toFixed(2)
来源：http://hqw.jinqigufen.top

Java: String.format("%.2f", 3.14159)
来源：http://agj.wangshuangyany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hvs.birdmap.top

Ruby: format("%.2f", 3.14159)
来源：http://fzf.yonumen.top

C#:   3.14159.ToString("F2")
来源：http://xss.jinyuanbaomall.cn

[A22] 获取字符串长度
来源：http://dwk.yvedp.cn

Py:   len(s)
来源：http://ugc.jiagoushi.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tal.zhijiandao.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nfh.zhongyouzk.top

TS:   s.length
来源：http://hnd.kuanghao11.cn

Java: s.length()
来源：http://jkd.havefunace.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cpq.dashuyun.cn

Ruby: s.length
来源：http://tix.dianchejie.cn

C#:   s.Length
来源：http://ijv.tarul.cn

[A23] 大小写转换
来源：http://fod.hammf.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wee.ydjk.org.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://map.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ogs.tarul.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://klj.ehwqpu.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lxl.sxryk.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dht.hfpthk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xub.ehwqpu.com

C#:   s.ToUpper(); s.ToLower()
来源：http://bmo.jinyuanbaomall.cn

[A24] 去除首尾空白
来源：http://lwf.smart0.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ldr.yuxming.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sjz.xziqi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://igq.chenlongwang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sbw.svipenyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://itu.sweek.top

Go:   strings.TrimSpace(s)
来源：http://kon.yueranfly.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zjw.uphjek.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tgi.birdmap.top

[A25] 字符串比较
来源：http://qbo.sxryk.cn

Py:   s1 == s2; s1 != s2
来源：http://aaq.hysaishi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vgg.aizwys.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rkw.ydzc1.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xet.ctjpmb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cnp.nanxuanxn.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xhb.zhongyouzk.top

Ruby: s1 == s2; s1 <=> s2
来源：http://irj.yuxming.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gff.gaohongyu789.top

[A26] 类型转换总览
来源：http://jps.guannengcc.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gxq.zhixingplan.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ioy.havefunace.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zte.gotoacloud.top

TS:   Number() String() Boolean() x as number
来源：http://jgn.shzxlz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oav.bjfxy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ndo.daria6918.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ntp.yongpay.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hqt.smart0.xyz

================================================================================
来源：http://quh.havefunace.top

B. 流程控制
来源：http://crk.nwbrower.top

================================================================================
来源：http://zel.jinqigufen.top

[B01] 条件判断 if / else
来源：http://aev.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ngy.yj20258888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ite.gogol.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kvx.zdbjq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://znn.svipenyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dgm.hcnkem.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fbn.mhx1999.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cin.jqgufenzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://awl.chenzaomai.com

[B02] 多分支 else if / elif
来源：http://osn.snrcjt.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rsz.fktsv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wvh.jinqigufen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rhg.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ism.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://coe.jiagoushi.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ikm.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rnj.gzhubu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ihe.havefunace.top

[B03] switch / match / case
来源：http://ziz.fzhhl.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ztm.pycfn.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dsr.jlsjyb.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wtn.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bcy.zdqjudy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ihp.sysykeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zas.bjfxy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qto.zhiwuduotai.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yla.zhoulong.xyz

[B04] for 计数循环
来源：http://vgr.xuanzx.com

Py:   for i in range(10): print(i)
来源：http://iwe.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fsc.hywenlv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vag.xuanzx.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mrq.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bst.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rvl.aizwys.cn

Ruby: 10.times { |i| puts i }
来源：http://hxt.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qmd.wangdashe.top

[B05] 遍历数组 / 列表
来源：http://prj.meibo888.top

Py:   for item in arr: print(item)
来源：http://gyl.nwbrower.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lgf.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bir.xinyue.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://hjn.zdqjudy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jmh.gaohongyu789.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zze.ppjwa.cn

Ruby: arr.each { |item| puts item }
来源：http://oug.wangshuangyany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aeh.wangshuangyany.cn

[B06] 遍历字典 / 对象
来源：http://bwm.yangfankeji.com

Py:   for k, v in d.items(): print(k, v)
来源：http://ixv.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ywi.zdbjq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aaq.andypj.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://foe.xingfuxueyuan.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oyj.bjfxy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ejy.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ibi.hcnkem.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bun.ppjwa.cn

[B07] while 循环
来源：http://wcx.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://dip.ehwqpu.com

PHP:  while ($i < 10) { $i++; }
来源：http://pjy.ivvv.top

JS:   while (i < 10) { i++; }
来源：http://jwm.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://fot.hfpthk.cn

Java: while (i < 10) { i++; }
来源：http://xic.yuanzhike.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wsk.aizwys.cn

Ruby: while i < 10; i += 1; end
来源：http://yyo.ydjk.org.cn

C#:   while (i < 10) { i++; }
来源：http://kfn.epnwcf.com

[B08] do-while（至少执行一次）
来源：http://mox.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://jmg.zhaomingkeji.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://ldr.daria6918.cn

JS:   do { i++; } while (i < 10);
来源：http://nhl.daxiang520.top

TS:   do { i++; } while (i < 10);
来源：http://vxe.sweek.top

Java: do { i++; } while (i < 10);
来源：http://oij.yj20258.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ugz.iojbl.cn

Ruby: begin; i += 1; end while i < 10
来源：http://szg.haohaochexian.top

C#:   do { i++; } while (i < 10);
来源：http://eox.zycfv.cn

[B09] break 与 continue
来源：http://vuq.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fvj.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uhl.yvedp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wot.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uaw.zdbjq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kgy.fanxiaobao.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://osm.hammf.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tnb.tanke756.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bad.yanxiufei.cn

[B10] 遍历同时拿索引
来源：http://jhn.xingfuxueyuan.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qsy.yfazqb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eyq.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://njm.snrcjt.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rlu.nanxuanxn.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://akt.hcnkem.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gdr.jiagoushi.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wal.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vmd.sweek.top

[B11] 生成数字序列 / 区间
来源：http://vaf.nwbrower.top

Py:   list(range(0, 10, 2))
来源：http://fxt.dianchejie.cn

PHP:  range(0, 10, 2);
来源：http://jbu.redwolf501.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uuv.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zaa.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qzq.chenzaomai.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tay.tarul.cn

Ruby: (0...10).step(2).to_a
来源：http://xyt.sjlbkw.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lil.zhiwuduotai.top

[B12] 跳出多层循环
来源：http://sde.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tbg.pycfn.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://itw.daria6918.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nqd.guannengcc.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ysg.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tqu.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ktg.tanke756.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://adc.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zrc.zhongyouzk.top

[B13] 判断是否为数字
来源：http://yxc.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://lsa.316326.xyz

PHP:  is_numeric($x)
来源：http://mvn.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zya.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mlj.yvedp.cn

Java: x instanceof Number
来源：http://pxi.wangdashe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jss.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://pwe.fehbvm.com

C#:   x is int or double or decimal
来源：http://wuc.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://uuq.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gcj.gzhubu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ehk.tanke756.top

JS:   [1, 2, 3].includes(x)
来源：http://sfm.cheryme.top

TS:   [1, 2, 3].includes(x)
来源：http://nlr.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zpg.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dgy.shanyushiyangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://yxb.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lik.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://oao.gaohongyu789.top

Py:   a and b or not c
来源：http://pmh.ehwqpu.com

PHP:  $a && $b || !$c
来源：http://lsf.nwbrower.top

JS:   a && b || !c
来源：http://gbq.ehwqpu.com

TS:   a && b || !c
来源：http://ttf.hysaishi.cn

Java: a && b || !c
来源：http://ebu.aibaodan.cn

Go:   a && b || !c
来源：http://jks.zhoulong.xyz

Ruby: a && b || !c
来源：http://cly.jinqigfzy.top

C#:   a && b || !c
来源：http://pqv.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://zvg.fktsv.cn

Py:   if not data: return
来源：http://stz.pycfn.com

PHP:  if (!$data) { return; }
来源：http://txi.fehbvm.com

JS:   if (!data) return;
来源：http://szd.jqgfzy.top

TS:   if (!data) return;
来源：http://gww.zhixingplan.top

Java: if (data == null) return;
来源：http://ohn.chenlongwang.top

Go:   if data == nil { return }
来源：http://dkq.jianghu66.top

Ruby: return if data.nil?
来源：http://yxb.xinyue.icu

C#:   if (data == null) return;
来源：http://qla.shangyingyoupin.top

================================================================================
来源：http://mye.feifeiyinyue.top

C. 函数与作用域
来源：http://qpx.vehdjk.com

================================================================================
来源：http://yiq.yonumen.top

[C01] 定义函数
来源：http://dkr.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://hfz.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gpg.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://qnw.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sgc.jqgfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ope.yueranfly.top

Go:   func add(a, b int) int { return a + b }
来源：http://vqw.sweek.top

Ruby: def add(a, b); a + b; end
来源：http://yks.zhongyouzk.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pjp.hammf.cn

[C02] 默认参数
来源：http://lgv.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://gne.shuidangran.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kwt.aibaodan.cn

JS:   function greet(name = "World") { return name; }
来源：http://lwq.cdnleiting.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sxc.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xhe.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ejx.quarkkingdee.top

Ruby: def greet(name = "World") = name
来源：http://ndo.nwbrower.top

C#:   string Greet(string name = "World") => name;
来源：http://wvz.zhiwuduotai.top

[C03] 可变参数
来源：http://ohp.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://fut.yongpay.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tfb.jlsjyb.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ino.ctjpmb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://noq.vehdjk.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mxn.hnqzz.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lgh.gaohongyu789.top

Ruby: def total(*nums); nums.sum; end
来源：http://eds.smart0.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bmr.gotoacloud.top

[C04] 命名参数 / 关键字参数
来源：http://ftg.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jlf.hcnkem.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ltz.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zgn.bjfxy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pbi.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://uaj.ywan-chungtsiang.top

Go:   // 无：用配置结构体参数
来源：http://dmu.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://wjl.jlsjyb.cn

C#:   f(a: 1, b: 2)
来源：http://uyw.ydjk.org.cn

[C05] 返回多个值
来源：http://kfu.haohaochexian.top

Py:   return a, b
来源：http://byi.zdqjudy.top

PHP:  return [$a, $b];
来源：http://lxd.cashguo.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jhc.yonumen.top

TS:   return { a, b };
来源：http://mwb.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tmp.havefunace.top

Go:   return a, b
来源：http://joo.hywenlv.cn

Ruby: return a, b
来源：http://usr.vehdjk.com

C#:   return (a, b);              // ValueTuple
来源：http://szr.jqgfzy.top

[C06] 匿名函数 / lambda
来源：http://vzq.gogol.net.cn

Py:   square = lambda x: x * x
来源：http://cyl.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nqm.ppjwa.cn

JS:   const square = x => x * x;
来源：http://vqk.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://txx.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ueg.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://sei.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://ogi.quarkkingdee.top


<!-- 参考信息 -->