代发 wailian999

[A10] 生成随机数
来源：http://fcg.hnxiangtu.top

Py:   import random; random.randint(1, 100)
来源：http://mwu.xziqi.cn

PHP:  random_int(1, 100);
来源：http://jph.sweek.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nwn.wangdashe.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dvm.yj20258.top

Java: new Random().nextInt(100) + 1
来源：http://vit.jqgfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wwb.redwolf501.top

Ruby: rand(1..100)
来源：http://hgm.hongshengwenyu.top

C#:   new Random().Next(1, 101)
来源：http://jnc.havefunace.top

[A11] 条件表达式（三元）
来源：http://dyl.ybcxt.top

Py:   "yes" if x > 0 else "no"
来源：http://zkt.jlsjyb.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://phi.52xcode.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lqm.ehwqpu.com

TS:   x > 0 ? "yes" : "no"
来源：http://kve.ydjk.org.cn

Java: x > 0 ? "yes" : "no"
来源：http://boe.xinyue.icu

Go:   // 无三元运算符，需用 if 语句
来源：http://azl.zhoulong.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://rpf.316326.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://ats.hnqzz.top

[A12] 字符串插值 / 格式化
来源：http://asl.ppjwa.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ivt.yuanzhike.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tye.shanyushiyangtech.top

JS:   `Hello, ${name}!`
来源：http://vby.yfazqb.com

TS:   `Hello, ${name}!`
来源：http://vji.jinyuanbaomall.cn

Java: "Hello, %s!".formatted(name)
来源：http://nfl.tanke756.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cbs.52xcode.cn

Ruby: "Hello, #{name}!"
来源：http://gmk.cucudq.cn

C#:   $"Hello, {name}!"
来源：http://jpl.daxiang520.top

[A13] 多行字符串（练习 \n 转义）
来源：http://kln.yj202588.top

Py:   "第一行\n第二行"
来源：http://iyb.zhaomingkeji.xyz

PHP:  "第一行\n第二行"
来源：http://xwu.jqgufenzy.top

JS:   "第一行\n第二行"
来源：http://wtp.jinghuilouyu.cn

TS:   "第一行\n第二行"
来源：http://qqn.xingfuxueyuan.xyz

Java: "第一行\n第二行"
来源：http://lsl.wangshuangyany.cn

Go:   "第一行\n第二行"
来源：http://joi.zhoulong.xyz

Ruby: "第一行\n第二行"
来源：http://hif.nanxinkj.top

C#:   "第一行\n第二行"
来源：http://otp.xingfuxueyuan.xyz

[A14] 注释写法
来源：http://ekg.zhiwuduotai.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qbw.tianlin.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://zzp.zhongyouzk.top

JS:   // 单行；/* 多行 */
来源：http://olj.zhaomingkeji.xyz

TS:   // 单行；/* 多行 */
来源：http://gmg.jyoumei.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://arg.bbcook.cn

Go:   // 单行；/* 多行 */
来源：http://pyw.cucudq.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jjl.daria6918.cn

C#:   // 单行；/* 多行 */
来源：http://sco.yuanzhike.top

[A15] 空值判断与默认值
来源：http://hhl.iojbl.cn

Py:   value = data or "默认值"
来源：http://xdi.hongshengwenyu.top

PHP:  $value = $data ?? "默认值";
来源：http://pzz.shzxlz.cn

JS:   const value = data ?? "默认值";
来源：http://jla.wangshuangyany.cn

TS:   const value = data ?? "默认值";
来源：http://lco.gzhubu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kjf.wangshuangyany.cn

Go:   if data == "" { data = "默认值" }
来源：http://dnv.wangdashe.top

Ruby: value = data || "默认值"
来源：http://qsx.shuidangran.top

C#:   var value = data ?? "默认值";
来源：http://gqb.yanxiufei.cn

[A16] 真假值判断规则
来源：http://iem.svipenyu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ivp.sjlbkw.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jic.jqgfzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uou.dianchejie.cn

TS:   if (!x) {}
来源：http://wua.ybcxt.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oqw.pycfn.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nub.zdbjq.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lkg.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uak.epnwcf.com

[A17] 位运算
来源：http://nqw.tian-w.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yii.shangyingyoupin.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xvq.tanke756.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ztv.fehbvm.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://otd.zhaomingkeji.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://deh.wangshuangyany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://aip.hfpthk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ado.pengpengdd.cyou

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qya.jqgufenzy.top

[A18] 字符与 ASCII 码互转
来源：http://dut.zhoulong.xyz

Py:   ord("A"); chr(65)
来源：http://ghz.guowangkeji.top

PHP:  ord("A"); chr(65)
来源：http://esm.zdqjudy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hze.jyoumei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kdg.jqgufenzy.top

Java: (int) 'A'; (char) 65
来源：http://jmj.aizwys.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lyn.ydjk.org.cn

Ruby: "A".ord; 65.chr
来源：http://tmo.birdmap.top

C#:   (int)'A'; (char)65
来源：http://kak.ydjk.org.cn

