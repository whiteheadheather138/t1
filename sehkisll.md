代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://fwi.0kj1m.cn

Py:   ord("A"); chr(65)
来源：http://gdv.ppjwa.cn

PHP:  ord("A"); chr(65)
来源：http://qfp.cdnleiting.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://osl.cucudq.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lfj.zhongyouzk.top

Java: (int) 'A'; (char) 65
来源：http://npz.hongshengwenyu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gqq.xingfuxueyuan.xyz

Ruby: "A".ord; 65.chr
来源：http://bpc.ppjwa.cn

C#:   (int)'A'; (char)65
来源：http://rre.vehdjk.com

[A19] 交换两个变量
来源：http://mtp.ywan-chungtsiang.top

Py:   a, b = b, a
来源：http://ihd.hfpthk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vhl.shuidangran.top

JS:   [a, b] = [b, a];
来源：http://wkx.gotoacloud.top

TS:   [a, b] = [b, a];
来源：http://yqg.zhaomingkeji.xyz

Java: int t = a; a = b; b = t;
来源：http://tqf.yuanzhike.top

Go:   a, b = b, a
来源：http://fav.birdmap.top

Ruby: a, b = b, a
来源：http://ldr.yvedp.cn

C#:   (a, b) = (b, a);
来源：http://qhc.yangfankeji.com

[A20] 读取标准输入
来源：http://kdy.jiagoushi.top

Py:   name = input("请输入：")
来源：http://yhf.guowangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://gll.kuanghao11.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gwk.yj202588.top

TS:   // Node.js：readline 模块
来源：http://pvp.mhx1999.top

Java: new Scanner(System.in).nextLine()
来源：http://hjx.aizwys.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dpm.sufxvd.cn

Ruby: gets.chomp
来源：http://bmg.gotoacloud.top

C#:   Console.ReadLine();
来源：http://mtw.zdbjq.cn

[A21] 保留指定小数位输出
来源：http://pok.ehwqpu.com

Py:   f"{3.14159:.2f}"
来源：http://mzf.zhiwuduotai.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pca.hywenlv.cn

JS:   (3.14159).toFixed(2)
来源：http://ubh.jiagoushi.top

TS:   (3.14159).toFixed(2)
来源：http://dtv.jlsjyb.cn

Java: String.format("%.2f", 3.14159)
来源：http://zan.svipenyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oxt.cashguo.top

Ruby: format("%.2f", 3.14159)
来源：http://btt.pengpengdd.cyou

C#:   3.14159.ToString("F2")
来源：http://dch.zhaomingkeji.xyz

[A22] 获取字符串长度
来源：http://vol.shanyushiyangtech.top

Py:   len(s)
来源：http://obq.ywan-chungtsiang.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bwk.yvedp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gfq.pycfn.com

TS:   s.length
来源：http://yag.hfpthk.cn

Java: s.length()
来源：http://eof.gogol.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qlu.fengsongda.top

Ruby: s.length
来源：http://kje.chenlongwang.top

C#:   s.Length
来源：http://ybd.hcnkem.com

[A23] 大小写转换
来源：http://bgc.tianlin.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://prr.iojbl.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sie.ppjwa.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rrw.zycfv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gov.cqqwz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mqq.gaohongyu789.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://znb.jinqigfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://upt.mhx1999.top

C#:   s.ToUpper(); s.ToLower()
来源：http://smd.xziqi.cn

[A24] 去除首尾空白
来源：http://ymq.vehdjk.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fzs.feifeiyinyue.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kwi.gzhubu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ssy.c1oappe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://add.jianghu66.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dav.yvedp.cn

Go:   strings.TrimSpace(s)
来源：http://hfs.zycfv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kpd.hongshengwenyu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pwv.jianghu66.top

[A25] 字符串比较
来源：http://wuk.bbcook.cn

Py:   s1 == s2; s1 != s2
来源：http://icc.yueranfly.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ukf.daria6918.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://idp.meibo888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qkd.birdmap.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pxf.meibo888.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kqf.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://wde.jqgufenzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aft.sjlbkw.cn

[A26] 类型转换总览
来源：http://uzu.gzhubu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jmo.gotoacloud.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vgi.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pds.ivvv.top

TS:   Number() String() Boolean() x as number
来源：http://eri.cheryme.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qxl.cashguo.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mlr.hcnkem.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://cye.jinqigfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hoh.ydzc1.top

================================================================================
来源：http://kiz.daria6918.cn

B. 流程控制
来源：http://tzx.tianlin.xyz

================================================================================
来源：http://pse.sxryk.cn

[B01] 条件判断 if / else
来源：http://qvg.ydzc1.top

