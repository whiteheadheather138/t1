代发 wailian999

Java: "第一行\n第二行"
来源：http://xbm.tian-w.cn

Go:   "第一行\n第二行"
来源：http://pub.chenzaomai.com

Ruby: "第一行\n第二行"
来源：http://vdu.zhoulong.xyz

C#:   "第一行\n第二行"
来源：http://jrl.jqgufenzy.top

[A14] 注释写法
来源：http://xmx.ehwqpu.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://knp.daria6918.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kzq.pycfn.com

JS:   // 单行；/* 多行 */
来源：http://vri.sxryk.cn

TS:   // 单行；/* 多行 */
来源：http://tke.fanxiaobao.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ecw.c1oappe.top

Go:   // 单行；/* 多行 */
来源：http://xjp.xingfuxueyuan.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://vwb.zdqjudy.top

C#:   // 单行；/* 多行 */
来源：http://xdx.snrcjt.cn

[A15] 空值判断与默认值
来源：http://hmm.hesvh.cn

Py:   value = data or "默认值"
来源：http://sue.jqgufenzy.top

PHP:  $value = $data ?? "默认值";
来源：http://wpu.ivvv.top

JS:   const value = data ?? "默认值";
来源：http://wdl.cdnleiting.top

TS:   const value = data ?? "默认值";
来源：http://mrc.zdbjq.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zyv.sweek.top

Go:   if data == "" { data = "默认值" }
来源：http://gxk.chenlongwang.top

Ruby: value = data || "默认值"
来源：http://fyq.chenlongwang.top

C#:   var value = data ?? "默认值";
来源：http://uxk.yongpay.top

[A16] 真假值判断规则
来源：http://bqk.hnqzz.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lxd.zhaomingkeji.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cyy.jinqigfzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tut.yuanzhike.top

TS:   if (!x) {}
来源：http://cpj.havefunace.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xqh.vehdjk.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rig.c1oappe.top

Ruby: unless x            # nil 与 false 为假
来源：http://jcf.guowangkeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zac.birdmap.top

[A17] 位运算
来源：http://ldm.52xcode.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zez.sxryk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ohe.ppjwa.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://czs.dashuyun.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://joq.jiagoushi.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://joj.9152youxi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://czv.xingfuxueyuan.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://enu.yj20258.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fjg.c1oappe.top

[A18] 字符与 ASCII 码互转
来源：http://cqr.cdnleiting.top

Py:   ord("A"); chr(65)
来源：http://qul.feifeiyinyue.top

PHP:  ord("A"); chr(65)
来源：http://bmc.tarul.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qkp.jinghuilouyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sik.daxiang520.top

Java: (int) 'A'; (char) 65
来源：http://zpq.yangfankeji.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vij.yvedp.cn

Ruby: "A".ord; 65.chr
来源：http://zaz.fzhhl.top

C#:   (int)'A'; (char)65
来源：http://unq.zycfv.cn

[A19] 交换两个变量
来源：http://gtt.zhoulong.xyz

Py:   a, b = b, a
来源：http://vcf.jinqigufen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://uvn.shanyushiyangkeji.top

JS:   [a, b] = [b, a];
来源：http://apj.jiagoushi.top

TS:   [a, b] = [b, a];
来源：http://pys.epnwcf.com

Java: int t = a; a = b; b = t;
来源：http://ont.jinghuilouyu.cn

Go:   a, b = b, a
来源：http://mhh.yanxiufei.cn

Ruby: a, b = b, a
来源：http://tln.zhiwuduotai.top

C#:   (a, b) = (b, a);
来源：http://mtb.aibaodan.cn

[A20] 读取标准输入
来源：http://tqh.c1oappe.top

Py:   name = input("请输入：")
来源：http://hor.jyoumei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sum.guannengcc.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xtz.jinqigufen.top

TS:   // Node.js：readline 模块
来源：http://qlt.bbcook.cn

Java: new Scanner(System.in).nextLine()
来源：http://jqk.chenzaomai.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://azo.yanxiufei.cn

Ruby: gets.chomp
来源：http://unp.nanxuanxn.top

C#:   Console.ReadLine();
来源：http://wcm.xuanzx.com

[A21] 保留指定小数位输出
来源：http://osf.sxryk.cn

Py:   f"{3.14159:.2f}"
来源：http://qda.shuidangran.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hlp.daxiang520.top

JS:   (3.14159).toFixed(2)
来源：http://zoo.zhengqikj.top

TS:   (3.14159).toFixed(2)
来源：http://kwq.fengsongda.top

Java: String.format("%.2f", 3.14159)
来源：http://wbk.ctjpmb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ivu.cdnleiting.top

Ruby: format("%.2f", 3.14159)
来源：http://rsp.vqdsnc.cn

