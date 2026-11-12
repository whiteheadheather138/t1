代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oom.316326.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hfn.yonumen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qck.jqgufenzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://aaf.havefunace.top

[A10] 生成随机数
来源：http://xmx.9152youxi.cn

Py:   import random; random.randint(1, 100)
来源：http://csr.zhixingplan.top

PHP:  random_int(1, 100);
来源：http://kfn.zhixingplan.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wcl.dashuyun.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rwq.zhiwuduotai.top

Java: new Random().nextInt(100) + 1
来源：http://kzn.jyoumei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zbt.ydjk.org.cn

Ruby: rand(1..100)
来源：http://ydr.gaohongyu789.top

C#:   new Random().Next(1, 101)
来源：http://rnq.sysykeji.top

[A11] 条件表达式（三元）
来源：http://xwx.mhx1999.top

Py:   "yes" if x > 0 else "no"
来源：http://ldc.cucudq.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zzk.nwbrower.top

JS:   x > 0 ? "yes" : "no"
来源：http://vze.tian-w.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rrq.cheryme.top

Java: x > 0 ? "yes" : "no"
来源：http://sdm.vqdsnc.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rcz.pycfn.com

Ruby: x > 0 ? "yes" : "no"
来源：http://xhd.yfazqb.com

C#:   x > 0 ? "yes" : "no"
来源：http://hxo.ybcxt.top

[A12] 字符串插值 / 格式化
来源：http://mgu.yj20258.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bcd.sjlbkw.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ppu.dianchejie.cn

JS:   `Hello, ${name}!`
来源：http://kdz.redwolf501.top

TS:   `Hello, ${name}!`
来源：http://uep.ybcxt.top

Java: "Hello, %s!".formatted(name)
来源：http://uva.vehdjk.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cyu.yueranfly.top

Ruby: "Hello, #{name}!"
来源：http://xul.pengpengdd.cyou

C#:   $"Hello, {name}!"
来源：http://ywo.fktsv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bqv.jinqigfzy.top

Py:   "第一行\n第二行"
来源：http://kij.yongpay.top

PHP:  "第一行\n第二行"
来源：http://vdj.fanxiaobao.xyz

JS:   "第一行\n第二行"
来源：http://exl.dianchejie.cn

TS:   "第一行\n第二行"
来源：http://mtr.yueranfly.top

Java: "第一行\n第二行"
来源：http://seh.zhijiandao.cn

Go:   "第一行\n第二行"
来源：http://cet.shangyingyoupin.top

Ruby: "第一行\n第二行"
来源：http://flf.iojbl.cn

C#:   "第一行\n第二行"
来源：http://pyf.zhengqikj.top

[A14] 注释写法
来源：http://ugv.chenjidiqi.icu

Py:   # 单行；三引号字符串可作多行说明
来源：http://fks.hysaishi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://smr.hfpthk.cn

JS:   // 单行；/* 多行 */
来源：http://jtw.jinghuilouyu.cn

TS:   // 单行；/* 多行 */
来源：http://ukj.mhx1999.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oyp.sufxvd.cn

Go:   // 单行；/* 多行 */
来源：http://blf.tianlin.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://qya.guowangkeji.top

C#:   // 单行；/* 多行 */
来源：http://jma.nanxinkj.top

[A15] 空值判断与默认值
来源：http://zvp.iojbl.cn

Py:   value = data or "默认值"
来源：http://eeb.ywan-chungtsiang.top

PHP:  $value = $data ?? "默认值";
来源：http://get.svipenyu.cn

JS:   const value = data ?? "默认值";
来源：http://voq.wangshuangyany.cn

TS:   const value = data ?? "默认值";
来源：http://mvv.daria6918.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ali.nanxinkj.top

Go:   if data == "" { data = "默认值" }
来源：http://kna.uphjek.com

Ruby: value = data || "默认值"
来源：http://awa.xinyue.icu

C#:   var value = data ?? "默认值";
来源：http://vdq.shzxlz.cn

[A16] 真假值判断规则
来源：http://ejq.feifeiyinyue.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://otl.zdqjudy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vnc.feifeiyinyue.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rqp.jlsjyb.cn

TS:   if (!x) {}
来源：http://gqc.zdbjq.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bcj.ppjwa.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ohv.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://uzk.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oqq.uphjek.com

[A17] 位运算
来源：http://ymg.gogol.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pbc.shanyushiyangkeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vwv.yj20258.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dfp.ctjpmb.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zwu.guannengcc.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iyu.ivvv.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://aco.sysykeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ezg.pengpengdd.cyou

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vka.uphjek.com

[A18] 字符与 ASCII 码互转
来源：http://iow.sxryk.cn

Py:   ord("A"); chr(65)
来源：http://ysv.zhijiandao.cn

