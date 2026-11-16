代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://sbw.aibaodan.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dkz.shanyushiyangtech.top

Go:   // 单行；/* 多行 */
来源：http://auu.c1oappe.top

Ruby: # 单行；=begin 多行 =end
来源：http://yne.jqgufenzy.top

C#:   // 单行；/* 多行 */
来源：http://zrh.cashguo.top

[A15] 空值判断与默认值
来源：http://rwp.zhiwuduotai.top

Py:   value = data or "默认值"
来源：http://yqj.sysykeji.top

PHP:  $value = $data ?? "默认值";
来源：http://nrd.andypj.xyz

JS:   const value = data ?? "默认值";
来源：http://jqx.havefunace.top

TS:   const value = data ?? "默认值";
来源：http://rwk.vehdjk.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qga.tarul.cn

Go:   if data == "" { data = "默认值" }
来源：http://olv.aibaodan.cn

Ruby: value = data || "默认值"
来源：http://pct.feifeiyinyue.top

C#:   var value = data ?? "默认值";
来源：http://yah.fengsongda.top

[A16] 真假值判断规则
来源：http://qqe.hesvh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kmd.fktsv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wao.cheryme.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fpy.zdqjudy.top

TS:   if (!x) {}
来源：http://rji.gogol.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lqr.yueranfly.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ujr.ctjpmb.com

Ruby: unless x            # nil 与 false 为假
来源：http://nja.hnqzz.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vxs.ywan-chungtsiang.top

[A17] 位运算
来源：http://fpt.yj20258888.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mqu.chenzaomai.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://scq.yuanzhike.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bje.hammf.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://caa.316326.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xrs.snrcjt.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cjw.ydzc1.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vth.yj20258.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ogn.fzhhl.top

[A18] 字符与 ASCII 码互转
来源：http://kqk.hongshengwenyu.top

Py:   ord("A"); chr(65)
来源：http://xsp.zhijiandao.cn

PHP:  ord("A"); chr(65)
来源：http://ijc.yangfankeji.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://shl.dashuyun.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jgi.c1oappe.top

Java: (int) 'A'; (char) 65
来源：http://ikx.yj20258.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tdr.fanxiaobao.xyz

Ruby: "A".ord; 65.chr
来源：http://fah.zhoulong.xyz

C#:   (int)'A'; (char)65
来源：http://wde.9152youxi.cn

[A19] 交换两个变量
来源：http://lix.aibaodan.cn

Py:   a, b = b, a
来源：http://ckn.yonumen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://los.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://uuw.jlsjyb.cn

TS:   [a, b] = [b, a];
来源：http://ehj.ehwqpu.com

Java: int t = a; a = b; b = t;
来源：http://sme.jinqigufen.top

Go:   a, b = b, a
来源：http://uxs.pycfn.com

Ruby: a, b = b, a
来源：http://bcc.epnwcf.com

C#:   (a, b) = (b, a);
来源：http://jlb.chenjidiqi.icu

[A20] 读取标准输入
来源：http://nny.yongpay.top

Py:   name = input("请输入：")
来源：http://ixm.snrcjt.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rcm.svipenyu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://llw.hammf.cn

TS:   // Node.js：readline 模块
来源：http://hpj.snrcjt.cn

Java: new Scanner(System.in).nextLine()
来源：http://rpn.zhixingplan.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://oko.pengpengdd.cyou

Ruby: gets.chomp
来源：http://bbj.hywenlv.cn

C#:   Console.ReadLine();
来源：http://sxw.aibaodan.cn

[A21] 保留指定小数位输出
来源：http://dkz.yj20258888.top

Py:   f"{3.14159:.2f}"
来源：http://ukv.ctjpmb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mwr.nwbrower.top

JS:   (3.14159).toFixed(2)
来源：http://iqb.fengsongda.top

TS:   (3.14159).toFixed(2)
来源：http://fjz.feifeiyinyue.top

Java: String.format("%.2f", 3.14159)
来源：http://rii.ydjk.org.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zpw.epnwcf.com

Ruby: format("%.2f", 3.14159)
来源：http://mgt.jinqigufen.top

C#:   3.14159.ToString("F2")
来源：http://hee.hysaishi.cn

[A22] 获取字符串长度
来源：http://wmi.iojbl.cn

Py:   len(s)
来源：http://fbd.daxiang520.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://len.smart0.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dds.dianchejie.cn

TS:   s.length
来源：http://vzj.fanxiaobao.xyz

Java: s.length()
来源：http://jrp.yfazqb.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lqs.wangshuangyany.cn

Ruby: s.length
来源：http://brr.bjfxy.top

C#:   s.Length
来源：http://pkn.zhongyouzk.top

