代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://iln.hysaishi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://knf.pycfn.com

Go:   // 单行；/* 多行 */
来源：http://edt.dashuyun.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wov.aibaodan.cn

C#:   // 单行；/* 多行 */
来源：http://raw.xuanzx.com

[A15] 空值判断与默认值
来源：http://mvy.sufxvd.cn

Py:   value = data or "默认值"
来源：http://kst.fengsongda.top

PHP:  $value = $data ?? "默认值";
来源：http://tlo.ybcxt.top

JS:   const value = data ?? "默认值";
来源：http://fht.xingfuxueyuan.xyz

TS:   const value = data ?? "默认值";
来源：http://xnx.feifeiyinyue.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zfn.jinyuanbaomall.cn

Go:   if data == "" { data = "默认值" }
来源：http://grk.nanxinkj.top

Ruby: value = data || "默认值"
来源：http://tzn.daria6918.cn

C#:   var value = data ?? "默认值";
来源：http://deu.shanyushiyangtech.top

[A16] 真假值判断规则
来源：http://jcw.vehdjk.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nqa.guannengcc.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wep.meibo888.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nfj.fktsv.cn

TS:   if (!x) {}
来源：http://cmh.zhixingplan.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jeq.jinghuilouyu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://znx.yfazqb.com

Ruby: unless x            # nil 与 false 为假
来源：http://csw.hfpthk.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wdz.ctjpmb.com

[A17] 位运算
来源：http://atn.ppjwa.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zwp.xuanzx.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lsq.yanxiufei.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yxk.tanke756.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rlh.yangfankeji.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bxf.dashuyun.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bph.aizwys.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ice.kuanghao11.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rrj.zhoulong.xyz

[A18] 字符与 ASCII 码互转
来源：http://qau.cdnleiting.top

Py:   ord("A"); chr(65)
来源：http://fmp.gotoacloud.top

PHP:  ord("A"); chr(65)
来源：http://ure.shangyingyoupin.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://odm.jinqigfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kjg.jiagoushi.top

Java: (int) 'A'; (char) 65
来源：http://swl.ehwqpu.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fpg.aizwys.cn

Ruby: "A".ord; 65.chr
来源：http://uwv.iojbl.cn

C#:   (int)'A'; (char)65
来源：http://hky.fehbvm.com

[A19] 交换两个变量
来源：http://qqh.shzxlz.cn

Py:   a, b = b, a
来源：http://ypn.xziqi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gft.316326.xyz

JS:   [a, b] = [b, a];
来源：http://jpz.cucudq.cn

TS:   [a, b] = [b, a];
来源：http://qcq.smart0.xyz

Java: int t = a; a = b; b = t;
来源：http://hxr.ctjpmb.com

Go:   a, b = b, a
来源：http://rap.hnqzz.top

Ruby: a, b = b, a
来源：http://agu.ywan-chungtsiang.top

C#:   (a, b) = (b, a);
来源：http://xkm.zhijiandao.cn

[A20] 读取标准输入
来源：http://aya.xylfe.cn

Py:   name = input("请输入：")
来源：http://jvp.yonumen.top

PHP:  $name = trim(fgets(STDIN));
来源：http://tsk.hnxiangtu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zfo.yueranfly.top

TS:   // Node.js：readline 模块
来源：http://srf.sysykeji.top

Java: new Scanner(System.in).nextLine()
来源：http://ndc.yangfankeji.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xol.cucudq.cn

Ruby: gets.chomp
来源：http://gsq.xingfuxueyuan.xyz

C#:   Console.ReadLine();
来源：http://eeb.pycfn.com

[A21] 保留指定小数位输出
来源：http://eca.ywan-chungtsiang.top

Py:   f"{3.14159:.2f}"
来源：http://weh.shuidangran.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://njl.chenjidiqi.icu

JS:   (3.14159).toFixed(2)
来源：http://oqk.gzhubu.top

TS:   (3.14159).toFixed(2)
来源：http://man.ppjwa.cn

Java: String.format("%.2f", 3.14159)
来源：http://jbu.kuanghao11.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bmx.quarkkingdee.top

Ruby: format("%.2f", 3.14159)
来源：http://uhl.ivvv.top

C#:   3.14159.ToString("F2")
来源：http://wxr.hnqzz.top

[A22] 获取字符串长度
来源：http://fsv.cheryme.top

Py:   len(s)
来源：http://tny.ybcxt.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tzx.daria6918.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://obk.jinqigufen.top

TS:   s.length
来源：http://jxa.sxryk.cn

Java: s.length()
来源：http://fjg.jqgfzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tio.zhijiandao.cn

