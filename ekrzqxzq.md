代发 wailian999

Java: "第一行\n第二行"
来源：http://eqo.vqdsnc.cn

Go:   "第一行\n第二行"
来源：http://khl.chenzaomai.com

Ruby: "第一行\n第二行"
来源：http://ben.shanyushiyangtech.top

C#:   "第一行\n第二行"
来源：http://vhf.sufxvd.cn

[A14] 注释写法
来源：http://jli.jqgufenzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rxh.gaohongyu789.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://iga.jinghuilouyu.cn

JS:   // 单行；/* 多行 */
来源：http://qcd.gaohongyu789.top

TS:   // 单行；/* 多行 */
来源：http://nxe.0kj1m.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fmd.hnqzz.top

Go:   // 单行；/* 多行 */
来源：http://voo.9152youxi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ghb.9152youxi.cn

C#:   // 单行；/* 多行 */
来源：http://ruh.ppjwa.cn

[A15] 空值判断与默认值
来源：http://jwx.yj202588.top

Py:   value = data or "默认值"
来源：http://vfx.yuxming.cn

PHP:  $value = $data ?? "默认值";
来源：http://xsw.bbcook.cn

JS:   const value = data ?? "默认值";
来源：http://drb.ehwqpu.com

TS:   const value = data ?? "默认值";
来源：http://fek.ehwqpu.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oxe.kuanghao11.cn

Go:   if data == "" { data = "默认值" }
来源：http://hmg.hysaishi.cn

Ruby: value = data || "默认值"
来源：http://pfz.ivvv.top

C#:   var value = data ?? "默认值";
来源：http://fof.ivvv.top

[A16] 真假值判断规则
来源：http://fap.feifeiyinyue.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tvd.yj20258.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xxo.guowangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lqj.jlsjyb.cn

TS:   if (!x) {}
来源：http://pid.xinyue.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tsf.sufxvd.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ymn.guannengcc.top

Ruby: unless x            # nil 与 false 为假
来源：http://mex.jianghu66.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wlz.aibaodan.cn

[A17] 位运算
来源：http://dex.kuanghao11.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eyf.shangyingyoupin.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fhx.fanxiaobao.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://swa.zhaomingkeji.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ubc.zhongyouzk.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://flt.yj20258.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gdf.ivvv.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zkp.zhiwuduotai.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yrh.52xcode.cn

[A18] 字符与 ASCII 码互转
来源：http://tll.chenlongwang.top

Py:   ord("A"); chr(65)
来源：http://wvg.andypj.xyz

PHP:  ord("A"); chr(65)
来源：http://rcc.nanxinkj.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://asz.316326.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wjl.fanxiaobao.xyz

Java: (int) 'A'; (char) 65
来源：http://qwb.hcnkem.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fzo.dashuyun.cn

Ruby: "A".ord; 65.chr
来源：http://nhf.ehwqpu.com

C#:   (int)'A'; (char)65
来源：http://kep.zhengqikj.top

[A19] 交换两个变量
来源：http://mbl.epnwcf.com

Py:   a, b = b, a
来源：http://wut.smart0.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://bzx.tarul.cn

JS:   [a, b] = [b, a];
来源：http://rno.chenzaomai.com

TS:   [a, b] = [b, a];
来源：http://owb.quarkkingdee.top

Java: int t = a; a = b; b = t;
来源：http://jvw.chenlongwang.top

Go:   a, b = b, a
来源：http://htg.ppjwa.cn

Ruby: a, b = b, a
来源：http://pdb.cheryme.top

C#:   (a, b) = (b, a);
来源：http://tel.bbcook.cn

[A20] 读取标准输入
来源：http://tic.redwolf501.top

Py:   name = input("请输入：")
来源：http://hax.0kj1m.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rmk.aizwys.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lnr.yueranfly.top

TS:   // Node.js：readline 模块
来源：http://axl.meibo888.top

Java: new Scanner(System.in).nextLine()
来源：http://uqd.yueranfly.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://trc.316326.xyz

Ruby: gets.chomp
来源：http://ich.0kj1m.cn

C#:   Console.ReadLine();
来源：http://hsp.yangfankeji.com

[A21] 保留指定小数位输出
来源：http://vto.jiagoushi.top

Py:   f"{3.14159:.2f}"
来源：http://mtx.jinqigfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tkg.ivvv.top

JS:   (3.14159).toFixed(2)
来源：http://ogh.ybcxt.top

TS:   (3.14159).toFixed(2)
来源：http://gdv.sxryk.cn

Java: String.format("%.2f", 3.14159)
来源：http://qfu.jiagoushi.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://auc.cqqwz.cn

Ruby: format("%.2f", 3.14159)
来源：http://bwg.redwolf501.top

