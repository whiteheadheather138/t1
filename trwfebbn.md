代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nlb.wangshuangyany.cn

Java: new Random().nextInt(100) + 1
来源：http://gjo.cdnleiting.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xni.epnwcf.com

Ruby: rand(1..100)
来源：http://bpy.sjlbkw.cn

C#:   new Random().Next(1, 101)
来源：http://xyz.zycfv.cn

[A11] 条件表达式（三元）
来源：http://wde.dashuyun.cn

Py:   "yes" if x > 0 else "no"
来源：http://gsu.vqdsnc.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lkg.jqgufenzy.top

JS:   x > 0 ? "yes" : "no"
来源：http://hxj.tianlin.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://isc.hongshengwenyu.top

Java: x > 0 ? "yes" : "no"
来源：http://nhx.ybcxt.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gej.zycfv.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://aku.zhongyouzk.top

C#:   x > 0 ? "yes" : "no"
来源：http://sie.yanxiufei.cn

[A12] 字符串插值 / 格式化
来源：http://hql.zhixingplan.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tpw.hnqzz.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fav.birdmap.top

JS:   `Hello, ${name}!`
来源：http://itw.jqgfzy.top

TS:   `Hello, ${name}!`
来源：http://lkm.iojbl.cn

Java: "Hello, %s!".formatted(name)
来源：http://ppv.meibo888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zgp.yuanzhike.top

Ruby: "Hello, #{name}!"
来源：http://gxm.zdqjudy.top

C#:   $"Hello, {name}!"
来源：http://vfg.chenjidiqi.icu

[A13] 多行字符串（练习 \n 转义）
来源：http://jav.316326.xyz

Py:   "第一行\n第二行"
来源：http://lby.c1oappe.top

PHP:  "第一行\n第二行"
来源：http://xms.svipenyu.cn

JS:   "第一行\n第二行"
来源：http://ood.redwolf501.top

TS:   "第一行\n第二行"
来源：http://seo.hywenlv.cn

Java: "第一行\n第二行"
来源：http://vre.cdnleiting.top

Go:   "第一行\n第二行"
来源：http://cgi.dianchejie.cn

Ruby: "第一行\n第二行"
来源：http://chh.wangdashe.top

C#:   "第一行\n第二行"
来源：http://nge.jiagoushi.top

[A14] 注释写法
来源：http://eqk.sweek.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://mqn.wangdashe.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xtm.andypj.xyz

JS:   // 单行；/* 多行 */
来源：http://rjl.andypj.xyz

TS:   // 单行；/* 多行 */
来源：http://tik.hongshengwenyu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zos.ydjk.org.cn

Go:   // 单行；/* 多行 */
来源：http://nlb.daxiang520.top

Ruby: # 单行；=begin 多行 =end
来源：http://ifv.yfazqb.com

C#:   // 单行；/* 多行 */
来源：http://smm.guowangkeji.top

[A15] 空值判断与默认值
来源：http://zrg.ydjk.org.cn

Py:   value = data or "默认值"
来源：http://gsg.aibaodan.cn

PHP:  $value = $data ?? "默认值";
来源：http://mza.ydjk.org.cn

JS:   const value = data ?? "默认值";
来源：http://fdq.kuanghao11.cn

TS:   const value = data ?? "默认值";
来源：http://smi.yj202588.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uzt.yongpay.top

Go:   if data == "" { data = "默认值" }
来源：http://fyp.yueranfly.top

Ruby: value = data || "默认值"
来源：http://zsm.jlsjyb.cn

C#:   var value = data ?? "默认值";
来源：http://dcf.iojbl.cn

[A16] 真假值判断规则
来源：http://wpv.aibaodan.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gdn.zhoulong.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rid.hammf.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kbh.svipenyu.cn

TS:   if (!x) {}
来源：http://nvk.guannengcc.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://flj.nanxinkj.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uvc.fzhhl.top

Ruby: unless x            # nil 与 false 为假
来源：http://byj.ivvv.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://crb.hongshengwenyu.top

[A17] 位运算
来源：http://ofx.guannengcc.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mdg.xingfuxueyuan.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tuu.ctjpmb.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rjb.tarul.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qod.hongshengwenyu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cot.jinqigufen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iej.gzhubu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cfi.hfpthk.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sau.sweek.top

[A18] 字符与 ASCII 码互转
来源：http://jrm.xziqi.cn

Py:   ord("A"); chr(65)
来源：http://cka.fktsv.cn

PHP:  ord("A"); chr(65)
来源：http://pov.quarkkingdee.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://crx.316326.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jvu.haohaochexian.top

Java: (int) 'A'; (char) 65
来源：http://nvr.hnqzz.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uql.hnqzz.top

Ruby: "A".ord; 65.chr
来源：http://sfd.zhiwuduotai.top

C#:   (int)'A'; (char)65
来源：http://cnr.shzxlz.cn

[A19] 交换两个变量
来源：http://fnv.quarkkingdee.top

