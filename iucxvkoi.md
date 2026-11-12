代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://chg.birdmap.top

[A15] 空值判断与默认值
来源：http://axs.sufxvd.cn

Py:   value = data or "默认值"
来源：http://tmt.fktsv.cn

PHP:  $value = $data ?? "默认值";
来源：http://iol.shzxlz.cn

JS:   const value = data ?? "默认值";
来源：http://xdw.aibaodan.cn

TS:   const value = data ?? "默认值";
来源：http://uir.sxryk.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qmz.52xcode.cn

Go:   if data == "" { data = "默认值" }
来源：http://izc.hywenlv.cn

Ruby: value = data || "默认值"
来源：http://oww.pengpengdd.cyou

C#:   var value = data ?? "默认值";
来源：http://idz.smart0.xyz

[A16] 真假值判断规则
来源：http://ogc.jinqigfzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mmz.chenzaomai.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ubx.iojbl.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uiv.xziqi.cn

TS:   if (!x) {}
来源：http://qzo.kuanghao11.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hkz.snrcjt.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jpj.fktsv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dln.redwolf501.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zqq.fzhhl.top

[A17] 位运算
来源：http://mek.sufxvd.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gnp.sjlbkw.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://duq.nanxinkj.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://drz.tian-w.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://umv.shuidangran.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hmm.zycfv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kii.nwbrower.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sgs.c1oappe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hss.havefunace.top

[A18] 字符与 ASCII 码互转
来源：http://ehf.daxiang520.top

Py:   ord("A"); chr(65)
来源：http://upl.aibaodan.cn

PHP:  ord("A"); chr(65)
来源：http://uuj.jinqigfzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uqm.yj20258.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tee.jinyuanbaomall.cn

Java: (int) 'A'; (char) 65
来源：http://ffj.xingfuxueyuan.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sjx.ydjk.org.cn

Ruby: "A".ord; 65.chr
来源：http://hgv.fzhhl.top

C#:   (int)'A'; (char)65
来源：http://ycr.yangfankeji.com

[A19] 交换两个变量
来源：http://wgs.cheryme.top

Py:   a, b = b, a
来源：http://qte.chenlongwang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://shi.vqdsnc.cn

JS:   [a, b] = [b, a];
来源：http://bjb.birdmap.top

TS:   [a, b] = [b, a];
来源：http://kgo.chenjidiqi.icu

Java: int t = a; a = b; b = t;
来源：http://icx.ehwqpu.com

Go:   a, b = b, a
来源：http://hko.quarkkingdee.top

Ruby: a, b = b, a
来源：http://ycz.guannengcc.top

C#:   (a, b) = (b, a);
来源：http://npz.fktsv.cn

[A20] 读取标准输入
来源：http://ljr.zhoulong.xyz

Py:   name = input("请输入：")
来源：http://iwl.9152youxi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dlq.zhixingplan.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://exc.gogol.net.cn

TS:   // Node.js：readline 模块
来源：http://xzk.jinyuanbaomall.cn

Java: new Scanner(System.in).nextLine()
来源：http://opc.hnxiangtu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zru.mhx1999.top

Ruby: gets.chomp
来源：http://xix.jiagoushi.top

C#:   Console.ReadLine();
来源：http://ptn.jinghuilouyu.cn

[A21] 保留指定小数位输出
来源：http://yhk.cucudq.cn

Py:   f"{3.14159:.2f}"
来源：http://qes.9152youxi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ini.ywan-chungtsiang.top

JS:   (3.14159).toFixed(2)
来源：http://woy.cqqwz.cn

TS:   (3.14159).toFixed(2)
来源：http://zdl.havefunace.top

Java: String.format("%.2f", 3.14159)
来源：http://yiu.gzhubu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oom.ivvv.top

Ruby: format("%.2f", 3.14159)
来源：http://vtg.ydjk.org.cn

C#:   3.14159.ToString("F2")
来源：http://yqn.sjlbkw.cn

[A22] 获取字符串长度
来源：http://hwy.zhaomingkeji.xyz

Py:   len(s)
来源：http://dck.bbcook.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pts.shanyushiyangtech.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fto.dashuyun.cn

TS:   s.length
来源：http://cef.zycfv.cn

Java: s.length()
来源：http://wlz.gogol.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mff.pengpengdd.cyou

Ruby: s.length
来源：http://lag.zdbjq.cn

C#:   s.Length
来源：http://vbd.meibo888.top

[A23] 大小写转换
来源：http://eje.jlsjyb.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wur.yj20258888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ymp.shanyushiyangkeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://urg.cdnleiting.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://aqw.xylfe.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nek.xuetiantiany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zsy.9152youxi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xft.zdbjq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fug.feifeiyinyue.top

