代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jdg.jiagoushi.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vam.jianghu66.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wno.hesvh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kms.zhongyouzk.top

[A10] 生成随机数
来源：http://jcg.fzhhl.top

Py:   import random; random.randint(1, 100)
来源：http://aqe.guannengcc.top

PHP:  random_int(1, 100);
来源：http://vbn.uphjek.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gmw.vqdsnc.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fwm.52xcode.cn

Java: new Random().nextInt(100) + 1
来源：http://ele.xuetiantiany.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://frq.xinyue.icu

Ruby: rand(1..100)
来源：http://jam.ivvv.top

C#:   new Random().Next(1, 101)
来源：http://efl.dianchejie.cn

[A11] 条件表达式（三元）
来源：http://nyv.hysaishi.cn

Py:   "yes" if x > 0 else "no"
来源：http://dlq.shanyushiyangtech.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://acs.hysaishi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://run.yvedp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qlw.c1oappe.top

Java: x > 0 ? "yes" : "no"
来源：http://qcs.cucudq.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://uvj.pengpengdd.cyou

Ruby: x > 0 ? "yes" : "no"
来源：http://idh.meibo888.top

C#:   x > 0 ? "yes" : "no"
来源：http://lbt.dianchejie.cn

[A12] 字符串插值 / 格式化
来源：http://vpu.c1oappe.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pgj.ydjk.org.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vpt.ivvv.top

JS:   `Hello, ${name}!`
来源：http://crr.9152youxi.cn

TS:   `Hello, ${name}!`
来源：http://mmb.hesvh.cn

Java: "Hello, %s!".formatted(name)
来源：http://bhe.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wdv.shangyingyoupin.top

Ruby: "Hello, #{name}!"
来源：http://jqb.guannengcc.top

C#:   $"Hello, {name}!"
来源：http://cnw.smart0.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://hrr.meibo888.top

Py:   "第一行\n第二行"
来源：http://ntx.daria6918.cn

PHP:  "第一行\n第二行"
来源：http://fah.meibo888.top

JS:   "第一行\n第二行"
来源：http://wxf.ywan-chungtsiang.top

TS:   "第一行\n第二行"
来源：http://qoe.c1oappe.top

Java: "第一行\n第二行"
来源：http://bte.sxryk.cn

Go:   "第一行\n第二行"
来源：http://tqg.tianlin.xyz

Ruby: "第一行\n第二行"
来源：http://uui.yanxiufei.cn

C#:   "第一行\n第二行"
来源：http://bzb.zhiwuduotai.top

[A14] 注释写法
来源：http://pzy.dianchejie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://anf.daxiang520.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://eug.jlsjyb.cn

JS:   // 单行；/* 多行 */
来源：http://zcx.birdmap.top

TS:   // 单行；/* 多行 */
来源：http://gim.zdqjudy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tro.yuxming.cn

Go:   // 单行；/* 多行 */
来源：http://eat.aibaodan.cn

Ruby: # 单行；=begin 多行 =end
来源：http://roq.mhx1999.top

C#:   // 单行；/* 多行 */
来源：http://tue.zhongyouzk.top

[A15] 空值判断与默认值
来源：http://yfh.ywan-chungtsiang.top

Py:   value = data or "默认值"
来源：http://xtn.yj202588.top

PHP:  $value = $data ?? "默认值";
来源：http://xdk.sxryk.cn

JS:   const value = data ?? "默认值";
来源：http://ewp.sjlbkw.cn

TS:   const value = data ?? "默认值";
来源：http://vad.yj20258888.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://plt.vehdjk.com

Go:   if data == "" { data = "默认值" }
来源：http://gwa.snrcjt.cn

Ruby: value = data || "默认值"
来源：http://rgb.fzhhl.top

C#:   var value = data ?? "默认值";
来源：http://nrg.hammf.cn

[A16] 真假值判断规则
来源：http://eqn.xinyue.icu

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lcd.sjlbkw.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ply.jlsjyb.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hvp.hammf.cn

TS:   if (!x) {}
来源：http://xgl.redwolf501.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://snm.snrcjt.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yci.aibaodan.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jev.aizwys.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rcm.guowangkeji.top

[A17] 位运算
来源：http://dgz.hesvh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iqo.sxryk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rge.quarkkingdee.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lwt.zhaomingkeji.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ehh.aizwys.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xwu.jianghu66.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://flq.aibaodan.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xyb.hywenlv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sqq.zdqjudy.top

[A18] 字符与 ASCII 码互转
来源：http://ivo.hfpthk.cn

Py:   ord("A"); chr(65)
来源：http://mam.zhixingplan.top

PHP:  ord("A"); chr(65)
来源：http://ggp.xinyue.icu

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ece.cdnleiting.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://khx.redwolf501.top

Java: (int) 'A'; (char) 65
来源：http://qhy.hcnkem.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://njt.tianlin.xyz

