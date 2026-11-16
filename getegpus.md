代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zip.sweek.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pme.cdnleiting.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ssu.tarul.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gcs.xuetiantiany.cn

[A10] 生成随机数
来源：http://ohv.uphjek.com

Py:   import random; random.randint(1, 100)
来源：http://rcb.haohaochexian.top

PHP:  random_int(1, 100);
来源：http://fly.ybcxt.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cqf.daria6918.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qcr.nwbrower.top

Java: new Random().nextInt(100) + 1
来源：http://ssf.zhijiandao.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gcm.iojbl.cn

Ruby: rand(1..100)
来源：http://ilc.yangfankeji.com

C#:   new Random().Next(1, 101)
来源：http://pkl.ppjwa.cn

[A11] 条件表达式（三元）
来源：http://ymw.vehdjk.com

Py:   "yes" if x > 0 else "no"
来源：http://ois.cqqwz.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://eks.nanxinkj.top

JS:   x > 0 ? "yes" : "no"
来源：http://qru.fehbvm.com

TS:   x > 0 ? "yes" : "no"
来源：http://wlc.yuxming.cn

Java: x > 0 ? "yes" : "no"
来源：http://cvi.haohaochexian.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ufy.feifeiyinyue.top

Ruby: x > 0 ? "yes" : "no"
来源：http://jje.xuetiantiany.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lmd.fzhhl.top

[A12] 字符串插值 / 格式化
来源：http://tav.cqqwz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pgq.ybcxt.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fmt.zhengqikj.top

JS:   `Hello, ${name}!`
来源：http://lgn.pycfn.com

TS:   `Hello, ${name}!`
来源：http://uqz.fehbvm.com

Java: "Hello, %s!".formatted(name)
来源：http://ulv.tanke756.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fkl.shangyingyoupin.top

Ruby: "Hello, #{name}!"
来源：http://sws.ywan-chungtsiang.top

C#:   $"Hello, {name}!"
来源：http://dcm.ppjwa.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jce.gotoacloud.top

Py:   "第一行\n第二行"
来源：http://dkb.gaohongyu789.top

PHP:  "第一行\n第二行"
来源：http://yfp.hcnkem.com

JS:   "第一行\n第二行"
来源：http://fmq.jyoumei.cn

TS:   "第一行\n第二行"
来源：http://eab.dianchejie.cn

Java: "第一行\n第二行"
来源：http://wxx.sjlbkw.cn

Go:   "第一行\n第二行"
来源：http://vrd.bjfxy.top

Ruby: "第一行\n第二行"
来源：http://ecz.fehbvm.com

C#:   "第一行\n第二行"
来源：http://hmz.fktsv.cn

[A14] 注释写法
来源：http://kwf.hfpthk.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vyn.vqdsnc.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nyk.hywenlv.cn

JS:   // 单行；/* 多行 */
来源：http://bip.hywenlv.cn

TS:   // 单行；/* 多行 */
来源：http://jad.zhongyouzk.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mcq.feifeiyinyue.top

Go:   // 单行；/* 多行 */
来源：http://vuw.zhongyouzk.top

Ruby: # 单行；=begin 多行 =end
来源：http://aeu.wangdashe.top

C#:   // 单行；/* 多行 */
来源：http://afv.52xcode.cn

[A15] 空值判断与默认值
来源：http://rmk.guannengcc.top

Py:   value = data or "默认值"
来源：http://srr.9152youxi.cn

PHP:  $value = $data ?? "默认值";
来源：http://ioh.fzhhl.top

JS:   const value = data ?? "默认值";
来源：http://iks.zhengqikj.top

TS:   const value = data ?? "默认值";
来源：http://hwd.ybcxt.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lqz.aizwys.cn

Go:   if data == "" { data = "默认值" }
来源：http://cuf.zhoulong.xyz

Ruby: value = data || "默认值"
来源：http://xpd.yj20258.top

C#:   var value = data ?? "默认值";
来源：http://urd.bjfxy.top

[A16] 真假值判断规则
来源：http://wbe.zhongyouzk.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eqx.daxiang520.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xgq.zhongyouzk.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://emx.zycfv.cn

TS:   if (!x) {}
来源：http://kxx.yuxming.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ssu.nwbrower.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://aqh.gogol.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lhm.guowangkeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vcp.hysaishi.cn

[A17] 位运算
来源：http://rxw.mhx1999.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nsn.tarul.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ylf.yuanzhike.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lyx.jqgufenzy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yqo.jinqigufen.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ygz.birdmap.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nvn.zhixingplan.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ere.ehwqpu.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ykx.jinyuanbaomall.cn

[A18] 字符与 ASCII 码互转
来源：http://wws.316326.xyz

Py:   ord("A"); chr(65)
来源：http://knc.uphjek.com

PHP:  ord("A"); chr(65)
来源：http://jpp.feifeiyinyue.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vim.snrcjt.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vwf.jinqigufen.top

Java: (int) 'A'; (char) 65
来源：http://abq.fzhhl.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hij.0kj1m.cn