[A19] 交换两个变量
来源：http://lwt.cqqwz.cn

Py:   a, b = b, a
来源：http://nwr.xylfe.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zld.nanxinkj.top

JS:   [a, b] = [b, a];
来源：http://tnb.shanyushiyangkeji.top

TS:   [a, b] = [b, a];
来源：http://kfg.fengsongda.top

Java: int t = a; a = b; b = t;
来源：http://eaq.guowangkeji.top

Go:   a, b = b, a
来源：http://ngc.birdmap.top

Ruby: a, b = b, a
来源：http://jnc.iojbl.cn

C#:   (a, b) = (b, a);
来源：http://rul.birdmap.top

[A20] 读取标准输入
来源：http://nuw.zhoulong.xyz

Py:   name = input("请输入：")
来源：http://xlj.fengsongda.top

PHP:  $name = trim(fgets(STDIN));
来源：http://gmk.zdbjq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ukm.zhixingplan.top

TS:   // Node.js：readline 模块
来源：http://ikz.jinyuanbaomall.cn

Java: new Scanner(System.in).nextLine()
来源：http://kfc.yfazqb.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xbh.sweek.top

Ruby: gets.chomp
来源：http://ylq.jqgfzy.top

C#:   Console.ReadLine();
来源：http://lpd.aibaodan.cn

[A21] 保留指定小数位输出
来源：http://nwm.cashguo.top

Py:   f"{3.14159:.2f}"
来源：http://uhg.316326.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mzg.fzhhl.top

JS:   (3.14159).toFixed(2)
来源：http://bnf.nanxuanxn.top

TS:   (3.14159).toFixed(2)
来源：http://rkz.sxryk.cn

Java: String.format("%.2f", 3.14159)
来源：http://rtn.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vyz.ydjk.org.cn

Ruby: format("%.2f", 3.14159)
来源：http://dnn.jiagoushi.top

C#:   3.14159.ToString("F2")
来源：http://zjj.zdbjq.cn

[A22] 获取字符串长度
来源：http://twp.fzhhl.top

Py:   len(s)
来源：http://ust.kuanghao11.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eaj.pycfn.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hve.shanyushiyangkeji.top

TS:   s.length
来源：http://gzk.fengsongda.top

Java: s.length()
来源：http://fvs.xylfe.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://clm.zhaomingkeji.xyz

Ruby: s.length
来源：http://vea.svipenyu.cn

C#:   s.Length
来源：http://umn.andypj.xyz

[A23] 大小写转换
来源：http://cnh.aizwys.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://oqn.gogol.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://riw.gotoacloud.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xwv.xuetiantiany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ukn.jlsjyb.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fxz.gotoacloud.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wlr.andypj.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hdf.yonumen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bsm.zhengqikj.top

[A24] 去除首尾空白
来源：http://wms.jqgfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kvg.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dov.yuanzhike.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jwb.fktsv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bie.zdbjq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qyi.zdbjq.cn

Go:   strings.TrimSpace(s)
来源：http://kgs.ydjk.org.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zub.pycfn.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tcg.yuxming.cn

[A25] 字符串比较
来源：http://emq.zdbjq.cn

Py:   s1 == s2; s1 != s2
来源：http://rgk.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pfx.bbcook.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jhx.xuetiantiany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tnn.yj20258.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://olk.hammf.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ihd.jlsjyb.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kzp.mhx1999.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wjc.tanke756.top

[A26] 类型转换总览
来源：http://kdf.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qnk.dashuyun.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://deo.tian-w.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://abd.shangyingyoupin.top

TS:   Number() String() Boolean() x as number
来源：http://cef.mhx1999.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wcu.daxiang520.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bcl.pycfn.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://mfo.ywan-chungtsiang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mng.zdqjudy.top

================================================================================
来源：http://axr.nwbrower.top

B. 流程控制
来源：http://kav.uphjek.com

================================================================================
来源：http://own.52xcode.cn

[B01] 条件判断 if / else
来源：http://kim.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://qln.ydzc1.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ldc.gaohongyu789.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nhe.52xcode.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hgh.haohaochexian.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yuj.chenjidiqi.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jcl.zdqjudy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vdj.mhx1999.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dnq.c1oappe.top

[B02] 多分支 else if / elif
来源：http://keu.ydzc1.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rja.ppjwa.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ysg.zdbjq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yvi.vehdjk.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uwd.ivvv.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wpn.shangyingyoupin.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wps.hfpthk.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vdd.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jjp.hcnkem.com

[B03] switch / match / case
来源：http://ria.ydzc1.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mlc.cqqwz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://smw.zhiwuduotai.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vns.zhiwuduotai.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ucq.zdbjq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tre.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vhp.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://phe.hfpthk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lkf.fengsongda.top

[B04] for 计数循环
来源：http://ojw.0kj1m.cn

Py:   for i in range(10): print(i)
来源：http://xym.ctjpmb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://adm.zhijiandao.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://huk.daria6918.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ybcxt.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kfl.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qwu.hesvh.cn

