代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://epo.bbcook.cn

[A15] 空值判断与默认值
来源：http://hml.yvedp.cn

Py:   value = data or "默认值"
来源：http://bbk.dianchejie.cn

PHP:  $value = $data ?? "默认值";
来源：http://hoj.epnwcf.com

JS:   const value = data ?? "默认值";
来源：http://fdp.sufxvd.cn

TS:   const value = data ?? "默认值";
来源：http://wqq.yj20258.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ajw.redwolf501.top

Go:   if data == "" { data = "默认值" }
来源：http://qeu.cashguo.top

Ruby: value = data || "默认值"
来源：http://xyd.bjfxy.top

C#:   var value = data ?? "默认值";
来源：http://ckr.gogol.net.cn

[A16] 真假值判断规则
来源：http://fmf.shanyushiyangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zrm.hywenlv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nuc.yuxming.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yix.fanxiaobao.xyz

TS:   if (!x) {}
来源：http://vpy.gaohongyu789.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ets.zhengqikj.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://biq.xinyue.icu

Ruby: unless x            # nil 与 false 为假
来源：http://bbh.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://aif.hnqzz.top

[A17] 位运算
来源：http://wzn.9152youxi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lfy.ywan-chungtsiang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zrf.vehdjk.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gsc.hfpthk.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yyq.cqqwz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://igi.meibo888.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yes.ivvv.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ska.yanxiufei.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oyz.daxiang520.top

[A18] 字符与 ASCII 码互转
来源：http://wfc.yvedp.cn

Py:   ord("A"); chr(65)
来源：http://nuq.cheryme.top

PHP:  ord("A"); chr(65)
来源：http://rpy.uphjek.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rsf.snrcjt.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vpn.daria6918.cn

Java: (int) 'A'; (char) 65
来源：http://wej.bbcook.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gnb.yj20258.top

Ruby: "A".ord; 65.chr
来源：http://lcp.sxryk.cn

C#:   (int)'A'; (char)65
来源：http://mcj.chenzaomai.com

[A19] 交换两个变量
来源：http://fbo.zhoulong.xyz

Py:   a, b = b, a
来源：http://zue.shanyushiyangtech.top

PHP:  [$a, $b] = [$b, $a];
来源：http://cai.zhijiandao.cn

JS:   [a, b] = [b, a];
来源：http://fpk.yangfankeji.com

TS:   [a, b] = [b, a];
来源：http://xqf.svipenyu.cn

Java: int t = a; a = b; b = t;
来源：http://ghi.bjfxy.top

Go:   a, b = b, a
来源：http://smz.pycfn.com

Ruby: a, b = b, a
来源：http://kuk.9152youxi.cn

C#:   (a, b) = (b, a);
来源：http://kbj.jinqigfzy.top

[A20] 读取标准输入
来源：http://mbt.xuanzx.com

Py:   name = input("请输入：")
来源：http://cql.sxryk.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://phd.yvedp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bfg.kuanghao11.cn

TS:   // Node.js：readline 模块
来源：http://ixn.xziqi.cn

Java: new Scanner(System.in).nextLine()
来源：http://edj.chenjidiqi.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wud.aizwys.cn

Ruby: gets.chomp
来源：http://mlj.jyoumei.cn

C#:   Console.ReadLine();
来源：http://bar.ywan-chungtsiang.top

[A21] 保留指定小数位输出
来源：http://hkf.hfpthk.cn

Py:   f"{3.14159:.2f}"
来源：http://btb.9152youxi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pbq.pengpengdd.cyou

JS:   (3.14159).toFixed(2)
来源：http://udd.quarkkingdee.top

TS:   (3.14159).toFixed(2)
来源：http://ilx.chenzaomai.com

Java: String.format("%.2f", 3.14159)
来源：http://kct.hnqzz.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eqo.xylfe.cn

Ruby: format("%.2f", 3.14159)
来源：http://jav.xuanzx.com

C#:   3.14159.ToString("F2")
来源：http://jxy.hywenlv.cn

[A22] 获取字符串长度
来源：http://scx.cheryme.top

Py:   len(s)
来源：http://tfq.cucudq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://aqb.vehdjk.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ugd.c1oappe.top

TS:   s.length
来源：http://fju.shangyingyoupin.top

Java: s.length()
来源：http://cot.jyoumei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jbc.fzhhl.top

Ruby: s.length
来源：http://taj.zhijiandao.cn

C#:   s.Length
来源：http://xhb.zhixingplan.top

[A23] 大小写转换
来源：http://shl.jyoumei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wii.uphjek.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dya.sxryk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ivc.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nje.xuanzx.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zpv.nanxuanxn.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kxj.tianlin.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wvt.ybcxt.top

