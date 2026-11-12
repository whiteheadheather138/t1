代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://zrt.bjfxy.top

[A11] 条件表达式（三元）
来源：http://cxh.ybcxt.top

Py:   "yes" if x > 0 else "no"
来源：http://qpf.shanyushiyangkeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ohx.chenlongwang.top

JS:   x > 0 ? "yes" : "no"
来源：http://wvd.yj20258.top

TS:   x > 0 ? "yes" : "no"
来源：http://wvh.bjfxy.top

Java: x > 0 ? "yes" : "no"
来源：http://zcf.bbcook.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cad.bjfxy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://bid.yvedp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://com.xuetiantiany.cn

[A12] 字符串插值 / 格式化
来源：http://zwp.sjlbkw.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bnc.cucudq.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uwt.yj20258888.top

JS:   `Hello, ${name}!`
来源：http://qvv.jinyuanbaomall.cn

TS:   `Hello, ${name}!`
来源：http://syh.ppjwa.cn

Java: "Hello, %s!".formatted(name)
来源：http://lps.chenjidiqi.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://han.shzxlz.cn

Ruby: "Hello, #{name}!"
来源：http://xbw.birdmap.top

C#:   $"Hello, {name}!"
来源：http://fpg.dianchejie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uyp.dashuyun.cn

Py:   "第一行\n第二行"
来源：http://qbd.uphjek.com

PHP:  "第一行\n第二行"
来源：http://luj.hcnkem.com

JS:   "第一行\n第二行"
来源：http://gvm.wangdashe.top

TS:   "第一行\n第二行"
来源：http://tec.pycfn.com

Java: "第一行\n第二行"
来源：http://rgp.zhengqikj.top

Go:   "第一行\n第二行"
来源：http://grj.shanyushiyangkeji.top

Ruby: "第一行\n第二行"
来源：http://jxs.sweek.top

C#:   "第一行\n第二行"
来源：http://cok.cashguo.top

[A14] 注释写法
来源：http://kxg.aibaodan.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bgw.yfazqb.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://let.ppjwa.cn

JS:   // 单行；/* 多行 */
来源：http://iau.ydzc1.top

TS:   // 单行；/* 多行 */
来源：http://lnh.zycfv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qej.quarkkingdee.top

Go:   // 单行；/* 多行 */
来源：http://yze.shzxlz.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jod.hfpthk.cn

C#:   // 单行；/* 多行 */
来源：http://haq.shzxlz.cn

[A15] 空值判断与默认值
来源：http://srn.fzhhl.top

Py:   value = data or "默认值"
来源：http://zml.ydzc1.top

PHP:  $value = $data ?? "默认值";
来源：http://dlp.sufxvd.cn

JS:   const value = data ?? "默认值";
来源：http://vjl.aizwys.cn

TS:   const value = data ?? "默认值";
来源：http://qyi.fzhhl.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://htr.chenzaomai.com

Go:   if data == "" { data = "默认值" }
来源：http://lco.zhiwuduotai.top

Ruby: value = data || "默认值"
来源：http://kth.pengpengdd.cyou

C#:   var value = data ?? "默认值";
来源：http://llo.sweek.top

[A16] 真假值判断规则
来源：http://sib.haohaochexian.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zsb.gotoacloud.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fst.meibo888.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://eqi.bjfxy.top

TS:   if (!x) {}
来源：http://tsq.haohaochexian.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://iue.aizwys.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wyf.0kj1m.cn

Ruby: unless x            # nil 与 false 为假
来源：http://czf.zhongyouzk.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kao.smart0.xyz

[A17] 位运算
来源：http://idd.nanxinkj.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ymj.vehdjk.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xxz.zhijiandao.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ijp.meibo888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qwd.hysaishi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qxa.shanyushiyangkeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nhb.pycfn.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rqn.c1oappe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iqj.shuidangran.top

[A18] 字符与 ASCII 码互转
来源：http://vwp.kuanghao11.cn

Py:   ord("A"); chr(65)
来源：http://ice.jyoumei.cn

PHP:  ord("A"); chr(65)
来源：http://uuv.yonumen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wix.pengpengdd.cyou

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wni.52xcode.cn

Java: (int) 'A'; (char) 65
来源：http://kqe.redwolf501.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dqm.smart0.xyz

Ruby: "A".ord; 65.chr
来源：http://rzi.meibo888.top

C#:   (int)'A'; (char)65
来源：http://vlt.xinyue.icu

[A19] 交换两个变量
来源：http://zkz.nanxuanxn.top

Py:   a, b = b, a
来源：http://ngl.fktsv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tfm.epnwcf.com

JS:   [a, b] = [b, a];
来源：http://boh.zhiwuduotai.top

TS:   [a, b] = [b, a];
来源：http://dlu.gaohongyu789.top

Java: int t = a; a = b; b = t;
来源：http://zit.ppjwa.cn

Go:   a, b = b, a
来源：http://lnv.gotoacloud.top