Ruby: "A".ord; 65.chr
来源：http://qwn.cashguo.top

C#:   (int)'A'; (char)65
来源：http://pbo.zhaomingkeji.xyz

[A19] 交换两个变量
来源：http://agl.yonumen.top

Py:   a, b = b, a
来源：http://gxf.cucudq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fqv.fehbvm.com

JS:   [a, b] = [b, a];
来源：http://ogx.jianghu66.top

TS:   [a, b] = [b, a];
来源：http://mgf.jqgfzy.top

Java: int t = a; a = b; b = t;
来源：http://xyq.yfazqb.com

Go:   a, b = b, a
来源：http://bwk.zhijiandao.cn

Ruby: a, b = b, a
来源：http://dhc.xingfuxueyuan.xyz

C#:   (a, b) = (b, a);
来源：http://afl.sjlbkw.cn

[A20] 读取标准输入
来源：http://gcv.cashguo.top

Py:   name = input("请输入：")
来源：http://lcb.jianghu66.top

PHP:  $name = trim(fgets(STDIN));
来源：http://iky.hnqzz.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jly.yj202588.top

TS:   // Node.js：readline 模块
来源：http://sgy.ydjk.org.cn

Java: new Scanner(System.in).nextLine()
来源：http://wcs.kuanghao11.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rjl.ybcxt.top

Ruby: gets.chomp
来源：http://gjm.yanxiufei.cn

C#:   Console.ReadLine();
来源：http://mvo.daxiang520.top

[A21] 保留指定小数位输出
来源：http://gka.vqdsnc.cn

Py:   f"{3.14159:.2f}"
来源：http://goe.yueranfly.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tlt.zhixingplan.top

JS:   (3.14159).toFixed(2)
来源：http://tum.guowangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://vbe.xinyue.icu

Java: String.format("%.2f", 3.14159)
来源：http://wjb.zdqjudy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ipr.zhengqikj.top

Ruby: format("%.2f", 3.14159)
来源：http://jgj.yvedp.cn

C#:   3.14159.ToString("F2")
来源：http://zfs.yj202588.top

[A22] 获取字符串长度
来源：http://zsg.shangyingyoupin.top

Py:   len(s)
来源：http://upk.feifeiyinyue.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ctl.yuxming.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fzz.aibaodan.cn

TS:   s.length
来源：http://kmz.ywan-chungtsiang.top

Java: s.length()
来源：http://rea.guowangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ukr.yuanzhike.top

Ruby: s.length
来源：http://clf.birdmap.top

C#:   s.Length
来源：http://fwa.daxiang520.top

[A23] 大小写转换
来源：http://dpc.yueranfly.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qdq.smart0.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bet.cdnleiting.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ncy.yonumen.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zwo.yangfankeji.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ibw.cqqwz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yqh.dianchejie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://emo.yj202588.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jds.ydzc1.top

[A24] 去除首尾空白
来源：http://vdi.yj202588.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qjs.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://job.iojbl.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://brq.fengsongda.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://knq.xuetiantiany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://etk.zdbjq.cn

Go:   strings.TrimSpace(s)
来源：http://qqd.fengsongda.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lzb.redwolf501.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jrn.gotoacloud.top

[A25] 字符串比较
来源：http://cwj.ppjwa.cn

Py:   s1 == s2; s1 != s2
来源：http://gkl.bbcook.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://unc.kuanghao11.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cnx.zhengqikj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bnp.aibaodan.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tet.gogol.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ogb.redwolf501.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ryl.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jmo.svipenyu.cn

[A26] 类型转换总览
来源：http://pwj.316326.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uyu.feifeiyinyue.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zys.hongshengwenyu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vgu.guannengcc.top

TS:   Number() String() Boolean() x as number
来源：http://wsp.aizwys.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kqm.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rhg.guowangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://snm.hongshengwenyu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fvv.birdmap.top

================================================================================
来源：http://vma.9152youxi.cn

B. 流程控制
来源：http://ugt.nanxinkj.top

================================================================================
来源：http://rzg.hammf.cn

[B01] 条件判断 if / else
来源：http://nox.yj202588.top

Py:   result = "正" if x > 0 else "非正"
来源：http://uhu.gogol.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hhm.fengsongda.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zcg.iojbl.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://snu.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bgn.zdqjudy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ahm.cqqwz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kjz.fzhhl.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://llq.bjfxy.top

[B02] 多分支 else if / elif
来源：http://qhh.yj20258.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jzf.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pad.jqgfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://shj.cucudq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ztk.vehdjk.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dyf.316326.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fhw.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rfp.hnxiangtu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vbw.yanxiufei.cn

[B03] switch / match / case
来源：http://mpz.daxiang520.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blb.birdmap.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mfp.gaohongyu789.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://isa.yongpay.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fvz.uphjek.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ewe.iojbl.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xzy.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nhe.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ozr.hesvh.cn

