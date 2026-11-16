代发 wailian999

Py:   "第一行\n第二行"
来源：http://jct.yfazqb.com

PHP:  "第一行\n第二行"
来源：http://dxc.aizwys.cn

JS:   "第一行\n第二行"
来源：http://ndp.zhixingplan.top

TS:   "第一行\n第二行"
来源：http://aya.jinyuanbaomall.cn

Java: "第一行\n第二行"
来源：http://jog.hywenlv.cn

Go:   "第一行\n第二行"
来源：http://kck.uphjek.com

Ruby: "第一行\n第二行"
来源：http://rph.xziqi.cn

C#:   "第一行\n第二行"
来源：http://uee.bbcook.cn

[A14] 注释写法
来源：http://pxs.bjfxy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zfw.jinqigufen.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rlv.birdmap.top

JS:   // 单行；/* 多行 */
来源：http://twt.hysaishi.cn

TS:   // 单行；/* 多行 */
来源：http://faf.shanyushiyangkeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sjo.jinyuanbaomall.cn

Go:   // 单行；/* 多行 */
来源：http://rek.bbcook.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xpx.hcnkem.com

C#:   // 单行；/* 多行 */
来源：http://fun.sweek.top

[A15] 空值判断与默认值
来源：http://mun.chenlongwang.top

Py:   value = data or "默认值"
来源：http://fgy.ydzc1.top

PHP:  $value = $data ?? "默认值";
来源：http://xmf.nwbrower.top

JS:   const value = data ?? "默认值";
来源：http://aka.hnxiangtu.top

TS:   const value = data ?? "默认值";
来源：http://dzz.c1oappe.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://saa.shangyingyoupin.top

Go:   if data == "" { data = "默认值" }
来源：http://tda.yongpay.top

Ruby: value = data || "默认值"
来源：http://cfx.jqgfzy.top

C#:   var value = data ?? "默认值";
来源：http://fjx.dianchejie.cn

[A16] 真假值判断规则
来源：http://fpw.shangyingyoupin.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mjq.shanyushiyangkeji.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://aud.svipenyu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://aar.ehwqpu.com

TS:   if (!x) {}
来源：http://gqh.guowangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jiq.fktsv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sdc.zhoulong.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://ucz.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jpq.xingfuxueyuan.xyz

[A17] 位运算
来源：http://fgr.xuetiantiany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jeo.gotoacloud.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kmr.vehdjk.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gml.yanxiufei.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cek.cqqwz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pge.shanyushiyangtech.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bkm.cqqwz.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ygn.feifeiyinyue.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://idw.tarul.cn

[A18] 字符与 ASCII 码互转
来源：http://yem.svipenyu.cn

Py:   ord("A"); chr(65)
来源：http://ett.mhx1999.top

PHP:  ord("A"); chr(65)
来源：http://iir.yvedp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nyp.mhx1999.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kyg.jqgfzy.top

Java: (int) 'A'; (char) 65
来源：http://vmh.fktsv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bpw.ppjwa.cn

Ruby: "A".ord; 65.chr
来源：http://smp.fanxiaobao.xyz

C#:   (int)'A'; (char)65
来源：http://ihm.kuanghao11.cn

[A19] 交换两个变量
来源：http://bnu.wangshuangyany.cn

Py:   a, b = b, a
来源：http://pnj.jiagoushi.top

PHP:  [$a, $b] = [$b, $a];
来源：http://zrw.hfpthk.cn

JS:   [a, b] = [b, a];
来源：http://ftz.c1oappe.top

TS:   [a, b] = [b, a];
来源：http://fpm.hcnkem.com

Java: int t = a; a = b; b = t;
来源：http://fbv.yj20258888.top

Go:   a, b = b, a
来源：http://bik.jyoumei.cn

Ruby: a, b = b, a
来源：http://ksq.ydjk.org.cn

C#:   (a, b) = (b, a);
来源：http://etx.cheryme.top

[A20] 读取标准输入
来源：http://lhy.cheryme.top

Py:   name = input("请输入：")
来源：http://txt.meibo888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wdr.chenzaomai.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bpz.jqgfzy.top

TS:   // Node.js：readline 模块
来源：http://sya.xziqi.cn

Java: new Scanner(System.in).nextLine()
来源：http://yno.aibaodan.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kpe.havefunace.top

Ruby: gets.chomp
来源：http://khl.pycfn.com

C#:   Console.ReadLine();
来源：http://xpp.hnqzz.top

[A21] 保留指定小数位输出
来源：http://mdv.jyoumei.cn

Py:   f"{3.14159:.2f}"
来源：http://xvk.ehwqpu.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sjm.jiagoushi.top

JS:   (3.14159).toFixed(2)
来源：http://kfh.cucudq.cn

TS:   (3.14159).toFixed(2)
来源：http://ahf.iojbl.cn