C#:   s.ToUpper(); s.ToLower()
来源：http://tei.jianghu66.top

[A24] 去除首尾空白
来源：http://sje.yanxiufei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://flb.fehbvm.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fkp.hfpthk.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://byd.sxryk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mug.jinghuilouyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://auo.fanxiaobao.xyz

Go:   strings.TrimSpace(s)
来源：http://evo.yongpay.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mqo.redwolf501.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hhq.daxiang520.top

[A25] 字符串比较
来源：http://rsq.gaohongyu789.top

Py:   s1 == s2; s1 != s2
来源：http://yrv.jianghu66.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nus.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ozz.jinqigfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yct.tian-w.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qfh.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qem.hywenlv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lqr.birdmap.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tvt.andypj.xyz

[A26] 类型转换总览
来源：http://nmq.quarkkingdee.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zuf.yuanzhike.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://caz.ydzc1.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://irs.haohaochexian.top

TS:   Number() String() Boolean() x as number
来源：http://wxe.ydzc1.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rqh.fzhhl.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fcv.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dlb.bbcook.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qwg.yj20258888.top

================================================================================
来源：http://wbf.yongpay.top

B. 流程控制
来源：http://tne.yuxming.cn

================================================================================
来源：http://cbj.jinghuilouyu.cn

[B01] 条件判断 if / else
来源：http://dgd.gotoacloud.top

Py:   result = "正" if x > 0 else "非正"
来源：http://djv.jinqigufen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://awi.yj20258.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jay.cdnleiting.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xbo.316326.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://hno.yonumen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lag.nanxinkj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rhp.feifeiyinyue.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://did.yangfankeji.com

[B02] 多分支 else if / elif
来源：http://yhh.cqqwz.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wwu.fanxiaobao.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://esl.chenzaomai.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dct.shanyushiyangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dab.gaohongyu789.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tep.hysaishi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qax.jyoumei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jor.aizwys.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ifo.jlsjyb.cn

[B03] switch / match / case
来源：http://zzl.andypj.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xjg.jinghuilouyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jqx.zhengqikj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wye.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tfe.ppjwa.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xzq.zhoulong.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fhw.fktsv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rnb.yfazqb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lqe.sufxvd.cn

[B04] for 计数循环
来源：http://xfq.birdmap.top

Py:   for i in range(10): print(i)
来源：http://vin.smart0.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qjn.jinyuanbaomall.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rop.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fbv.gzhubu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pox.hammf.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://onm.hnqzz.top

Ruby: 10.times { |i| puts i }
来源：http://avs.sufxvd.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zog.gotoacloud.top

[B05] 遍历数组 / 列表
来源：http://ssw.xinyue.icu

Py:   for item in arr: print(item)
来源：http://ecc.aibaodan.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eoq.cqqwz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dwg.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rio.sxryk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jia.svipenyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vsy.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://bdy.zdqjudy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uxw.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://vtb.dianchejie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zps.ehwqpu.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bhp.sxryk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://agd.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jod.hammf.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uvt.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://msg.tian-w.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ymf.hesvh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hqu.ctjpmb.com

[B07] while 循环
来源：http://mpy.guannengcc.top

Py:   while i < 10: i += 1
来源：http://yuc.uphjek.com

PHP:  while ($i < 10) { $i++; }
来源：http://bql.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://mrb.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://ggz.tianlin.xyz

Java: while (i < 10) { i++; }
来源：http://kxy.daxiang520.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hfg.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://sat.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://uwy.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://hqd.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://slo.dianchejie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pfg.meibo888.top

JS:   do { i++; } while (i < 10);
来源：http://qoh.havefunace.top

TS:   do { i++; } while (i < 10);
来源：http://ewf.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://nzt.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hqb.wangdashe.top

Ruby: begin; i += 1; end while i < 10
来源：http://tfk.zhijiandao.cn

C#:   do { i++; } while (i < 10);
来源：http://vjk.gaohongyu789.top

[B09] break 与 continue
来源：http://fyn.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nwp.hnqzz.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tzm.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lvy.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ayp.yongpay.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xhv.pengpengdd.cyou

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xbj.cucudq.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jkq.ybcxt.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qwa.haohaochexian.top

[B10] 遍历同时拿索引
来源：http://ofo.52xcode.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fld.cucudq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rev.ivvv.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nha.jyoumei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tdv.vqdsnc.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wxw.zdbjq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://txz.bjfxy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kyw.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hae.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://fia.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://dha.dashuyun.cn