PHP:  ord("A"); chr(65)
来源：http://aej.yangfankeji.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iuf.xziqi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fsl.fktsv.cn

Java: (int) 'A'; (char) 65
来源：http://kcf.ywan-chungtsiang.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gog.ctjpmb.com

Ruby: "A".ord; 65.chr
来源：http://gse.jyoumei.cn

C#:   (int)'A'; (char)65
来源：http://ssg.uphjek.com

[A19] 交换两个变量
来源：http://igp.hfpthk.cn

Py:   a, b = b, a
来源：http://yae.xylfe.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pdy.wangshuangyany.cn

JS:   [a, b] = [b, a];
来源：http://pev.ivvv.top

TS:   [a, b] = [b, a];
来源：http://brh.dianchejie.cn

Java: int t = a; a = b; b = t;
来源：http://sai.zhiwuduotai.top

Go:   a, b = b, a
来源：http://lfc.sjlbkw.cn

Ruby: a, b = b, a
来源：http://asf.aizwys.cn

C#:   (a, b) = (b, a);
来源：http://cky.pycfn.com

[A20] 读取标准输入
来源：http://jwh.shuidangran.top

Py:   name = input("请输入：")
来源：http://qrv.52xcode.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://aog.xziqi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kdi.nwbrower.top

TS:   // Node.js：readline 模块
来源：http://kqc.0kj1m.cn

Java: new Scanner(System.in).nextLine()
来源：http://rpn.316326.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vyn.zhixingplan.top

Ruby: gets.chomp
来源：http://xdp.ydjk.org.cn

C#:   Console.ReadLine();
来源：http://keg.epnwcf.com

[A21] 保留指定小数位输出
来源：http://oni.havefunace.top

Py:   f"{3.14159:.2f}"
来源：http://wta.yuxming.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mxf.gotoacloud.top

JS:   (3.14159).toFixed(2)
来源：http://lla.fehbvm.com

TS:   (3.14159).toFixed(2)
来源：http://wqq.yueranfly.top

Java: String.format("%.2f", 3.14159)
来源：http://ppc.jinyuanbaomall.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nka.chenjidiqi.icu

Ruby: format("%.2f", 3.14159)
来源：http://xhn.shangyingyoupin.top

C#:   3.14159.ToString("F2")
来源：http://auy.jqgufenzy.top

[A22] 获取字符串长度
来源：http://slk.shanyushiyangtech.top

Py:   len(s)
来源：http://iie.jqgfzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://edd.dashuyun.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tko.andypj.xyz

TS:   s.length
来源：http://mez.redwolf501.top

Java: s.length()
来源：http://xri.yonumen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sbr.bjfxy.top

Ruby: s.length
来源：http://xhy.hammf.cn

C#:   s.Length
来源：http://kci.yfazqb.com

[A23] 大小写转换
来源：http://hxs.daria6918.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hkk.birdmap.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rxr.feifeiyinyue.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://orc.gotoacloud.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://now.yueranfly.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mho.pycfn.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wjv.chenlongwang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dnw.quarkkingdee.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ecd.zdqjudy.top

[A24] 去除首尾空白
来源：http://qpn.fzhhl.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://khe.9152youxi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wzt.zycfv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://izo.yfazqb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jxj.yangfankeji.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fat.yfazqb.com

Go:   strings.TrimSpace(s)
来源：http://jct.sjlbkw.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ucb.gzhubu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gln.ehwqpu.com

[A25] 字符串比较
来源：http://tly.ybcxt.top

Py:   s1 == s2; s1 != s2
来源：http://voo.jlsjyb.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uid.birdmap.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oay.yueranfly.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dau.9152youxi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://unq.yj202588.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jra.zdbjq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xxi.chenzaomai.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zon.hongshengwenyu.top

[A26] 类型转换总览
来源：http://awe.jinqigfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cld.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fkn.nanxinkj.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mge.ywan-chungtsiang.top

TS:   Number() String() Boolean() x as number
来源：http://gra.jianghu66.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rrr.9152youxi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hne.birdmap.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vfw.tanke756.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cgi.dashuyun.cn

================================================================================
来源：http://mmp.hnxiangtu.top

B. 流程控制
来源：http://kdr.wangshuangyany.cn

================================================================================
来源：http://ujq.zycfv.cn

[B01] 条件判断 if / else
来源：http://edb.gzhubu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mvv.sufxvd.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kcq.wangshuangyany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ajh.havefunace.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qrn.jyoumei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sni.wangdashe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gvs.shzxlz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sah.hfpthk.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://isq.tarul.cn

[B02] 多分支 else if / elif
来源：http://kyg.ywan-chungtsiang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ixg.yfazqb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tem.bbcook.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sxq.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ohk.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cdp.fehbvm.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://squ.shuidangran.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ije.ywan-chungtsiang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wnq.gogol.net.cn