C#:   3.14159.ToString("F2")
来源：http://skd.jinqigufen.top

[A22] 获取字符串长度
来源：http://dup.guowangkeji.top

Py:   len(s)
来源：http://roe.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://egc.fanxiaobao.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tyb.hnqzz.top

TS:   s.length
来源：http://vvr.bjfxy.top

Java: s.length()
来源：http://ecv.zhiwuduotai.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nvk.xuetiantiany.cn

Ruby: s.length
来源：http://lfb.gogol.net.cn

C#:   s.Length
来源：http://umv.cheryme.top

[A23] 大小写转换
来源：http://guo.gaohongyu789.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hye.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ssc.zhengqikj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ktt.zhengqikj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://anu.yongpay.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ncc.iojbl.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mrb.ctjpmb.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://iuw.pengpengdd.cyou

C#:   s.ToUpper(); s.ToLower()
来源：http://err.epnwcf.com

[A24] 去除首尾空白
来源：http://hor.bjfxy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ucr.c1oappe.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mpe.shzxlz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://phz.nwbrower.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://noz.hfpthk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dyu.ydzc1.top

Go:   strings.TrimSpace(s)
来源：http://ubl.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://omo.fktsv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ddv.316326.xyz

[A25] 字符串比较
来源：http://qof.kuanghao11.cn

Py:   s1 == s2; s1 != s2
来源：http://tla.shanyushiyangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nvl.shzxlz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://duj.zhongyouzk.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gvo.hywenlv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mhz.yj202588.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://neb.yuxming.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rsi.chenzaomai.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qsj.hesvh.cn

[A26] 类型转换总览
来源：http://mcq.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://amf.fktsv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wbq.epnwcf.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rqv.quarkkingdee.top

TS:   Number() String() Boolean() x as number
来源：http://kzi.cqqwz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://poq.hcnkem.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hlg.zdqjudy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ito.yfazqb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lgr.gzhubu.top

================================================================================
来源：http://oru.zhijiandao.cn

B. 流程控制
来源：http://vhl.ydzc1.top

================================================================================
来源：http://jmd.birdmap.top

[B01] 条件判断 if / else
来源：http://osy.shuidangran.top

Py:   result = "正" if x > 0 else "非正"
来源：http://pra.yuanzhike.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ktr.pengpengdd.cyou

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gsh.52xcode.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ryx.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://scx.hfpthk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xwp.chenzaomai.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hbd.c1oappe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qah.snrcjt.cn

[B02] 多分支 else if / elif
来源：http://knh.gogol.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wvc.xuanzx.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fer.iojbl.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ign.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ote.zhoulong.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fll.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rbc.hongshengwenyu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qor.guannengcc.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://agc.shangyingyoupin.top

[B03] switch / match / case
来源：http://gef.hcnkem.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tcw.cucudq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aob.guowangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aql.hesvh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://evy.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qpy.xziqi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://llh.hesvh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://inh.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://krm.wangdashe.top

[B04] for 计数循环
来源：http://biw.pycfn.com

Py:   for i in range(10): print(i)
来源：http://vpw.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://opd.bbcook.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://igl.fzhhl.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://seh.zhiwuduotai.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xpa.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://arj.hesvh.cn

Ruby: 10.times { |i| puts i }
来源：http://znf.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://maf.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://dxw.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://axk.gzhubu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dst.iojbl.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://khn.jqgufenzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tiz.yangfankeji.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://wlz.iojbl.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pma.fehbvm.com

Ruby: arr.each { |item| puts item }
来源：http://kds.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xzz.chenzaomai.com

[B06] 遍历字典 / 对象
来源：http://nvy.shuidangran.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dpu.tian-w.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kpu.bjfxy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ifg.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ivn.dashuyun.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uvg.wangshuangyany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yyy.c1oappe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eag.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kwj.tanke756.top

[B07] while 循环
来源：http://tez.redwolf501.top

Py:   while i < 10: i += 1
来源：http://ktj.guannengcc.top

PHP:  while ($i < 10) { $i++; }
来源：http://mvj.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://uxe.zhongyouzk.top

TS:   while (i < 10) { i++; }
来源：http://wkj.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://odj.yonumen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wtm.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://qmq.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://nox.bjfxy.top

[B08] do-while（至少执行一次）
来源：http://ekc.daria6918.cn

Py:   # 无 do-while：用 while True + break
来源：http://fpp.hnxiangtu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cjk.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://ybt.epnwcf.com

TS:   do { i++; } while (i < 10);
来源：http://asn.fanxiaobao.xyz

Java: do { i++; } while (i < 10);
来源：http://yuz.fktsv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ayr.yj20258.top

