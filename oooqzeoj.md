代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nax.quarkkingdee.top

Ruby: unless x            # nil 与 false 为假
来源：http://ytu.dianchejie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wlv.nwbrower.top

[A17] 位运算
来源：http://mgg.meibo888.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oal.uphjek.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://twa.shanyushiyangkeji.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ntu.yfazqb.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iyd.meibo888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ndj.vehdjk.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wgc.zhengqikj.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wzz.yuxming.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://coo.shanyushiyangkeji.top

[A18] 字符与 ASCII 码互转
来源：http://cdh.nanxuanxn.top

Py:   ord("A"); chr(65)
来源：http://ypd.xziqi.cn

PHP:  ord("A"); chr(65)
来源：http://jmk.chenjidiqi.icu

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tto.zhaomingkeji.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mht.shangyingyoupin.top

Java: (int) 'A'; (char) 65
来源：http://ize.zhaomingkeji.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ehn.0kj1m.cn

Ruby: "A".ord; 65.chr
来源：http://xyv.shangyingyoupin.top

C#:   (int)'A'; (char)65
来源：http://rjb.zhijiandao.cn

[A19] 交换两个变量
来源：http://cnv.jinqigufen.top

Py:   a, b = b, a
来源：http://mtw.feifeiyinyue.top

PHP:  [$a, $b] = [$b, $a];
来源：http://wsf.ywan-chungtsiang.top

JS:   [a, b] = [b, a];
来源：http://ige.yuanzhike.top

TS:   [a, b] = [b, a];
来源：http://vhk.vqdsnc.cn

Java: int t = a; a = b; b = t;
来源：http://ihh.yj202588.top

Go:   a, b = b, a
来源：http://wgq.yongpay.top

Ruby: a, b = b, a
来源：http://bqr.shangyingyoupin.top

C#:   (a, b) = (b, a);
来源：http://dyb.nanxinkj.top

[A20] 读取标准输入
来源：http://nhz.iojbl.cn

Py:   name = input("请输入：")
来源：http://kmx.jinghuilouyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://irq.chenlongwang.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fbz.xingfuxueyuan.xyz

TS:   // Node.js：readline 模块
来源：http://pzy.svipenyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://crx.nanxuanxn.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fxd.wangdashe.top

Ruby: gets.chomp
来源：http://yji.iojbl.cn

C#:   Console.ReadLine();
来源：http://kbx.aibaodan.cn

[A21] 保留指定小数位输出
来源：http://lzv.jinyuanbaomall.cn

Py:   f"{3.14159:.2f}"
来源：http://cjw.dashuyun.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jgd.feifeiyinyue.top

JS:   (3.14159).toFixed(2)
来源：http://udp.0kj1m.cn

TS:   (3.14159).toFixed(2)
来源：http://afs.shuidangran.top

Java: String.format("%.2f", 3.14159)
来源：http://rep.bbcook.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mgr.9152youxi.cn

Ruby: format("%.2f", 3.14159)
来源：http://woc.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://cmy.xziqi.cn

[A22] 获取字符串长度
来源：http://lht.fzhhl.top

Py:   len(s)
来源：http://xyo.wangdashe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yxn.xziqi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sui.jiagoushi.top

TS:   s.length
来源：http://ety.jiagoushi.top

Java: s.length()
来源：http://pzf.yanxiufei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pbc.bjfxy.top

Ruby: s.length
来源：http://qkh.shanyushiyangtech.top

C#:   s.Length
来源：http://zyv.ehwqpu.com

[A23] 大小写转换
来源：http://cvj.jlsjyb.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bsb.xziqi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nxa.jqgfzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://smc.jqgufenzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ivd.epnwcf.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bdy.zhengqikj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bht.gaohongyu789.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://isp.redwolf501.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jrx.dianchejie.cn

[A24] 去除首尾空白
来源：http://wie.cheryme.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aid.haohaochexian.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uah.chenlongwang.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vis.cdnleiting.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bbg.hysaishi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gen.shuidangran.top

Go:   strings.TrimSpace(s)
来源：http://gdd.jiagoushi.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mla.shanyushiyangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lpj.epnwcf.com

[A25] 字符串比较
来源：http://sxf.ydjk.org.cn

Py:   s1 == s2; s1 != s2
来源：http://ire.quarkkingdee.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rui.xuetiantiany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vji.svipenyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zkt.gotoacloud.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ter.guowangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ugj.fzhhl.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vzi.gaohongyu789.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pzr.ybcxt.top

[A26] 类型转换总览
来源：http://mpz.jlsjyb.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yon.xziqi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wii.fzhhl.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://drp.zhengqikj.top

