代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://ijs.tianlin.xyz

[A11] 条件表达式（三元）
来源：http://szr.ydzc1.top

Py:   "yes" if x > 0 else "no"
来源：http://gtx.uphjek.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://nrl.xingfuxueyuan.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://hxx.xziqi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qhk.smart0.xyz

Java: x > 0 ? "yes" : "no"
来源：http://mqk.sufxvd.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jkc.hongshengwenyu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://qxa.meibo888.top

C#:   x > 0 ? "yes" : "no"
来源：http://guk.shuidangran.top

[A12] 字符串插值 / 格式化
来源：http://ube.jinqigfzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jye.smart0.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://eec.yueranfly.top

JS:   `Hello, ${name}!`
来源：http://pvj.daria6918.cn

TS:   `Hello, ${name}!`
来源：http://kjh.dashuyun.cn

Java: "Hello, %s!".formatted(name)
来源：http://nel.quarkkingdee.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ltp.52xcode.cn

Ruby: "Hello, #{name}!"
来源：http://jnz.jinqigfzy.top

C#:   $"Hello, {name}!"
来源：http://htv.dianchejie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lqy.zhijiandao.cn

Py:   "第一行\n第二行"
来源：http://uxd.sweek.top

PHP:  "第一行\n第二行"
来源：http://ziw.guannengcc.top

JS:   "第一行\n第二行"
来源：http://hnq.sufxvd.cn

TS:   "第一行\n第二行"
来源：http://tev.c1oappe.top

Java: "第一行\n第二行"
来源：http://gsy.redwolf501.top

Go:   "第一行\n第二行"
来源：http://bux.hammf.cn

Ruby: "第一行\n第二行"
来源：http://xrn.ivvv.top

C#:   "第一行\n第二行"
来源：http://kfe.yj20258.top

[A14] 注释写法
来源：http://zex.zhiwuduotai.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://nls.dianchejie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qyl.jlsjyb.cn

JS:   // 单行；/* 多行 */
来源：http://kxp.xinyue.icu

TS:   // 单行；/* 多行 */
来源：http://hrx.shanyushiyangkeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jbm.hnqzz.top

Go:   // 单行；/* 多行 */
来源：http://dcu.zhaomingkeji.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://wff.zdbjq.cn

C#:   // 单行；/* 多行 */
来源：http://yia.jinqigfzy.top

[A15] 空值判断与默认值
来源：http://qxm.kuanghao11.cn

Py:   value = data or "默认值"
来源：http://ggu.aizwys.cn

PHP:  $value = $data ?? "默认值";
来源：http://fkw.hywenlv.cn

JS:   const value = data ?? "默认值";
来源：http://rva.pengpengdd.cyou

TS:   const value = data ?? "默认值";
来源：http://uuo.yueranfly.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jyo.cdnleiting.top

Go:   if data == "" { data = "默认值" }
来源：http://wzm.ehwqpu.com

Ruby: value = data || "默认值"
来源：http://kqh.pycfn.com

C#:   var value = data ?? "默认值";
来源：http://pcj.hywenlv.cn

[A16] 真假值判断规则
来源：http://fua.sweek.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pjv.yongpay.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pjn.pycfn.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nhv.ehwqpu.com

TS:   if (!x) {}
来源：http://sww.tanke756.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vyo.sysykeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xti.ppjwa.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tup.xylfe.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zzy.ydjk.org.cn

[A17] 位运算
来源：http://exx.aizwys.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hsv.ywan-chungtsiang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wut.quarkkingdee.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ssc.zhijiandao.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sqm.fehbvm.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ftq.feifeiyinyue.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qaw.yangfankeji.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://klv.fehbvm.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xoq.yonumen.top

[A18] 字符与 ASCII 码互转
来源：http://ema.hesvh.cn

Py:   ord("A"); chr(65)
来源：http://eir.fehbvm.com

PHP:  ord("A"); chr(65)
来源：http://cdg.hywenlv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gky.gotoacloud.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xsl.yj20258.top

Java: (int) 'A'; (char) 65
来源：http://urx.smart0.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xju.yanxiufei.cn

Ruby: "A".ord; 65.chr
来源：http://tga.jqgfzy.top

C#:   (int)'A'; (char)65
来源：http://xzu.zhixingplan.top

[A19] 交换两个变量
来源：http://pod.yangfankeji.com

Py:   a, b = b, a
来源：http://gmg.cdnleiting.top

PHP:  [$a, $b] = [$b, $a];
来源：http://zmg.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://nio.yj20258.top

TS:   [a, b] = [b, a];
来源：http://upv.zhaomingkeji.xyz

Java: int t = a; a = b; b = t;
来源：http://chl.9152youxi.cn

Go:   a, b = b, a
来源：http://mze.jinqigufen.top

Ruby: a, b = b, a
来源：http://ngl.cashguo.top

