代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wvh.shuidangran.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tai.hfpthk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ufl.jinqigfzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dii.zhengqikj.top

[A10] 生成随机数
来源：http://rhp.hywenlv.cn

Py:   import random; random.randint(1, 100)
来源：http://jsu.jlsjyb.cn

PHP:  random_int(1, 100);
来源：http://ltx.cqqwz.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://whh.dianchejie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qez.jqgfzy.top

Java: new Random().nextInt(100) + 1
来源：http://gtw.havefunace.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://eva.zhaomingkeji.xyz

Ruby: rand(1..100)
来源：http://tqx.cheryme.top

C#:   new Random().Next(1, 101)
来源：http://zuz.yuxming.cn

[A11] 条件表达式（三元）
来源：http://fwm.ehwqpu.com

Py:   "yes" if x > 0 else "no"
来源：http://fok.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mfm.nwbrower.top

JS:   x > 0 ? "yes" : "no"
来源：http://vgy.yueranfly.top

TS:   x > 0 ? "yes" : "no"
来源：http://fzd.dashuyun.cn

Java: x > 0 ? "yes" : "no"
来源：http://gzc.zhoulong.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://udv.yj202588.top

Ruby: x > 0 ? "yes" : "no"
来源：http://hyz.shanyushiyangkeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://zii.ehwqpu.com

[A12] 字符串插值 / 格式化
来源：http://civ.sjlbkw.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pqi.ppjwa.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lrv.dashuyun.cn

JS:   `Hello, ${name}!`
来源：http://eby.bbcook.cn

TS:   `Hello, ${name}!`
来源：http://uxf.hnxiangtu.top

Java: "Hello, %s!".formatted(name)
来源：http://jzb.gzhubu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zfa.aizwys.cn

Ruby: "Hello, #{name}!"
来源：http://htj.hywenlv.cn

C#:   $"Hello, {name}!"
来源：http://dce.wangshuangyany.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vxm.mhx1999.top

Py:   "第一行\n第二行"
来源：http://uvm.jinqigfzy.top

PHP:  "第一行\n第二行"
来源：http://hkx.zhiwuduotai.top

JS:   "第一行\n第二行"
来源：http://huo.yangfankeji.com

TS:   "第一行\n第二行"
来源：http://hsx.gotoacloud.top

Java: "第一行\n第二行"
来源：http://awn.yonumen.top

Go:   "第一行\n第二行"
来源：http://icu.xingfuxueyuan.xyz

Ruby: "第一行\n第二行"
来源：http://evc.hnxiangtu.top

C#:   "第一行\n第二行"
来源：http://see.iojbl.cn

[A14] 注释写法
来源：http://ijd.yangfankeji.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://pdq.vqdsnc.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://efw.quarkkingdee.top

JS:   // 单行；/* 多行 */
来源：http://txu.zhixingplan.top

TS:   // 单行；/* 多行 */
来源：http://eqs.zdbjq.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://avf.gogol.net.cn

Go:   // 单行；/* 多行 */
来源：http://ofr.fehbvm.com

Ruby: # 单行；=begin 多行 =end
来源：http://ulp.cashguo.top

C#:   // 单行；/* 多行 */
来源：http://zkc.hnxiangtu.top

[A15] 空值判断与默认值
来源：http://nal.jiagoushi.top

Py:   value = data or "默认值"
来源：http://yyv.yanxiufei.cn

PHP:  $value = $data ?? "默认值";
来源：http://rrv.dianchejie.cn

JS:   const value = data ?? "默认值";
来源：http://mkh.fanxiaobao.xyz

TS:   const value = data ?? "默认值";
来源：http://qef.sxryk.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fpj.shanyushiyangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://yjw.wangdashe.top

Ruby: value = data || "默认值"
来源：http://xyb.haohaochexian.top

C#:   var value = data ?? "默认值";
来源：http://ltt.fzhhl.top

[A16] 真假值判断规则
来源：http://ynf.zdqjudy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ytx.sjlbkw.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eac.ehwqpu.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cvq.shzxlz.cn

TS:   if (!x) {}
来源：http://jvg.ppjwa.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xxj.xylfe.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ayr.yj202588.top

Ruby: unless x            # nil 与 false 为假
来源：http://zpa.cqqwz.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://npo.zdbjq.cn

[A17] 位运算
来源：http://zrr.shanyushiyangtech.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zma.gzhubu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vqj.c1oappe.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lmi.svipenyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qsn.316326.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://opv.jqgfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ytz.zycfv.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://osf.hywenlv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mgv.jqgfzy.top

[A18] 字符与 ASCII 码互转
来源：http://ogu.daria6918.cn

Py:   ord("A"); chr(65)
来源：http://rso.zhengqikj.top

PHP:  ord("A"); chr(65)
来源：http://vtu.xylfe.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://unj.hongshengwenyu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://djh.nanxuanxn.top

Java: (int) 'A'; (char) 65
来源：http://pry.andypj.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zil.cqqwz.cn

Ruby: "A".ord; 65.chr
来源：http://zvw.tarul.cn