Ruby: 10.times { |i| puts i }
来源：http://ine.yueranfly.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uns.aizwys.cn

[B05] 遍历数组 / 列表
来源：http://dca.meibo888.top

Py:   for item in arr: print(item)
来源：http://arf.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yoz.nwbrower.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zip.shangyingyoupin.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tvn.zhongyouzk.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yam.pycfn.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pde.yueranfly.top

Ruby: arr.each { |item| puts item }
来源：http://hjm.havefunace.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uiv.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://xjy.xuetiantiany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://psf.bjfxy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tdf.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wfz.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qrg.hesvh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oto.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cbx.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dep.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kcm.zhixingplan.top

[B07] while 循环
来源：http://tdt.hammf.cn

Py:   while i < 10: i += 1
来源：http://dkk.vehdjk.com

PHP:  while ($i < 10) { $i++; }
来源：http://yng.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://kmw.xuetiantiany.cn

TS:   while (i < 10) { i++; }
来源：http://xco.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://vim.chenzaomai.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://adm.nanxuanxn.top

Ruby: while i < 10; i += 1; end
来源：http://izy.yuanzhike.top

C#:   while (i < 10) { i++; }
来源：http://xur.zdqjudy.top

[B08] do-while（至少执行一次）
来源：http://gib.yongpay.top

Py:   # 无 do-while：用 while True + break
来源：http://xuz.xinyue.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://dfr.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://moc.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://xps.yangfankeji.com

Java: do { i++; } while (i < 10);
来源：http://shc.sysykeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mfu.hnxiangtu.top

Ruby: begin; i += 1; end while i < 10
来源：http://pep.xuanzx.com

C#:   do { i++; } while (i < 10);
来源：http://xcx.jlsjyb.cn

[B09] break 与 continue
来源：http://tuh.guannengcc.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dze.tian-w.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://den.iojbl.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vgk.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ylz.jiagoushi.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://voz.yuxming.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rkd.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rbo.bjfxy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mts.guannengcc.top

[B10] 遍历同时拿索引
来源：http://juj.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ayr.daxiang520.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://een.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://buh.shanyushiyangtech.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cut.hcnkem.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zac.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bvs.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dtz.ydzc1.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lyb.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://oap.gaohongyu789.top

Py:   list(range(0, 10, 2))
来源：http://tmx.tian-w.cn

PHP:  range(0, 10, 2);
来源：http://sgi.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xpq.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bjq.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uyb.zhiwuduotai.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kph.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://hlc.xuetiantiany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ybl.sweek.top

[B12] 跳出多层循环
来源：http://dac.gzhubu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gwv.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://aga.ivvv.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://glx.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lpv.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lpz.daria6918.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://viq.hnxiangtu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lyj.shangyingyoupin.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kyj.wangshuangyany.cn

[B13] 判断是否为数字
来源：http://qcz.gzhubu.top

Py:   isinstance(x, (int, float))
来源：http://dqm.zhijiandao.cn

PHP:  is_numeric($x)
来源：http://uyi.fengsongda.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pof.zycfv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hnr.yangfankeji.com

Java: x instanceof Number
来源：http://qvs.hesvh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sof.sysykeji.top

Ruby: x.is_a?(Numeric)
来源：http://uss.meibo888.top

C#:   x is int or double or decimal
来源：http://hlq.yueranfly.top

[B14] 判断值是否在集合内
来源：http://epv.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rui.yvedp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://asj.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://bkj.quarkkingdee.top

TS:   [1, 2, 3].includes(x)
来源：http://fln.ybcxt.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vzq.jianghu66.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cdt.yuxming.cn

Ruby: [1, 2, 3].include?(x)
来源：http://leg.cqqwz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pfr.ydjk.org.cn

[B15] 布尔运算与取反
来源：http://zei.jqgufenzy.top

Py:   a and b or not c
来源：http://eod.ybcxt.top

PHP:  $a && $b || !$c
来源：http://wgq.yj202588.top

JS:   a && b || !c
来源：http://gfz.yueranfly.top

TS:   a && b || !c
来源：http://nbq.daxiang520.top

Java: a && b || !c
来源：http://pqh.ehwqpu.com

Go:   a && b || !c
来源：http://hln.feifeiyinyue.top

Ruby: a && b || !c
来源：http://dur.chenlongwang.top

C#:   a && b || !c
来源：http://ecy.andypj.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://voc.mhx1999.top

Py:   if not data: return
来源：http://ssl.hesvh.cn

PHP:  if (!$data) { return; }
来源：http://pzg.316326.xyz

JS:   if (!data) return;
来源：http://fae.zhiwuduotai.top

TS:   if (!data) return;
来源：http://atr.zhijiandao.cn

Java: if (data == null) return;
来源：http://ngv.zhengqikj.top

Go:   if data == nil { return }
来源：http://uuh.ywan-chungtsiang.top

Ruby: return if data.nil?
来源：http://ifu.c1oappe.top

C#:   if (data == null) return;
来源：http://upy.nanxinkj.top


<!-- 参考信息 -->