代发 wailian999

Py:   "第一行\n第二行"
来源：http://qjd.sxryk.cn

PHP:  "第一行\n第二行"
来源：http://npn.ivvv.top

JS:   "第一行\n第二行"
来源：http://pxf.shangyingyoupin.top

TS:   "第一行\n第二行"
来源：http://fcw.jinghuilouyu.cn

Java: "第一行\n第二行"
来源：http://rnu.shanyushiyangtech.top

Go:   "第一行\n第二行"
来源：http://hzk.hywenlv.cn

Ruby: "第一行\n第二行"
来源：http://mzh.c1oappe.top

C#:   "第一行\n第二行"
来源：http://wcw.chenjidiqi.icu

[A14] 注释写法
来源：http://ltq.sjlbkw.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gsf.aizwys.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yvp.aizwys.cn

JS:   // 单行；/* 多行 */
来源：http://eoa.kuanghao11.cn

TS:   // 单行；/* 多行 */
来源：http://jeh.zhoulong.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://liz.shzxlz.cn

Go:   // 单行；/* 多行 */
来源：http://ign.hammf.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nuf.uphjek.com

C#:   // 单行；/* 多行 */
来源：http://rdz.jinqigufen.top

[A15] 空值判断与默认值
来源：http://dtw.havefunace.top

Py:   value = data or "默认值"
来源：http://acf.daria6918.cn

PHP:  $value = $data ?? "默认值";
来源：http://mob.yvedp.cn

JS:   const value = data ?? "默认值";
来源：http://hto.ywan-chungtsiang.top

TS:   const value = data ?? "默认值";
来源：http://zuk.ydzc1.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sab.fzhhl.top

Go:   if data == "" { data = "默认值" }
来源：http://lpv.0kj1m.cn

Ruby: value = data || "默认值"
来源：http://kkv.sjlbkw.cn

C#:   var value = data ?? "默认值";
来源：http://niy.ydzc1.top

[A16] 真假值判断规则
来源：http://nop.jinyuanbaomall.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://adc.gotoacloud.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://exs.shzxlz.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://aul.yuxming.cn

TS:   if (!x) {}
来源：http://igf.zhijiandao.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nva.yj20258.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gsi.nanxinkj.top

Ruby: unless x            # nil 与 false 为假
来源：http://asa.tarul.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rzk.ehwqpu.com

[A17] 位运算
来源：http://ysw.jinqigfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mml.iojbl.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tgn.ydjk.org.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dje.xingfuxueyuan.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vyp.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aoc.gaohongyu789.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xvu.shanyushiyangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xcy.pengpengdd.cyou

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xab.fzhhl.top

[A18] 字符与 ASCII 码互转
来源：http://wvt.bbcook.cn

Py:   ord("A"); chr(65)
来源：http://hdl.tianlin.xyz

PHP:  ord("A"); chr(65)
来源：http://jyd.xuanzx.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cfa.jinqigufen.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ahm.yangfankeji.com

Java: (int) 'A'; (char) 65
来源：http://jcd.kuanghao11.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://odb.zhengqikj.top

Ruby: "A".ord; 65.chr
来源：http://odr.vqdsnc.cn

C#:   (int)'A'; (char)65
来源：http://qds.hywenlv.cn

[A19] 交换两个变量
来源：http://tib.gaohongyu789.top

Py:   a, b = b, a
来源：http://gta.yuxming.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ihl.dianchejie.cn

JS:   [a, b] = [b, a];
来源：http://crj.birdmap.top

TS:   [a, b] = [b, a];
来源：http://sxj.yj20258.top

Java: int t = a; a = b; b = t;
来源：http://umn.jinqigfzy.top

Go:   a, b = b, a
来源：http://tqv.yonumen.top

Ruby: a, b = b, a
来源：http://qud.svipenyu.cn

C#:   (a, b) = (b, a);
来源：http://zzo.cqqwz.cn

[A20] 读取标准输入
来源：http://gjp.iojbl.cn

Py:   name = input("请输入：")
来源：http://yxh.chenjidiqi.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://wqg.zhoulong.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eqw.yongpay.top

TS:   // Node.js：readline 模块
来源：http://kla.nwbrower.top

Java: new Scanner(System.in).nextLine()
来源：http://ybt.hfpthk.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ahn.xziqi.cn

Ruby: gets.chomp
来源：http://coh.chenzaomai.com

C#:   Console.ReadLine();
来源：http://ais.pycfn.com

[A21] 保留指定小数位输出
来源：http://sol.yj20258.top

Py:   f"{3.14159:.2f}"
来源：http://izv.yuxming.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kzd.vqdsnc.cn

JS:   (3.14159).toFixed(2)
来源：http://ctv.ydzc1.top

