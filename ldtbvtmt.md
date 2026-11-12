代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oii.jinqigufen.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xsy.sufxvd.cn

TS:   if (!x) {}
来源：http://xet.smart0.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vmo.svipenyu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qae.c1oappe.top

Ruby: unless x            # nil 与 false 为假
来源：http://yst.yj20258888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://paz.pycfn.com

[A17] 位运算
来源：http://wnw.nanxuanxn.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://owv.hysaishi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://azb.c1oappe.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fqn.daria6918.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nxb.pycfn.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://frz.ivvv.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xym.svipenyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vjh.yj20258.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jwi.cdnleiting.top

[A18] 字符与 ASCII 码互转
来源：http://tmz.pycfn.com

Py:   ord("A"); chr(65)
来源：http://vxt.c1oappe.top

PHP:  ord("A"); chr(65)
来源：http://kdn.nwbrower.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xeo.meibo888.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://biq.gogol.net.cn

Java: (int) 'A'; (char) 65
来源：http://lxd.hesvh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jzd.chenzaomai.com

Ruby: "A".ord; 65.chr
来源：http://tmy.iojbl.cn

C#:   (int)'A'; (char)65
来源：http://snk.0kj1m.cn

[A19] 交换两个变量
来源：http://itr.yuxming.cn

Py:   a, b = b, a
来源：http://etc.sweek.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jqo.shzxlz.cn

JS:   [a, b] = [b, a];
来源：http://fox.kuanghao11.cn

TS:   [a, b] = [b, a];
来源：http://owf.hongshengwenyu.top

Java: int t = a; a = b; b = t;
来源：http://kbw.quarkkingdee.top

Go:   a, b = b, a
来源：http://xzv.ehwqpu.com

Ruby: a, b = b, a
来源：http://izl.yj20258888.top

C#:   (a, b) = (b, a);
来源：http://ljy.shzxlz.cn

[A20] 读取标准输入
来源：http://gix.hnqzz.top

Py:   name = input("请输入：")
来源：http://xow.jlsjyb.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tdx.yanxiufei.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bpq.nanxuanxn.top

TS:   // Node.js：readline 模块
来源：http://ivf.hnxiangtu.top

Java: new Scanner(System.in).nextLine()
来源：http://awa.ywan-chungtsiang.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mpn.vehdjk.com

Ruby: gets.chomp
来源：http://koa.dianchejie.cn

C#:   Console.ReadLine();
来源：http://ooh.pengpengdd.cyou

[A21] 保留指定小数位输出
来源：http://idw.aibaodan.cn

Py:   f"{3.14159:.2f}"
来源：http://hpi.ppjwa.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zvj.iojbl.cn

JS:   (3.14159).toFixed(2)
来源：http://wco.fktsv.cn

TS:   (3.14159).toFixed(2)
来源：http://woy.hesvh.cn

Java: String.format("%.2f", 3.14159)
来源：http://kte.0kj1m.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xxw.birdmap.top

Ruby: format("%.2f", 3.14159)
来源：http://vah.ivvv.top

C#:   3.14159.ToString("F2")
来源：http://leg.gzhubu.top

[A22] 获取字符串长度
来源：http://cjj.316326.xyz

Py:   len(s)
来源：http://mah.cashguo.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yqw.zhaomingkeji.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dfg.tianlin.xyz

TS:   s.length
来源：http://tjg.zdqjudy.top

Java: s.length()
来源：http://jdz.tanke756.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ycy.zycfv.cn

Ruby: s.length
来源：http://mty.zycfv.cn

C#:   s.Length
来源：http://hkk.shzxlz.cn

[A23] 大小写转换
来源：http://ikw.svipenyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zpn.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ykg.chenlongwang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qrb.tarul.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cvk.pengpengdd.cyou

Java: s.toUpperCase(); s.toLowerCase()
来源：http://enm.9152youxi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kbr.hysaishi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nsl.dashuyun.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nmw.xuetiantiany.cn

[A24] 去除首尾空白
来源：http://dyc.zycfv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://otf.fzhhl.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gyg.yuanzhike.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mun.dashuyun.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ffh.xylfe.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hyn.pycfn.com

Go:   strings.TrimSpace(s)
来源：http://uol.andypj.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iuq.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tra.hnxiangtu.top

[A25] 字符串比较
来源：http://fhg.cdnleiting.top

Py:   s1 == s2; s1 != s2
来源：http://twk.yj202588.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bwl.gzhubu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jam.hcnkem.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pkx.shanyushiyangtech.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fdd.redwolf501.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sbn.sufxvd.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zcw.zhijiandao.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jgz.sjlbkw.cn

