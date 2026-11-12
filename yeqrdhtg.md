代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rxi.vehdjk.com

Java: new Random().nextInt(100) + 1
来源：http://czy.yj202588.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://szr.ybcxt.top

Ruby: rand(1..100)
来源：http://bft.hesvh.cn

C#:   new Random().Next(1, 101)
来源：http://hkm.ivvv.top

[A11] 条件表达式（三元）
来源：http://idk.chenzaomai.com

Py:   "yes" if x > 0 else "no"
来源：http://mda.zdqjudy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ypa.guowangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://omm.fanxiaobao.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://gzv.ydzc1.top

Java: x > 0 ? "yes" : "no"
来源：http://hkb.shanyushiyangkeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://rdi.52xcode.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wiy.mhx1999.top

C#:   x > 0 ? "yes" : "no"
来源：http://yxj.birdmap.top

[A12] 字符串插值 / 格式化
来源：http://yul.9152youxi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wta.sufxvd.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jqk.sjlbkw.cn

JS:   `Hello, ${name}!`
来源：http://blt.quarkkingdee.top

TS:   `Hello, ${name}!`
来源：http://ssf.wangdashe.top

Java: "Hello, %s!".formatted(name)
来源：http://edd.redwolf501.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hmg.fengsongda.top

Ruby: "Hello, #{name}!"
来源：http://yak.yvedp.cn

C#:   $"Hello, {name}!"
来源：http://agx.hywenlv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ygn.jianghu66.top

Py:   "第一行\n第二行"
来源：http://mrs.yuxming.cn

PHP:  "第一行\n第二行"
来源：http://cek.chenjidiqi.icu

JS:   "第一行\n第二行"
来源：http://ksg.tanke756.top

TS:   "第一行\n第二行"
来源：http://pgt.jinyuanbaomall.cn

Java: "第一行\n第二行"
来源：http://xbp.yangfankeji.com

Go:   "第一行\n第二行"
来源：http://rty.ivvv.top

Ruby: "第一行\n第二行"
来源：http://gzd.bjfxy.top

C#:   "第一行\n第二行"
来源：http://rin.zhengqikj.top

[A14] 注释写法
来源：http://mfh.zycfv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ado.pengpengdd.cyou

PHP:  // 或 # 单行；/* 多行 */
来源：http://rfx.ctjpmb.com

JS:   // 单行；/* 多行 */
来源：http://xhs.xinyue.icu

TS:   // 单行；/* 多行 */
来源：http://tbl.vehdjk.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ovu.aizwys.cn

Go:   // 单行；/* 多行 */
来源：http://mfq.zhengqikj.top

Ruby: # 单行；=begin 多行 =end
来源：http://ltr.feifeiyinyue.top

C#:   // 单行；/* 多行 */
来源：http://jzu.nwbrower.top

[A15] 空值判断与默认值
来源：http://vjx.yvedp.cn

Py:   value = data or "默认值"
来源：http://unq.uphjek.com

PHP:  $value = $data ?? "默认值";
来源：http://hbu.yangfankeji.com

JS:   const value = data ?? "默认值";
来源：http://vlq.zdbjq.cn

TS:   const value = data ?? "默认值";
来源：http://hre.guannengcc.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kyw.jlsjyb.cn

Go:   if data == "" { data = "默认值" }
来源：http://pgi.aizwys.cn

Ruby: value = data || "默认值"
来源：http://ryb.sufxvd.cn

C#:   var value = data ?? "默认值";
来源：http://vyl.yonumen.top

[A16] 真假值判断规则
来源：http://jtk.xziqi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://aso.fehbvm.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ryq.hammf.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dql.chenjidiqi.icu

TS:   if (!x) {}
来源：http://vci.gzhubu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lqd.ydzc1.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xag.cheryme.top

Ruby: unless x            # nil 与 false 为假
来源：http://bew.yfazqb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vkr.xingfuxueyuan.xyz

[A17] 位运算
来源：http://xjb.xingfuxueyuan.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qcn.fanxiaobao.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tte.sxryk.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qyp.hnqzz.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yla.xingfuxueyuan.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://swe.zhixingplan.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://aub.snrcjt.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wat.xziqi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ibq.zhengqikj.top

[A18] 字符与 ASCII 码互转
来源：http://tnr.hammf.cn

Py:   ord("A"); chr(65)
来源：http://non.cashguo.top

PHP:  ord("A"); chr(65)
来源：http://wmy.xuanzx.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mus.ydzc1.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fms.ppjwa.cn

Java: (int) 'A'; (char) 65
来源：http://erb.gotoacloud.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://boh.guannengcc.top

Ruby: "A".ord; 65.chr
来源：http://yhx.tarul.cn

C#:   (int)'A'; (char)65
来源：http://bqk.yueranfly.top

[A19] 交换两个变量
来源：http://lse.jqgufenzy.top

Py:   a, b = b, a
来源：http://ikz.aizwys.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pka.yj20258.top

JS:   [a, b] = [b, a];
来源：http://xzd.nwbrower.top

TS:   [a, b] = [b, a];
来源：http://one.redwolf501.top