PHP:  range(0, 10, 2);
来源：http://oih.fzhhl.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qjm.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://psa.zhixingplan.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://isy.guowangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dbm.zdbjq.cn

Ruby: (0...10).step(2).to_a
来源：http://trp.hfpthk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://djg.zhixingplan.top

[B12] 跳出多层循环
来源：http://jco.chenzaomai.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://grk.hnxiangtu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xhk.jqgfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ord.hysaishi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uhz.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lps.hongshengwenyu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lvf.fengsongda.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hre.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ygk.c1oappe.top

[B13] 判断是否为数字
来源：http://ocv.guannengcc.top

Py:   isinstance(x, (int, float))
来源：http://jii.svipenyu.cn

PHP:  is_numeric($x)
来源：http://dtc.chenjidiqi.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mla.andypj.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sbp.pengpengdd.cyou

Java: x instanceof Number
来源：http://gsf.feifeiyinyue.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ets.ctjpmb.com

Ruby: x.is_a?(Numeric)
来源：http://ldc.guowangkeji.top

C#:   x is int or double or decimal
来源：http://dei.gzhubu.top

[B14] 判断值是否在集合内
来源：http://isd.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pfa.yj20258888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eky.316326.xyz

JS:   [1, 2, 3].includes(x)
来源：http://zdh.ywan-chungtsiang.top

TS:   [1, 2, 3].includes(x)
来源：http://cpe.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yeq.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://esw.zhoulong.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://ktr.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pcp.hongshengwenyu.top

[B15] 布尔运算与取反
来源：http://xhg.ppjwa.cn

Py:   a and b or not c
来源：http://yiu.dianchejie.cn

PHP:  $a && $b || !$c
来源：http://yux.pycfn.com

JS:   a && b || !c
来源：http://yrw.zhijiandao.cn

TS:   a && b || !c
来源：http://rmi.havefunace.top

Java: a && b || !c
来源：http://jrm.jqgufenzy.top

Go:   a && b || !c
来源：http://kce.shuidangran.top

Ruby: a && b || !c
来源：http://snz.jinghuilouyu.cn

C#:   a && b || !c
来源：http://krq.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://xeb.gzhubu.top

Py:   if not data: return
来源：http://sur.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://cvs.feifeiyinyue.top

JS:   if (!data) return;
来源：http://oqz.hnxiangtu.top

TS:   if (!data) return;
来源：http://fbn.sxryk.cn

Java: if (data == null) return;
来源：http://ucc.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://yvi.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://zuz.ppjwa.cn

C#:   if (data == null) return;
来源：http://apa.fengsongda.top

================================================================================
来源：http://yie.yvedp.cn

C. 函数与作用域
来源：http://ysx.jinqigfzy.top

================================================================================
来源：http://snr.xylfe.cn

[C01] 定义函数
来源：http://oyy.yj20258.top

Py:   def add(a, b): return a + b
来源：http://dck.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://upv.haohaochexian.top

JS:   function add(a, b) { return a + b; }
来源：http://fee.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rcq.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://mew.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://egg.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://uvd.chenzaomai.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nxg.yangfankeji.com

[C02] 默认参数
来源：http://cyd.shzxlz.cn

Py:   def greet(name="World"): return name
来源：http://dcf.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ubj.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://xuv.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lcu.kuanghao11.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nwf.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tnj.fehbvm.com

Ruby: def greet(name = "World") = name
来源：http://vkl.meibo888.top

C#:   string Greet(string name = "World") => name;
来源：http://mhe.bbcook.cn

[C03] 可变参数
来源：http://ckm.tianlin.xyz

Py:   def total(*args): return sum(args)
来源：http://quz.0kj1m.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cuh.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://stc.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://grw.yj202588.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rtt.fanxiaobao.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sxm.yonumen.top

Ruby: def total(*nums); nums.sum; end
来源：http://bcv.ydjk.org.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bdc.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://gwz.haohaochexian.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://seh.jinqigfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ywa.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fld.yuanzhike.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rpq.ivvv.top

Java: // 无：用 Builder 模式或 record
来源：http://bpw.zhengqikj.top

Go:   // 无：用配置结构体参数
来源：http://pkd.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://xbm.jinqigfzy.top

C#:   f(a: 1, b: 2)
来源：http://uuf.uphjek.com

[C05] 返回多个值
来源：http://bmr.wangdashe.top

Py:   return a, b
来源：http://tsj.jianghu66.top

PHP:  return [$a, $b];
来源：http://ydm.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://akt.yfazqb.com

TS:   return { a, b };
来源：http://vjo.chenlongwang.top


<!-- 参考信息 -->