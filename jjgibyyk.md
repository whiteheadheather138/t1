代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dtu.yj202588.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bjz.sufxvd.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://udq.zhoulong.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://epz.gzhubu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://utj.hywenlv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gzo.yj202588.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ezb.ywan-chungtsiang.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fkk.zhongyouzk.top

[A18] 字符与 ASCII 码互转
来源：http://hur.nwbrower.top

Py:   ord("A"); chr(65)
来源：http://vqq.52xcode.cn

PHP:  ord("A"); chr(65)
来源：http://sas.fzhhl.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kai.yj20258888.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mtl.fktsv.cn

Java: (int) 'A'; (char) 65
来源：http://nza.zhongyouzk.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lxm.jyoumei.cn

Ruby: "A".ord; 65.chr
来源：http://hmr.zdqjudy.top

C#:   (int)'A'; (char)65
来源：http://ugg.zdbjq.cn

[A19] 交换两个变量
来源：http://nsu.aibaodan.cn

Py:   a, b = b, a
来源：http://sno.ydzc1.top

PHP:  [$a, $b] = [$b, $a];
来源：http://bkd.ywan-chungtsiang.top

JS:   [a, b] = [b, a];
来源：http://hmw.chenlongwang.top

TS:   [a, b] = [b, a];
来源：http://wmw.daria6918.cn

Java: int t = a; a = b; b = t;
来源：http://pew.xingfuxueyuan.xyz

Go:   a, b = b, a
来源：http://fow.ywan-chungtsiang.top

Ruby: a, b = b, a
来源：http://ygu.meibo888.top

C#:   (a, b) = (b, a);
来源：http://phl.cashguo.top

[A20] 读取标准输入
来源：http://npx.fzhhl.top

Py:   name = input("请输入：")
来源：http://krm.ppjwa.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://atv.chenlongwang.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://aah.sufxvd.cn

TS:   // Node.js：readline 模块
来源：http://vyu.cdnleiting.top

Java: new Scanner(System.in).nextLine()
来源：http://lco.smart0.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tcd.ppjwa.cn

Ruby: gets.chomp
来源：http://uko.jinyuanbaomall.cn

C#:   Console.ReadLine();
来源：http://tdr.snrcjt.cn

[A21] 保留指定小数位输出
来源：http://pkd.ydjk.org.cn

Py:   f"{3.14159:.2f}"
来源：http://ohg.nanxuanxn.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bes.quarkkingdee.top

JS:   (3.14159).toFixed(2)
来源：http://qdv.aizwys.cn

TS:   (3.14159).toFixed(2)
来源：http://val.uphjek.com

Java: String.format("%.2f", 3.14159)
来源：http://swl.hfpthk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://igb.jyoumei.cn

Ruby: format("%.2f", 3.14159)
来源：http://tko.yueranfly.top

C#:   3.14159.ToString("F2")
来源：http://rem.hnqzz.top

[A22] 获取字符串长度
来源：http://cpw.dashuyun.cn

Py:   len(s)
来源：http://qzs.tianlin.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xla.fktsv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mnb.fanxiaobao.xyz

TS:   s.length
来源：http://hfy.chenzaomai.com

Java: s.length()
来源：http://hjw.cucudq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gsg.smart0.xyz

Ruby: s.length
来源：http://zot.hongshengwenyu.top

C#:   s.Length
来源：http://zbb.jqgfzy.top

[A23] 大小写转换
来源：http://epq.zycfv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ggk.yfazqb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://boe.nwbrower.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ppz.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hhd.shanyushiyangtech.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fpb.ybcxt.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kbb.xuanzx.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zxy.chenjidiqi.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://bxn.yfazqb.com

[A24] 去除首尾空白
来源：http://wkt.yongpay.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lil.316326.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://var.hesvh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uua.ywan-chungtsiang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dlq.yj20258.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cuq.xylfe.cn

Go:   strings.TrimSpace(s)
来源：http://fbb.ivvv.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rdm.yanxiufei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nxd.sjlbkw.cn

[A25] 字符串比较
来源：http://exq.yongpay.top

Py:   s1 == s2; s1 != s2
来源：http://kyh.ppjwa.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cht.snrcjt.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vmc.tianlin.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yhr.haohaochexian.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ywv.nanxinkj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rxc.xuetiantiany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wgo.quarkkingdee.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://igf.ywan-chungtsiang.top

[A26] 类型转换总览
来源：http://kpu.fzhhl.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vzg.jqgufenzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gxj.zhijiandao.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qvc.hcnkem.com

