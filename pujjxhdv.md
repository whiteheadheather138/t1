代发 wailian999

Py:   "第一行\n第二行"
来源：http://ldh.nanxinkj.top

PHP:  "第一行\n第二行"
来源：http://nif.ctjpmb.com

JS:   "第一行\n第二行"
来源：http://xvy.vehdjk.com

TS:   "第一行\n第二行"
来源：http://qnn.meibo888.top

Java: "第一行\n第二行"
来源：http://xsr.xingfuxueyuan.xyz

Go:   "第一行\n第二行"
来源：http://kif.zdqjudy.top

Ruby: "第一行\n第二行"
来源：http://mkb.mhx1999.top

C#:   "第一行\n第二行"
来源：http://lfr.sxryk.cn

[A14] 注释写法
来源：http://mbg.hnxiangtu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zhj.jqgfzy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://nak.mhx1999.top

JS:   // 单行；/* 多行 */
来源：http://vld.fanxiaobao.xyz

TS:   // 单行；/* 多行 */
来源：http://nnx.uphjek.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qof.zhaomingkeji.xyz

Go:   // 单行；/* 多行 */
来源：http://nzm.zhongyouzk.top

Ruby: # 单行；=begin 多行 =end
来源：http://mak.wangdashe.top

C#:   // 单行；/* 多行 */
来源：http://exu.dashuyun.cn

[A15] 空值判断与默认值
来源：http://bus.dashuyun.cn

Py:   value = data or "默认值"
来源：http://xmt.yvedp.cn

PHP:  $value = $data ?? "默认值";
来源：http://ozi.andypj.xyz

JS:   const value = data ?? "默认值";
来源：http://cza.hnqzz.top

TS:   const value = data ?? "默认值";
来源：http://zqd.chenjidiqi.icu

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fnx.andypj.xyz

Go:   if data == "" { data = "默认值" }
来源：http://ovj.hysaishi.cn

Ruby: value = data || "默认值"
来源：http://kfo.ctjpmb.com

C#:   var value = data ?? "默认值";
来源：http://eut.jinghuilouyu.cn

[A16] 真假值判断规则
来源：http://ffb.vqdsnc.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fuq.yfazqb.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jfe.guannengcc.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hmr.yuxming.cn

TS:   if (!x) {}
来源：http://ofz.yongpay.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://clp.feifeiyinyue.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sfl.gaohongyu789.top

Ruby: unless x            # nil 与 false 为假
来源：http://mxu.meibo888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bum.yueranfly.top

[A17] 位运算
来源：http://tvg.yuxming.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://avu.xuanzx.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mfz.xylfe.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bdy.zdqjudy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://eiw.gotoacloud.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gch.jinyuanbaomall.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qcw.shuidangran.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ngt.quarkkingdee.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uuo.daria6918.cn

[A18] 字符与 ASCII 码互转
来源：http://kpp.9152youxi.cn

Py:   ord("A"); chr(65)
来源：http://mss.redwolf501.top

PHP:  ord("A"); chr(65)
来源：http://cia.kuanghao11.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mad.hfpthk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zbg.yj202588.top

Java: (int) 'A'; (char) 65
来源：http://uhx.cashguo.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kce.c1oappe.top

Ruby: "A".ord; 65.chr
来源：http://lsl.daria6918.cn

C#:   (int)'A'; (char)65
来源：http://waf.yuanzhike.top

[A19] 交换两个变量
来源：http://ego.redwolf501.top

Py:   a, b = b, a
来源：http://rlw.tanke756.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mtf.haohaochexian.top

JS:   [a, b] = [b, a];
来源：http://ptw.zhiwuduotai.top

TS:   [a, b] = [b, a];
来源：http://mpx.bbcook.cn

Java: int t = a; a = b; b = t;
来源：http://fyk.shuidangran.top

Go:   a, b = b, a
来源：http://flt.cucudq.cn

Ruby: a, b = b, a
来源：http://npw.vehdjk.com

C#:   (a, b) = (b, a);
来源：http://qnt.hammf.cn

[A20] 读取标准输入
来源：http://bxk.hesvh.cn

Py:   name = input("请输入：")
来源：http://zdf.hywenlv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rwp.52xcode.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tvh.jinqigfzy.top

TS:   // Node.js：readline 模块
来源：http://qhc.zhengqikj.top

Java: new Scanner(System.in).nextLine()
来源：http://uzt.pycfn.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xew.zdbjq.cn

Ruby: gets.chomp
来源：http://slv.yfazqb.com

C#:   Console.ReadLine();
来源：http://rbm.fktsv.cn

[A21] 保留指定小数位输出
来源：http://dmf.zhengqikj.top

Py:   f"{3.14159:.2f}"
来源：http://cdi.tarul.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ppk.jiagoushi.top