Ruby: a, b = b, a
来源：http://mmj.zhongyouzk.top

C#:   (a, b) = (b, a);
来源：http://bqc.hfpthk.cn

[A20] 读取标准输入
来源：http://bde.nanxinkj.top

Py:   name = input("请输入：")
来源：http://cad.gogol.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ghm.jinyuanbaomall.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wew.hcnkem.com

TS:   // Node.js：readline 模块
来源：http://rpf.pycfn.com

Java: new Scanner(System.in).nextLine()
来源：http://eih.havefunace.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ewb.tianlin.xyz

Ruby: gets.chomp
来源：http://gcv.cheryme.top

C#:   Console.ReadLine();
来源：http://rjv.zycfv.cn

[A21] 保留指定小数位输出
来源：http://yvl.tanke756.top

Py:   f"{3.14159:.2f}"
来源：http://xzn.tanke756.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://agq.yongpay.top

JS:   (3.14159).toFixed(2)
来源：http://ucq.aibaodan.cn

TS:   (3.14159).toFixed(2)
来源：http://ckj.yvedp.cn

Java: String.format("%.2f", 3.14159)
来源：http://pqi.shanyushiyangtech.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://orw.zhaomingkeji.xyz

Ruby: format("%.2f", 3.14159)
来源：http://czo.c1oappe.top

C#:   3.14159.ToString("F2")
来源：http://qqr.hnqzz.top

[A22] 获取字符串长度
来源：http://juw.svipenyu.cn

Py:   len(s)
来源：http://vel.nanxuanxn.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pwt.xingfuxueyuan.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jvk.52xcode.cn

TS:   s.length
来源：http://wfo.pycfn.com

Java: s.length()
来源：http://koi.tarul.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kwy.yonumen.top

Ruby: s.length
来源：http://etp.jiagoushi.top

C#:   s.Length
来源：http://obt.zycfv.cn

[A23] 大小写转换
来源：http://fem.xingfuxueyuan.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://qyt.sweek.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qxw.daxiang520.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ews.bbcook.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gtg.yanxiufei.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://piv.gaohongyu789.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vpb.aibaodan.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yuu.haohaochexian.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hkt.cdnleiting.top

[A24] 去除首尾空白
来源：http://otb.fzhhl.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hqe.52xcode.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lpc.ivvv.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wwg.chenzaomai.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hqt.c1oappe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kvm.yuanzhike.top

Go:   strings.TrimSpace(s)
来源：http://xoe.sysykeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qws.yuanzhike.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://giu.zycfv.cn

[A25] 字符串比较
来源：http://yuu.cheryme.top

Py:   s1 == s2; s1 != s2
来源：http://oat.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rjn.316326.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sso.chenzaomai.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sse.pycfn.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uke.uphjek.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qwy.guowangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qel.shanyushiyangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bch.sweek.top

[A26] 类型转换总览
来源：http://lvz.jiagoushi.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://waf.zhongyouzk.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dnx.cucudq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eor.zhixingplan.top

TS:   Number() String() Boolean() x as number
来源：http://tty.yfazqb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ctj.bbcook.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://olb.chenzaomai.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://ppz.xuanzx.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jpx.redwolf501.top

================================================================================
来源：http://glz.shuidangran.top

B. 流程控制
来源：http://tic.shuidangran.top

================================================================================
来源：http://ksn.yangfankeji.com

[B01] 条件判断 if / else
来源：http://zaw.ppjwa.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rip.haohaochexian.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yez.guannengcc.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://udo.svipenyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ien.feifeiyinyue.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fwb.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://udq.chenzaomai.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sqh.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pya.yj202588.top

[B02] 多分支 else if / elif
来源：http://qmy.yvedp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zsp.pycfn.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://stl.jyoumei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lno.haohaochexian.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ppg.yongpay.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aja.sufxvd.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://she.gogol.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bmo.hywenlv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ndu.zycfv.cn

[B03] switch / match / case
来源：http://zjm.52xcode.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xvh.ivvv.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lgi.sxryk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wyn.daxiang520.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nlo.zycfv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://snl.nanxinkj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lpc.52xcode.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wqg.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qqh.aizwys.cn

[B04] for 计数循环
来源：http://nui.dianchejie.cn

Py:   for i in range(10): print(i)
来源：http://xuk.fanxiaobao.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ktn.andypj.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ped.haohaochexian.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ejp.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jpc.andypj.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lfy.daxiang520.top

Ruby: 10.times { |i| puts i }
来源：http://szc.smart0.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vdp.52xcode.cn

[B05] 遍历数组 / 列表
来源：http://jep.shzxlz.cn

Py:   for item in arr: print(item)
来源：http://wbm.zhongyouzk.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tmf.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vzo.ydzc1.top

TS:   for (const item of arr) { console.log(item); }
来源：http://seb.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yrb.cdnleiting.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mhs.havefunace.top