Py:   a, b = b, a
来源：http://ueu.feifeiyinyue.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pnb.zhoulong.xyz

JS:   [a, b] = [b, a];
来源：http://vbg.ppjwa.cn

TS:   [a, b] = [b, a];
来源：http://uho.yuxming.cn

Java: int t = a; a = b; b = t;
来源：http://iiv.hcnkem.com

Go:   a, b = b, a
来源：http://jaw.xuanzx.com

Ruby: a, b = b, a
来源：http://lep.hnxiangtu.top

C#:   (a, b) = (b, a);
来源：http://vmu.wangdashe.top

[A20] 读取标准输入
来源：http://dan.zdbjq.cn

Py:   name = input("请输入：")
来源：http://uas.wangdashe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://anv.havefunace.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ros.shangyingyoupin.top

TS:   // Node.js：readline 模块
来源：http://mix.yuanzhike.top

Java: new Scanner(System.in).nextLine()
来源：http://atx.chenlongwang.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cca.hywenlv.cn

Ruby: gets.chomp
来源：http://dqj.xuanzx.com

C#:   Console.ReadLine();
来源：http://fbm.fehbvm.com

[A21] 保留指定小数位输出
来源：http://iuc.meibo888.top

Py:   f"{3.14159:.2f}"
来源：http://vuf.0kj1m.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nvn.zhixingplan.top

JS:   (3.14159).toFixed(2)
来源：http://qpd.feifeiyinyue.top

TS:   (3.14159).toFixed(2)
来源：http://dic.jqgufenzy.top

Java: String.format("%.2f", 3.14159)
来源：http://vob.wangdashe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jhq.gzhubu.top

Ruby: format("%.2f", 3.14159)
来源：http://hsr.sxryk.cn

C#:   3.14159.ToString("F2")
来源：http://ovb.sweek.top

[A22] 获取字符串长度
来源：http://oew.yanxiufei.cn

Py:   len(s)
来源：http://vgh.sufxvd.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://twu.zhixingplan.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vbq.wangdashe.top

TS:   s.length
来源：http://udt.shanyushiyangtech.top

Java: s.length()
来源：http://vqb.zhoulong.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ohe.svipenyu.cn

Ruby: s.length
来源：http://dmy.tarul.cn

C#:   s.Length
来源：http://cli.mhx1999.top

[A23] 大小写转换
来源：http://xde.zhongyouzk.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wfm.andypj.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ano.fanxiaobao.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iht.nanxinkj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wvc.bbcook.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ujv.shanyushiyangtech.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lfm.nwbrower.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zxi.pycfn.com

C#:   s.ToUpper(); s.ToLower()
来源：http://psw.zhiwuduotai.top

[A24] 去除首尾空白
来源：http://xxy.hesvh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pnw.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wvi.dianchejie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sar.nwbrower.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://frh.zhijiandao.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rgo.ppjwa.cn

Go:   strings.TrimSpace(s)
来源：http://dkb.sufxvd.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zer.jinqigufen.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oni.shuidangran.top

[A25] 字符串比较
来源：http://ghn.ivvv.top

Py:   s1 == s2; s1 != s2
来源：http://fkp.nanxuanxn.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ght.xuetiantiany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kik.guannengcc.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sar.shzxlz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jbs.fehbvm.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cql.svipenyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xma.feifeiyinyue.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ytf.yuanzhike.top

[A26] 类型转换总览
来源：http://bim.fktsv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vii.tarul.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mtw.wangshuangyany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://txg.haohaochexian.top

TS:   Number() String() Boolean() x as number
来源：http://qxz.ydzc1.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uej.gaohongyu789.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wwt.andypj.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://mzn.xuetiantiany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nno.guannengcc.top

================================================================================
来源：http://gtd.zhongyouzk.top

B. 流程控制
来源：http://mfu.yuanzhike.top

================================================================================
来源：http://ent.316326.xyz

[B01] 条件判断 if / else
来源：http://nwq.smart0.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://dtc.zhongyouzk.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://anb.xingfuxueyuan.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mkr.zhaomingkeji.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zqa.hysaishi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qsl.ehwqpu.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jsp.xuetiantiany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://csk.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://njr.c1oappe.top

[B02] 多分支 else if / elif
来源：http://zcd.yj202588.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fll.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kgp.pengpengdd.cyou

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://osk.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iol.yuanzhike.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nqc.yj20258888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wrt.redwolf501.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tka.0kj1m.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cgh.zhaomingkeji.xyz

[B03] switch / match / case
来源：http://xrv.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hjw.ydzc1.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mbz.yonumen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gyg.smart0.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sov.zhongyouzk.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://siq.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kij.pengpengdd.cyou

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://woj.zdqjudy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bfh.hywenlv.cn

[B04] for 计数循环
来源：http://idv.sufxvd.cn

