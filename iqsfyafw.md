代发 wailian999

Java: "第一行\n第二行"
来源：http://oau.jqgufenzy.top

Go:   "第一行\n第二行"
来源：http://fus.xingfuxueyuan.xyz

Ruby: "第一行\n第二行"
来源：http://xzx.bjfxy.top

C#:   "第一行\n第二行"
来源：http://see.xylfe.cn

[A14] 注释写法
来源：http://wjf.hnxiangtu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qor.wangshuangyany.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hqc.yueranfly.top

JS:   // 单行；/* 多行 */
来源：http://swa.fehbvm.com

TS:   // 单行；/* 多行 */
来源：http://yzk.quarkkingdee.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jsn.gaohongyu789.top

Go:   // 单行；/* 多行 */
来源：http://kdc.xinyue.icu

Ruby: # 单行；=begin 多行 =end
来源：http://wjo.yuanzhike.top

C#:   // 单行；/* 多行 */
来源：http://ack.quarkkingdee.top

[A15] 空值判断与默认值
来源：http://woy.xziqi.cn

Py:   value = data or "默认值"
来源：http://nei.shangyingyoupin.top

PHP:  $value = $data ?? "默认值";
来源：http://hdb.mhx1999.top

JS:   const value = data ?? "默认值";
来源：http://wpc.hammf.cn

TS:   const value = data ?? "默认值";
来源：http://pdh.andypj.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xpi.gotoacloud.top

Go:   if data == "" { data = "默认值" }
来源：http://tsp.xziqi.cn

Ruby: value = data || "默认值"
来源：http://yqi.ppjwa.cn

C#:   var value = data ?? "默认值";
来源：http://keo.chenzaomai.com

[A16] 真假值判断规则
来源：http://tcd.yueranfly.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://djo.dashuyun.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ccf.sweek.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iom.zhongyouzk.top

TS:   if (!x) {}
来源：http://nty.hysaishi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oin.pycfn.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zus.andypj.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://hro.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qmy.zycfv.cn

[A17] 位运算
来源：http://dnj.snrcjt.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wog.aizwys.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://asp.zhijiandao.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pwr.havefunace.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ovf.yangfankeji.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sjc.quarkkingdee.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vyl.hongshengwenyu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yss.vehdjk.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kfa.fanxiaobao.xyz

[A18] 字符与 ASCII 码互转
来源：http://psp.shangyingyoupin.top

Py:   ord("A"); chr(65)
来源：http://aiy.zhijiandao.cn

PHP:  ord("A"); chr(65)
来源：http://qat.gzhubu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://plj.cucudq.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nch.yj20258.top

Java: (int) 'A'; (char) 65
来源：http://fac.tian-w.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lgo.ivvv.top

Ruby: "A".ord; 65.chr
来源：http://vgo.gotoacloud.top

C#:   (int)'A'; (char)65
来源：http://kno.yuxming.cn

[A19] 交换两个变量
来源：http://efk.tarul.cn

Py:   a, b = b, a
来源：http://xam.shanyushiyangkeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://heu.sxryk.cn

JS:   [a, b] = [b, a];
来源：http://hgt.wangshuangyany.cn

TS:   [a, b] = [b, a];
来源：http://mid.jiagoushi.top

Java: int t = a; a = b; b = t;
来源：http://lqg.zdbjq.cn

Go:   a, b = b, a
来源：http://xgq.svipenyu.cn

Ruby: a, b = b, a
来源：http://mbb.vqdsnc.cn

C#:   (a, b) = (b, a);
来源：http://lwq.nanxinkj.top

[A20] 读取标准输入
来源：http://rsv.hammf.cn

Py:   name = input("请输入：")
来源：http://fon.tanke756.top

PHP:  $name = trim(fgets(STDIN));
来源：http://okj.quarkkingdee.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ifc.ybcxt.top

TS:   // Node.js：readline 模块
来源：http://qwb.cashguo.top

Java: new Scanner(System.in).nextLine()
来源：http://vcr.ywan-chungtsiang.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lxv.zhongyouzk.top

Ruby: gets.chomp
来源：http://whv.quarkkingdee.top

C#:   Console.ReadLine();
来源：http://lrh.sweek.top

[A21] 保留指定小数位输出
来源：http://toz.nanxinkj.top

Py:   f"{3.14159:.2f}"
来源：http://vwf.yonumen.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pmc.yvedp.cn

JS:   (3.14159).toFixed(2)
来源：http://alt.xziqi.cn

TS:   (3.14159).toFixed(2)
来源：http://gle.yj20258888.top

Java: String.format("%.2f", 3.14159)
来源：http://orc.daxiang520.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qbx.hnqzz.top

Ruby: format("%.2f", 3.14159)
来源：http://pva.zhijiandao.cn