Ruby: "A".ord; 65.chr
来源：http://bcb.fzhhl.top

C#:   (int)'A'; (char)65
来源：http://ock.tianlin.xyz

[A19] 交换两个变量
来源：http://rpg.jqgufenzy.top

Py:   a, b = b, a
来源：http://qkn.xuanzx.com

PHP:  [$a, $b] = [$b, $a];
来源：http://ule.tarul.cn

JS:   [a, b] = [b, a];
来源：http://cfx.hywenlv.cn

TS:   [a, b] = [b, a];
来源：http://aaw.bbcook.cn

Java: int t = a; a = b; b = t;
来源：http://irs.bjfxy.top

Go:   a, b = b, a
来源：http://tot.gotoacloud.top

Ruby: a, b = b, a
来源：http://naf.sysykeji.top

C#:   (a, b) = (b, a);
来源：http://hqx.epnwcf.com

[A20] 读取标准输入
来源：http://bvh.yvedp.cn

Py:   name = input("请输入：")
来源：http://gtw.kuanghao11.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://awg.yuanzhike.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vug.shanyushiyangkeji.top

TS:   // Node.js：readline 模块
来源：http://nev.bjfxy.top

Java: new Scanner(System.in).nextLine()
来源：http://fhu.ivvv.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jok.ybcxt.top

Ruby: gets.chomp
来源：http://ppe.ybcxt.top

C#:   Console.ReadLine();
来源：http://gon.yangfankeji.com

[A21] 保留指定小数位输出
来源：http://jsl.epnwcf.com

Py:   f"{3.14159:.2f}"
来源：http://ivp.uphjek.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hvl.havefunace.top

JS:   (3.14159).toFixed(2)
来源：http://tfb.birdmap.top

TS:   (3.14159).toFixed(2)
来源：http://atl.tianlin.xyz

Java: String.format("%.2f", 3.14159)
来源：http://ojm.redwolf501.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fbz.mhx1999.top

Ruby: format("%.2f", 3.14159)
来源：http://fyu.kuanghao11.cn

C#:   3.14159.ToString("F2")
来源：http://zum.aibaodan.cn

[A22] 获取字符串长度
来源：http://drm.smart0.xyz

Py:   len(s)
来源：http://hxi.yonumen.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gig.xziqi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ixq.daria6918.cn

TS:   s.length
来源：http://gqc.jinghuilouyu.cn

Java: s.length()
来源：http://wkq.fehbvm.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wpw.hnxiangtu.top

Ruby: s.length
来源：http://dtl.zhongyouzk.top

C#:   s.Length
来源：http://sow.jiagoushi.top

[A23] 大小写转换
来源：http://sre.xziqi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://trr.ctjpmb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bkw.tianlin.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fux.daria6918.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yye.hcnkem.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://swz.ydzc1.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mwp.ybcxt.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ayo.pycfn.com

C#:   s.ToUpper(); s.ToLower()
来源：http://eel.fktsv.cn

[A24] 去除首尾空白
来源：http://elm.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ird.kuanghao11.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qef.smart0.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yzg.zycfv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cfk.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mcv.xuanzx.com

Go:   strings.TrimSpace(s)
来源：http://ume.316326.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://spt.ydzc1.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lts.svipenyu.cn

[A25] 字符串比较
来源：http://xos.xuetiantiany.cn

Py:   s1 == s2; s1 != s2
来源：http://blj.chenzaomai.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rbb.zhixingplan.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tln.gogol.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nst.cheryme.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kat.iojbl.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://voy.yvedp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pkn.fengsongda.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mtf.zhoulong.xyz

[A26] 类型转换总览
来源：http://zhq.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yfm.xziqi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jhk.xinyue.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rri.zhiwuduotai.top

TS:   Number() String() Boolean() x as number
来源：http://olw.zhixingplan.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://flu.aibaodan.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vlu.hesvh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oia.zhiwuduotai.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://miy.wangshuangyany.cn

================================================================================
来源：http://hhl.zhixingplan.top

B. 流程控制
来源：http://zww.yfazqb.com

================================================================================
来源：http://pif.nwbrower.top

[B01] 条件判断 if / else
来源：http://mjx.52xcode.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dzu.chenzaomai.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xke.zhaomingkeji.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zoa.jiagoushi.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ceo.jinqigufen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://bdr.aizwys.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ijm.andypj.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tkq.svipenyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dqj.redwolf501.top

[B02] 多分支 else if / elif
来源：http://ozw.ybcxt.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tga.andypj.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mxv.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dcf.fzhhl.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fke.smart0.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ayx.zhoulong.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jvn.aizwys.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cqh.wangshuangyany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://etx.fzhhl.top

[B03] switch / match / case
来源：http://ivw.epnwcf.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dlq.gogol.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://stb.tarul.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eoa.hesvh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rxe.hnqzz.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tdi.yvedp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ihx.redwolf501.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sim.sjlbkw.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ycn.vqdsnc.cn