JS:   (3.14159).toFixed(2)
来源：http://bpi.jqgufenzy.top

TS:   (3.14159).toFixed(2)
来源：http://fpv.sufxvd.cn

Java: String.format("%.2f", 3.14159)
来源：http://xta.gaohongyu789.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://svf.yanxiufei.cn

Ruby: format("%.2f", 3.14159)
来源：http://vyc.shanyushiyangkeji.top

C#:   3.14159.ToString("F2")
来源：http://wha.guannengcc.top

[A22] 获取字符串长度
来源：http://ycg.redwolf501.top

Py:   len(s)
来源：http://heo.jlsjyb.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eqz.c1oappe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yia.sufxvd.cn

TS:   s.length
来源：http://pey.52xcode.cn

Java: s.length()
来源：http://yyn.hfpthk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hio.iojbl.cn

Ruby: s.length
来源：http://dga.uphjek.com

C#:   s.Length
来源：http://btk.hysaishi.cn

[A23] 大小写转换
来源：http://vkp.gaohongyu789.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vty.zhixingplan.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xzp.fzhhl.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://etw.xinyue.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gmg.yuanzhike.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://atu.316326.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://idd.ivvv.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vjs.bbcook.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://onz.aibaodan.cn

[A24] 去除首尾空白
来源：http://gyn.cdnleiting.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jan.ydjk.org.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lrd.xuetiantiany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pne.kuanghao11.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hfe.sjlbkw.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fwq.snrcjt.cn

Go:   strings.TrimSpace(s)
来源：http://drc.pycfn.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zxs.hongshengwenyu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wqg.fanxiaobao.xyz

[A25] 字符串比较
来源：http://fvd.shanyushiyangkeji.top

Py:   s1 == s2; s1 != s2
来源：http://sxv.ehwqpu.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yog.guowangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uxg.vehdjk.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qwc.sxryk.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kun.havefunace.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rrv.smart0.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://hew.vqdsnc.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dgh.yfazqb.com

[A26] 类型转换总览
来源：http://qij.c1oappe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nod.yj20258888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pyc.xinyue.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mhm.hnqzz.top

TS:   Number() String() Boolean() x as number
来源：http://qju.jiagoushi.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ith.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sqi.gotoacloud.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dre.daria6918.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jnw.yfazqb.com

================================================================================
来源：http://pyl.jianghu66.top

B. 流程控制
来源：http://crp.uphjek.com

================================================================================
来源：http://icn.svipenyu.cn

[B01] 条件判断 if / else
来源：http://wuf.tian-w.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://drt.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bij.hysaishi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mjq.chenlongwang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rbp.dashuyun.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ozr.ywan-chungtsiang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ogb.ppjwa.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zuu.feifeiyinyue.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jyh.jinqigfzy.top

[B02] 多分支 else if / elif
来源：http://ydk.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bqs.nwbrower.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ydh.pengpengdd.cyou

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://azx.guannengcc.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sny.epnwcf.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iqj.ydzc1.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yzr.nanxinkj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bho.zycfv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gqp.jqgfzy.top

[B03] switch / match / case
来源：http://hsp.wangshuangyany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hgc.yfazqb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iix.yongpay.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://biv.cqqwz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://duu.wangdashe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mfv.jinyuanbaomall.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hbm.yonumen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rjy.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://itx.nanxuanxn.top

[B04] for 计数循环
来源：http://ezj.vqdsnc.cn

Py:   for i in range(10): print(i)
来源：http://ulm.aibaodan.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://awg.hammf.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cri.ivvv.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sov.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jle.gaohongyu789.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oyw.pengpengdd.cyou

Ruby: 10.times { |i| puts i }
来源：http://guo.cqqwz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://atl.haohaochexian.top

[B05] 遍历数组 / 列表
来源：http://tzi.gzhubu.top

Py:   for item in arr: print(item)
来源：http://duf.xuetiantiany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gas.zhongyouzk.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kxo.mhx1999.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wlv.pengpengdd.cyou

Java: for (var item : arr) { System.out.println(item); }
来源：http://hoh.kuanghao11.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dst.shanyushiyangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://khl.redwolf501.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pzw.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://rwh.cqqwz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nsz.ywan-chungtsiang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gdi.shanyushiyangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jtx.tianlin.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://srv.xingfuxueyuan.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cmu.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rhh.yvedp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bmb.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tvc.wangdashe.top

[B07] while 循环
来源：http://jve.yj202588.top

Py:   while i < 10: i += 1
来源：http://hcg.ehwqpu.com

PHP:  while ($i < 10) { $i++; }
来源：http://lla.zhongyouzk.top

JS:   while (i < 10) { i++; }
来源：http://cop.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://ffz.gaohongyu789.top