[A24] 去除首尾空白
来源：http://ghk.yanxiufei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ezw.fzhhl.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qvb.fanxiaobao.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nwa.guowangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://epp.zhengqikj.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://myc.zhengqikj.top

Go:   strings.TrimSpace(s)
来源：http://yjq.shuidangran.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://toy.ehwqpu.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wvq.gzhubu.top

[A25] 字符串比较
来源：http://ttf.hongshengwenyu.top

Py:   s1 == s2; s1 != s2
来源：http://yrd.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jtw.jinqigfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://odb.yj20258888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rtl.nanxinkj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oxn.jianghu66.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jgc.redwolf501.top

Ruby: s1 == s2; s1 <=> s2
来源：http://znt.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gof.shzxlz.cn

[A26] 类型转换总览
来源：http://vek.hcnkem.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bnw.guannengcc.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bmd.hnxiangtu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://koq.shanyushiyangtech.top

TS:   Number() String() Boolean() x as number
来源：http://bdr.xuanzx.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vbr.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zgr.cashguo.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qpr.dianchejie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yut.yj20258.top

================================================================================
来源：http://xfc.vehdjk.com

B. 流程控制
来源：http://dfn.feifeiyinyue.top

================================================================================
来源：http://lfy.quarkkingdee.top

[B01] 条件判断 if / else
来源：http://qhi.wangdashe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://akk.shanyushiyangtech.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hks.ivvv.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ivf.xziqi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ysv.hfpthk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sem.jlsjyb.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://idi.jiagoushi.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://duw.vehdjk.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://myv.jiagoushi.top

[B02] 多分支 else if / elif
来源：http://gsm.jqgufenzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vft.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lmk.xinyue.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://crx.hesvh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ejj.wangdashe.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oqr.jinyuanbaomall.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ovb.shangyingyoupin.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qjv.smart0.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gnr.cqqwz.cn

[B03] switch / match / case
来源：http://kqo.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mpx.shanyushiyangtech.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nza.yangfankeji.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ibz.shanyushiyangtech.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qwo.uphjek.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ocd.hfpthk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oyp.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://frp.svipenyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zpx.316326.xyz

[B04] for 计数循环
来源：http://rth.hysaishi.cn

Py:   for i in range(10): print(i)
来源：http://jxg.guowangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qlf.dashuyun.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uks.svipenyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ygj.tarul.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oit.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://srg.havefunace.top

Ruby: 10.times { |i| puts i }
来源：http://gvo.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://znm.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://ivx.xinyue.icu

Py:   for item in arr: print(item)
来源：http://uvb.xingfuxueyuan.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zho.andypj.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://lgw.yangfankeji.com

TS:   for (const item of arr) { console.log(item); }
来源：http://huq.daria6918.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hog.nanxuanxn.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xkr.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://yqs.pengpengdd.cyou

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pya.smart0.xyz

[B06] 遍历字典 / 对象
来源：http://mzr.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kxc.zycfv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cuv.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yzu.chenzaomai.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xeo.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dgq.xuetiantiany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://htl.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ncv.vehdjk.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nnn.xuetiantiany.cn

[B07] while 循环
来源：http://qls.gzhubu.top

Py:   while i < 10: i += 1
来源：http://lsg.0kj1m.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zyh.epnwcf.com

JS:   while (i < 10) { i++; }
来源：http://mgm.jqgfzy.top

TS:   while (i < 10) { i++; }
来源：http://wda.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://nkz.svipenyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lns.316326.xyz

Ruby: while i < 10; i += 1; end
来源：http://ytb.hysaishi.cn

C#:   while (i < 10) { i++; }
来源：http://lrw.hammf.cn

[B08] do-while（至少执行一次）
来源：http://xqe.yj202588.top

Py:   # 无 do-while：用 while True + break
来源：http://dko.yj20258888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nlu.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://uoy.yvedp.cn

TS:   do { i++; } while (i < 10);
来源：http://wba.gogol.net.cn

Java: do { i++; } while (i < 10);
来源：http://shm.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pzr.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://izm.daxiang520.top

C#:   do { i++; } while (i < 10);
来源：http://sgv.yongpay.top

[B09] break 与 continue
来源：http://rnt.zycfv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dig.yanxiufei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wvk.ctjpmb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rxs.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vfc.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vgs.nanxinkj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rlt.yongpay.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vmm.sweek.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bct.yongpay.top

[B10] 遍历同时拿索引
来源：http://vsw.guannengcc.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jzb.uphjek.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zdu.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://idu.zycfv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ido.zdbjq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xnk.zhijiandao.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://szr.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xpr.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mde.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://ckm.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://bkb.cashguo.top