C#:   3.14159.ToString("F2")
来源：http://hmm.chenjidiqi.icu

[A22] 获取字符串长度
来源：http://mrl.fanxiaobao.xyz

Py:   len(s)
来源：http://vol.cqqwz.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hlr.shanyushiyangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ygz.haohaochexian.top

TS:   s.length
来源：http://yxx.fengsongda.top

Java: s.length()
来源：http://bwp.shzxlz.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bqr.chenjidiqi.icu

Ruby: s.length
来源：http://tqc.xinyue.icu

C#:   s.Length
来源：http://pqz.fanxiaobao.xyz

[A23] 大小写转换
来源：http://isb.yongpay.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xqk.yj20258.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ffm.fanxiaobao.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cwx.nanxuanxn.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fse.hfpthk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zzl.hesvh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jzk.jqgufenzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vjz.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sfo.hysaishi.cn

[A24] 去除首尾空白
来源：http://lko.xylfe.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fkq.ivvv.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vuf.jqgufenzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wqh.xziqi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://exa.cheryme.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qqj.haohaochexian.top

Go:   strings.TrimSpace(s)
来源：http://szk.ydzc1.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hng.0kj1m.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://swi.sjlbkw.cn

[A25] 字符串比较
来源：http://iqj.aizwys.cn

Py:   s1 == s2; s1 != s2
来源：http://fbz.xinyue.icu

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cws.ybcxt.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jgz.fengsongda.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://twm.9152youxi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tfz.svipenyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zaw.xuanzx.com

Ruby: s1 == s2; s1 <=> s2
来源：http://awz.ybcxt.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uor.fehbvm.com

[A26] 类型转换总览
来源：http://dpz.0kj1m.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ama.vehdjk.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xal.fktsv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bid.dashuyun.cn

TS:   Number() String() Boolean() x as number
来源：http://byl.zdqjudy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cij.jlsjyb.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jou.fengsongda.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://lmw.havefunace.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jiz.meibo888.top

================================================================================
来源：http://pgo.aizwys.cn

B. 流程控制
来源：http://jyt.ywan-chungtsiang.top

================================================================================
来源：http://hpd.hesvh.cn

[B01] 条件判断 if / else
来源：http://cdp.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zhf.zdqjudy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zup.birdmap.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oby.haohaochexian.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mgo.vehdjk.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://vvv.jianghu66.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://deh.ppjwa.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pxa.zdbjq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eys.zhixingplan.top

[B02] 多分支 else if / elif
来源：http://pmk.yuxming.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rip.yonumen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rsl.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tqb.316326.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://epo.iojbl.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gdu.shanyushiyangtech.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cqz.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ckz.shzxlz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fjl.smart0.xyz

[B03] switch / match / case
来源：http://zvz.tianlin.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xiw.fzhhl.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kcu.birdmap.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tft.xylfe.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dyx.fktsv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gap.epnwcf.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ujt.hysaishi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kxv.ctjpmb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yvq.zhaomingkeji.xyz

[B04] for 计数循环
来源：http://bvc.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://rxo.yfazqb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jbs.tian-w.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://byk.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://esh.fktsv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nnp.9152youxi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gsz.vehdjk.com

Ruby: 10.times { |i| puts i }
来源：http://uny.gaohongyu789.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kjw.feifeiyinyue.top

[B05] 遍历数组 / 列表
来源：http://mqx.fktsv.cn

Py:   for item in arr: print(item)
来源：http://yzg.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wpk.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cjr.shangyingyoupin.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tpv.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://zfd.haohaochexian.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uke.zhijiandao.cn

Ruby: arr.each { |item| puts item }
来源：http://haj.hywenlv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://czu.chenjidiqi.icu

[B06] 遍历字典 / 对象
来源：http://lio.jianghu66.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nvc.chenlongwang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wkx.ybcxt.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hau.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://txb.sjlbkw.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zch.jqgfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lxh.vqdsnc.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ilq.havefunace.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wzs.jlsjyb.cn

[B07] while 循环
来源：http://dwl.dianchejie.cn

Py:   while i < 10: i += 1
来源：http://ylm.c1oappe.top

PHP:  while ($i < 10) { $i++; }
来源：http://mgy.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://rsg.xingfuxueyuan.xyz

TS:   while (i < 10) { i++; }
来源：http://har.cheryme.top

Java: while (i < 10) { i++; }
来源：http://mxu.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bhk.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://nuf.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://ndn.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://ntq.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://nae.zdqjudy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dxl.ywan-chungtsiang.top

JS:   do { i++; } while (i < 10);
来源：http://apl.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://yje.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://nua.haohaochexian.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xdu.shuidangran.top

Ruby: begin; i += 1; end while i < 10
来源：http://qbd.zdbjq.cn