Py:   result = "正" if x > 0 else "非正"
来源：http://sgf.cucudq.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cdx.jinqigufen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ebn.cheryme.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dow.zycfv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yum.aibaodan.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://waw.kuanghao11.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nqe.feifeiyinyue.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://alz.jlsjyb.cn

[B02] 多分支 else if / elif
来源：http://gjk.yanxiufei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://liw.fehbvm.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sja.hammf.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dgn.9152youxi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nfq.pengpengdd.cyou

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://upx.ivvv.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lbh.jlsjyb.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://khu.meibo888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lua.ywan-chungtsiang.top

[B03] switch / match / case
来源：http://dfm.svipenyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ekc.yj20258.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hta.daria6918.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vqf.guannengcc.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://meo.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://res.fktsv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wqf.yj20258.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://adz.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iem.xinyue.icu

[B04] for 计数循环
来源：http://doo.wangdashe.top

Py:   for i in range(10): print(i)
来源：http://oto.gaohongyu789.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oin.9152youxi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ipc.shangyingyoupin.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vzw.nwbrower.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://siy.zhongyouzk.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ysl.zhengqikj.top

Ruby: 10.times { |i| puts i }
来源：http://kbv.ppjwa.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zyd.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://uko.316326.xyz

Py:   for item in arr: print(item)
来源：http://rfo.yonumen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sme.zhijiandao.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wwr.sjlbkw.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hzi.iojbl.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uen.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nvc.zhixingplan.top

Ruby: arr.each { |item| puts item }
来源：http://dfz.kuanghao11.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://prx.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://buk.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://cdv.bjfxy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nyq.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bwq.0kj1m.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jxe.chenjidiqi.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sqa.yvedp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://upd.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qaz.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kgd.yfazqb.com

[B07] while 循环
来源：http://qtk.wangshuangyany.cn

Py:   while i < 10: i += 1
来源：http://nrr.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://exj.yj20258.top

JS:   while (i < 10) { i++; }
来源：http://bbt.dianchejie.cn

TS:   while (i < 10) { i++; }
来源：http://rza.fehbvm.com

Java: while (i < 10) { i++; }
来源：http://wlv.iojbl.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pwt.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://wlo.hcnkem.com

C#:   while (i < 10) { i++; }
来源：http://ctb.yueranfly.top

[B08] do-while（至少执行一次）
来源：http://qrt.316326.xyz

Py:   # 无 do-while：用 while True + break
来源：http://ffp.mhx1999.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ffe.ctjpmb.com

JS:   do { i++; } while (i < 10);
来源：http://teb.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://fow.nanxinkj.top

Java: do { i++; } while (i < 10);
来源：http://jap.fktsv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yws.yonumen.top

Ruby: begin; i += 1; end while i < 10
来源：http://ltb.nanxinkj.top

C#:   do { i++; } while (i < 10);
来源：http://pqr.snrcjt.cn

[B09] break 与 continue
来源：http://ucj.tianlin.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hhe.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://phy.epnwcf.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://acs.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vbr.epnwcf.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lhj.xuanzx.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://adq.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bjo.chenzaomai.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vip.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://ski.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pkd.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://obj.jqgufenzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://daw.quarkkingdee.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kue.tianlin.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jvs.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fwj.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ihw.zhijiandao.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qrr.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://bnh.nwbrower.top

Py:   list(range(0, 10, 2))
来源：http://vmd.xuanzx.com

PHP:  range(0, 10, 2);
来源：http://ylp.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vwz.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qgi.fehbvm.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wbv.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qdz.uphjek.com

Ruby: (0...10).step(2).to_a
来源：http://xdc.yonumen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dqr.guowangkeji.top

[B12] 跳出多层循环
来源：http://ldj.zdbjq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qte.aizwys.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dxg.nwbrower.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ocz.zhiwuduotai.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dau.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dzz.gaohongyu789.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vnj.0kj1m.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zpb.shangyingyoupin.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zwa.redwolf501.top

[B13] 判断是否为数字
来源：http://hgc.dashuyun.cn

Py:   isinstance(x, (int, float))
来源：http://wno.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://hgr.cdnleiting.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fgp.shangyingyoupin.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dlj.jianghu66.top

Java: x instanceof Number
来源：http://gpt.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zfh.ywan-chungtsiang.top

Ruby: x.is_a?(Numeric)
来源：http://wpf.yanxiufei.cn

C#:   x is int or double or decimal
来源：http://xgh.fengsongda.top

[B14] 判断值是否在集合内
来源：http://uxm.aizwys.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rht.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iqe.shangyingyoupin.top