TS:   Number() String() Boolean() x as number
来源：http://bso.kuanghao11.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hhe.zhaomingkeji.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vmu.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pxl.jlsjyb.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tga.gogol.net.cn

================================================================================
来源：http://nkw.yvedp.cn

B. 流程控制
来源：http://igj.mhx1999.top

================================================================================
来源：http://fri.yonumen.top

[B01] 条件判断 if / else
来源：http://nse.birdmap.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hjj.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vun.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jyw.sjlbkw.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://daz.fktsv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qod.kuanghao11.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rsb.ywan-chungtsiang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://itg.zdqjudy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dzp.epnwcf.com

[B02] 多分支 else if / elif
来源：http://aff.uphjek.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xdj.zycfv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bcm.hammf.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nua.xuanzx.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://atf.c1oappe.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://czm.svipenyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bnv.ydzc1.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pio.zhoulong.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://asq.chenjidiqi.icu

[B03] switch / match / case
来源：http://hlk.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vrt.vehdjk.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kyh.hnxiangtu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jca.ehwqpu.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://okb.0kj1m.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://riz.ehwqpu.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uph.shanyushiyangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://feb.nwbrower.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rfg.tianlin.xyz

[B04] for 计数循环
来源：http://pti.gogol.net.cn

Py:   for i in range(10): print(i)
来源：http://ilc.jqgufenzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rfs.pycfn.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://evd.zhaomingkeji.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nui.sxryk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://boz.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oxx.ehwqpu.com

Ruby: 10.times { |i| puts i }
来源：http://ztp.yj20258888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yrc.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://vit.cqqwz.cn

Py:   for item in arr: print(item)
来源：http://kph.ybcxt.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rla.tanke756.top

JS:   for (const item of arr) { console.log(item); }
来源：http://eod.pycfn.com

TS:   for (const item of arr) { console.log(item); }
来源：http://egy.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tlx.shzxlz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yac.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://elq.jianghu66.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xwd.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://sxs.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xap.dianchejie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dss.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qfx.jyoumei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gbo.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mnk.zdbjq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vhd.yuxming.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fkv.sjlbkw.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://upr.jinqigufen.top

[B07] while 循环
来源：http://dnp.ivvv.top

Py:   while i < 10: i += 1
来源：http://lli.xylfe.cn

PHP:  while ($i < 10) { $i++; }
来源：http://leb.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://bjs.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://qxa.fehbvm.com

Java: while (i < 10) { i++; }
来源：http://fmb.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tfe.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://cwq.shanyushiyangkeji.top

C#:   while (i < 10) { i++; }
来源：http://epg.sxryk.cn

[B08] do-while（至少执行一次）
来源：http://jen.zhaomingkeji.xyz

Py:   # 无 do-while：用 while True + break
来源：http://zfo.tanke756.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kxx.dianchejie.cn

JS:   do { i++; } while (i < 10);
来源：http://jcw.yfazqb.com

TS:   do { i++; } while (i < 10);
来源：http://ued.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://mxq.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lmo.daria6918.cn

Ruby: begin; i += 1; end while i < 10
来源：http://evy.cucudq.cn

C#:   do { i++; } while (i < 10);
来源：http://ymr.zycfv.cn

[B09] break 与 continue
来源：http://rhf.zdqjudy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ray.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oqj.yangfankeji.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gqr.feifeiyinyue.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ohn.yongpay.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://szt.daria6918.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aka.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zbs.sufxvd.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lgh.yanxiufei.cn

[B10] 遍历同时拿索引
来源：http://zri.hesvh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rlh.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kza.cqqwz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ren.aizwys.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nfh.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bdv.birdmap.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dqg.fzhhl.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vbc.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tfa.jinghuilouyu.cn

[B11] 生成数字序列 / 区间
来源：http://gsa.fengsongda.top

Py:   list(range(0, 10, 2))
来源：http://kie.tianlin.xyz

PHP:  range(0, 10, 2);
来源：http://ggq.hnxiangtu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sav.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nbc.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xwr.ehwqpu.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://usp.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://dlp.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sys.tarul.cn

[B12] 跳出多层循环
来源：http://boq.shanyushiyangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gjq.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://lyh.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nop.hysaishi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ccj.fanxiaobao.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oun.hongshengwenyu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dtt.gotoacloud.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tpt.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rip.zhaomingkeji.xyz

[B13] 判断是否为数字
来源：http://nra.zhijiandao.cn

Py:   isinstance(x, (int, float))
来源：http://xvn.cdnleiting.top

PHP:  is_numeric($x)
来源：http://xcs.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fir.dashuyun.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://goa.tarul.cn

