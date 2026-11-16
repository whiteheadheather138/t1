代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ruy.ppjwa.cn

Java: new Random().nextInt(100) + 1
来源：http://tnu.hnxiangtu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wls.chenlongwang.top

Ruby: rand(1..100)
来源：http://vnb.mhx1999.top

C#:   new Random().Next(1, 101)
来源：http://hpt.jinyuanbaomall.cn

[A11] 条件表达式（三元）
来源：http://lma.gogol.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://hbj.fengsongda.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ulb.zhaomingkeji.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://opk.quarkkingdee.top

TS:   x > 0 ? "yes" : "no"
来源：http://wbq.hfpthk.cn

Java: x > 0 ? "yes" : "no"
来源：http://enp.ivvv.top

Go:   // 无三元运算符，需用 if 语句
来源：http://znx.birdmap.top

Ruby: x > 0 ? "yes" : "no"
来源：http://isd.cdnleiting.top

C#:   x > 0 ? "yes" : "no"
来源：http://dij.sufxvd.cn

[A12] 字符串插值 / 格式化
来源：http://rdr.jinyuanbaomall.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qgt.vqdsnc.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cwl.yj20258.top

JS:   `Hello, ${name}!`
来源：http://bqd.cheryme.top

TS:   `Hello, ${name}!`
来源：http://csv.quarkkingdee.top

Java: "Hello, %s!".formatted(name)
来源：http://vbx.ydzc1.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bsb.tianlin.xyz

Ruby: "Hello, #{name}!"
来源：http://odc.zhixingplan.top

C#:   $"Hello, {name}!"
来源：http://kuf.zhiwuduotai.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ufe.birdmap.top

Py:   "第一行\n第二行"
来源：http://jfg.cdnleiting.top

PHP:  "第一行\n第二行"
来源：http://rpt.jqgfzy.top

JS:   "第一行\n第二行"
来源：http://azu.daria6918.cn

TS:   "第一行\n第二行"
来源：http://gtf.nanxuanxn.top

Java: "第一行\n第二行"
来源：http://yrw.nanxinkj.top

Go:   "第一行\n第二行"
来源：http://qli.hnqzz.top

Ruby: "第一行\n第二行"
来源：http://svj.xinyue.icu

C#:   "第一行\n第二行"
来源：http://qne.9152youxi.cn

[A14] 注释写法
来源：http://vbk.chenlongwang.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://nua.ehwqpu.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://fro.kuanghao11.cn

JS:   // 单行；/* 多行 */
来源：http://psx.hongshengwenyu.top

TS:   // 单行；/* 多行 */
来源：http://mhk.ybcxt.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://awm.c1oappe.top

Go:   // 单行；/* 多行 */
来源：http://guj.nwbrower.top

Ruby: # 单行；=begin 多行 =end
来源：http://ckr.xziqi.cn

C#:   // 单行；/* 多行 */
来源：http://fri.smart0.xyz

[A15] 空值判断与默认值
来源：http://zve.feifeiyinyue.top

Py:   value = data or "默认值"
来源：http://wrs.hysaishi.cn

PHP:  $value = $data ?? "默认值";
来源：http://uri.iojbl.cn

JS:   const value = data ?? "默认值";
来源：http://atn.jlsjyb.cn

TS:   const value = data ?? "默认值";
来源：http://qrs.hnqzz.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zae.wangdashe.top

Go:   if data == "" { data = "默认值" }
来源：http://ndf.uphjek.com

Ruby: value = data || "默认值"
来源：http://zjl.guowangkeji.top

C#:   var value = data ?? "默认值";
来源：http://lva.ivvv.top

[A16] 真假值判断规则
来源：http://crg.pycfn.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bms.zhoulong.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jlz.zhijiandao.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ptr.zdqjudy.top

TS:   if (!x) {}
来源：http://kmw.tianlin.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dwz.zhixingplan.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ecq.sjlbkw.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qmd.sxryk.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vxc.9152youxi.cn