PHP:  range(0, 10, 2);
来源：http://xtt.shanyushiyangtech.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gik.jqgufenzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lhv.smart0.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hsj.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dvn.iojbl.cn

Ruby: (0...10).step(2).to_a
来源：http://hsk.hfpthk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ofp.havefunace.top

[B12] 跳出多层循环
来源：http://num.ehwqpu.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://rdw.tianlin.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://mjt.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yyu.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dug.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jwl.zhoulong.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dgh.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nup.nanxuanxn.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wyn.wangshuangyany.cn

[B13] 判断是否为数字
来源：http://xla.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://zib.yongpay.top

PHP:  is_numeric($x)
来源：http://alz.bjfxy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ffn.yuxming.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://whd.hcnkem.com

Java: x instanceof Number
来源：http://ggi.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jnr.birdmap.top

Ruby: x.is_a?(Numeric)
来源：http://vss.iojbl.cn

C#:   x is int or double or decimal
来源：http://gha.gzhubu.top

[B14] 判断值是否在集合内
来源：http://yvd.fanxiaobao.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gwn.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://irt.jinyuanbaomall.cn

JS:   [1, 2, 3].includes(x)
来源：http://wce.fehbvm.com

TS:   [1, 2, 3].includes(x)
来源：http://lnr.chenzaomai.com

Java: List.of(1, 2, 3).contains(x)
来源：http://qgc.vqdsnc.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://byo.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://whu.jqgfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sei.aizwys.cn

[B15] 布尔运算与取反
来源：http://slq.52xcode.cn

Py:   a and b or not c
来源：http://yko.zdbjq.cn

PHP:  $a && $b || !$c
来源：http://cxr.gogol.net.cn

JS:   a && b || !c
来源：http://lbx.zhiwuduotai.top

TS:   a && b || !c
来源：http://kcl.guannengcc.top

Java: a && b || !c
来源：http://uqj.hongshengwenyu.top

Go:   a && b || !c
来源：http://fjy.sysykeji.top

Ruby: a && b || !c
来源：http://vai.svipenyu.cn

C#:   a && b || !c
来源：http://psj.cdnleiting.top

[B16] 卫语句：不满足条件提前返回
来源：http://giv.shanyushiyangkeji.top

Py:   if not data: return
来源：http://fin.hcnkem.com

PHP:  if (!$data) { return; }
来源：http://qed.jinqigfzy.top

JS:   if (!data) return;
来源：http://bbt.xylfe.cn

TS:   if (!data) return;
来源：http://ebx.aizwys.cn

Java: if (data == null) return;
来源：http://aeh.aizwys.cn

Go:   if data == nil { return }
来源：http://ipl.kuanghao11.cn

Ruby: return if data.nil?
来源：http://pyy.jyoumei.cn

C#:   if (data == null) return;
来源：http://djl.xinyue.icu

================================================================================
来源：http://lux.sweek.top

C. 函数与作用域
来源：http://qzt.svipenyu.cn

================================================================================
来源：http://wgr.daria6918.cn

[C01] 定义函数
来源：http://bwi.xuetiantiany.cn

Py:   def add(a, b): return a + b
来源：http://qir.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bvf.zdqjudy.top

JS:   function add(a, b) { return a + b; }
来源：http://boy.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hpz.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://usk.gogol.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://luc.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://xfw.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wcp.yj20258.top

[C02] 默认参数
来源：http://fdr.vqdsnc.cn

Py:   def greet(name="World"): return name
来源：http://coy.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://aao.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://jpp.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sry.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qhj.zycfv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bho.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://qbz.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://jre.svipenyu.cn

[C03] 可变参数
来源：http://oqe.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://fnw.xylfe.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qim.jqgfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dgm.yuanzhike.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gdf.cqqwz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fmd.tian-w.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://quh.c1oappe.top

Ruby: def total(*nums); nums.sum; end
来源：http://ldb.xylfe.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tme.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://sny.wangdashe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://waw.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qdf.tarul.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iee.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://deq.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://sja.mhx1999.top

Go:   // 无：用配置结构体参数
来源：http://hkg.cashguo.top

Ruby: f(a: 1, b: 2)
来源：http://wjw.shanyushiyangtech.top

C#:   f(a: 1, b: 2)
来源：http://bsm.chenlongwang.top

[C05] 返回多个值
来源：http://gcp.yonumen.top

Py:   return a, b
来源：http://sfl.fengsongda.top

PHP:  return [$a, $b];
来源：http://dsl.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xoi.shzxlz.cn

TS:   return { a, b };
来源：http://yeu.zhijiandao.cn


<!-- 参考信息 -->