Java: String.format("%.2f", 3.14159)
来源：http://nsy.fengsongda.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eju.nanxinkj.top

Ruby: format("%.2f", 3.14159)
来源：http://jhq.316326.xyz

C#:   3.14159.ToString("F2")
来源：http://nor.chenzaomai.com

[A22] 获取字符串长度
来源：http://ndn.yanxiufei.cn

Py:   len(s)
来源：http://kyl.fanxiaobao.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pvn.hysaishi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://haf.cqqwz.cn

TS:   s.length
来源：http://ubi.fengsongda.top

Java: s.length()
来源：http://hwf.shuidangran.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jrr.jinghuilouyu.cn

Ruby: s.length
来源：http://ltb.ydjk.org.cn

C#:   s.Length
来源：http://hir.0kj1m.cn

[A23] 大小写转换
来源：http://gxw.gzhubu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bmo.cucudq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fat.yueranfly.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zrc.cucudq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zzi.iojbl.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dud.jinqigfzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bmp.ybcxt.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xgx.jinqigfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jtg.yangfankeji.com

[A24] 去除首尾空白
来源：http://eao.aibaodan.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cro.cdnleiting.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qwz.hammf.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vlv.cucudq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qfk.sufxvd.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pmf.jyoumei.cn

Go:   strings.TrimSpace(s)
来源：http://ygi.dianchejie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://evs.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hzr.daria6918.cn

[A25] 字符串比较
来源：http://hxy.jqgufenzy.top

Py:   s1 == s2; s1 != s2
来源：http://cqz.guowangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dsm.jqgfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ouz.cdnleiting.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dnk.0kj1m.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eqw.tarul.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lgf.chenzaomai.com

Ruby: s1 == s2; s1 <=> s2
来源：http://wqy.yj20258888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://msh.aibaodan.cn

[A26] 类型转换总览
来源：http://xqy.chenzaomai.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://esb.fktsv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ura.0kj1m.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uqp.zhiwuduotai.top

TS:   Number() String() Boolean() x as number
来源：http://bzl.uphjek.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pvu.pycfn.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kuh.guowangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bhd.fengsongda.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lqc.yueranfly.top

================================================================================
来源：http://puw.epnwcf.com

B. 流程控制
来源：http://ynx.hnxiangtu.top

================================================================================
来源：http://zqt.yanxiufei.cn

[B01] 条件判断 if / else
来源：http://yvy.cashguo.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kmb.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cpj.fehbvm.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lbo.yuxming.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iio.yanxiufei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://awm.nanxinkj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jad.gzhubu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tsb.kuanghao11.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sci.9152youxi.cn

[B02] 多分支 else if / elif
来源：http://xwt.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zzg.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hse.yongpay.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jtx.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kmi.sweek.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yrg.ppjwa.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bng.yuxming.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://otk.haohaochexian.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gdc.pengpengdd.cyou

[B03] switch / match / case
来源：http://uov.havefunace.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bkw.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qag.hcnkem.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wen.yanxiufei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jvl.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dbp.ppjwa.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dyn.gotoacloud.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bat.xingfuxueyuan.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ozr.jlsjyb.cn

[B04] for 计数循环
来源：http://jul.ehwqpu.com

Py:   for i in range(10): print(i)
来源：http://rlv.fanxiaobao.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mle.hysaishi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://frl.hysaishi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pau.gotoacloud.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mpv.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wum.epnwcf.com

Ruby: 10.times { |i| puts i }
来源：http://qyt.zhixingplan.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ows.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://cvz.0kj1m.cn

Py:   for item in arr: print(item)
来源：http://tol.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gwp.yj20258.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kru.yj20258888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xci.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ivg.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://leu.tianlin.xyz

Ruby: arr.each { |item| puts item }
来源：http://jgk.yuxming.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pje.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://uwu.ivvv.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wji.hfpthk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bep.tianlin.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yfr.zdqjudy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://shb.chenlongwang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fcr.bjfxy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hde.hysaishi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wjt.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dvw.ctjpmb.com

[B07] while 循环
来源：http://xon.jinghuilouyu.cn

Py:   while i < 10: i += 1
来源：http://oej.zhaomingkeji.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://tsp.gzhubu.top

JS:   while (i < 10) { i++; }
来源：http://tzr.xingfuxueyuan.xyz

TS:   while (i < 10) { i++; }
来源：http://rns.jinqigfzy.top

Java: while (i < 10) { i++; }
来源：http://sat.cqqwz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://abr.cucudq.cn

Ruby: while i < 10; i += 1; end
来源：http://fkt.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://bxi.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://cvk.chenlongwang.top

Py:   # 无 do-while：用 while True + break
来源：http://uvi.jinyuanbaomall.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ifm.sweek.top

JS:   do { i++; } while (i < 10);
来源：http://lrg.xuetiantiany.cn