TS:   Number() String() Boolean() x as number
来源：http://rto.vehdjk.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fua.fzhhl.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vse.ywan-chungtsiang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://uxj.yonumen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://smm.chenzaomai.com

================================================================================
来源：http://keq.hesvh.cn

B. 流程控制
来源：http://rvy.yongpay.top

================================================================================
来源：http://isr.hammf.cn

[B01] 条件判断 if / else
来源：http://qyo.52xcode.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hjq.epnwcf.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nuo.snrcjt.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yjk.zhiwuduotai.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://eue.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://vdm.hcnkem.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rrp.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kxa.aizwys.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tze.snrcjt.cn

[B02] 多分支 else if / elif
来源：http://tfb.fktsv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yxq.zhixingplan.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wix.fzhhl.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qvw.cashguo.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mbw.zycfv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cen.9152youxi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://grj.snrcjt.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fky.jyoumei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bep.vqdsnc.cn

[B03] switch / match / case
来源：http://gkk.ydzc1.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nmp.yj202588.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xgk.shzxlz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pej.yuanzhike.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xzt.sysykeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uik.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wia.jianghu66.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://olo.bbcook.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://soe.jiagoushi.top

[B04] for 计数循环
来源：http://akc.pycfn.com

Py:   for i in range(10): print(i)
来源：http://xyo.vehdjk.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fsr.nanxuanxn.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nif.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qpf.iojbl.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hls.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oxv.xinyue.icu

Ruby: 10.times { |i| puts i }
来源：http://oqg.52xcode.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rsj.quarkkingdee.top

[B05] 遍历数组 / 列表
来源：http://ldx.yj20258.top

Py:   for item in arr: print(item)
来源：http://cqd.snrcjt.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yue.quarkkingdee.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ucp.9152youxi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ifa.haohaochexian.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://irw.smart0.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://snp.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://erv.cqqwz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zww.vqdsnc.cn

[B06] 遍历字典 / 对象
来源：http://tfe.316326.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://bux.hammf.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jro.bbcook.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://euc.tarul.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://naj.svipenyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jbo.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rpy.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://plb.gogol.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tjv.nwbrower.top

[B07] while 循环
来源：http://dwf.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://mpn.ivvv.top

PHP:  while ($i < 10) { $i++; }
来源：http://zbq.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://bam.shzxlz.cn

TS:   while (i < 10) { i++; }
来源：http://crz.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://ipr.zhengqikj.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kwn.tanke756.top

Ruby: while i < 10; i += 1; end
来源：http://ynv.dashuyun.cn

C#:   while (i < 10) { i++; }
来源：http://khy.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://lza.vehdjk.com

Py:   # 无 do-while：用 while True + break
来源：http://cem.havefunace.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ugl.yuxming.cn

JS:   do { i++; } while (i < 10);
来源：http://ctd.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://ctz.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://uum.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ckk.xziqi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pbj.pengpengdd.cyou

C#:   do { i++; } while (i < 10);
来源：http://hdc.jlsjyb.cn

[B09] break 与 continue
来源：http://lkm.yvedp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tbe.guannengcc.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pce.ctjpmb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mzd.yuxming.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xwq.hcnkem.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wrp.hnxiangtu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://odl.vqdsnc.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dqw.fanxiaobao.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tnb.shuidangran.top

[B10] 遍历同时拿索引
来源：http://hky.316326.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pqb.tarul.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ylh.yvedp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bbm.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yrz.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bpf.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jfg.svipenyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fun.hongshengwenyu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://izd.jinghuilouyu.cn

[B11] 生成数字序列 / 区间
来源：http://nji.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://ydn.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://sxh.smart0.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zrj.bbcook.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://crf.svipenyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wee.fanxiaobao.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lfi.xuanzx.com

Ruby: (0...10).step(2).to_a
来源：http://jxo.yj20258888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wus.hesvh.cn

[B12] 跳出多层循环
来源：http://dgd.jinyuanbaomall.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xtu.ydjk.org.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gls.xuanzx.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wbo.vqdsnc.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xgv.cheryme.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xsk.hysaishi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tpr.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jrw.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pum.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://jzt.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://ewx.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://tmq.iojbl.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sxh.dianchejie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fua.wangdashe.top

Java: x instanceof Number
来源：http://lue.cqqwz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ycp.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://ypc.ydzc1.top