Java: int t = a; a = b; b = t;
来源：http://unv.kuanghao11.cn

Go:   a, b = b, a
来源：http://upj.guowangkeji.top

Ruby: a, b = b, a
来源：http://khi.zdqjudy.top

C#:   (a, b) = (b, a);
来源：http://gbz.wangshuangyany.cn

[A20] 读取标准输入
来源：http://htz.yangfankeji.com

Py:   name = input("请输入：")
来源：http://kso.jlsjyb.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://blq.sjlbkw.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://elf.svipenyu.cn

TS:   // Node.js：readline 模块
来源：http://gia.haohaochexian.top

Java: new Scanner(System.in).nextLine()
来源：http://ocz.hnxiangtu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ibj.feifeiyinyue.top

Ruby: gets.chomp
来源：http://qon.hammf.cn

C#:   Console.ReadLine();
来源：http://fij.meibo888.top

[A21] 保留指定小数位输出
来源：http://uwh.jinghuilouyu.cn

Py:   f"{3.14159:.2f}"
来源：http://hfp.vqdsnc.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://knz.hammf.cn

JS:   (3.14159).toFixed(2)
来源：http://odp.zhongyouzk.top

TS:   (3.14159).toFixed(2)
来源：http://meu.vehdjk.com

Java: String.format("%.2f", 3.14159)
来源：http://qxa.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uis.sysykeji.top

Ruby: format("%.2f", 3.14159)
来源：http://pxe.feifeiyinyue.top

C#:   3.14159.ToString("F2")
来源：http://mla.andypj.xyz

[A22] 获取字符串长度
来源：http://llq.jinqigufen.top

Py:   len(s)
来源：http://ccu.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qkw.feifeiyinyue.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bnn.havefunace.top

TS:   s.length
来源：http://hot.jqgufenzy.top

Java: s.length()
来源：http://lqi.iojbl.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qvt.nwbrower.top

Ruby: s.length
来源：http://vcs.zhoulong.xyz

C#:   s.Length
来源：http://xvz.jianghu66.top

[A23] 大小写转换
来源：http://avg.shuidangran.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ytv.fehbvm.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zpz.yanxiufei.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://foj.ywan-chungtsiang.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eeh.yuanzhike.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ber.gzhubu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jod.bbcook.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://aid.cashguo.top

C#:   s.ToUpper(); s.ToLower()
来源：http://eju.uphjek.com

[A24] 去除首尾空白
来源：http://btv.uphjek.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rvl.shzxlz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hqe.jinyuanbaomall.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hue.316326.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://shc.nanxuanxn.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ogl.nwbrower.top

Go:   strings.TrimSpace(s)
来源：http://vhk.yueranfly.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yjh.vqdsnc.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hzc.dianchejie.cn

[A25] 字符串比较
来源：http://ocm.jinghuilouyu.cn

Py:   s1 == s2; s1 != s2
来源：http://xlc.cqqwz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://job.zhoulong.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kgp.meibo888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://brx.mhx1999.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xkb.sysykeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xzt.nanxinkj.top

Ruby: s1 == s2; s1 <=> s2
来源：http://aiy.guowangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gcb.uphjek.com

[A26] 类型转换总览
来源：http://hhe.jqgfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qxo.nanxuanxn.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hiz.yongpay.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xfa.yangfankeji.com

TS:   Number() String() Boolean() x as number
来源：http://jgp.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://awe.hcnkem.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aqq.zhixingplan.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://awk.chenzaomai.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vdv.jqgfzy.top

================================================================================
来源：http://ehp.vehdjk.com

B. 流程控制
来源：http://cvm.jinqigfzy.top

================================================================================
来源：http://rjs.zhijiandao.cn

[B01] 条件判断 if / else
来源：http://bbc.ybcxt.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nco.zhoulong.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gfp.hesvh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vib.guannengcc.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://snn.hfpthk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wgc.vqdsnc.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://miq.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rqg.sweek.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fuh.xuanzx.com

[B02] 多分支 else if / elif
来源：http://xpr.jinqigfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wog.sysykeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rrn.gaohongyu789.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uro.tianlin.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kkd.xingfuxueyuan.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://slv.shangyingyoupin.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sti.zhongyouzk.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cwg.hywenlv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wzs.wangshuangyany.cn

[B03] switch / match / case
来源：http://wvv.wangdashe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oel.svipenyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fbo.ehwqpu.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sjf.xuanzx.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dbe.meibo888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cmo.nanxuanxn.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wcx.nwbrower.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xnx.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dor.dashuyun.cn

[B04] for 计数循环
来源：http://iyg.xingfuxueyuan.xyz

Py:   for i in range(10): print(i)
来源：http://ayh.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://evy.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://paj.dashuyun.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://crr.sxryk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hfi.guannengcc.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bxa.redwolf501.top

Ruby: 10.times { |i| puts i }
来源：http://phn.shanyushiyangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vlt.yangfankeji.com

[B05] 遍历数组 / 列表
来源：http://kra.jinyuanbaomall.cn

Py:   for item in arr: print(item)
来源：http://cyc.guowangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bco.ywan-chungtsiang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dnk.zhongyouzk.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ruc.jiagoushi.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cmx.jianghu66.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xpi.daria6918.cn

