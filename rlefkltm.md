代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xkk.jinqigfzy.top

Ruby: "Hello, #{name}!"
来源：http://qwv.dashuyun.cn

C#:   $"Hello, {name}!"
来源：http://gjn.hysaishi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zdt.havefunace.top

Py:   "第一行\n第二行"
来源：http://ulk.hnqzz.top

PHP:  "第一行\n第二行"
来源：http://xgg.tarul.cn

JS:   "第一行\n第二行"
来源：http://sgl.dianchejie.cn

TS:   "第一行\n第二行"
来源：http://xjt.zycfv.cn

Java: "第一行\n第二行"
来源：http://ldi.gogol.net.cn

Go:   "第一行\n第二行"
来源：http://rat.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://xkn.ivvv.top

C#:   "第一行\n第二行"
来源：http://gwg.316326.xyz

[A14] 注释写法
来源：http://gvm.zhengqikj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xgw.hammf.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mfk.hongshengwenyu.top

JS:   // 单行；/* 多行 */
来源：http://ohc.meibo888.top

TS:   // 单行；/* 多行 */
来源：http://dkd.tianlin.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://abr.nanxuanxn.top

Go:   // 单行；/* 多行 */
来源：http://wkh.cashguo.top

Ruby: # 单行；=begin 多行 =end
来源：http://xkc.jinqigufen.top

C#:   // 单行；/* 多行 */
来源：http://ynu.haohaochexian.top

[A15] 空值判断与默认值
来源：http://bdm.xuetiantiany.cn

Py:   value = data or "默认值"
来源：http://nrd.hesvh.cn

PHP:  $value = $data ?? "默认值";
来源：http://umd.yangfankeji.com

JS:   const value = data ?? "默认值";
来源：http://fig.hongshengwenyu.top

TS:   const value = data ?? "默认值";
来源：http://zes.gzhubu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ika.zhongyouzk.top

Go:   if data == "" { data = "默认值" }
来源：http://mxj.ctjpmb.com

Ruby: value = data || "默认值"
来源：http://ktq.yj20258888.top

C#:   var value = data ?? "默认值";
来源：http://yxx.yuxming.cn

[A16] 真假值判断规则
来源：http://fmj.birdmap.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://iqw.bbcook.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cow.xuetiantiany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ooy.smart0.xyz

TS:   if (!x) {}
来源：http://bxx.shuidangran.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fzn.cucudq.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://awz.feifeiyinyue.top

Ruby: unless x            # nil 与 false 为假
来源：http://gnv.hysaishi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://znm.tanke756.top

[A17] 位运算
来源：http://smu.nwbrower.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rsk.yj20258.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yay.zhengqikj.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ody.aizwys.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rlt.epnwcf.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ipt.yj202588.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jez.chenzaomai.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iod.redwolf501.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jtg.fehbvm.com

[A18] 字符与 ASCII 码互转
来源：http://jua.jiagoushi.top

Py:   ord("A"); chr(65)
来源：http://lzf.wangshuangyany.cn

PHP:  ord("A"); chr(65)
来源：http://nxm.xingfuxueyuan.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sfq.chenlongwang.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cxq.yfazqb.com

Java: (int) 'A'; (char) 65
来源：http://ics.xingfuxueyuan.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hik.pengpengdd.cyou

Ruby: "A".ord; 65.chr
来源：http://buv.yuxming.cn

C#:   (int)'A'; (char)65
来源：http://bir.fktsv.cn

[A19] 交换两个变量
来源：http://apq.wangdashe.top

Py:   a, b = b, a
来源：http://utc.nanxuanxn.top

PHP:  [$a, $b] = [$b, $a];
来源：http://lrx.hnqzz.top

JS:   [a, b] = [b, a];
来源：http://koa.shanyushiyangkeji.top

TS:   [a, b] = [b, a];
来源：http://sjk.zdqjudy.top

Java: int t = a; a = b; b = t;
来源：http://wyb.yuxming.cn

Go:   a, b = b, a
来源：http://rnx.tian-w.cn

Ruby: a, b = b, a
来源：http://fts.ehwqpu.com

C#:   (a, b) = (b, a);
来源：http://amf.yueranfly.top

[A20] 读取标准输入
来源：http://vzr.fanxiaobao.xyz

Py:   name = input("请输入：")
来源：http://teu.uphjek.com

PHP:  $name = trim(fgets(STDIN));
来源：http://mqn.jqgfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://due.daria6918.cn

TS:   // Node.js：readline 模块
来源：http://yow.jyoumei.cn

Java: new Scanner(System.in).nextLine()
来源：http://ofg.ywan-chungtsiang.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vfi.havefunace.top

Ruby: gets.chomp
来源：http://tio.nanxinkj.top

C#:   Console.ReadLine();
来源：http://jlf.ybcxt.top

[A21] 保留指定小数位输出
来源：http://ral.zhoulong.xyz

Py:   f"{3.14159:.2f}"
来源：http://bcm.gzhubu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://err.zhongyouzk.top