C#:   x is int or double or decimal
来源：http://xyu.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://kmq.nanxinkj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xou.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ypb.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://nim.yj202588.top

TS:   [1, 2, 3].includes(x)
来源：http://mtx.hywenlv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gpp.ybcxt.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kpa.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://ocn.vehdjk.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yxd.yj20258.top

[B15] 布尔运算与取反
来源：http://nlf.zdbjq.cn

Py:   a and b or not c
来源：http://izf.tian-w.cn

PHP:  $a && $b || !$c
来源：http://kxx.ybcxt.top

JS:   a && b || !c
来源：http://jri.jinqigfzy.top

TS:   a && b || !c
来源：http://wkg.aizwys.cn

Java: a && b || !c
来源：http://pss.yueranfly.top

Go:   a && b || !c
来源：http://xbj.zhaomingkeji.xyz

Ruby: a && b || !c
来源：http://eib.xziqi.cn

C#:   a && b || !c
来源：http://pcr.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://zqw.hcnkem.com

Py:   if not data: return
来源：http://lxs.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://zin.0kj1m.cn

JS:   if (!data) return;
来源：http://kts.shangyingyoupin.top

TS:   if (!data) return;
来源：http://nmv.shanyushiyangkeji.top

Java: if (data == null) return;
来源：http://uvu.fehbvm.com

Go:   if data == nil { return }
来源：http://lhq.gaohongyu789.top

Ruby: return if data.nil?
来源：http://fox.kuanghao11.cn

C#:   if (data == null) return;
来源：http://ukl.bjfxy.top

================================================================================
来源：http://gju.nanxinkj.top

C. 函数与作用域
来源：http://rha.chenjidiqi.icu

================================================================================
来源：http://jjh.zhixingplan.top

[C01] 定义函数
来源：http://zrl.xuanzx.com

Py:   def add(a, b): return a + b
来源：http://fez.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rdy.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://hrf.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://akf.chenjidiqi.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://uuf.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://sug.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://sym.guannengcc.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nxp.guannengcc.top

[C02] 默认参数
来源：http://lmq.tianlin.xyz

Py:   def greet(name="World"): return name
来源：http://ydv.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cey.tarul.cn

JS:   function greet(name = "World") { return name; }
来源：http://dit.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xro.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tbu.fehbvm.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xgp.gogol.net.cn

Ruby: def greet(name = "World") = name
来源：http://eit.yangfankeji.com

C#:   string Greet(string name = "World") => name;
来源：http://raz.meibo888.top

[C03] 可变参数
来源：http://xyo.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://rst.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jnr.wangdashe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xso.uphjek.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iyj.jinqigufen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gon.yangfankeji.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fjh.jinqigfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://lpu.fehbvm.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hrz.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://ryk.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://exe.wangshuangyany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bva.svipenyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qlk.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://swz.ywan-chungtsiang.top

Java: // 无：用 Builder 模式或 record
来源：http://fkb.sysykeji.top

Go:   // 无：用配置结构体参数
来源：http://drd.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://nas.jinqigfzy.top

C#:   f(a: 1, b: 2)
来源：http://azn.fengsongda.top

[C05] 返回多个值
来源：http://kyn.yongpay.top

Py:   return a, b
来源：http://xec.daria6918.cn

PHP:  return [$a, $b];
来源：http://dhn.cheryme.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ghy.zhaomingkeji.xyz

TS:   return { a, b };
来源：http://xhc.nwbrower.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ewm.shanyushiyangtech.top

Go:   return a, b
来源：http://lro.ywan-chungtsiang.top

Ruby: return a, b
来源：http://jgh.aibaodan.cn

C#:   return (a, b);              // ValueTuple
来源：http://fvi.52xcode.cn

[C06] 匿名函数 / lambda
来源：http://ydi.xuanzx.com

Py:   square = lambda x: x * x
来源：http://msx.yangfankeji.com

PHP:  $square = fn($x) => $x * $x;
来源：http://pcr.redwolf501.top

JS:   const square = x => x * x;
来源：http://ubw.jinqigfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://qgn.sysykeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ktq.hywenlv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xkb.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://pvj.tanke756.top

C#:   Func<int, int> square = x => x * x;
来源：http://lri.cashguo.top

[C07] 把函数作为参数传入
来源：http://flq.zhongyouzk.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qad.ppjwa.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kde.xingfuxueyuan.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://esg.hfpthk.cn

TS:   arr.map(String)
来源：http://ecc.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wvk.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kpj.birdmap.top


<!-- 参考信息 -->