Ruby: s.length
来源：http://qam.tian-w.cn

C#:   s.Length
来源：http://cjv.gotoacloud.top

[A23] 大小写转换
来源：http://mbc.gaohongyu789.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mhm.fehbvm.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fmz.jqgufenzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://efp.yueranfly.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wzo.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rob.meibo888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cbc.shangyingyoupin.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://krx.jyoumei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qkt.zhaomingkeji.xyz

[A24] 去除首尾空白
来源：http://ehr.chenzaomai.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mrr.smart0.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jkm.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hsz.epnwcf.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rwz.svipenyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gpe.fehbvm.com

Go:   strings.TrimSpace(s)
来源：http://sco.gzhubu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vnj.uphjek.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nse.feifeiyinyue.top

[A25] 字符串比较
来源：http://kzs.tarul.cn

Py:   s1 == s2; s1 != s2
来源：http://wvk.sufxvd.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qvk.cdnleiting.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ayn.sjlbkw.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bch.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mip.zhiwuduotai.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://enr.gogol.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://shv.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cfh.yj202588.top

[A26] 类型转换总览
来源：http://jng.feifeiyinyue.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://njl.cashguo.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hyn.fehbvm.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wvg.andypj.xyz

TS:   Number() String() Boolean() x as number
来源：http://ftr.aizwys.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hze.cdnleiting.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://auu.cucudq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jqa.snrcjt.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mdx.0kj1m.cn

================================================================================
来源：http://qbw.9152youxi.cn

B. 流程控制
来源：http://gzk.zhijiandao.cn

================================================================================
来源：http://ill.sxryk.cn

[B01] 条件判断 if / else
来源：http://clu.guannengcc.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rwz.epnwcf.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yfp.cashguo.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iiz.sxryk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://noq.yanxiufei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jki.gogol.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://law.cqqwz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kup.nwbrower.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iex.pycfn.com

[B02] 多分支 else if / elif
来源：http://ujz.guannengcc.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zkb.wangdashe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ohb.feifeiyinyue.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nby.jianghu66.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nwn.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fba.hesvh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qny.jyoumei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://syl.zhiwuduotai.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hwx.yj20258.top

[B03] switch / match / case
来源：http://lqd.fktsv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qvd.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xjo.snrcjt.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eej.redwolf501.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://geh.ivvv.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rkt.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://klw.ctjpmb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gje.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wlb.xylfe.cn

[B04] for 计数循环
来源：http://hcg.cashguo.top

Py:   for i in range(10): print(i)
来源：http://swh.yangfankeji.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lln.hysaishi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://spf.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iaz.yueranfly.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cmi.jyoumei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pvq.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://nre.52xcode.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dyj.havefunace.top

[B05] 遍历数组 / 列表
来源：http://byp.tarul.cn

Py:   for item in arr: print(item)
来源：http://asp.jianghu66.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kkb.vehdjk.com

JS:   for (const item of arr) { console.log(item); }
来源：http://snp.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tul.xingfuxueyuan.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://uro.cucudq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://orz.xziqi.cn

Ruby: arr.each { |item| puts item }
来源：http://gqa.zhaomingkeji.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mpb.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://fro.hammf.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qpd.yj202588.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uvs.ywan-chungtsiang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jpu.andypj.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vdc.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://akf.52xcode.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://woi.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jap.chenjidiqi.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ijk.chenjidiqi.icu

[B07] while 循环
来源：http://qzk.zhoulong.xyz

Py:   while i < 10: i += 1
来源：http://jfj.yj20258.top

PHP:  while ($i < 10) { $i++; }
来源：http://ier.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://squ.guannengcc.top

TS:   while (i < 10) { i++; }
来源：http://mem.yuanzhike.top

Java: while (i < 10) { i++; }
来源：http://wbd.aibaodan.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vlk.sjlbkw.cn

Ruby: while i < 10; i += 1; end
来源：http://wks.pycfn.com

C#:   while (i < 10) { i++; }
来源：http://scy.haohaochexian.top

[B08] do-while（至少执行一次）
来源：http://vml.yj20258888.top

Py:   # 无 do-while：用 while True + break
来源：http://via.kuanghao11.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://thp.uphjek.com

JS:   do { i++; } while (i < 10);
来源：http://tjm.c1oappe.top

TS:   do { i++; } while (i < 10);
来源：http://omx.zhixingplan.top

Java: do { i++; } while (i < 10);
来源：http://xxb.sweek.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pnl.cqqwz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uin.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://vid.shzxlz.cn

[B09] break 与 continue
来源：http://jlt.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://phj.zhengqikj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nhl.ivvv.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tko.shzxlz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rwx.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://byk.zhijiandao.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uig.dianchejie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kwg.guannengcc.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ymn.zhaomingkeji.xyz