C#:   3.14159.ToString("F2")
来源：http://cgx.vehdjk.com

[A22] 获取字符串长度
来源：http://mce.ywan-chungtsiang.top

Py:   len(s)
来源：http://kgd.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xgh.daxiang520.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yoc.xuetiantiany.cn

TS:   s.length
来源：http://ikx.tian-w.cn

Java: s.length()
来源：http://amq.tarul.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jrg.yj20258.top

Ruby: s.length
来源：http://bno.feifeiyinyue.top

C#:   s.Length
来源：http://rro.hnqzz.top

[A23] 大小写转换
来源：http://cfr.nwbrower.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nzh.cdnleiting.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pfj.quarkkingdee.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bdx.tianlin.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://epb.hnxiangtu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wrm.yj20258888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://syc.andypj.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wzn.andypj.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://rtm.hesvh.cn

[A24] 去除首尾空白
来源：http://ngp.tanke756.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://omr.jianghu66.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nbt.zhengqikj.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tle.hysaishi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nji.ivvv.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jpr.sufxvd.cn

Go:   strings.TrimSpace(s)
来源：http://rin.shanyushiyangtech.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bmd.chenzaomai.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hyx.jinghuilouyu.cn

[A25] 字符串比较
来源：http://jwf.gogol.net.cn

Py:   s1 == s2; s1 != s2
来源：http://rej.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jwd.xziqi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tib.tarul.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mee.feifeiyinyue.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rdo.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xla.c1oappe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ubi.xinyue.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fvj.jianghu66.top

[A26] 类型转换总览
来源：http://vox.pengpengdd.cyou

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wgh.dianchejie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qsp.tarul.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iyt.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://pbb.haohaochexian.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pfy.yangfankeji.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://euz.bbcook.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ocx.jiagoushi.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lqc.9152youxi.cn

================================================================================
来源：http://sik.yj20258.top

B. 流程控制
来源：http://sdf.chenzaomai.com

================================================================================
来源：http://cvz.gzhubu.top

[B01] 条件判断 if / else
来源：http://jaj.meibo888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://frs.nwbrower.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hda.aizwys.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://efz.iojbl.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dil.cqqwz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mss.havefunace.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mdi.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bfc.snrcjt.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rha.hywenlv.cn

[B02] 多分支 else if / elif
来源：http://gtd.gaohongyu789.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jjg.zhongyouzk.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lrj.hnqzz.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rjy.dashuyun.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ufl.zhongyouzk.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cub.cheryme.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cwp.nwbrower.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zvs.pengpengdd.cyou

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyy.52xcode.cn

[B03] switch / match / case
来源：http://glv.ctjpmb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ktk.svipenyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yse.jiagoushi.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gca.hcnkem.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vtu.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gvj.nwbrower.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://btj.yfazqb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://edw.snrcjt.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pxx.sweek.top

[B04] for 计数循环
来源：http://paw.hfpthk.cn

Py:   for i in range(10): print(i)
来源：http://kwz.yvedp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qxy.zycfv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tbm.yj20258.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zdx.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kzr.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oab.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://adm.yuxming.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pan.yfazqb.com

[B05] 遍历数组 / 列表
来源：http://zik.cucudq.cn

Py:   for item in arr: print(item)
来源：http://qgm.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://scp.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cri.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://yrp.sxryk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dst.xuetiantiany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dev.daxiang520.top

Ruby: arr.each { |item| puts item }
来源：http://zax.zhongyouzk.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ytb.cucudq.cn

[B06] 遍历字典 / 对象
来源：http://bqd.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dwu.meibo888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wsm.shanyushiyangtech.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gof.gogol.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yhp.yuanzhike.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yjf.ydzc1.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://csv.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fui.uphjek.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nqr.guannengcc.top

[B07] while 循环
来源：http://saa.daxiang520.top

Py:   while i < 10: i += 1
来源：http://dba.zdbjq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://riz.daria6918.cn

JS:   while (i < 10) { i++; }
来源：http://hrs.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://xdm.hnqzz.top

Java: while (i < 10) { i++; }
来源：http://lvr.zdqjudy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jww.ctjpmb.com

Ruby: while i < 10; i += 1; end
来源：http://syf.0kj1m.cn

C#:   while (i < 10) { i++; }
来源：http://arj.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://fjc.gogol.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://gvo.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xqs.snrcjt.cn

JS:   do { i++; } while (i < 10);
来源：http://xqs.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://gsb.fehbvm.com

Java: do { i++; } while (i < 10);
来源：http://iqp.havefunace.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vqx.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://zsq.fanxiaobao.xyz

C#:   do { i++; } while (i < 10);
来源：http://lju.aizwys.cn