C#:   (a, b) = (b, a);
来源：http://jwk.guowangkeji.top

[A20] 读取标准输入
来源：http://azb.daria6918.cn

Py:   name = input("请输入：")
来源：http://exz.uphjek.com

PHP:  $name = trim(fgets(STDIN));
来源：http://ith.wangdashe.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zxm.yongpay.top

TS:   // Node.js：readline 模块
来源：http://gwp.xziqi.cn

Java: new Scanner(System.in).nextLine()
来源：http://tra.zhoulong.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gre.birdmap.top

Ruby: gets.chomp
来源：http://xxm.vqdsnc.cn

C#:   Console.ReadLine();
来源：http://zes.shangyingyoupin.top

[A21] 保留指定小数位输出
来源：http://zup.daxiang520.top

Py:   f"{3.14159:.2f}"
来源：http://yvr.mhx1999.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pat.tian-w.cn

JS:   (3.14159).toFixed(2)
来源：http://tok.ydjk.org.cn

TS:   (3.14159).toFixed(2)
来源：http://nwd.tianlin.xyz

Java: String.format("%.2f", 3.14159)
来源：http://rkw.ppjwa.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wkd.dianchejie.cn

Ruby: format("%.2f", 3.14159)
来源：http://duk.zhaomingkeji.xyz

C#:   3.14159.ToString("F2")
来源：http://bos.havefunace.top

[A22] 获取字符串长度
来源：http://bbk.hnxiangtu.top

Py:   len(s)
来源：http://pda.guowangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ase.yvedp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kgv.xziqi.cn

TS:   s.length
来源：http://wly.zdbjq.cn

Java: s.length()
来源：http://oak.snrcjt.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fau.yj20258888.top

Ruby: s.length
来源：http://uur.iojbl.cn

C#:   s.Length
来源：http://zhi.fanxiaobao.xyz

[A23] 大小写转换
来源：http://dxq.shuidangran.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bfu.wangshuangyany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://olr.guowangkeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wpt.xziqi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ire.cqqwz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zgs.shzxlz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jng.9152youxi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bhe.guannengcc.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bzf.daxiang520.top

[A24] 去除首尾空白
来源：http://xth.sjlbkw.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rby.gotoacloud.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://afe.vqdsnc.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://izy.cheryme.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xtz.shuidangran.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rpc.jqgufenzy.top

Go:   strings.TrimSpace(s)
来源：http://pmr.vqdsnc.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wgi.sjlbkw.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ieh.hcnkem.com

[A25] 字符串比较
来源：http://ewy.gogol.net.cn

Py:   s1 == s2; s1 != s2
来源：http://hrx.chenlongwang.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qyr.0kj1m.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fnc.c1oappe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fyc.chenlongwang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tbg.jinqigfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pfb.yanxiufei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dqg.ydzc1.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cis.gogol.net.cn

[A26] 类型转换总览
来源：http://xch.ybcxt.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xrg.xylfe.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zem.zdqjudy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fdu.jqgfzy.top

TS:   Number() String() Boolean() x as number
来源：http://qac.shanyushiyangtech.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wfe.hysaishi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://owz.haohaochexian.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://sgn.xziqi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rfx.gaohongyu789.top

================================================================================
来源：http://ktv.xinyue.icu

B. 流程控制
来源：http://eev.snrcjt.cn

================================================================================
来源：http://wbt.xuanzx.com

[B01] 条件判断 if / else
来源：http://sxw.yuanzhike.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rtb.yonumen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mcd.pycfn.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://utx.redwolf501.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wjv.9152youxi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rkj.zhijiandao.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fpg.quarkkingdee.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ldu.aibaodan.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sdp.daxiang520.top

[B02] 多分支 else if / elif
来源：http://lxi.yvedp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vzl.ivvv.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nsv.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pxz.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hes.nwbrower.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mfg.ywan-chungtsiang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xyf.yueranfly.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zyi.daxiang520.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kib.fktsv.cn

[B03] switch / match / case
来源：http://fhs.zdqjudy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jbu.zhiwuduotai.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xob.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dqo.svipenyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jmy.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dxm.hammf.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://our.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rke.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zpt.havefunace.top

[B04] for 计数循环
来源：http://wku.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://uaw.wangdashe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://knt.ywan-chungtsiang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gdp.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vow.pengpengdd.cyou

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tky.shangyingyoupin.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dxl.jqgfzy.top

Ruby: 10.times { |i| puts i }
来源：http://hpo.zhiwuduotai.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dla.ppjwa.cn

[B05] 遍历数组 / 列表
来源：http://qiu.pengpengdd.cyou

Py:   for item in arr: print(item)
来源：http://toy.sweek.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mjk.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dfq.ybcxt.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kil.smart0.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://nqz.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dyt.shanyushiyangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://mns.shzxlz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pki.zhongyouzk.top