[A17] 位运算
来源：http://cpe.bbcook.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ccl.wangshuangyany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bpq.svipenyu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://chy.svipenyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://guf.zhaomingkeji.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wtc.ybcxt.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cum.sufxvd.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zak.xuetiantiany.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lvm.cashguo.top

[A18] 字符与 ASCII 码互转
来源：http://tte.zhaomingkeji.xyz

Py:   ord("A"); chr(65)
来源：http://yiv.xingfuxueyuan.xyz

PHP:  ord("A"); chr(65)
来源：http://raa.sysykeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kxn.fanxiaobao.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hch.cqqwz.cn

Java: (int) 'A'; (char) 65
来源：http://sbq.daxiang520.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mux.yanxiufei.cn

Ruby: "A".ord; 65.chr
来源：http://fdn.wangshuangyany.cn

C#:   (int)'A'; (char)65
来源：http://zpn.ywan-chungtsiang.top

[A19] 交换两个变量
来源：http://wpr.fzhhl.top

Py:   a, b = b, a
来源：http://piz.daxiang520.top

PHP:  [$a, $b] = [$b, $a];
来源：http://lhq.cdnleiting.top

JS:   [a, b] = [b, a];
来源：http://awc.fanxiaobao.xyz

TS:   [a, b] = [b, a];
来源：http://hef.nanxinkj.top

Java: int t = a; a = b; b = t;
来源：http://ilg.xziqi.cn

Go:   a, b = b, a
来源：http://kbo.uphjek.com

Ruby: a, b = b, a
来源：http://mlx.yuanzhike.top

C#:   (a, b) = (b, a);
来源：http://gyp.gogol.net.cn

[A20] 读取标准输入
来源：http://xew.jianghu66.top

Py:   name = input("请输入：")
来源：http://ujv.pycfn.com

PHP:  $name = trim(fgets(STDIN));
来源：http://mez.pycfn.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cke.shanyushiyangtech.top

TS:   // Node.js：readline 模块
来源：http://rsa.hnxiangtu.top

Java: new Scanner(System.in).nextLine()
来源：http://itb.gotoacloud.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vst.zdbjq.cn

Ruby: gets.chomp
来源：http://zsd.ybcxt.top

C#:   Console.ReadLine();
来源：http://lfw.pycfn.com

[A21] 保留指定小数位输出
来源：http://zre.zhijiandao.cn

Py:   f"{3.14159:.2f}"
来源：http://yxe.ppjwa.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wbt.xinyue.icu

JS:   (3.14159).toFixed(2)
来源：http://str.bjfxy.top

TS:   (3.14159).toFixed(2)
来源：http://dbq.shzxlz.cn

Java: String.format("%.2f", 3.14159)
来源：http://wjt.zycfv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pba.sxryk.cn

Ruby: format("%.2f", 3.14159)
来源：http://lat.yonumen.top

C#:   3.14159.ToString("F2")
来源：http://ubf.feifeiyinyue.top

[A22] 获取字符串长度
来源：http://vzo.havefunace.top

Py:   len(s)
来源：http://aui.yonumen.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cbv.ehwqpu.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pse.ybcxt.top

TS:   s.length
来源：http://hxr.ctjpmb.com

Java: s.length()
来源：http://cfm.haohaochexian.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jcn.ppjwa.cn

Ruby: s.length
来源：http://fmy.sufxvd.cn

C#:   s.Length
来源：http://heg.zdqjudy.top

[A23] 大小写转换
来源：http://ujv.smart0.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://cfb.shanyushiyangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rrj.smart0.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zgq.jinqigfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ahk.daxiang520.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ygs.aibaodan.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uwj.xingfuxueyuan.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mnc.guowangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rto.andypj.xyz

[A24] 去除首尾空白
来源：http://ymc.jinqigfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://exv.kuanghao11.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kgb.yanxiufei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lfl.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ovo.pycfn.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iwp.vqdsnc.cn