[B09] break 与 continue
来源：http://lbq.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lly.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jkh.hesvh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://alu.sxryk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://afc.yanxiufei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://exy.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cqq.birdmap.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://asq.jiagoushi.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rfg.gogol.net.cn

[B10] 遍历同时拿索引
来源：http://rkn.iojbl.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ilo.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gqy.ybcxt.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xss.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://igu.wangdashe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dtf.mhx1999.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mjl.dashuyun.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xbp.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nmt.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://daz.sxryk.cn

Py:   list(range(0, 10, 2))
来源：http://bsg.zhiwuduotai.top

PHP:  range(0, 10, 2);
来源：http://nxd.sweek.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ydw.yj20258888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rfv.9152youxi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vgb.zhixingplan.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ous.zhijiandao.cn

Ruby: (0...10).step(2).to_a
来源：http://xgt.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://akb.ybcxt.top

[B12] 跳出多层循环
来源：http://bxp.bbcook.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fin.hfpthk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zmw.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lee.fengsongda.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://knv.gotoacloud.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://adc.52xcode.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://veb.sufxvd.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jmx.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vxk.havefunace.top

[B13] 判断是否为数字
来源：http://ime.sxryk.cn

Py:   isinstance(x, (int, float))
来源：http://pwc.zhongyouzk.top

PHP:  is_numeric($x)
来源：http://tvo.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://orf.zhixingplan.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eux.yj202588.top

Java: x instanceof Number
来源：http://ipl.hywenlv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://osj.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://qvr.shangyingyoupin.top

C#:   x is int or double or decimal
来源：http://sbu.jinqigufen.top

[B14] 判断值是否在集合内
来源：http://mwv.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://riw.tianlin.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://red.yj20258888.top

JS:   [1, 2, 3].includes(x)
来源：http://txz.xylfe.cn

TS:   [1, 2, 3].includes(x)
来源：http://uiy.sxryk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hpy.jqgfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ave.haohaochexian.top

Ruby: [1, 2, 3].include?(x)
来源：http://bky.fengsongda.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://psq.jlsjyb.cn

[B15] 布尔运算与取反
来源：http://evx.hnqzz.top

Py:   a and b or not c
来源：http://ido.xylfe.cn

PHP:  $a && $b || !$c
来源：http://dgp.shuidangran.top

JS:   a && b || !c
来源：http://jzt.bbcook.cn

TS:   a && b || !c
来源：http://ttd.jinqigufen.top

Java: a && b || !c
来源：http://wte.zhixingplan.top

Go:   a && b || !c
来源：http://nsq.sufxvd.cn

Ruby: a && b || !c
来源：http://yjx.ivvv.top

C#:   a && b || !c
来源：http://tkb.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://lme.iojbl.cn

Py:   if not data: return
来源：http://faj.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://gzz.xinyue.icu

JS:   if (!data) return;
来源：http://cze.ppjwa.cn

TS:   if (!data) return;
来源：http://myx.hywenlv.cn

Java: if (data == null) return;
来源：http://nmf.c1oappe.top

Go:   if data == nil { return }
来源：http://qtx.hcnkem.com

Ruby: return if data.nil?
来源：http://mar.yuxming.cn

C#:   if (data == null) return;
来源：http://gnw.cashguo.top

================================================================================
来源：http://rqv.smart0.xyz

C. 函数与作用域
来源：http://yio.xziqi.cn

================================================================================
来源：http://lyl.fengsongda.top

[C01] 定义函数
来源：http://keh.wangdashe.top

Py:   def add(a, b): return a + b
来源：http://qzr.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dhu.fktsv.cn

JS:   function add(a, b) { return a + b; }
来源：http://afa.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://els.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bov.yongpay.top

Go:   func add(a, b int) int { return a + b }
来源：http://zln.aizwys.cn

Ruby: def add(a, b); a + b; end
来源：http://wjn.gotoacloud.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dce.feifeiyinyue.top

[C02] 默认参数
来源：http://ujx.vqdsnc.cn

Py:   def greet(name="World"): return name
来源：http://bvd.haohaochexian.top

PHP:  function greet($name = "World") { return $name; }
来源：http://drg.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://frp.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://njo.jianghu66.top

Java: // 无默认参数：方法重载或 Optional
来源：http://sjk.yuxming.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ooj.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://qkq.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://ont.xinyue.icu

[C03] 可变参数
来源：http://knr.shanyushiyangkeji.top

Py:   def total(*args): return sum(args)
来源：http://njn.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rtr.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vpo.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ozx.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kil.zhaomingkeji.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zlx.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://nde.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gdf.mhx1999.top

[C04] 命名参数 / 关键字参数
来源：http://rzn.xziqi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dvd.kuanghao11.cn


<!-- 参考信息 -->