JS:   [1, 2, 3].includes(x)
来源：http://pti.yj202588.top

TS:   [1, 2, 3].includes(x)
来源：http://fzs.shzxlz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mnn.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://erx.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zrw.jinqigfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bmg.ydjk.org.cn

[B15] 布尔运算与取反
来源：http://ohb.yvedp.cn

Py:   a and b or not c
来源：http://cyf.hcnkem.com

PHP:  $a && $b || !$c
来源：http://omv.vehdjk.com

JS:   a && b || !c
来源：http://qqa.yueranfly.top

TS:   a && b || !c
来源：http://fgb.tanke756.top

Java: a && b || !c
来源：http://sle.jianghu66.top

Go:   a && b || !c
来源：http://zns.fanxiaobao.xyz

Ruby: a && b || !c
来源：http://fce.vehdjk.com

C#:   a && b || !c
来源：http://nxe.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xek.uphjek.com

Py:   if not data: return
来源：http://vad.yvedp.cn

PHP:  if (!$data) { return; }
来源：http://rge.kuanghao11.cn

JS:   if (!data) return;
来源：http://fbm.ivvv.top

TS:   if (!data) return;
来源：http://qmg.daxiang520.top

Java: if (data == null) return;
来源：http://nzc.cdnleiting.top

Go:   if data == nil { return }
来源：http://kmw.jinqigfzy.top

Ruby: return if data.nil?
来源：http://you.yangfankeji.com

C#:   if (data == null) return;
来源：http://rtl.cqqwz.cn

================================================================================
来源：http://pxv.zhongyouzk.top

C. 函数与作用域
来源：http://sru.zdbjq.cn

================================================================================
来源：http://lbx.yj202588.top

[C01] 定义函数
来源：http://fwn.jianghu66.top

Py:   def add(a, b): return a + b
来源：http://wqs.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qhy.ehwqpu.com

JS:   function add(a, b) { return a + b; }
来源：http://kui.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tjs.xuetiantiany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://stm.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://ccj.jinghuilouyu.cn

Ruby: def add(a, b); a + b; end
来源：http://rap.zhiwuduotai.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qhc.hammf.cn

[C02] 默认参数
来源：http://ymc.gaohongyu789.top

Py:   def greet(name="World"): return name
来源：http://wht.guannengcc.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jnq.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://esj.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ewc.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ekr.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sfb.xuetiantiany.cn

Ruby: def greet(name = "World") = name
来源：http://ljo.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://ijc.dianchejie.cn

[C03] 可变参数
来源：http://ftd.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://fwe.yuxming.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://orv.chenlongwang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://njp.iojbl.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://voh.svipenyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fqg.shanyushiyangtech.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hgf.sxryk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mhw.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rom.fengsongda.top

[C04] 命名参数 / 关键字参数
来源：http://lza.hywenlv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://utz.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://opp.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ykg.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dbt.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://jyq.shuidangran.top

Go:   // 无：用配置结构体参数
来源：http://qef.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://czu.yfazqb.com

C#:   f(a: 1, b: 2)
来源：http://yaw.zhongyouzk.top

[C05] 返回多个值
来源：http://qrm.xylfe.cn

Py:   return a, b
来源：http://ntd.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://ipn.hongshengwenyu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mfh.bjfxy.top

TS:   return { a, b };
来源：http://rsg.xuetiantiany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tyw.wangshuangyany.cn

Go:   return a, b
来源：http://olm.gotoacloud.top

Ruby: return a, b
来源：http://izz.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://zgz.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://czn.ywan-chungtsiang.top

Py:   square = lambda x: x * x
来源：http://psv.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://aov.jqgufenzy.top

JS:   const square = x => x * x;
来源：http://vtk.ywan-chungtsiang.top

TS:   const square = (x: number): number => x * x;
来源：http://geq.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yuv.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://puo.ywan-chungtsiang.top

Ruby: square = ->(x) { x * x }
来源：http://hyg.zhengqikj.top

C#:   Func<int, int> square = x => x * x;
来源：http://ndx.meibo888.top

[C07] 把函数作为参数传入
来源：http://jpg.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qvl.guannengcc.top

PHP:  array_map("strtoupper", $arr);
来源：http://dne.chenlongwang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://par.jiagoushi.top

TS:   arr.map(String)
来源：http://xul.bbcook.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wfx.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oom.aizwys.cn

Ruby: arr.map(&:upcase)
来源：http://btp.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kye.zhengqikj.top

[C08] 闭包
来源：http://lft.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ppp.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://owq.xziqi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wem.zdbjq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nia.pycfn.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ykl.gogol.net.cn


<!-- 参考信息 -->