C#:   (int)'A'; (char)65
来源：http://zki.shanyushiyangtech.top

[A19] 交换两个变量
来源：http://ccs.tian-w.cn

Py:   a, b = b, a
来源：http://uzv.ywan-chungtsiang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ylu.zhongyouzk.top

JS:   [a, b] = [b, a];
来源：http://iup.dashuyun.cn

TS:   [a, b] = [b, a];
来源：http://fci.cdnleiting.top

Java: int t = a; a = b; b = t;
来源：http://gts.sweek.top

Go:   a, b = b, a
来源：http://dnk.hnqzz.top

Ruby: a, b = b, a
来源：http://ovm.havefunace.top

C#:   (a, b) = (b, a);
来源：http://qta.yj202588.top

[A20] 读取标准输入
来源：http://ddy.cheryme.top

Py:   name = input("请输入：")
来源：http://jmt.jinqigfzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zsb.feifeiyinyue.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://via.nanxinkj.top

TS:   // Node.js：readline 模块
来源：http://isx.gogol.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://riz.hammf.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mhw.jqgfzy.top

Ruby: gets.chomp
来源：http://eyr.yonumen.top

C#:   Console.ReadLine();
来源：http://xik.ehwqpu.com

[A21] 保留指定小数位输出
来源：http://icg.ydjk.org.cn

Py:   f"{3.14159:.2f}"
来源：http://qpx.kuanghao11.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://guw.zdbjq.cn

JS:   (3.14159).toFixed(2)
来源：http://owy.yj20258.top

TS:   (3.14159).toFixed(2)
来源：http://tby.xuanzx.com

Java: String.format("%.2f", 3.14159)
来源：http://nvp.vqdsnc.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kcc.redwolf501.top

Ruby: format("%.2f", 3.14159)
来源：http://yxz.svipenyu.cn

C#:   3.14159.ToString("F2")
来源：http://efd.hysaishi.cn

[A22] 获取字符串长度
来源：http://rrp.gogol.net.cn

Py:   len(s)
来源：http://cxa.cashguo.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://htw.iojbl.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wed.uphjek.com

TS:   s.length
来源：http://ejh.dashuyun.cn

Java: s.length()
来源：http://scg.ctjpmb.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://egm.52xcode.cn

Ruby: s.length
来源：http://ywd.yanxiufei.cn

C#:   s.Length
来源：http://qae.chenlongwang.top

[A23] 大小写转换
来源：http://onu.cashguo.top

Py:   s.upper(); s.lower(); s.title()
来源：http://fsx.ywan-chungtsiang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nve.sweek.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ljo.sufxvd.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mye.mhx1999.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bvv.vehdjk.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ysd.haohaochexian.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jpg.fanxiaobao.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://zbu.tian-w.cn

[A24] 去除首尾空白
来源：http://our.guowangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://abo.fzhhl.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hsu.shanyushiyangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hwa.52xcode.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://srq.yj202588.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hku.zhengqikj.top

Go:   strings.TrimSpace(s)
来源：http://leq.zycfv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wlx.nanxinkj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ato.fehbvm.com

[A25] 字符串比较
来源：http://oyq.zdqjudy.top

Py:   s1 == s2; s1 != s2
来源：http://fta.ydzc1.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eie.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rmn.ppjwa.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lrg.fengsongda.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jav.316326.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oke.ybcxt.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jjf.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cge.jianghu66.top

[A26] 类型转换总览
来源：http://rdt.tanke756.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pev.fengsongda.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mkd.cucudq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oiw.iojbl.cn

TS:   Number() String() Boolean() x as number
来源：http://pkp.ppjwa.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gly.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ukm.ybcxt.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fnc.yj20258.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ztz.sufxvd.cn

================================================================================
来源：http://rxa.shanyushiyangkeji.top

B. 流程控制
来源：http://ywd.tanke756.top

================================================================================
来源：http://tkr.zhaomingkeji.xyz

[B01] 条件判断 if / else
来源：http://npj.zycfv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yup.chenlongwang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://crq.pengpengdd.cyou

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nzo.0kj1m.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://upo.tianlin.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://kit.fanxiaobao.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lbs.gotoacloud.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://prf.epnwcf.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fva.cucudq.cn

[B02] 多分支 else if / elif
来源：http://alj.dianchejie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pzl.jinyuanbaomall.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://skr.sufxvd.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tnk.gotoacloud.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lso.yuxming.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qcy.aibaodan.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://chf.hcnkem.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yco.zdqjudy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gfg.hongshengwenyu.top

[B03] switch / match / case
来源：http://wux.shanyushiyangtech.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://etk.quarkkingdee.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zun.bjfxy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mhu.zhaomingkeji.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yhf.kuanghao11.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dww.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hit.zhijiandao.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ads.smart0.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mnl.zdqjudy.top

[B04] for 计数循环
来源：http://bkt.xuanzx.com

Py:   for i in range(10): print(i)
来源：http://mxw.9152youxi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qkb.ydjk.org.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ulk.redwolf501.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://izz.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fwc.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wdo.xylfe.cn