[B03] switch / match / case
来源：http://fty.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hxj.yongpay.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://czx.ydjk.org.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tbj.cdnleiting.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://knx.hysaishi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ofe.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bru.vehdjk.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vte.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rag.52xcode.cn

[B04] for 计数循环
来源：http://xrw.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://bjy.sysykeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iil.aizwys.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ulf.jinqigufen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fwz.xingfuxueyuan.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ldw.yongpay.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hpu.ydzc1.top

Ruby: 10.times { |i| puts i }
来源：http://yvg.0kj1m.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jan.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://nag.mhx1999.top

Py:   for item in arr: print(item)
来源：http://vux.kuanghao11.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://akq.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nud.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nzw.bbcook.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sjt.jyoumei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nib.jianghu66.top

Ruby: arr.each { |item| puts item }
来源：http://fmg.yvedp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xpt.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://fnl.tian-w.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yhj.shanyushiyangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pls.sufxvd.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rwo.sxryk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qua.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pcy.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ayj.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hpg.haohaochexian.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ptc.hnxiangtu.top

[B07] while 循环
来源：http://sfl.fzhhl.top

Py:   while i < 10: i += 1
来源：http://lzb.snrcjt.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uur.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://mtn.andypj.xyz

TS:   while (i < 10) { i++; }
来源：http://hmh.fanxiaobao.xyz

Java: while (i < 10) { i++; }
来源：http://gxu.fzhhl.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bfz.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://pwz.zhoulong.xyz

C#:   while (i < 10) { i++; }
来源：http://gxl.yj202588.top

[B08] do-while（至少执行一次）
来源：http://nku.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://vud.ydzc1.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pgq.cqqwz.cn

JS:   do { i++; } while (i < 10);
来源：http://ogb.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://osj.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://aio.nanxinkj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://aat.jinyuanbaomall.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nlh.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://dfe.bbcook.cn

[B09] break 与 continue
来源：http://jzs.birdmap.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zzg.yj20258.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kjq.haohaochexian.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gmn.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sjw.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tgs.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rss.quarkkingdee.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iho.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ieh.bjfxy.top

[B10] 遍历同时拿索引
来源：http://yzs.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jfj.zhaomingkeji.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bwg.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rfe.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ztl.jinqigufen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nov.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kht.sysykeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fys.ivvv.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oyw.yanxiufei.cn

[B11] 生成数字序列 / 区间
来源：http://mun.smart0.xyz

Py:   list(range(0, 10, 2))
来源：http://rxt.jqgfzy.top

PHP:  range(0, 10, 2);
来源：http://zbc.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jus.cucudq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tcj.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qbr.epnwcf.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oof.vehdjk.com

Ruby: (0...10).step(2).to_a
来源：http://dya.yuanzhike.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mqq.hnqzz.top

[B12] 跳出多层循环
来源：http://tlm.ppjwa.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gsq.birdmap.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nqz.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tnz.bjfxy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lwz.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wrp.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rna.tianlin.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jki.yuxming.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xkj.hfpthk.cn

[B13] 判断是否为数字
来源：http://wjs.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://hbw.tanke756.top

PHP:  is_numeric($x)
来源：http://hrd.feifeiyinyue.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oso.9152youxi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pap.jinqigufen.top

Java: x instanceof Number
来源：http://hoq.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ccp.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://rlw.daxiang520.top

C#:   x is int or double or decimal
来源：http://dbx.bbcook.cn

[B14] 判断值是否在集合内
来源：http://yda.aizwys.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vmw.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lub.yj20258.top

JS:   [1, 2, 3].includes(x)
来源：http://fnv.tanke756.top

TS:   [1, 2, 3].includes(x)
来源：http://hlv.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://beu.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://giu.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jpx.mhx1999.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sac.jianghu66.top

[B15] 布尔运算与取反
来源：http://whb.andypj.xyz

Py:   a and b or not c
来源：http://ndi.hnxiangtu.top

PHP:  $a && $b || !$c
来源：http://xjg.jqgfzy.top

JS:   a && b || !c
来源：http://sku.pengpengdd.cyou

TS:   a && b || !c
来源：http://isi.epnwcf.com

Java: a && b || !c
来源：http://lut.cucudq.cn

Go:   a && b || !c
来源：http://vsg.chenjidiqi.icu

Ruby: a && b || !c
来源：http://jxi.cucudq.cn

C#:   a && b || !c
来源：http://coz.yuanzhike.top

[B16] 卫语句：不满足条件提前返回
来源：http://yus.ctjpmb.com

Py:   if not data: return
来源：http://upd.gzhubu.top

PHP:  if (!$data) { return; }
来源：http://orn.wangshuangyany.cn

JS:   if (!data) return;
来源：http://zge.fehbvm.com

TS:   if (!data) return;
来源：http://tds.yvedp.cn


<!-- 参考信息 -->