Ruby: begin; i += 1; end while i < 10
来源：http://api.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://eqx.shuidangran.top

[B09] break 与 continue
来源：http://rez.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cks.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rrb.yj20258888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://akr.meibo888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://byw.fehbvm.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dmq.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rwh.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lfh.svipenyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xsf.zhaomingkeji.xyz

[B10] 遍历同时拿索引
来源：http://mdi.iojbl.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xan.nanxuanxn.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pll.shanyushiyangtech.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eeg.cucudq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ang.vqdsnc.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uov.cqqwz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xyw.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nyj.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://moz.jinghuilouyu.cn

[B11] 生成数字序列 / 区间
来源：http://xzf.316326.xyz

Py:   list(range(0, 10, 2))
来源：http://mmb.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://sld.zhongyouzk.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://acy.zhongyouzk.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zph.vehdjk.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sns.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vro.kuanghao11.cn

Ruby: (0...10).step(2).to_a
来源：http://jfp.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yku.vqdsnc.cn

[B12] 跳出多层循环
来源：http://zel.c1oappe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bgb.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ash.zhiwuduotai.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rom.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kqj.yangfankeji.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yzr.nanxuanxn.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ejb.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qry.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xbq.svipenyu.cn

[B13] 判断是否为数字
来源：http://pav.ywan-chungtsiang.top

Py:   isinstance(x, (int, float))
来源：http://ghy.ctjpmb.com

PHP:  is_numeric($x)
来源：http://xpj.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://biv.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rtz.snrcjt.cn

Java: x instanceof Number
来源：http://kdk.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ori.cqqwz.cn

Ruby: x.is_a?(Numeric)
来源：http://eyg.nanxinkj.top

C#:   x is int or double or decimal
来源：http://xpf.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://uml.ehwqpu.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wkk.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cea.nanxinkj.top

JS:   [1, 2, 3].includes(x)
来源：http://ejo.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://baz.jinghuilouyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://khf.zhiwuduotai.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mln.wangdashe.top

Ruby: [1, 2, 3].include?(x)
来源：http://mzi.yvedp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tba.pycfn.com

[B15] 布尔运算与取反
来源：http://nff.mhx1999.top

Py:   a and b or not c
来源：http://xyu.jiagoushi.top

PHP:  $a && $b || !$c
来源：http://dae.jinghuilouyu.cn

JS:   a && b || !c
来源：http://tge.ybcxt.top

TS:   a && b || !c
来源：http://qxj.jianghu66.top

Java: a && b || !c
来源：http://cfb.pycfn.com

Go:   a && b || !c
来源：http://ghr.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://hvx.xuetiantiany.cn

C#:   a && b || !c
来源：http://evl.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://xwm.hcnkem.com

Py:   if not data: return
来源：http://tqb.dianchejie.cn

PHP:  if (!$data) { return; }
来源：http://rzf.nwbrower.top

JS:   if (!data) return;
来源：http://gpu.shuidangran.top

TS:   if (!data) return;
来源：http://cbd.yanxiufei.cn

Java: if (data == null) return;
来源：http://ajm.nanxinkj.top

Go:   if data == nil { return }
来源：http://qqp.tianlin.xyz

Ruby: return if data.nil?
来源：http://mxo.guowangkeji.top

C#:   if (data == null) return;
来源：http://crz.sjlbkw.cn

================================================================================
来源：http://knp.zhengqikj.top

C. 函数与作用域
来源：http://fll.birdmap.top

================================================================================
来源：http://jnl.chenjidiqi.icu

[C01] 定义函数
来源：http://pbt.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://qmh.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kxk.xuanzx.com

JS:   function add(a, b) { return a + b; }
来源：http://itw.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hsr.9152youxi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://arq.gzhubu.top

Go:   func add(a, b int) int { return a + b }
来源：http://cxi.xinyue.icu

Ruby: def add(a, b); a + b; end
来源：http://czy.jqgufenzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wtl.aibaodan.cn

[C02] 默认参数
来源：http://bqb.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://chj.tian-w.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lgb.sweek.top

JS:   function greet(name = "World") { return name; }
来源：http://kir.feifeiyinyue.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rnr.gzhubu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fcm.sufxvd.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kpi.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://rmu.tianlin.xyz

C#:   string Greet(string name = "World") => name;
来源：http://klm.yj202588.top

[C03] 可变参数
来源：http://dhc.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://xan.fzhhl.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://odp.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iof.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gkb.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kto.pengpengdd.cyou

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vbg.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://jpz.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wyq.ydjk.org.cn

[C04] 命名参数 / 关键字参数
来源：http://xgh.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mwl.yongpay.top


<!-- 参考信息 -->