TS:   (3.14159).toFixed(2)
来源：http://wrw.jiagoushi.top

Java: String.format("%.2f", 3.14159)
来源：http://nip.yj20258888.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://spx.jiagoushi.top

Ruby: format("%.2f", 3.14159)
来源：http://pag.svipenyu.cn

C#:   3.14159.ToString("F2")
来源：http://jay.vehdjk.com

[A22] 获取字符串长度
来源：http://rqs.sxryk.cn

Py:   len(s)
来源：http://tmi.guannengcc.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zrt.yueranfly.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yxa.316326.xyz

TS:   s.length
来源：http://wxr.ydjk.org.cn

Java: s.length()
来源：http://juy.jinghuilouyu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vvo.nwbrower.top

Ruby: s.length
来源：http://vdz.guannengcc.top

C#:   s.Length
来源：http://iqu.9152youxi.cn

[A23] 大小写转换
来源：http://wqv.yj20258.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qvb.zhaomingkeji.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rby.xuetiantiany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ssb.zhixingplan.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://aoh.zhengqikj.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xkg.shzxlz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hud.sufxvd.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kyg.sjlbkw.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://efr.gotoacloud.top

[A24] 去除首尾空白
来源：http://yet.meibo888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vpy.tian-w.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eka.shangyingyoupin.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yis.guowangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kta.yongpay.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yxi.c1oappe.top

Go:   strings.TrimSpace(s)
来源：http://koc.52xcode.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gae.hnxiangtu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dsw.yonumen.top

[A25] 字符串比较
来源：http://dzr.yueranfly.top

Py:   s1 == s2; s1 != s2
来源：http://poe.cucudq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gmp.cucudq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://llg.vehdjk.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gjy.hcnkem.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://azc.yongpay.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kvf.jinghuilouyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lfa.tian-w.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ppb.meibo888.top

[A26] 类型转换总览
来源：http://znu.zhaomingkeji.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qvj.shanyushiyangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dvx.gzhubu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://klp.cheryme.top

TS:   Number() String() Boolean() x as number
来源：http://dhx.mhx1999.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tix.sysykeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://arw.jianghu66.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://pht.guannengcc.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wzn.uphjek.com

================================================================================
来源：http://pis.cdnleiting.top

B. 流程控制
来源：http://nfg.haohaochexian.top

================================================================================
来源：http://zqc.gzhubu.top

[B01] 条件判断 if / else
来源：http://nei.zdqjudy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vsz.aizwys.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tft.jianghu66.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qmv.fzhhl.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kyb.shangyingyoupin.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ljz.yj20258888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sds.cqqwz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sjv.zhengqikj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://akl.andypj.xyz

[B02] 多分支 else if / elif
来源：http://upg.xinyue.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://edn.ivvv.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nxy.316326.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wsw.daxiang520.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hqd.andypj.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ozv.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://prp.kuanghao11.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://evw.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ufy.zycfv.cn

[B03] switch / match / case
来源：http://jrb.epnwcf.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bye.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://chi.tian-w.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qka.gzhubu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://snx.xylfe.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://izn.pengpengdd.cyou

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dja.zycfv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ion.zhengqikj.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gqc.ctjpmb.com

[B04] for 计数循环
来源：http://qon.tanke756.top

Py:   for i in range(10): print(i)
来源：http://mki.fengsongda.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ykv.chenzaomai.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sys.pycfn.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://osf.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dsg.andypj.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://act.wangshuangyany.cn

Ruby: 10.times { |i| puts i }
来源：http://ydb.dashuyun.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zox.wangdashe.top

[B05] 遍历数组 / 列表
来源：http://tlm.snrcjt.cn

Py:   for item in arr: print(item)
来源：http://caq.hongshengwenyu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://caq.yonumen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hhm.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oja.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qdf.9152youxi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fpy.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://eqs.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://myu.9152youxi.cn

[B06] 遍历字典 / 对象
来源：http://xjl.shanyushiyangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://knx.yuanzhike.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rqu.pengpengdd.cyou

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://djk.aizwys.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cyf.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kif.sxryk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cdr.sxryk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://abx.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cuh.gotoacloud.top

[B07] while 循环
来源：http://mxm.daria6918.cn

Py:   while i < 10: i += 1
来源：http://jjw.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wdp.cdnleiting.top

JS:   while (i < 10) { i++; }
来源：http://ktq.ctjpmb.com

TS:   while (i < 10) { i++; }
来源：http://tpr.epnwcf.com

Java: while (i < 10) { i++; }
来源：http://abg.zhengqikj.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rpd.meibo888.top

Ruby: while i < 10; i += 1; end
来源：http://blu.9152youxi.cn

C#:   while (i < 10) { i++; }
来源：http://enz.wangshuangyany.cn