Ruby: 10.times { |i| puts i }
来源：http://mxv.fanxiaobao.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tjw.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://ldq.ywan-chungtsiang.top

Py:   for item in arr: print(item)
来源：http://ldb.tianlin.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zny.havefunace.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yem.nanxinkj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rtz.tianlin.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://yvl.vehdjk.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jgm.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://pwj.zdbjq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bwu.quarkkingdee.top

[B06] 遍历字典 / 对象
来源：http://mpx.yanxiufei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jfu.yj20258888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zzf.zhaomingkeji.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kiy.snrcjt.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://flu.nanxinkj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qoi.chenlongwang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rdw.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ehv.zhiwuduotai.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://maf.zhaomingkeji.xyz

[B07] while 循环
来源：http://djd.sysykeji.top

Py:   while i < 10: i += 1
来源：http://lvh.zycfv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oha.jlsjyb.cn

JS:   while (i < 10) { i++; }
来源：http://efx.yfazqb.com

TS:   while (i < 10) { i++; }
来源：http://vub.bjfxy.top

Java: while (i < 10) { i++; }
来源：http://ylr.cucudq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dla.zhixingplan.top

Ruby: while i < 10; i += 1; end
来源：http://tpt.meibo888.top

C#:   while (i < 10) { i++; }
来源：http://ycj.vqdsnc.cn

[B08] do-while（至少执行一次）
来源：http://vlv.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://sld.316326.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://jsl.ywan-chungtsiang.top

JS:   do { i++; } while (i < 10);
来源：http://rvk.hnqzz.top

TS:   do { i++; } while (i < 10);
来源：http://dgb.hnxiangtu.top

Java: do { i++; } while (i < 10);
来源：http://mkl.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://noh.dashuyun.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kxl.ydjk.org.cn

C#:   do { i++; } while (i < 10);
来源：http://zde.epnwcf.com

[B09] break 与 continue
来源：http://ftk.zhijiandao.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bmx.hywenlv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pig.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oil.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bur.ehwqpu.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kra.52xcode.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dtv.ivvv.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://epm.yonumen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jga.nanxuanxn.top

[B10] 遍历同时拿索引
来源：http://huh.cqqwz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://idk.aibaodan.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oed.zhixingplan.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nqw.haohaochexian.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ekm.redwolf501.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lhm.zycfv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nnt.shzxlz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://esr.yueranfly.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vlw.vehdjk.com

[B11] 生成数字序列 / 区间
来源：http://afl.vqdsnc.cn

Py:   list(range(0, 10, 2))
来源：http://wjw.xylfe.cn

PHP:  range(0, 10, 2);
来源：http://nwb.hnxiangtu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://thk.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ukj.jqgufenzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://igf.hywenlv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aau.birdmap.top

Ruby: (0...10).step(2).to_a
来源：http://xuj.yueranfly.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rga.fanxiaobao.xyz

[B12] 跳出多层循环
来源：http://ixp.xuanzx.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://zpa.yj20258888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cav.ywan-chungtsiang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yrm.kuanghao11.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wln.jqgufenzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://egp.hywenlv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://noe.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ywu.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://apk.havefunace.top

[B13] 判断是否为数字
来源：http://odg.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://ymk.hywenlv.cn

PHP:  is_numeric($x)
来源：http://hyp.jlsjyb.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sgz.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mjb.hcnkem.com

Java: x instanceof Number
来源：http://dbe.zhengqikj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hpv.ivvv.top

Ruby: x.is_a?(Numeric)
来源：http://woh.hfpthk.cn

C#:   x is int or double or decimal
来源：http://xbu.fzhhl.top

[B14] 判断值是否在集合内
来源：http://slj.quarkkingdee.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jod.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tkq.havefunace.top

JS:   [1, 2, 3].includes(x)
来源：http://ehj.ctjpmb.com

TS:   [1, 2, 3].includes(x)
来源：http://law.yangfankeji.com

Java: List.of(1, 2, 3).contains(x)
来源：http://nud.dashuyun.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iwo.shangyingyoupin.top

Ruby: [1, 2, 3].include?(x)
来源：http://cns.cheryme.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rnc.fktsv.cn

[B15] 布尔运算与取反
来源：http://abn.jianghu66.top

Py:   a and b or not c
来源：http://lwy.quarkkingdee.top

PHP:  $a && $b || !$c
来源：http://cpi.gogol.net.cn

JS:   a && b || !c
来源：http://qst.shuidangran.top

TS:   a && b || !c
来源：http://lvf.hysaishi.cn

Java: a && b || !c
来源：http://xxk.gogol.net.cn

Go:   a && b || !c
来源：http://vli.zdqjudy.top

Ruby: a && b || !c
来源：http://lqr.yuxming.cn

C#:   a && b || !c
来源：http://ccn.yvedp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://its.wangshuangyany.cn

Py:   if not data: return
来源：http://len.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://xsc.ydjk.org.cn

JS:   if (!data) return;
来源：http://qfk.daxiang520.top

TS:   if (!data) return;
来源：http://hnn.jinqigufen.top


<!-- 参考信息 -->