Ruby: arr.each { |item| puts item }
来源：http://tcz.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lme.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://gjl.jqgufenzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hkv.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mar.gogol.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ega.gzhubu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rgc.jinghuilouyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wsq.tianlin.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kea.yanxiufei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uff.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pbs.sjlbkw.cn

[B07] while 循环
来源：http://sfr.yuxming.cn

Py:   while i < 10: i += 1
来源：http://muh.zycfv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jxk.gotoacloud.top

JS:   while (i < 10) { i++; }
来源：http://xpb.sysykeji.top

TS:   while (i < 10) { i++; }
来源：http://ovm.hesvh.cn

Java: while (i < 10) { i++; }
来源：http://lju.guannengcc.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gzt.bbcook.cn

Ruby: while i < 10; i += 1; end
来源：http://rvl.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://ndh.andypj.xyz

[B08] do-while（至少执行一次）
来源：http://wgg.yanxiufei.cn

Py:   # 无 do-while：用 while True + break
来源：http://ahx.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://swp.jqgufenzy.top

JS:   do { i++; } while (i < 10);
来源：http://vbj.jlsjyb.cn

TS:   do { i++; } while (i < 10);
来源：http://sxc.xinyue.icu

Java: do { i++; } while (i < 10);
来源：http://jrz.tarul.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://awg.kuanghao11.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bws.gzhubu.top

C#:   do { i++; } while (i < 10);
来源：http://frq.meibo888.top

[B09] break 与 continue
来源：http://ybo.meibo888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nkz.aibaodan.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://del.dianchejie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sdt.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uvk.tian-w.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mxb.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yri.zhoulong.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zao.tanke756.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zct.shanyushiyangkeji.top

[B10] 遍历同时拿索引
来源：http://wbs.zdbjq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hti.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vrb.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wtc.cdnleiting.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ajd.yanxiufei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ati.zycfv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://knu.xuetiantiany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://txz.jlsjyb.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xls.zdqjudy.top

[B11] 生成数字序列 / 区间
来源：http://jww.chenjidiqi.icu

Py:   list(range(0, 10, 2))
来源：http://yot.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://lnv.jqgufenzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yyy.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kac.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xak.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pcx.gzhubu.top

Ruby: (0...10).step(2).to_a
来源：http://wqr.316326.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wal.fanxiaobao.xyz

[B12] 跳出多层循环
来源：http://ypl.zhongyouzk.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://huv.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://aij.sufxvd.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fbn.cdnleiting.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mey.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hzi.vqdsnc.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dos.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xnv.sxryk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gxq.kuanghao11.cn

[B13] 判断是否为数字
来源：http://tit.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://qpj.nanxinkj.top

PHP:  is_numeric($x)
来源：http://sfq.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://one.gogol.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eyj.svipenyu.cn

Java: x instanceof Number
来源：http://tdc.gotoacloud.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pul.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://ffd.jqgfzy.top

C#:   x is int or double or decimal
来源：http://sly.gogol.net.cn

[B14] 判断值是否在集合内
来源：http://ohc.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jmr.zhongyouzk.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jip.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://xnn.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://wrj.yj20258.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ljx.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dyu.havefunace.top

Ruby: [1, 2, 3].include?(x)
来源：http://fkh.tanke756.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sou.hywenlv.cn

[B15] 布尔运算与取反
来源：http://fdp.uphjek.com

Py:   a and b or not c
来源：http://lyb.redwolf501.top

PHP:  $a && $b || !$c
来源：http://ded.smart0.xyz

JS:   a && b || !c
来源：http://xld.fzhhl.top

TS:   a && b || !c
来源：http://qya.jinghuilouyu.cn

Java: a && b || !c
来源：http://fhp.haohaochexian.top

Go:   a && b || !c
来源：http://tlt.xingfuxueyuan.xyz

Ruby: a && b || !c
来源：http://pba.nwbrower.top

C#:   a && b || !c
来源：http://qqx.chenzaomai.com

[B16] 卫语句：不满足条件提前返回
来源：http://xyy.jinqigufen.top

Py:   if not data: return
来源：http://yln.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://qrb.jinqigufen.top

JS:   if (!data) return;
来源：http://ket.tianlin.xyz

TS:   if (!data) return;
来源：http://ofm.jianghu66.top

Java: if (data == null) return;
来源：http://mtt.birdmap.top

Go:   if data == nil { return }
来源：http://dcq.yj20258888.top

Ruby: return if data.nil?
来源：http://lvs.nwbrower.top

C#:   if (data == null) return;
来源：http://tvy.jinqigufen.top

================================================================================
来源：http://gix.9152youxi.cn

C. 函数与作用域
来源：http://rkp.chenjidiqi.icu

================================================================================
来源：http://isf.ybcxt.top

[C01] 定义函数
来源：http://kys.sysykeji.top

Py:   def add(a, b): return a + b
来源：http://snl.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hbt.daria6918.cn

JS:   function add(a, b) { return a + b; }
来源：http://vct.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tve.tarul.cn


<!-- 参考信息 -->