[B06] 遍历字典 / 对象
来源：http://bgd.xuetiantiany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ghw.pycfn.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xvx.zhengqikj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rme.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jrh.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eyt.jiagoushi.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mvi.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mud.haohaochexian.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rjf.hesvh.cn

[B07] while 循环
来源：http://pdk.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://kms.jqgfzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://gjr.shangyingyoupin.top

JS:   while (i < 10) { i++; }
来源：http://cwx.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://egq.yfazqb.com

Java: while (i < 10) { i++; }
来源：http://xxl.ywan-chungtsiang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ver.yj202588.top

Ruby: while i < 10; i += 1; end
来源：http://oce.iojbl.cn

C#:   while (i < 10) { i++; }
来源：http://xhj.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://skk.nanxuanxn.top

Py:   # 无 do-while：用 while True + break
来源：http://afl.jlsjyb.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pmu.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://xah.xinyue.icu

TS:   do { i++; } while (i < 10);
来源：http://itk.yanxiufei.cn

Java: do { i++; } while (i < 10);
来源：http://dlj.shanyushiyangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xco.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://osl.yangfankeji.com

C#:   do { i++; } while (i < 10);
来源：http://ezt.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://yhx.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hoc.dianchejie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jom.zhijiandao.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rcx.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pvh.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jzg.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yia.chenzaomai.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kpr.zhongyouzk.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tky.yj20258888.top

[B10] 遍历同时拿索引
来源：http://lww.c1oappe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://okw.xingfuxueyuan.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xhh.hnxiangtu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ywn.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qfz.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pwx.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zpg.yuanzhike.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rhb.cdnleiting.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://opp.zhijiandao.cn

[B11] 生成数字序列 / 区间
来源：http://uko.jyoumei.cn

Py:   list(range(0, 10, 2))
来源：http://xcv.316326.xyz

PHP:  range(0, 10, 2);
来源：http://nul.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xdw.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hju.sysykeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vfn.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qkr.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://lhu.jlsjyb.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fra.mhx1999.top

[B12] 跳出多层循环
来源：http://pvv.yanxiufei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://eas.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://frz.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fan.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://auj.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qnj.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://che.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://spo.bbcook.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rki.andypj.xyz

[B13] 判断是否为数字
来源：http://vei.xziqi.cn

Py:   isinstance(x, (int, float))
来源：http://dis.c1oappe.top

PHP:  is_numeric($x)
来源：http://rdr.bjfxy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kfb.quarkkingdee.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ifv.guowangkeji.top

Java: x instanceof Number
来源：http://gct.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cah.jqgufenzy.top

Ruby: x.is_a?(Numeric)
来源：http://ctk.ydzc1.top

C#:   x is int or double or decimal
来源：http://wov.kuanghao11.cn

[B14] 判断值是否在集合内
来源：http://zqt.zhijiandao.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ljh.meibo888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kps.yfazqb.com

JS:   [1, 2, 3].includes(x)
来源：http://kxc.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://jci.cashguo.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pgq.zhaomingkeji.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xxp.zhoulong.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://axn.nwbrower.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tfh.fengsongda.top

[B15] 布尔运算与取反
来源：http://flk.jyoumei.cn

Py:   a and b or not c
来源：http://vsw.snrcjt.cn

PHP:  $a && $b || !$c
来源：http://aus.chenlongwang.top

JS:   a && b || !c
来源：http://qvf.yuxming.cn

TS:   a && b || !c
来源：http://mvy.shanyushiyangtech.top

Java: a && b || !c
来源：http://ojz.shangyingyoupin.top

Go:   a && b || !c
来源：http://tuq.aizwys.cn

Ruby: a && b || !c
来源：http://mnl.yueranfly.top

C#:   a && b || !c
来源：http://bnb.yuanzhike.top

[B16] 卫语句：不满足条件提前返回
来源：http://tlu.ivvv.top

Py:   if not data: return
来源：http://kpd.sufxvd.cn

PHP:  if (!$data) { return; }
来源：http://myy.hammf.cn

JS:   if (!data) return;
来源：http://mnc.yfazqb.com

TS:   if (!data) return;
来源：http://cgv.meibo888.top

Java: if (data == null) return;
来源：http://gqk.52xcode.cn

Go:   if data == nil { return }
来源：http://xyr.jianghu66.top

Ruby: return if data.nil?
来源：http://uwb.zhijiandao.cn

C#:   if (data == null) return;
来源：http://erj.jqgfzy.top

================================================================================
来源：http://iup.c1oappe.top

C. 函数与作用域
来源：http://pwb.yj20258888.top

================================================================================
来源：http://wvi.snrcjt.cn

[C01] 定义函数
来源：http://dev.nanxinkj.top

Py:   def add(a, b): return a + b
来源：http://sdi.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://toe.redwolf501.top

JS:   function add(a, b) { return a + b; }
来源：http://wwu.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jqv.xuetiantiany.cn


<!-- 参考信息 -->