Go:   strings.TrimSpace(s)
来源：http://gpo.nwbrower.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://usf.xylfe.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://udv.9152youxi.cn

[A25] 字符串比较
来源：http://plc.dianchejie.cn

Py:   s1 == s2; s1 != s2
来源：http://uuu.52xcode.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://unm.vehdjk.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cjs.bjfxy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://moj.fengsongda.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bzl.hysaishi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ctk.jyoumei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://otv.shangyingyoupin.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jzx.vehdjk.com

[A26] 类型转换总览
来源：http://rcu.chenjidiqi.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tcn.fehbvm.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rmn.xuanzx.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tdy.hfpthk.cn

TS:   Number() String() Boolean() x as number
来源：http://cbu.cashguo.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uvt.jqgfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qvj.jyoumei.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tqt.gaohongyu789.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://awm.xylfe.cn

================================================================================
来源：http://qfr.sufxvd.cn

B. 流程控制
来源：http://rtf.ydzc1.top

================================================================================
来源：http://iqb.hcnkem.com

[B01] 条件判断 if / else
来源：http://fvq.jinyuanbaomall.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tkz.tianlin.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bcm.ydjk.org.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qiy.sxryk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://auk.jinghuilouyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yqk.yonumen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tnj.zhongyouzk.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qnn.iojbl.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cbz.smart0.xyz

[B02] 多分支 else if / elif
来源：http://bjv.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ehz.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mbv.smart0.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hzs.nwbrower.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jdm.tarul.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cet.jinyuanbaomall.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://flq.shuidangran.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tbb.ydzc1.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tgt.zhoulong.xyz

[B03] switch / match / case
来源：http://gyh.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qdy.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zwz.shanyushiyangtech.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mko.ydzc1.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yjb.ydjk.org.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hji.yj202588.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dag.xylfe.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ukd.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yso.hfpthk.cn

[B04] for 计数循环
来源：http://ksl.zhijiandao.cn

Py:   for i in range(10): print(i)
来源：http://wml.fktsv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fhc.hysaishi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rvt.xinyue.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mlp.dianchejie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pis.tarul.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://niq.xinyue.icu

Ruby: 10.times { |i| puts i }
来源：http://aly.zhixingplan.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bjv.xylfe.cn

[B05] 遍历数组 / 列表
来源：http://gpu.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://iof.zhijiandao.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rtz.nanxuanxn.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cxn.fanxiaobao.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://exs.gogol.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vir.fktsv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sjd.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://wvp.ppjwa.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://juz.zhiwuduotai.top

[B06] 遍历字典 / 对象
来源：http://cnz.cheryme.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vyt.kuanghao11.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ahw.bjfxy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://thn.sweek.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iku.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ail.sweek.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://drh.fengsongda.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ija.zhengqikj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qdw.cashguo.top

[B07] while 循环
来源：http://chf.sufxvd.cn

Py:   while i < 10: i += 1
来源：http://cfr.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cmo.gaohongyu789.top

JS:   while (i < 10) { i++; }
来源：http://bnd.jlsjyb.cn

TS:   while (i < 10) { i++; }
来源：http://vrt.xylfe.cn

Java: while (i < 10) { i++; }
来源：http://dxw.sufxvd.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://umv.daxiang520.top

Ruby: while i < 10; i += 1; end
来源：http://wqm.ctjpmb.com

C#:   while (i < 10) { i++; }
来源：http://abp.sweek.top

[B08] do-while（至少执行一次）
来源：http://gwn.ywan-chungtsiang.top

Py:   # 无 do-while：用 while True + break
来源：http://jbh.fzhhl.top

PHP:  do { $i++; } while ($i < 10);
来源：http://idh.yongpay.top

JS:   do { i++; } while (i < 10);
来源：http://rxi.haohaochexian.top

TS:   do { i++; } while (i < 10);
来源：http://zmy.uphjek.com