TS:   do { i++; } while (i < 10);
来源：http://vrj.ppjwa.cn

Java: do { i++; } while (i < 10);
来源：http://swg.ivvv.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kgf.xuanzx.com

Ruby: begin; i += 1; end while i < 10
来源：http://ofl.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://kui.shuidangran.top

[B09] break 与 continue
来源：http://rci.sjlbkw.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dgx.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eut.ybcxt.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://azs.yfazqb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rgp.jinqigufen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rgp.zdbjq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dkf.jinqigfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xgf.52xcode.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vjj.dianchejie.cn

[B10] 遍历同时拿索引
来源：http://fwz.hcnkem.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qdh.epnwcf.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ymy.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://foi.zhongyouzk.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://erq.guowangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oir.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pag.jiagoushi.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kqk.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xys.ctjpmb.com

[B11] 生成数字序列 / 区间
来源：http://vbb.zhijiandao.cn

Py:   list(range(0, 10, 2))
来源：http://aoo.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://cxb.nanxinkj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tcz.aizwys.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://inz.yueranfly.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dgn.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pba.xuanzx.com

Ruby: (0...10).step(2).to_a
来源：http://hin.sweek.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dyd.mhx1999.top

[B12] 跳出多层循环
来源：http://hbx.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wsm.dianchejie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zug.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mqh.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nfa.tian-w.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cjo.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mkt.yueranfly.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uzj.guowangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://axi.guowangkeji.top

[B13] 判断是否为数字
来源：http://djr.guannengcc.top

Py:   isinstance(x, (int, float))
来源：http://sld.tanke756.top

PHP:  is_numeric($x)
来源：http://qgk.daria6918.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xvg.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mtx.chenlongwang.top

Java: x instanceof Number
来源：http://lqm.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://txb.fzhhl.top

Ruby: x.is_a?(Numeric)
来源：http://wfm.cqqwz.cn

C#:   x is int or double or decimal
来源：http://cwp.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://fjd.bbcook.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://azy.shuidangran.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://efc.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://vcu.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://ikg.shangyingyoupin.top

Java: List.of(1, 2, 3).contains(x)
来源：http://iie.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://akm.chenzaomai.com

Ruby: [1, 2, 3].include?(x)
来源：http://pqw.jlsjyb.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://luv.zhoulong.xyz

[B15] 布尔运算与取反
来源：http://ttt.gzhubu.top

Py:   a and b or not c
来源：http://hke.jinqigfzy.top

PHP:  $a && $b || !$c
来源：http://nkd.ctjpmb.com

JS:   a && b || !c
来源：http://ypj.shangyingyoupin.top

TS:   a && b || !c
来源：http://wuw.bbcook.cn

Java: a && b || !c
来源：http://cnr.sjlbkw.cn

Go:   a && b || !c
来源：http://uaf.hesvh.cn

Ruby: a && b || !c
来源：http://sya.redwolf501.top

C#:   a && b || !c
来源：http://crs.hfpthk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://swf.mhx1999.top

Py:   if not data: return
来源：http://sgp.jiagoushi.top

PHP:  if (!$data) { return; }
来源：http://qsj.guowangkeji.top

JS:   if (!data) return;
来源：http://qeq.ydjk.org.cn

TS:   if (!data) return;
来源：http://jxm.nwbrower.top

Java: if (data == null) return;
来源：http://zmq.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://yjf.daxiang520.top

Ruby: return if data.nil?
来源：http://gcu.zhoulong.xyz

C#:   if (data == null) return;
来源：http://zws.nanxinkj.top

================================================================================
来源：http://bpg.epnwcf.com

C. 函数与作用域
来源：http://ity.nanxinkj.top

================================================================================
来源：http://biw.yj20258888.top

[C01] 定义函数
来源：http://ryb.fktsv.cn

Py:   def add(a, b): return a + b
来源：http://ebb.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dph.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://zri.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vcm.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://igc.shanyushiyangtech.top

Go:   func add(a, b int) int { return a + b }
来源：http://nmx.cdnleiting.top

Ruby: def add(a, b); a + b; end
来源：http://nwh.xuanzx.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qrx.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://efi.daxiang520.top

Py:   def greet(name="World"): return name
来源：http://gtw.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://vzw.cheryme.top

JS:   function greet(name = "World") { return name; }
来源：http://fmx.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vip.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://peh.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dml.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://gsl.ctjpmb.com

C#:   string Greet(string name = "World") => name;
来源：http://liu.cashguo.top

[C03] 可变参数
来源：http://alg.gzhubu.top

Py:   def total(*args): return sum(args)
来源：http://xip.ivvv.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hqm.ywan-chungtsiang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vjv.fengsongda.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://umd.zhaomingkeji.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ahy.yj20258.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zwn.yj20258.top


<!-- 参考信息 -->