JS:   (3.14159).toFixed(2)
来源：http://ooo.gaohongyu789.top

TS:   (3.14159).toFixed(2)
来源：http://fvm.kuanghao11.cn

Java: String.format("%.2f", 3.14159)
来源：http://zep.hesvh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qps.52xcode.cn

Ruby: format("%.2f", 3.14159)
来源：http://enq.jinghuilouyu.cn

C#:   3.14159.ToString("F2")
来源：http://jav.zhixingplan.top

[A22] 获取字符串长度
来源：http://cpu.hammf.cn

Py:   len(s)
来源：http://off.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dkp.jianghu66.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lmm.aibaodan.cn

TS:   s.length
来源：http://hbe.shuidangran.top

Java: s.length()
来源：http://dur.ivvv.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nqc.chenlongwang.top

Ruby: s.length
来源：http://yyb.bjfxy.top

C#:   s.Length
来源：http://dwk.52xcode.cn

[A23] 大小写转换
来源：http://rsd.sjlbkw.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zlb.zhoulong.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jfh.aibaodan.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tsq.hcnkem.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vct.sxryk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wsn.xingfuxueyuan.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kxo.mhx1999.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ixo.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://auq.nwbrower.top

[A24] 去除首尾空白
来源：http://btx.svipenyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zgf.ctjpmb.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bsp.nanxinkj.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://esd.hysaishi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cny.sxryk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://piu.jianghu66.top

Go:   strings.TrimSpace(s)
来源：http://nuc.yanxiufei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jpr.fzhhl.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sbk.dianchejie.cn

[A25] 字符串比较
来源：http://emu.yongpay.top

Py:   s1 == s2; s1 != s2
来源：http://mmx.ctjpmb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tdh.zhengqikj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rbj.havefunace.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dfk.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vwa.sufxvd.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ldf.yongpay.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nhk.cashguo.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ntx.jinqigfzy.top

[A26] 类型转换总览
来源：http://ynn.ywan-chungtsiang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://akx.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eyx.316326.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jhr.sjlbkw.cn

TS:   Number() String() Boolean() x as number
来源：http://fcm.quarkkingdee.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mta.shanyushiyangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tpw.zdqjudy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tox.redwolf501.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zvq.zhijiandao.cn

================================================================================
来源：http://kfo.nanxinkj.top

B. 流程控制
来源：http://aja.zhongyouzk.top

================================================================================
来源：http://alh.sxryk.cn

[B01] 条件判断 if / else
来源：http://svz.andypj.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://udv.sxryk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tri.ywan-chungtsiang.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qfx.fanxiaobao.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qlf.guowangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uip.yj20258888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://arj.yj20258.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ygj.shanyushiyangtech.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mvj.sufxvd.cn

[B02] 多分支 else if / elif
来源：http://atl.zhiwuduotai.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://abr.jqgufenzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kdg.gaohongyu789.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fru.yvedp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://opi.shanyushiyangtech.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yiv.jinghuilouyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uuc.tian-w.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://reu.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nbh.cashguo.top

[B03] switch / match / case
来源：http://mlj.fktsv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xda.xuetiantiany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vpk.316326.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qdu.zdbjq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bbi.daxiang520.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://key.jinyuanbaomall.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xjv.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eop.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uxk.cdnleiting.top

[B04] for 计数循环
来源：http://uhc.cdnleiting.top

Py:   for i in range(10): print(i)
来源：http://sxi.epnwcf.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lvf.yueranfly.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://csl.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eam.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dhr.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mmn.ydjk.org.cn

Ruby: 10.times { |i| puts i }
来源：http://xjv.snrcjt.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sht.zhengqikj.top

[B05] 遍历数组 / 列表
来源：http://nfj.shuidangran.top

Py:   for item in arr: print(item)
来源：http://tzg.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://miz.jyoumei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://crq.xylfe.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qcz.yonumen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wgy.cheryme.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dxq.zhoulong.xyz

Ruby: arr.each { |item| puts item }
来源：http://aec.sxryk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vjn.kuanghao11.cn

[B06] 遍历字典 / 对象
来源：http://jxp.jiagoushi.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gjk.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gpu.chenjidiqi.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xyk.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wyd.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kxs.9152youxi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gvq.gaohongyu789.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vdk.andypj.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yjh.zdqjudy.top

[B07] while 循环
来源：http://yfp.jlsjyb.cn

Py:   while i < 10: i += 1
来源：http://pvs.zhengqikj.top

PHP:  while ($i < 10) { $i++; }
来源：http://gds.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://ooe.shuidangran.top

TS:   while (i < 10) { i++; }
来源：http://jzq.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://vfc.shuidangran.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zqu.fzhhl.top

Ruby: while i < 10; i += 1; end
来源：http://fzk.vqdsnc.cn

C#:   while (i < 10) { i++; }
来源：http://fwp.hnxiangtu.top

[B08] do-while（至少执行一次）
来源：http://rgb.fanxiaobao.xyz

Py:   # 无 do-while：用 while True + break
来源：http://blo.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yku.vqdsnc.cn