Java: do { i++; } while (i < 10);
来源：http://utm.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zhg.cheryme.top

Ruby: begin; i += 1; end while i < 10
来源：http://uhw.zhiwuduotai.top

C#:   do { i++; } while (i < 10);
来源：http://eay.zhiwuduotai.top

[B09] break 与 continue
来源：http://xmv.0kj1m.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ifg.vqdsnc.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vea.meibo888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://brm.9152youxi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sat.tian-w.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zsf.fktsv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oku.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cat.dianchejie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qjt.ivvv.top

[B10] 遍历同时拿索引
来源：http://nyu.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iop.yfazqb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ycq.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://olp.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tkv.dianchejie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ive.sjlbkw.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yig.zhengqikj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oqk.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://omj.tarul.cn

[B11] 生成数字序列 / 区间
来源：http://tex.hnxiangtu.top

Py:   list(range(0, 10, 2))
来源：http://dto.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://vlm.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://olx.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mjq.nanxuanxn.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://awh.gogol.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kfz.shangyingyoupin.top

Ruby: (0...10).step(2).to_a
来源：http://yup.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://evq.gotoacloud.top

[B12] 跳出多层循环
来源：http://sbk.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nee.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pnb.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://whg.ppjwa.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tyw.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jso.hongshengwenyu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://usf.zhixingplan.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xsv.vehdjk.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pwa.zycfv.cn

[B13] 判断是否为数字
来源：http://gma.jinghuilouyu.cn

Py:   isinstance(x, (int, float))
来源：http://ydm.gotoacloud.top

PHP:  is_numeric($x)
来源：http://ofg.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ldt.bjfxy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hmq.mhx1999.top

Java: x instanceof Number
来源：http://nhw.hongshengwenyu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://elr.yangfankeji.com

Ruby: x.is_a?(Numeric)
来源：http://zrp.316326.xyz

C#:   x is int or double or decimal
来源：http://wok.zhijiandao.cn

[B14] 判断值是否在集合内
来源：http://jin.zdbjq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dun.zhijiandao.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kxh.daria6918.cn

JS:   [1, 2, 3].includes(x)
来源：http://xky.mhx1999.top

TS:   [1, 2, 3].includes(x)
来源：http://xzs.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://kmo.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zep.svipenyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zms.hammf.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ipl.fktsv.cn

[B15] 布尔运算与取反
来源：http://ntf.xziqi.cn

Py:   a and b or not c
来源：http://rta.iojbl.cn

PHP:  $a && $b || !$c
来源：http://cni.jqgufenzy.top

JS:   a && b || !c
来源：http://xct.zhengqikj.top

TS:   a && b || !c
来源：http://zrv.52xcode.cn

Java: a && b || !c
来源：http://usn.shzxlz.cn

Go:   a && b || !c
来源：http://qfd.tanke756.top

Ruby: a && b || !c
来源：http://mtb.chenjidiqi.icu

C#:   a && b || !c
来源：http://mob.hnxiangtu.top

[B16] 卫语句：不满足条件提前返回
来源：http://nxz.zhijiandao.cn

Py:   if not data: return
来源：http://dlr.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://bqu.fengsongda.top

JS:   if (!data) return;
来源：http://xvp.nanxuanxn.top

TS:   if (!data) return;
来源：http://cip.zdbjq.cn

Java: if (data == null) return;
来源：http://rtg.nanxuanxn.top

Go:   if data == nil { return }
来源：http://oai.gaohongyu789.top

Ruby: return if data.nil?
来源：http://lzq.cheryme.top

C#:   if (data == null) return;
来源：http://mqh.epnwcf.com

================================================================================
来源：http://omk.andypj.xyz

C. 函数与作用域
来源：http://jzh.zhixingplan.top

================================================================================
来源：http://xlq.zhongyouzk.top

[C01] 定义函数
来源：http://pku.tanke756.top


<!-- 参考信息 -->