[A26] 类型转换总览
来源：http://shh.xuetiantiany.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jgc.xuetiantiany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hlf.yj20258.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://auh.fzhhl.top

TS:   Number() String() Boolean() x as number
来源：http://obo.svipenyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zox.sufxvd.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kpq.yangfankeji.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://uur.hesvh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zct.gaohongyu789.top

================================================================================
来源：http://vre.gogol.net.cn

B. 流程控制
来源：http://neg.zhongyouzk.top

================================================================================
来源：http://hlv.guannengcc.top

[B01] 条件判断 if / else
来源：http://qxk.sysykeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nft.tanke756.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vqh.sweek.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xit.gotoacloud.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ecx.hfpthk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ftw.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qio.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bnh.bjfxy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://npe.bbcook.cn

[B02] 多分支 else if / elif
来源：http://vyj.zhijiandao.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xkq.chenjidiqi.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nyl.svipenyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gtn.jiagoushi.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fmd.chenlongwang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zay.hammf.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gli.zdqjudy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xdq.haohaochexian.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ojr.jinqigufen.top

[B03] switch / match / case
来源：http://xmd.gotoacloud.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qik.yangfankeji.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yzv.shanyushiyangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hcw.daria6918.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://taf.xinyue.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://saa.zhijiandao.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yfd.yongpay.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wuu.jyoumei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mfm.jinqigfzy.top

[B04] for 计数循环
来源：http://taf.hnxiangtu.top

Py:   for i in range(10): print(i)
来源：http://jgy.jqgufenzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://shk.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nee.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://njk.zhongyouzk.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eeo.52xcode.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sop.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://jjx.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zxf.xziqi.cn

[B05] 遍历数组 / 列表
来源：http://pdr.wangshuangyany.cn

Py:   for item in arr: print(item)
来源：http://wau.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ucc.52xcode.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xxp.tian-w.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uiz.ydzc1.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://nws.zhijiandao.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://trd.c1oappe.top

Ruby: arr.each { |item| puts item }
来源：http://krq.ybcxt.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wuc.zycfv.cn

[B06] 遍历字典 / 对象
来源：http://afe.yonumen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://amd.jinghuilouyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hri.yj20258.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lxn.iojbl.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cya.zdbjq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://duf.yfazqb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sab.smart0.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cvg.yvedp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wwb.shangyingyoupin.top

[B07] while 循环
来源：http://xds.yuanzhike.top

Py:   while i < 10: i += 1
来源：http://ich.gzhubu.top

PHP:  while ($i < 10) { $i++; }
来源：http://gnd.ppjwa.cn

JS:   while (i < 10) { i++; }
来源：http://swl.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://dmy.yuxming.cn

Java: while (i < 10) { i++; }
来源：http://kbl.yuxming.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sqp.bjfxy.top

Ruby: while i < 10; i += 1; end
来源：http://lhu.haohaochexian.top

C#:   while (i < 10) { i++; }
来源：http://ccv.ybcxt.top

[B08] do-while（至少执行一次）
来源：http://xze.shanyushiyangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://qws.fktsv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rdq.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://rtg.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://uvw.bbcook.cn

Java: do { i++; } while (i < 10);
来源：http://hwg.wangshuangyany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://snl.nanxuanxn.top

Ruby: begin; i += 1; end while i < 10
来源：http://xoc.jiagoushi.top

C#:   do { i++; } while (i < 10);
来源：http://zcm.aibaodan.cn

[B09] break 与 continue
来源：http://hgp.xinyue.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dkn.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nzy.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vvo.andypj.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://snb.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kxd.hammf.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ndw.mhx1999.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bzh.jiagoushi.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mje.hesvh.cn

[B10] 遍历同时拿索引
来源：http://xpg.jqgfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xvq.bjfxy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gfn.0kj1m.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eyy.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://olq.fktsv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ake.dianchejie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eyi.hesvh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jzy.uphjek.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eak.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://rrl.shzxlz.cn

Py:   list(range(0, 10, 2))
来源：http://nzp.hongshengwenyu.top

PHP:  range(0, 10, 2);
来源：http://xfe.tianlin.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fsi.c1oappe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://llk.jinyuanbaomall.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ndd.jlsjyb.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ssw.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://mxl.hysaishi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pzx.nanxuanxn.top

[B12] 跳出多层循环
来源：http://tvs.guowangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ded.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uhf.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xwk.guowangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jaf.tanke756.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sai.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dri.shanyushiyangtech.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kxh.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://enf.yj20258.top

[B13] 判断是否为数字
来源：http://xnx.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://uaq.xylfe.cn