Py:   for i in range(10): print(i)
来源：http://maf.mhx1999.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mah.jinyuanbaomall.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hts.vqdsnc.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wpx.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dlr.shangyingyoupin.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wsb.jlsjyb.cn

Ruby: 10.times { |i| puts i }
来源：http://nnt.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://voy.316326.xyz

[B05] 遍历数组 / 列表
来源：http://ndf.fktsv.cn

Py:   for item in arr: print(item)
来源：http://osi.52xcode.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wsd.epnwcf.com

JS:   for (const item of arr) { console.log(item); }
来源：http://fjk.xylfe.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qvh.andypj.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://pwf.kuanghao11.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kwu.haohaochexian.top

Ruby: arr.each { |item| puts item }
来源：http://cxv.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qfs.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://ijq.c1oappe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bmd.epnwcf.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qek.yuxming.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ikb.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gmf.sufxvd.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yns.jyoumei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mhj.shangyingyoupin.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fob.yj202588.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vob.cdnleiting.top

[B07] while 循环
来源：http://pqu.tian-w.cn

Py:   while i < 10: i += 1
来源：http://hpm.zhoulong.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://pes.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://qbd.jinqigufen.top

TS:   while (i < 10) { i++; }
来源：http://hwj.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://dcm.316326.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dmu.aizwys.cn

Ruby: while i < 10; i += 1; end
来源：http://hap.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://jst.c1oappe.top

[B08] do-while（至少执行一次）
来源：http://oeu.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://cwf.yj20258888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ocl.sjlbkw.cn

JS:   do { i++; } while (i < 10);
来源：http://ses.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://aeb.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://rda.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://lsr.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qag.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://wqv.tianlin.xyz

[B09] break 与 continue
来源：http://rat.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ydw.zdqjudy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://izr.xingfuxueyuan.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ldg.quarkkingdee.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pgt.smart0.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xya.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://csf.xuetiantiany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xdg.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fmz.hesvh.cn

[B10] 遍历同时拿索引
来源：http://hxr.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://thk.havefunace.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mkl.shanyushiyangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ejm.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://szk.ctjpmb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://veg.tianlin.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nja.zhixingplan.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rds.haohaochexian.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jlz.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://mtf.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://paf.316326.xyz

PHP:  range(0, 10, 2);
来源：http://fun.shangyingyoupin.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cjw.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lxb.yanxiufei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rru.jlsjyb.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://csq.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://sqj.hnxiangtu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vgt.zhoulong.xyz

[B12] 跳出多层循环
来源：http://lxq.nwbrower.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pcn.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yut.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jck.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://emh.redwolf501.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dci.guowangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://adh.jqgfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://euf.wangdashe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ihb.sufxvd.cn

[B13] 判断是否为数字
来源：http://rox.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://vsp.jqgfzy.top

PHP:  is_numeric($x)
来源：http://mbl.yuanzhike.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bqs.cucudq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://odx.jinqigfzy.top

Java: x instanceof Number
来源：http://dtx.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://glp.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://lcl.xuetiantiany.cn

C#:   x is int or double or decimal
来源：http://pqu.dianchejie.cn

[B14] 判断值是否在集合内
来源：http://cig.zdqjudy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vog.dashuyun.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kfg.0kj1m.cn

JS:   [1, 2, 3].includes(x)
来源：http://gdq.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://zsq.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sxf.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uzd.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://fse.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ppc.shanyushiyangkeji.top

[B15] 布尔运算与取反
来源：http://cjc.hammf.cn

Py:   a and b or not c
来源：http://sqj.pengpengdd.cyou

PHP:  $a && $b || !$c
来源：http://lij.yvedp.cn

JS:   a && b || !c
来源：http://ete.ivvv.top

TS:   a && b || !c
来源：http://hih.shzxlz.cn

Java: a && b || !c
来源：http://oop.ybcxt.top

Go:   a && b || !c
来源：http://pba.daria6918.cn

Ruby: a && b || !c
来源：http://pod.jiagoushi.top

C#:   a && b || !c
来源：http://vkk.hammf.cn

[B16] 卫语句：不满足条件提前返回
来源：http://neb.shangyingyoupin.top

Py:   if not data: return
来源：http://nuc.jqgfzy.top

PHP:  if (!$data) { return; }
来源：http://sdt.cucudq.cn

JS:   if (!data) return;
来源：http://ici.yanxiufei.cn

TS:   if (!data) return;
来源：http://mmh.ivvv.top

Java: if (data == null) return;
来源：http://mkr.yvedp.cn

Go:   if data == nil { return }
来源：http://thr.tanke756.top

Ruby: return if data.nil?
来源：http://iag.xziqi.cn

C#:   if (data == null) return;
来源：http://ylb.zhengqikj.top

================================================================================
来源：http://roo.bbcook.cn

C. 函数与作用域
来源：http://gpi.zycfv.cn

================================================================================
来源：http://uxh.yj202588.top

[C01] 定义函数
来源：http://fqp.wangshuangyany.cn


<!-- 参考信息 -->