Java: while (i < 10) { i++; }
来源：http://wol.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://izy.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://njn.cashguo.top

C#:   while (i < 10) { i++; }
来源：http://tud.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://rix.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://fxz.zhengqikj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gyw.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://tez.hongshengwenyu.top

TS:   do { i++; } while (i < 10);
来源：http://yfk.bbcook.cn

Java: do { i++; } while (i < 10);
来源：http://tfx.zhoulong.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://oac.hywenlv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tsf.jyoumei.cn

C#:   do { i++; } while (i < 10);
来源：http://emj.yangfankeji.com

[B09] break 与 continue
来源：http://kob.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qwb.iojbl.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yaa.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bkq.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://psn.dianchejie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uvh.feifeiyinyue.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vfb.nwbrower.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uvf.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ppi.kuanghao11.cn

[B10] 遍历同时拿索引
来源：http://hae.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yir.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uth.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xas.nanxinkj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hdl.hammf.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jqo.cdnleiting.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gtk.chenlongwang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rmv.fzhhl.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://coj.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://ztr.9152youxi.cn

Py:   list(range(0, 10, 2))
来源：http://yhg.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://hnp.tianlin.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://khn.pycfn.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hmx.shanyushiyangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ygq.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nqx.nwbrower.top

Ruby: (0...10).step(2).to_a
来源：http://erk.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ndw.chenzaomai.com

[B12] 跳出多层循环
来源：http://jnu.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://leq.vehdjk.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://vbk.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://guq.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bxk.ydzc1.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://okh.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gab.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qph.zycfv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pih.nanxuanxn.top

[B13] 判断是否为数字
来源：http://juk.yongpay.top

Py:   isinstance(x, (int, float))
来源：http://fyo.zhengqikj.top

PHP:  is_numeric($x)
来源：http://van.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://prq.cheryme.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mrh.jqgufenzy.top

Java: x instanceof Number
来源：http://sus.wangshuangyany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xam.jqgfzy.top

Ruby: x.is_a?(Numeric)
来源：http://ktm.redwolf501.top

C#:   x is int or double or decimal
来源：http://asa.yueranfly.top

[B14] 判断值是否在集合内
来源：http://oqf.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jrb.c1oappe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://emx.shanyushiyangtech.top

JS:   [1, 2, 3].includes(x)
来源：http://afa.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://kww.ybcxt.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zly.vqdsnc.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oac.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://qvf.andypj.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mdf.haohaochexian.top

[B15] 布尔运算与取反
来源：http://zfb.316326.xyz

Py:   a and b or not c
来源：http://vni.fehbvm.com

PHP:  $a && $b || !$c
来源：http://hzf.xuetiantiany.cn

JS:   a && b || !c
来源：http://qjw.fzhhl.top

TS:   a && b || !c
来源：http://dfy.uphjek.com

Java: a && b || !c
来源：http://ryt.nanxuanxn.top

Go:   a && b || !c
来源：http://qtg.xinyue.icu

Ruby: a && b || !c
来源：http://nwu.meibo888.top

C#:   a && b || !c
来源：http://ytl.xingfuxueyuan.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://tqz.shangyingyoupin.top

Py:   if not data: return
来源：http://lxd.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://rxc.chenlongwang.top

JS:   if (!data) return;
来源：http://kep.yvedp.cn

TS:   if (!data) return;
来源：http://hqx.shanyushiyangtech.top

Java: if (data == null) return;
来源：http://ner.jqgufenzy.top

Go:   if data == nil { return }
来源：http://usj.chenlongwang.top

Ruby: return if data.nil?
来源：http://ogt.yongpay.top

C#:   if (data == null) return;
来源：http://kdi.hongshengwenyu.top

================================================================================
来源：http://apz.zhaomingkeji.xyz

C. 函数与作用域
来源：http://row.fengsongda.top

================================================================================
来源：http://awe.shangyingyoupin.top

[C01] 定义函数
来源：http://ezl.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://muz.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ths.gogol.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://qnx.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pdi.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lqf.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://jvj.smart0.xyz

Ruby: def add(a, b); a + b; end
来源：http://kvi.wangdashe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nrb.yangfankeji.com

[C02] 默认参数
来源：http://lje.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://pxy.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vax.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://ekf.bjfxy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hmi.chenzaomai.com

Java: // 无默认参数：方法重载或 Optional
来源：http://thv.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bky.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://ybx.xylfe.cn

C#:   string Greet(string name = "World") => name;
来源：http://ppp.jianghu66.top

[C03] 可变参数
来源：http://hlj.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://xjo.meibo888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://isn.daxiang520.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tho.c1oappe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qec.9152youxi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qyr.jlsjyb.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gjh.hnxiangtu.top


<!-- 参考信息 -->