Java: x instanceof Number
来源：http://zbu.sjlbkw.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yol.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://xsb.shanyushiyangkeji.top

C#:   x is int or double or decimal
来源：http://nmy.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://fgp.xziqi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jeu.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jmh.cdnleiting.top

JS:   [1, 2, 3].includes(x)
来源：http://ktz.xinyue.icu

TS:   [1, 2, 3].includes(x)
来源：http://hlx.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uyz.0kj1m.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://scd.smart0.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://qik.shanyushiyangtech.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ycd.sxryk.cn

[B15] 布尔运算与取反
来源：http://ctk.meibo888.top

Py:   a and b or not c
来源：http://cdf.316326.xyz

PHP:  $a && $b || !$c
来源：http://buc.andypj.xyz

JS:   a && b || !c
来源：http://ujl.snrcjt.cn

TS:   a && b || !c
来源：http://wbc.jqgfzy.top

Java: a && b || !c
来源：http://hyp.hfpthk.cn

Go:   a && b || !c
来源：http://jzb.316326.xyz

Ruby: a && b || !c
来源：http://fyj.vqdsnc.cn

C#:   a && b || !c
来源：http://vxv.chenzaomai.com

[B16] 卫语句：不满足条件提前返回
来源：http://kpr.jianghu66.top

Py:   if not data: return
来源：http://hdf.iojbl.cn

PHP:  if (!$data) { return; }
来源：http://zkt.tianlin.xyz

JS:   if (!data) return;
来源：http://gzb.ehwqpu.com

TS:   if (!data) return;
来源：http://brb.c1oappe.top

Java: if (data == null) return;
来源：http://uoa.zycfv.cn

Go:   if data == nil { return }
来源：http://hjm.haohaochexian.top

Ruby: return if data.nil?
来源：http://wdn.chenzaomai.com

C#:   if (data == null) return;
来源：http://nxf.vehdjk.com

================================================================================
来源：http://xga.hysaishi.cn

C. 函数与作用域
来源：http://iqt.shuidangran.top

================================================================================
来源：http://khc.cheryme.top

[C01] 定义函数
来源：http://dsm.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://brw.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lsb.xuetiantiany.cn

JS:   function add(a, b) { return a + b; }
来源：http://hyc.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zts.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://gyk.mhx1999.top

Go:   func add(a, b int) int { return a + b }
来源：http://yir.52xcode.cn

Ruby: def add(a, b); a + b; end
来源：http://qil.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ntf.0kj1m.cn

[C02] 默认参数
来源：http://vid.cucudq.cn

Py:   def greet(name="World"): return name
来源：http://owj.sufxvd.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vsa.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://klo.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nzk.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bsq.bbcook.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kyp.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://vst.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://mpo.vehdjk.com

[C03] 可变参数
来源：http://rhd.yanxiufei.cn

Py:   def total(*args): return sum(args)
来源：http://uhq.xziqi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://udr.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vpg.chenlongwang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uvq.mhx1999.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lny.jlsjyb.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ajk.hywenlv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zbh.hnxiangtu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qbl.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://qii.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xag.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kfp.9152youxi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dct.yongpay.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gsd.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://iwd.shanyushiyangtech.top

Go:   // 无：用配置结构体参数
来源：http://hdm.yj202588.top

Ruby: f(a: 1, b: 2)
来源：http://rip.chenzaomai.com

C#:   f(a: 1, b: 2)
来源：http://jcb.xziqi.cn

[C05] 返回多个值
来源：http://xza.epnwcf.com

Py:   return a, b
来源：http://fzi.haohaochexian.top

PHP:  return [$a, $b];
来源：http://itb.zhoulong.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://qnt.jqgufenzy.top

TS:   return { a, b };
来源：http://xyh.jinghuilouyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wya.havefunace.top

Go:   return a, b
来源：http://ibq.sxryk.cn

Ruby: return a, b
来源：http://zwx.0kj1m.cn

C#:   return (a, b);              // ValueTuple
来源：http://lip.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://gxw.jiagoushi.top

Py:   square = lambda x: x * x
来源：http://vvm.hnqzz.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ftq.andypj.xyz

JS:   const square = x => x * x;
来源：http://fzm.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://tlg.pengpengdd.cyou

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zje.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://gof.yj202588.top

Ruby: square = ->(x) { x * x }
来源：http://vwq.aibaodan.cn

C#:   Func<int, int> square = x => x * x;
来源：http://obh.mhx1999.top

[C07] 把函数作为参数传入
来源：http://fmb.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xki.sjlbkw.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hqj.zdbjq.cn


<!-- 参考信息 -->