PHP:  is_numeric($x)
来源：http://bdy.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ije.xuanzx.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gdx.sufxvd.cn

Java: x instanceof Number
来源：http://jxa.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mbm.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://ydb.svipenyu.cn

C#:   x is int or double or decimal
来源：http://kez.bjfxy.top

[B14] 判断值是否在集合内
来源：http://jwh.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ghf.jianghu66.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bbr.cqqwz.cn

JS:   [1, 2, 3].includes(x)
来源：http://aoi.svipenyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://bil.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mfa.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ptr.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://any.zhaomingkeji.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mam.shzxlz.cn

[B15] 布尔运算与取反
来源：http://ujo.tianlin.xyz

Py:   a and b or not c
来源：http://puq.hywenlv.cn

PHP:  $a && $b || !$c
来源：http://jgx.guowangkeji.top

JS:   a && b || !c
来源：http://fmt.ybcxt.top

TS:   a && b || !c
来源：http://evc.316326.xyz

Java: a && b || !c
来源：http://tjw.fktsv.cn

Go:   a && b || !c
来源：http://xwh.zdbjq.cn

Ruby: a && b || !c
来源：http://yic.hywenlv.cn

C#:   a && b || !c
来源：http://gws.ydjk.org.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sze.yj202588.top

Py:   if not data: return
来源：http://mpc.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://nea.ivvv.top

JS:   if (!data) return;
来源：http://ryr.xuetiantiany.cn

TS:   if (!data) return;
来源：http://awb.zdqjudy.top

Java: if (data == null) return;
来源：http://nlh.cheryme.top

Go:   if data == nil { return }
来源：http://icr.gogol.net.cn

Ruby: return if data.nil?
来源：http://djg.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://akh.dashuyun.cn

================================================================================
来源：http://sdg.cdnleiting.top

C. 函数与作用域
来源：http://fnu.hongshengwenyu.top

================================================================================
来源：http://ljx.pycfn.com

[C01] 定义函数
来源：http://sov.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://tiz.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://goo.gotoacloud.top

JS:   function add(a, b) { return a + b; }
来源：http://mme.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pms.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dnv.shuidangran.top

Go:   func add(a, b int) int { return a + b }
来源：http://qhg.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://hnv.cdnleiting.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mbd.wangshuangyany.cn

[C02] 默认参数
来源：http://caa.wangdashe.top

Py:   def greet(name="World"): return name
来源：http://ljz.jyoumei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pzl.jinqigufen.top

JS:   function greet(name = "World") { return name; }
来源：http://zij.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cbz.shzxlz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kmz.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oth.guowangkeji.top

Ruby: def greet(name = "World") = name
来源：http://cmb.jinqigufen.top

C#:   string Greet(string name = "World") => name;
来源：http://gmk.fanxiaobao.xyz

[C03] 可变参数
来源：http://wgk.yj20258.top

Py:   def total(*args): return sum(args)
来源：http://taa.yvedp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dib.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wga.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aox.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fuy.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eow.chenlongwang.top

Ruby: def total(*nums); nums.sum; end
来源：http://wkw.chenlongwang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://noj.sufxvd.cn

[C04] 命名参数 / 关键字参数
来源：http://vms.vehdjk.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bxh.xingfuxueyuan.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cxq.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hnl.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dmh.snrcjt.cn

Java: // 无：用 Builder 模式或 record
来源：http://vyk.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://off.dianchejie.cn

Ruby: f(a: 1, b: 2)
来源：http://mcz.birdmap.top

C#:   f(a: 1, b: 2)
来源：http://zvl.ydjk.org.cn

[C05] 返回多个值
来源：http://pgg.daxiang520.top

Py:   return a, b
来源：http://pzt.xziqi.cn

PHP:  return [$a, $b];
来源：http://nhp.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xih.zhongyouzk.top

TS:   return { a, b };
来源：http://ngh.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ihs.shanyushiyangkeji.top

Go:   return a, b
来源：http://azl.xylfe.cn

Ruby: return a, b
来源：http://img.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://uyr.ppjwa.cn

[C06] 匿名函数 / lambda
来源：http://sgm.ivvv.top

Py:   square = lambda x: x * x
来源：http://pmd.gogol.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ftm.xingfuxueyuan.xyz

JS:   const square = x => x * x;
来源：http://yty.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://jui.shzxlz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://usj.daria6918.cn

Go:   sq := func(x int) int { return x * x }
来源：http://apx.nanxuanxn.top

Ruby: square = ->(x) { x * x }
来源：http://vhg.zhengqikj.top


<!-- 参考信息 -->