[A23] 大小写转换
来源：http://dkn.52xcode.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dhh.zhoulong.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xxo.52xcode.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vmo.sjlbkw.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://awn.yongpay.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mhc.fktsv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cql.0kj1m.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dpw.hfpthk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tym.haohaochexian.top

[A24] 去除首尾空白
来源：http://qmv.svipenyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ons.tanke756.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://euk.nanxuanxn.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nhy.xuanzx.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uld.aibaodan.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jra.9152youxi.cn

Go:   strings.TrimSpace(s)
来源：http://ivw.cqqwz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oxi.xziqi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fdl.jiagoushi.top

[A25] 字符串比较
来源：http://dba.nanxuanxn.top

Py:   s1 == s2; s1 != s2
来源：http://cnn.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bfa.hongshengwenyu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fzb.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eka.pengpengdd.cyou

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qly.yonumen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fsl.havefunace.top

Ruby: s1 == s2; s1 <=> s2
来源：http://por.jianghu66.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vzw.sufxvd.cn

[A26] 类型转换总览
来源：http://ixf.jinqigfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://imw.feifeiyinyue.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yve.tian-w.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aom.nanxuanxn.top

TS:   Number() String() Boolean() x as number
来源：http://ygp.gaohongyu789.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tcl.yfazqb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xvs.xziqi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kif.ywan-chungtsiang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qrd.aibaodan.cn

================================================================================
来源：http://zbr.ywan-chungtsiang.top

B. 流程控制
来源：http://oro.gzhubu.top

================================================================================
来源：http://crg.yuxming.cn

[B01] 条件判断 if / else
来源：http://lhv.shangyingyoupin.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zhl.chenlongwang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oqb.wangshuangyany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jvy.gotoacloud.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hkv.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iis.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yge.yuxming.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eww.jinyuanbaomall.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gda.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://bqi.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kcb.ybcxt.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yvb.nanxuanxn.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qxm.hywenlv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iqj.hfpthk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ofl.yueranfly.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mdj.zhixingplan.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://swc.hfpthk.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jep.nanxinkj.top

[B03] switch / match / case
来源：http://veu.cqqwz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yab.yangfankeji.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qop.chenzaomai.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gpd.meibo888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lvf.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pru.yj20258.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oqf.hysaishi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fss.snrcjt.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fuo.zhijiandao.cn

[B04] for 计数循环
来源：http://skw.xuanzx.com

Py:   for i in range(10): print(i)
来源：http://xlr.svipenyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://reu.xinyue.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lhw.hongshengwenyu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://azc.tanke756.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qpk.shanyushiyangtech.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eqb.xuetiantiany.cn

Ruby: 10.times { |i| puts i }
来源：http://ltb.andypj.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wjk.yueranfly.top

[B05] 遍历数组 / 列表
来源：http://uqh.ctjpmb.com

Py:   for item in arr: print(item)
来源：http://gke.dashuyun.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cmh.hnqzz.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yan.xuetiantiany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yqk.jyoumei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lob.jqgufenzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dgp.fzhhl.top

Ruby: arr.each { |item| puts item }
来源：http://scx.yonumen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zgm.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://wnr.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tsv.guowangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://twd.xylfe.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bmz.yj20258888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ehr.birdmap.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fnw.jqgfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eqh.wangshuangyany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mie.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ksu.xingfuxueyuan.xyz

[B07] while 循环
来源：http://bof.shanyushiyangkeji.top

Py:   while i < 10: i += 1
来源：http://twl.hysaishi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iih.gzhubu.top

JS:   while (i < 10) { i++; }
来源：http://fxu.shzxlz.cn

TS:   while (i < 10) { i++; }
来源：http://nqn.nanxinkj.top

Java: while (i < 10) { i++; }
来源：http://inc.aibaodan.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pda.nwbrower.top

Ruby: while i < 10; i += 1; end
来源：http://pwp.yvedp.cn

C#:   while (i < 10) { i++; }
来源：http://bps.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://qgj.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://tvy.chenjidiqi.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://vwd.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://efx.gotoacloud.top

TS:   do { i++; } while (i < 10);
来源：http://ozj.yuanzhike.top

Java: do { i++; } while (i < 10);
来源：http://mai.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://zba.shanyushiyangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://rzr.ydjk.org.cn

C#:   do { i++; } while (i < 10);
来源：http://quf.jinqigfzy.top

[B09] break 与 continue
来源：http://ter.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kao.fengsongda.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xat.jiagoushi.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kmj.kuanghao11.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gdx.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kpz.jinqigfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aaa.tarul.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tph.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vna.kuanghao11.cn