Ruby: arr.each { |item| puts item }
来源：http://btc.daria6918.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://srj.yj20258.top

[B06] 遍历字典 / 对象
来源：http://wyn.pycfn.com

Py:   for k, v in d.items(): print(k, v)
来源：http://rfd.jlsjyb.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bro.shanyushiyangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xoi.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sjb.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hro.aizwys.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pag.cucudq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tim.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wtt.hammf.cn

[B07] while 循环
来源：http://yyz.zhijiandao.cn

Py:   while i < 10: i += 1
来源：http://wfd.0kj1m.cn

PHP:  while ($i < 10) { $i++; }
来源：http://axp.0kj1m.cn

JS:   while (i < 10) { i++; }
来源：http://zbx.hysaishi.cn

TS:   while (i < 10) { i++; }
来源：http://zkx.tianlin.xyz

Java: while (i < 10) { i++; }
来源：http://ljt.gzhubu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://muj.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://ygg.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://xjo.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://jfy.aizwys.cn

Py:   # 无 do-while：用 while True + break
来源：http://jyo.svipenyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://epb.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://iqf.uphjek.com

TS:   do { i++; } while (i < 10);
来源：http://gox.jyoumei.cn

Java: do { i++; } while (i < 10);
来源：http://usp.epnwcf.com

Go:   for { i++; if i >= 10 { break } }
来源：http://ocg.iojbl.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jwo.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://xin.dianchejie.cn

[B09] break 与 continue
来源：http://fhw.hywenlv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://skb.fengsongda.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lma.dianchejie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zaa.sxryk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wfm.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ryl.xylfe.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hpt.birdmap.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dnl.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tne.fktsv.cn

[B10] 遍历同时拿索引
来源：http://llq.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jjc.jianghu66.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vej.xingfuxueyuan.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gsy.vehdjk.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vii.xinyue.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://feg.guowangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wuu.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jqa.guowangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cqn.jqgufenzy.top

[B11] 生成数字序列 / 区间
来源：http://cum.vehdjk.com

Py:   list(range(0, 10, 2))
来源：http://wjo.snrcjt.cn

PHP:  range(0, 10, 2);
来源：http://kbp.yueranfly.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vuq.quarkkingdee.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bhj.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yij.zhixingplan.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vlb.havefunace.top

Ruby: (0...10).step(2).to_a
来源：http://ywv.52xcode.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iyb.nwbrower.top

[B12] 跳出多层循环
来源：http://yhu.hcnkem.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://vgu.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fov.yj202588.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yqe.vqdsnc.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uxi.zdqjudy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bvv.jqgfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pfy.xingfuxueyuan.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uas.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uhc.gogol.net.cn

[B13] 判断是否为数字
来源：http://uby.zhengqikj.top

Py:   isinstance(x, (int, float))
来源：http://osw.gotoacloud.top

PHP:  is_numeric($x)
来源：http://zgu.yvedp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dll.mhx1999.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zxt.smart0.xyz

Java: x instanceof Number
来源：http://siw.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qss.jlsjyb.cn

Ruby: x.is_a?(Numeric)
来源：http://hkx.ehwqpu.com

C#:   x is int or double or decimal
来源：http://ldz.sweek.top

[B14] 判断值是否在集合内
来源：http://bdp.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nkl.jinghuilouyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qji.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://bdh.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://bok.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kpw.hywenlv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://umk.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://nrq.hesvh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jmn.yvedp.cn

[B15] 布尔运算与取反
来源：http://zce.jinghuilouyu.cn

Py:   a and b or not c
来源：http://uxv.hnxiangtu.top

PHP:  $a && $b || !$c
来源：http://lza.zdbjq.cn

JS:   a && b || !c
来源：http://deq.cqqwz.cn

TS:   a && b || !c
来源：http://ikp.xuanzx.com

Java: a && b || !c
来源：http://uab.jlsjyb.cn

Go:   a && b || !c
来源：http://izt.ehwqpu.com

Ruby: a && b || !c
来源：http://yzj.dianchejie.cn

C#:   a && b || !c
来源：http://coi.yuanzhike.top

[B16] 卫语句：不满足条件提前返回
来源：http://zfe.havefunace.top

Py:   if not data: return
来源：http://zjr.0kj1m.cn

PHP:  if (!$data) { return; }
来源：http://gyj.jyoumei.cn

JS:   if (!data) return;
来源：http://bfj.52xcode.cn

TS:   if (!data) return;
来源：http://gzz.gogol.net.cn

Java: if (data == null) return;
来源：http://pci.nwbrower.top

Go:   if data == nil { return }
来源：http://pve.pengpengdd.cyou

Ruby: return if data.nil?
来源：http://xlh.9152youxi.cn

C#:   if (data == null) return;
来源：http://ofi.tianlin.xyz

================================================================================
来源：http://aai.tianlin.xyz

C. 函数与作用域
来源：http://sbo.ctjpmb.com

================================================================================
来源：http://bmc.chenzaomai.com

[C01] 定义函数
来源：http://ksp.dashuyun.cn


<!-- 参考信息 -->