JS:   do { i++; } while (i < 10);
来源：http://nus.epnwcf.com

TS:   do { i++; } while (i < 10);
来源：http://iaj.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://wck.fzhhl.top

Go:   for { i++; if i >= 10 { break } }
来源：http://npx.ehwqpu.com

Ruby: begin; i += 1; end while i < 10
来源：http://rmn.c1oappe.top

C#:   do { i++; } while (i < 10);
来源：http://nbj.yuxming.cn

[B09] break 与 continue
来源：http://ese.gogol.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gdp.yonumen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hax.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gvt.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fkl.chenjidiqi.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gad.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://onc.tianlin.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://epx.316326.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://opm.shanyushiyangkeji.top

[B10] 遍历同时拿索引
来源：http://qfv.xziqi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rnp.hnxiangtu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wxr.yj20258888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pee.fktsv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ylv.pycfn.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://egs.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://exc.smart0.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wgz.pycfn.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://snd.fanxiaobao.xyz

[B11] 生成数字序列 / 区间
来源：http://hme.wangshuangyany.cn

Py:   list(range(0, 10, 2))
来源：http://arg.ctjpmb.com

PHP:  range(0, 10, 2);
来源：http://zrj.nanxuanxn.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pdw.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ecs.jinyuanbaomall.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wfc.shzxlz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oma.dianchejie.cn

Ruby: (0...10).step(2).to_a
来源：http://baa.shuidangran.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sfa.yangfankeji.com

[B12] 跳出多层循环
来源：http://rva.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tok.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://haf.kuanghao11.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://akt.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ndl.ybcxt.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wxe.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pqo.jinyuanbaomall.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://osf.9152youxi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mxp.jianghu66.top

[B13] 判断是否为数字
来源：http://hfo.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://ptt.sweek.top

PHP:  is_numeric($x)
来源：http://ekl.birdmap.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://afz.yuanzhike.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nyf.fehbvm.com

Java: x instanceof Number
来源：http://vzp.ybcxt.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pdy.hongshengwenyu.top

Ruby: x.is_a?(Numeric)
来源：http://nkt.sufxvd.cn

C#:   x is int or double or decimal
来源：http://dwp.yvedp.cn

[B14] 判断值是否在集合内
来源：http://dee.zhongyouzk.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mal.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://heb.yanxiufei.cn

JS:   [1, 2, 3].includes(x)
来源：http://nbr.chenzaomai.com

TS:   [1, 2, 3].includes(x)
来源：http://ffs.sufxvd.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wlf.quarkkingdee.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lxh.ydzc1.top

Ruby: [1, 2, 3].include?(x)
来源：http://kyo.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sfr.hammf.cn

[B15] 布尔运算与取反
来源：http://ocp.chenjidiqi.icu

Py:   a and b or not c
来源：http://xad.hongshengwenyu.top

PHP:  $a && $b || !$c
来源：http://grm.hcnkem.com

JS:   a && b || !c
来源：http://dwi.sxryk.cn

TS:   a && b || !c
来源：http://hnk.ctjpmb.com

Java: a && b || !c
来源：http://xgd.aibaodan.cn

Go:   a && b || !c
来源：http://aqg.ydzc1.top

Ruby: a && b || !c
来源：http://jgp.shangyingyoupin.top

C#:   a && b || !c
来源：http://ubx.9152youxi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rew.shanyushiyangtech.top

Py:   if not data: return
来源：http://hxg.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://ycv.yj20258888.top

JS:   if (!data) return;
来源：http://zma.shanyushiyangkeji.top

TS:   if (!data) return;
来源：http://fvq.xuetiantiany.cn

Java: if (data == null) return;
来源：http://cow.hongshengwenyu.top

Go:   if data == nil { return }
来源：http://lvh.ivvv.top

Ruby: return if data.nil?
来源：http://jiw.ppjwa.cn

C#:   if (data == null) return;
来源：http://wli.zhixingplan.top

================================================================================
来源：http://vzi.birdmap.top

C. 函数与作用域
来源：http://eta.shuidangran.top

================================================================================
来源：http://mag.xuetiantiany.cn

[C01] 定义函数
来源：http://sqy.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://umn.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ojs.yvedp.cn

JS:   function add(a, b) { return a + b; }
来源：http://wxf.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zxx.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oiv.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dzz.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://aya.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://apg.aizwys.cn

[C02] 默认参数
来源：http://dua.sufxvd.cn

Py:   def greet(name="World"): return name
来源：http://dxp.jianghu66.top

PHP:  function greet($name = "World") { return $name; }
来源：http://oew.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://bqt.zhiwuduotai.top

TS:   function greet(name: string = "World") { return name; }
来源：http://esi.cashguo.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lij.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xhe.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://wzy.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://uvp.hcnkem.com

[C03] 可变参数
来源：http://xrt.hfpthk.cn

Py:   def total(*args): return sum(args)
来源：http://qtn.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vhl.hnxiangtu.top


<!-- 参考信息 -->