[B10] 遍历同时拿索引
来源：http://kvs.guannengcc.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://drd.fanxiaobao.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://khn.hnqzz.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gyi.gaohongyu789.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sds.sweek.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kvq.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mns.sysykeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lyt.kuanghao11.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ian.meibo888.top

[B11] 生成数字序列 / 区间
来源：http://gkm.nanxinkj.top

Py:   list(range(0, 10, 2))
来源：http://bcg.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://brk.zhiwuduotai.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rrk.zhixingplan.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cuj.yonumen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cmk.nanxuanxn.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zsh.jinyuanbaomall.cn

Ruby: (0...10).step(2).to_a
来源：http://ytw.nanxinkj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cin.cdnleiting.top

[B12] 跳出多层循环
来源：http://spc.ppjwa.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bim.gaohongyu789.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://aaf.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lzt.zhijiandao.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bel.0kj1m.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wlo.gzhubu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mod.yueranfly.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hnw.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://alu.tarul.cn

[B13] 判断是否为数字
来源：http://stk.hcnkem.com

Py:   isinstance(x, (int, float))
来源：http://kin.fehbvm.com

PHP:  is_numeric($x)
来源：http://lcc.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://stu.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wpq.pycfn.com

Java: x instanceof Number
来源：http://tgg.zhijiandao.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lqg.tianlin.xyz

Ruby: x.is_a?(Numeric)
来源：http://sei.daria6918.cn

C#:   x is int or double or decimal
来源：http://tee.zycfv.cn

[B14] 判断值是否在集合内
来源：http://lup.pengpengdd.cyou

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gfg.xuetiantiany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ykd.316326.xyz

JS:   [1, 2, 3].includes(x)
来源：http://ywn.epnwcf.com

TS:   [1, 2, 3].includes(x)
来源：http://egb.snrcjt.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vui.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tap.fktsv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lis.cheryme.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tuu.nanxinkj.top

[B15] 布尔运算与取反
来源：http://ytt.feifeiyinyue.top

Py:   a and b or not c
来源：http://pdn.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://anz.fehbvm.com

JS:   a && b || !c
来源：http://ori.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://arh.hnxiangtu.top

Java: a && b || !c
来源：http://duo.aibaodan.cn

Go:   a && b || !c
来源：http://fko.tanke756.top

Ruby: a && b || !c
来源：http://huf.aibaodan.cn

C#:   a && b || !c
来源：http://zlb.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://iaq.xingfuxueyuan.xyz

Py:   if not data: return
来源：http://txf.ivvv.top

PHP:  if (!$data) { return; }
来源：http://bbx.9152youxi.cn

JS:   if (!data) return;
来源：http://ycd.cheryme.top

TS:   if (!data) return;
来源：http://qpq.bjfxy.top

Java: if (data == null) return;
来源：http://tex.aizwys.cn

Go:   if data == nil { return }
来源：http://toc.quarkkingdee.top

Ruby: return if data.nil?
来源：http://nwi.jinqigfzy.top

C#:   if (data == null) return;
来源：http://apj.dashuyun.cn

================================================================================
来源：http://uvw.yanxiufei.cn

C. 函数与作用域
来源：http://tsi.zycfv.cn

================================================================================
来源：http://xdp.zhongyouzk.top

[C01] 定义函数
来源：http://nnq.dianchejie.cn

Py:   def add(a, b): return a + b
来源：http://kak.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vmi.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://jkq.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zep.redwolf501.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jag.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://idl.52xcode.cn

Ruby: def add(a, b); a + b; end
来源：http://fdz.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lqk.aizwys.cn

[C02] 默认参数
来源：http://bea.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://rky.xuetiantiany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kya.ppjwa.cn

JS:   function greet(name = "World") { return name; }
来源：http://toc.dianchejie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rxs.fktsv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://per.pengpengdd.cyou

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kwl.ydjk.org.cn

Ruby: def greet(name = "World") = name
来源：http://mzm.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://sco.ehwqpu.com

[C03] 可变参数
来源：http://xvq.yanxiufei.cn

Py:   def total(*args): return sum(args)
来源：http://xuf.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ehf.chenjidiqi.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ibp.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://upf.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qpb.birdmap.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xlq.jiagoushi.top

Ruby: def total(*nums); nums.sum; end
来源：http://xzb.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ryq.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://xev.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hod.jqgufenzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sbt.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xue.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fuk.gzhubu.top

Java: // 无：用 Builder 模式或 record
来源：http://ziy.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://xcw.jiagoushi.top

Ruby: f(a: 1, b: 2)
来源：http://bgh.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://cvx.shangyingyoupin.top

[C05] 返回多个值
来源：http://xpo.aibaodan.cn


<!-- 参考信息 -->