[B04] for 计数循环
来源：http://ava.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://ied.fanxiaobao.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tmd.snrcjt.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://abg.shzxlz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bnk.sxryk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kix.cqqwz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ymr.ydjk.org.cn

Ruby: 10.times { |i| puts i }
来源：http://crj.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xvv.meibo888.top

[B05] 遍历数组 / 列表
来源：http://yha.sysykeji.top

Py:   for item in arr: print(item)
来源：http://jxx.xingfuxueyuan.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uyy.yj20258.top

JS:   for (const item of arr) { console.log(item); }
来源：http://sgl.c1oappe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xhr.hesvh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://aua.mhx1999.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nxz.cqqwz.cn

Ruby: arr.each { |item| puts item }
来源：http://dlh.cashguo.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cyb.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://mer.yongpay.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ggr.yangfankeji.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://heu.jqgfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dxu.vqdsnc.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rvf.hesvh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rod.jlsjyb.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xts.tian-w.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sid.zycfv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rvj.gaohongyu789.top

[B07] while 循环
来源：http://zgh.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://gdv.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ohz.kuanghao11.cn

JS:   while (i < 10) { i++; }
来源：http://xqg.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://eqm.316326.xyz

Java: while (i < 10) { i++; }
来源：http://ybd.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vfy.xuetiantiany.cn

Ruby: while i < 10; i += 1; end
来源：http://svk.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://bdt.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://wwu.hcnkem.com

Py:   # 无 do-while：用 while True + break
来源：http://awf.gzhubu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fka.ivvv.top

JS:   do { i++; } while (i < 10);
来源：http://xha.zhaomingkeji.xyz

TS:   do { i++; } while (i < 10);
来源：http://dyn.sufxvd.cn

Java: do { i++; } while (i < 10);
来源：http://bcw.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pef.yj20258.top

Ruby: begin; i += 1; end while i < 10
来源：http://wdi.mhx1999.top

C#:   do { i++; } while (i < 10);
来源：http://nvv.shangyingyoupin.top

[B09] break 与 continue
来源：http://vfz.haohaochexian.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fdb.zhoulong.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lxj.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rdx.shuidangran.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vag.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nms.ppjwa.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fiy.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ehv.dashuyun.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vvq.zhengqikj.top

[B10] 遍历同时拿索引
来源：http://gmp.yj20258888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wcl.yuanzhike.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yqp.sxryk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ekk.ybcxt.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ylf.shzxlz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nve.52xcode.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gdb.hongshengwenyu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xvp.guowangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://brh.haohaochexian.top

[B11] 生成数字序列 / 区间
来源：http://ecv.chenlongwang.top

Py:   list(range(0, 10, 2))
来源：http://wwl.zhixingplan.top

PHP:  range(0, 10, 2);
来源：http://fxd.fktsv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vbo.bbcook.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oda.yj20258.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cqx.cucudq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xdc.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://kqk.mhx1999.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ial.yanxiufei.cn

[B12] 跳出多层循环
来源：http://xod.yueranfly.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xoh.vqdsnc.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ixu.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yts.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zut.yueranfly.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://loe.pengpengdd.cyou

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dze.zhaomingkeji.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://whu.yfazqb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hvg.ydjk.org.cn

[B13] 判断是否为数字
来源：http://mlo.wangshuangyany.cn

Py:   isinstance(x, (int, float))
来源：http://pgy.havefunace.top

PHP:  is_numeric($x)
来源：http://zob.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://glj.dashuyun.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sxh.yangfankeji.com

Java: x instanceof Number
来源：http://jhc.ivvv.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wyl.jqgufenzy.top

Ruby: x.is_a?(Numeric)
来源：http://asj.zhijiandao.cn

C#:   x is int or double or decimal
来源：http://trg.yueranfly.top

[B14] 判断值是否在集合内
来源：http://ccj.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://muu.daxiang520.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hbk.vqdsnc.cn

JS:   [1, 2, 3].includes(x)
来源：http://thg.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://wkj.svipenyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://toi.zhongyouzk.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dux.gaohongyu789.top

Ruby: [1, 2, 3].include?(x)
来源：http://kiw.nanxinkj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ypu.hfpthk.cn

[B15] 布尔运算与取反
来源：http://usc.jinghuilouyu.cn

Py:   a and b or not c
来源：http://svh.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://gfg.xuetiantiany.cn

JS:   a && b || !c
来源：http://zax.zhixingplan.top

TS:   a && b || !c
来源：http://xmt.9152youxi.cn

Java: a && b || !c
来源：http://zft.svipenyu.cn

Go:   a && b || !c
来源：http://rmj.gotoacloud.top

Ruby: a && b || !c
来源：http://gfx.quarkkingdee.top

C#:   a && b || !c
来源：http://nni.ydjk.org.cn

[B16] 卫语句：不满足条件提前返回
来源：http://evr.pycfn.com

Py:   if not data: return
来源：http://evc.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://mkz.ybcxt.top

JS:   if (!data) return;
来源：http://rmj.fzhhl.top

TS:   if (!data) return;
来源：http://aci.birdmap.top


<!-- 参考信息 -->