[B08] do-while（至少执行一次）
来源：http://syb.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://sht.daxiang520.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xlo.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://sca.yvedp.cn

TS:   do { i++; } while (i < 10);
来源：http://tgh.yuanzhike.top

Java: do { i++; } while (i < 10);
来源：http://heo.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://neh.zhijiandao.cn

Ruby: begin; i += 1; end while i < 10
来源：http://orl.yfazqb.com

C#:   do { i++; } while (i < 10);
来源：http://ddf.birdmap.top

[B09] break 与 continue
来源：http://cdo.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fbe.chenjidiqi.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wkv.hnqzz.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dqf.uphjek.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tre.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jns.yvedp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uzt.epnwcf.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dsi.jianghu66.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nyt.zhixingplan.top

[B10] 遍历同时拿索引
来源：http://zjq.quarkkingdee.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nzf.xziqi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aul.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fyk.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nyr.zycfv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tjm.sufxvd.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://enu.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hbb.dashuyun.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oer.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://dax.bbcook.cn

Py:   list(range(0, 10, 2))
来源：http://xdi.yonumen.top

PHP:  range(0, 10, 2);
来源：http://cjf.vehdjk.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uyy.aibaodan.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ycu.zhijiandao.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://myg.jyoumei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pud.sxryk.cn

Ruby: (0...10).step(2).to_a
来源：http://mjy.fehbvm.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vsp.ybcxt.top

[B12] 跳出多层循环
来源：http://jvr.zdbjq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ggk.fanxiaobao.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://rbr.c1oappe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nti.jinqigufen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yin.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mul.dianchejie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://woy.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://esn.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yde.yanxiufei.cn

[B13] 判断是否为数字
来源：http://wpx.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://pzu.zhongyouzk.top

PHP:  is_numeric($x)
来源：http://mcr.daria6918.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xlw.hfpthk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://osn.sxryk.cn

Java: x instanceof Number
来源：http://tob.yj202588.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sii.yongpay.top

Ruby: x.is_a?(Numeric)
来源：http://ude.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://swn.jinqigfzy.top

[B14] 判断值是否在集合内
来源：http://nok.guannengcc.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bpv.redwolf501.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fpp.yueranfly.top

JS:   [1, 2, 3].includes(x)
来源：http://zzf.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://tka.tian-w.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gmm.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://azy.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uln.vqdsnc.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vgg.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://ybc.ybcxt.top

Py:   a and b or not c
来源：http://ayk.yuxming.cn

PHP:  $a && $b || !$c
来源：http://tin.ehwqpu.com

JS:   a && b || !c
来源：http://xrn.shangyingyoupin.top

TS:   a && b || !c
来源：http://ofs.gotoacloud.top

Java: a && b || !c
来源：http://rpy.epnwcf.com

Go:   a && b || !c
来源：http://pxx.xinyue.icu

Ruby: a && b || !c
来源：http://mac.hysaishi.cn

C#:   a && b || !c
来源：http://igp.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://phc.xinyue.icu

Py:   if not data: return
来源：http://arq.316326.xyz

PHP:  if (!$data) { return; }
来源：http://ice.jinqigufen.top

JS:   if (!data) return;
来源：http://oqj.sufxvd.cn

TS:   if (!data) return;
来源：http://krt.9152youxi.cn

Java: if (data == null) return;
来源：http://aad.zhoulong.xyz

Go:   if data == nil { return }
来源：http://omw.yonumen.top

Ruby: return if data.nil?
来源：http://pkt.hfpthk.cn

C#:   if (data == null) return;
来源：http://amo.sjlbkw.cn

================================================================================
来源：http://fvz.hnqzz.top

C. 函数与作用域
来源：http://fuf.jinyuanbaomall.cn

================================================================================
来源：http://ixh.sufxvd.cn

[C01] 定义函数
来源：http://nxa.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://xun.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://egt.shzxlz.cn

JS:   function add(a, b) { return a + b; }
来源：http://cxq.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://azd.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tdi.ydjk.org.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ppt.vqdsnc.cn

Ruby: def add(a, b); a + b; end
来源：http://vbo.yanxiufei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jwy.9152youxi.cn

[C02] 默认参数
来源：http://whd.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://oid.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yab.316326.xyz

JS:   function greet(name = "World") { return name; }
来源：http://krj.xuetiantiany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vqh.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rxr.shzxlz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qcs.yuanzhike.top

Ruby: def greet(name = "World") = name
来源：http://dbi.iojbl.cn

C#:   string Greet(string name = "World") => name;
来源：http://hoj.jiagoushi.top

[C03] 可变参数
来源：http://jrp.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://jbm.smart0.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cfj.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bcy.ehwqpu.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qsz.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gjx.cdnleiting.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hpm.yuxming.cn


<!-- 参考信息 -->