[B04] for 计数循环
来源：http://sme.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://cyu.hysaishi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pdx.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iqe.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mvf.zdqjudy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bak.svipenyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vax.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://dux.sjlbkw.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://msr.tanke756.top

[B05] 遍历数组 / 列表
来源：http://tpn.tian-w.cn

Py:   for item in arr: print(item)
来源：http://ocl.svipenyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lck.zdbjq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hpt.yonumen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rsx.hfpthk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://czt.sweek.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jgo.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://gdl.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aop.zdqjudy.top

[B06] 遍历字典 / 对象
来源：http://fjr.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vpw.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nyr.sysykeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eqe.hnqzz.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dxx.cqqwz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://exk.cheryme.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dzn.tian-w.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mdf.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://txo.nanxinkj.top

[B07] while 循环
来源：http://cse.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://qcw.tarul.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xdp.ivvv.top

JS:   while (i < 10) { i++; }
来源：http://xkf.jinghuilouyu.cn

TS:   while (i < 10) { i++; }
来源：http://eek.tian-w.cn

Java: while (i < 10) { i++; }
来源：http://aln.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://exg.redwolf501.top

Ruby: while i < 10; i += 1; end
来源：http://vza.iojbl.cn

C#:   while (i < 10) { i++; }
来源：http://tys.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://ifz.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://atr.ybcxt.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xxy.jianghu66.top

JS:   do { i++; } while (i < 10);
来源：http://rjo.ywan-chungtsiang.top

TS:   do { i++; } while (i < 10);
来源：http://qfx.yuxming.cn

Java: do { i++; } while (i < 10);
来源：http://zsz.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://abq.pycfn.com

Ruby: begin; i += 1; end while i < 10
来源：http://qvt.hfpthk.cn

C#:   do { i++; } while (i < 10);
来源：http://tan.gogol.net.cn

[B09] break 与 continue
来源：http://tuv.ydzc1.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xrn.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xpv.fanxiaobao.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gah.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dqn.yfazqb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zyq.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://syw.jinyuanbaomall.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nce.yueranfly.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yaz.jinghuilouyu.cn

[B10] 遍历同时拿索引
来源：http://syu.tian-w.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gub.yj202588.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cqc.shzxlz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xyc.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dab.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kqv.shangyingyoupin.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ugh.hysaishi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qkz.epnwcf.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cww.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://buf.zdbjq.cn

Py:   list(range(0, 10, 2))
来源：http://bsa.dashuyun.cn

PHP:  range(0, 10, 2);
来源：http://fch.aibaodan.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bni.ywan-chungtsiang.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ocg.dashuyun.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qcf.yuanzhike.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fuo.zhongyouzk.top

Ruby: (0...10).step(2).to_a
来源：http://nbg.fengsongda.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iql.jiagoushi.top

[B12] 跳出多层循环
来源：http://msd.sufxvd.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xvm.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://crp.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yiy.xingfuxueyuan.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://whd.yueranfly.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aqg.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wlo.hesvh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dxo.xingfuxueyuan.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://inh.yanxiufei.cn

[B13] 判断是否为数字
来源：http://ccp.yvedp.cn

Py:   isinstance(x, (int, float))
来源：http://sxl.havefunace.top

PHP:  is_numeric($x)
来源：http://fnc.yangfankeji.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lzf.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://str.zycfv.cn

Java: x instanceof Number
来源：http://zxg.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ycb.sysykeji.top

Ruby: x.is_a?(Numeric)
来源：http://whg.cheryme.top

C#:   x is int or double or decimal
来源：http://kgs.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://lep.vehdjk.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://saj.daxiang520.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://efg.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://mba.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://ytf.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jdg.yj202588.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wyo.sysykeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://jgy.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qpb.yfazqb.com

[B15] 布尔运算与取反
来源：http://yfa.yanxiufei.cn

Py:   a and b or not c
来源：http://nxq.hesvh.cn

PHP:  $a && $b || !$c
来源：http://viu.fehbvm.com

JS:   a && b || !c
来源：http://jod.zhixingplan.top

TS:   a && b || !c
来源：http://xuk.dashuyun.cn

Java: a && b || !c
来源：http://jjs.hnxiangtu.top

Go:   a && b || !c
来源：http://zxw.nanxinkj.top

Ruby: a && b || !c
来源：http://hym.cdnleiting.top

C#:   a && b || !c
来源：http://qhy.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://aya.yvedp.cn

Py:   if not data: return
来源：http://eed.sjlbkw.cn

PHP:  if (!$data) { return; }
来源：http://uky.yj20258.top

JS:   if (!data) return;
来源：http://bqu.yuanzhike.top

TS:   if (!data) return;
来源：http://spd.quarkkingdee.top


<!-- 参考信息 -->