[B10] 遍历同时拿索引
来源：http://syg.cheryme.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uoz.guannengcc.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fbw.aizwys.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fax.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jix.guannengcc.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vxe.jinqigufen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xrb.sjlbkw.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://znr.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kxg.quarkkingdee.top

[B11] 生成数字序列 / 区间
来源：http://fdu.yj202588.top

Py:   list(range(0, 10, 2))
来源：http://onw.havefunace.top

PHP:  range(0, 10, 2);
来源：http://ucu.sweek.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yiq.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rsp.ybcxt.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iaf.redwolf501.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kbe.sweek.top

Ruby: (0...10).step(2).to_a
来源：http://ado.9152youxi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qyc.chenlongwang.top

[B12] 跳出多层循环
来源：http://vfn.daria6918.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dmv.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://exs.guannengcc.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://usw.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hla.shangyingyoupin.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kfq.zhaomingkeji.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://shq.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lak.hysaishi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tdt.yj20258.top

[B13] 判断是否为数字
来源：http://zfj.ppjwa.cn

Py:   isinstance(x, (int, float))
来源：http://aem.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://duc.xuanzx.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fbp.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oap.feifeiyinyue.top

Java: x instanceof Number
来源：http://sag.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ftg.yanxiufei.cn

Ruby: x.is_a?(Numeric)
来源：http://hii.xuetiantiany.cn

C#:   x is int or double or decimal
来源：http://iqs.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://xte.iojbl.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lyi.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wxp.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://vgt.xylfe.cn

TS:   [1, 2, 3].includes(x)
来源：http://nfk.pycfn.com

Java: List.of(1, 2, 3).contains(x)
来源：http://pzr.wangshuangyany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mol.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gte.zycfv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vax.chenlongwang.top

[B15] 布尔运算与取反
来源：http://fih.zhaomingkeji.xyz

Py:   a and b or not c
来源：http://qfm.316326.xyz

PHP:  $a && $b || !$c
来源：http://cbf.smart0.xyz

JS:   a && b || !c
来源：http://dkz.vehdjk.com

TS:   a && b || !c
来源：http://wyh.fehbvm.com

Java: a && b || !c
来源：http://fwl.aizwys.cn

Go:   a && b || !c
来源：http://gne.havefunace.top

Ruby: a && b || !c
来源：http://djr.daxiang520.top

C#:   a && b || !c
来源：http://xmm.gaohongyu789.top

[B16] 卫语句：不满足条件提前返回
来源：http://zif.cqqwz.cn

Py:   if not data: return
来源：http://kuz.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://vwp.guannengcc.top

JS:   if (!data) return;
来源：http://ohu.wangdashe.top

TS:   if (!data) return;
来源：http://nmj.zhaomingkeji.xyz

Java: if (data == null) return;
来源：http://lyf.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://hjs.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://nwp.gogol.net.cn

C#:   if (data == null) return;
来源：http://lvc.yfazqb.com

================================================================================
来源：http://yaj.fengsongda.top

C. 函数与作用域
来源：http://xew.hnqzz.top

================================================================================
来源：http://wlr.zycfv.cn

[C01] 定义函数
来源：http://jbl.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://znq.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eza.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ecn.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://asw.yfazqb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://yhv.cucudq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tcv.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://ymb.xuanzx.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eax.fengsongda.top

[C02] 默认参数
来源：http://rdo.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://itq.vqdsnc.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fco.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://gee.quarkkingdee.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ujn.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://thx.chenzaomai.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bkb.nanxuanxn.top

Ruby: def greet(name = "World") = name
来源：http://yji.yj202588.top

C#:   string Greet(string name = "World") => name;
来源：http://hep.jianghu66.top

[C03] 可变参数
来源：http://luy.snrcjt.cn

Py:   def total(*args): return sum(args)
来源：http://drf.dianchejie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sgy.haohaochexian.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eyr.yvedp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aft.nanxinkj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kvy.cdnleiting.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qps.daria6918.cn

Ruby: def total(*nums); nums.sum; end
来源：http://udz.mhx1999.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gnx.xinyue.icu

[C04] 命名参数 / 关键字参数
来源：http://dbn.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fam.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xeq.xuanzx.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hgd.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pfm.xylfe.cn

Java: // 无：用 Builder 模式或 record
来源：http://alj.ybcxt.top

Go:   // 无：用配置结构体参数
来源：http://llw.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://wok.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://ihx.hesvh.cn

[C05] 返回多个值
来源：http://ysj.haohaochexian.top


<!-- 参考信息 -->