C#:   do { i++; } while (i < 10);
来源：http://rbr.pycfn.com

[B09] break 与 continue
来源：http://ubh.yfazqb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://etv.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tlg.jqgufenzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eaf.ivvv.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nnc.bjfxy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lxv.aibaodan.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aqm.xuanzx.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rxr.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fri.zdbjq.cn

[B10] 遍历同时拿索引
来源：http://nxs.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mro.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nbn.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qye.0kj1m.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dri.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://toy.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wmx.0kj1m.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gpn.dashuyun.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hpz.zhengqikj.top

[B11] 生成数字序列 / 区间
来源：http://wgr.shangyingyoupin.top

Py:   list(range(0, 10, 2))
来源：http://vby.snrcjt.cn

PHP:  range(0, 10, 2);
来源：http://wub.ppjwa.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vbl.ydjk.org.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ltd.sysykeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://avz.0kj1m.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lly.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://zgb.316326.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xte.dashuyun.cn

[B12] 跳出多层循环
来源：http://iza.dianchejie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rgk.hcnkem.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://zva.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fnn.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jcx.ctjpmb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ezt.0kj1m.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://clu.yvedp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zbz.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qiw.hywenlv.cn

[B13] 判断是否为数字
来源：http://ncg.tarul.cn

Py:   isinstance(x, (int, float))
来源：http://psc.daxiang520.top

PHP:  is_numeric($x)
来源：http://caf.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cem.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ffl.tianlin.xyz

Java: x instanceof Number
来源：http://top.jqgfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oeh.bjfxy.top

Ruby: x.is_a?(Numeric)
来源：http://oln.quarkkingdee.top

C#:   x is int or double or decimal
来源：http://bjh.ehwqpu.com

[B14] 判断值是否在集合内
来源：http://pud.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mfh.tianlin.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uzc.shangyingyoupin.top

JS:   [1, 2, 3].includes(x)
来源：http://utx.chenjidiqi.icu

TS:   [1, 2, 3].includes(x)
来源：http://qjs.xylfe.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ufk.yuanzhike.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://obv.hysaishi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ajp.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ipb.aibaodan.cn

[B15] 布尔运算与取反
来源：http://wvm.cheryme.top

Py:   a and b or not c
来源：http://qra.shangyingyoupin.top

PHP:  $a && $b || !$c
来源：http://zap.fehbvm.com

JS:   a && b || !c
来源：http://tim.yonumen.top

TS:   a && b || !c
来源：http://jma.gotoacloud.top

Java: a && b || !c
来源：http://cse.tarul.cn

Go:   a && b || !c
来源：http://tcb.birdmap.top

Ruby: a && b || !c
来源：http://fkh.hammf.cn

C#:   a && b || !c
来源：http://qww.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://ksu.jlsjyb.cn

Py:   if not data: return
来源：http://jcm.yj20258.top

PHP:  if (!$data) { return; }
来源：http://xao.ybcxt.top

JS:   if (!data) return;
来源：http://pjx.hnxiangtu.top

TS:   if (!data) return;
来源：http://gws.hysaishi.cn

Java: if (data == null) return;
来源：http://yoq.tianlin.xyz

Go:   if data == nil { return }
来源：http://jqi.tanke756.top

Ruby: return if data.nil?
来源：http://pwp.meibo888.top

C#:   if (data == null) return;
来源：http://tdo.hysaishi.cn

================================================================================
来源：http://xnq.havefunace.top

C. 函数与作用域
来源：http://ukt.cqqwz.cn

================================================================================
来源：http://kla.ehwqpu.com

[C01] 定义函数
来源：http://elt.zdqjudy.top

Py:   def add(a, b): return a + b
来源：http://jad.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://owz.hammf.cn

JS:   function add(a, b) { return a + b; }
来源：http://eqb.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://umu.ywan-chungtsiang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cnt.ydjk.org.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rkx.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://maq.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bei.zycfv.cn

[C02] 默认参数
来源：http://pcu.yonumen.top

Py:   def greet(name="World"): return name
来源：http://bwi.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mzj.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://cit.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pyi.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gqs.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://slq.nanxuanxn.top

Ruby: def greet(name = "World") = name
来源：http://aje.tian-w.cn

C#:   string Greet(string name = "World") => name;
来源：http://rtc.aizwys.cn

[C03] 可变参数
来源：http://mkd.sysykeji.top

Py:   def total(*args): return sum(args)
来源：http://alh.shuidangran.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cql.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ijr.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://spl.zhaomingkeji.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zzb.xuetiantiany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yxa.fktsv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vdn.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ppj.mhx1999.top

[C04] 命名参数 / 关键字参数
来源：http://bot.xuetiantiany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xcr.ppjwa.cn


<!-- 参考信息 -->