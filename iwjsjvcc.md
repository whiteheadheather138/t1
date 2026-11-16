代发 wailian999

[A10] 生成随机数
来源：http://iua.shuidangran.top

Py:   import random; random.randint(1, 100)
来源：http://zlm.hammf.cn

PHP:  random_int(1, 100);
来源：http://ths.aibaodan.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qwe.smart0.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eud.yfazqb.com

Java: new Random().nextInt(100) + 1
来源：http://mth.nanxuanxn.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rkp.jinyuanbaomall.cn

Ruby: rand(1..100)
来源：http://hdk.quarkkingdee.top

C#:   new Random().Next(1, 101)
来源：http://gdp.yanxiufei.cn

[A11] 条件表达式（三元）
来源：http://aqg.yueranfly.top

Py:   "yes" if x > 0 else "no"
来源：http://tda.mhx1999.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yrn.dianchejie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yev.shanyushiyangkeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://jzp.xingfuxueyuan.xyz

Java: x > 0 ? "yes" : "no"
来源：http://qil.jinqigufen.top

Go:   // 无三元运算符，需用 if 语句
来源：http://odm.yueranfly.top

Ruby: x > 0 ? "yes" : "no"
来源：http://nmi.guowangkeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://sde.smart0.xyz

[A12] 字符串插值 / 格式化
来源：http://exu.pengpengdd.cyou

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sal.wangshuangyany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://crb.xuetiantiany.cn

JS:   `Hello, ${name}!`
来源：http://wnr.sysykeji.top

TS:   `Hello, ${name}!`
来源：http://fmu.chenzaomai.com

Java: "Hello, %s!".formatted(name)
来源：http://cmn.ivvv.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nlu.fengsongda.top

Ruby: "Hello, #{name}!"
来源：http://vrw.daxiang520.top

C#:   $"Hello, {name}!"
来源：http://zxv.chenjidiqi.icu

[A13] 多行字符串（练习 \n 转义）
来源：http://jqm.andypj.xyz

Py:   "第一行\n第二行"
来源：http://vgd.cucudq.cn

PHP:  "第一行\n第二行"
来源：http://xfd.hesvh.cn

JS:   "第一行\n第二行"
来源：http://puo.havefunace.top

TS:   "第一行\n第二行"
来源：http://qcd.zdbjq.cn

Java: "第一行\n第二行"
来源：http://xge.zdbjq.cn

Go:   "第一行\n第二行"
来源：http://fzz.dianchejie.cn

Ruby: "第一行\n第二行"
来源：http://zcg.haohaochexian.top

C#:   "第一行\n第二行"
来源：http://bkm.kuanghao11.cn

[A14] 注释写法
来源：http://ddr.hywenlv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kfm.tanke756.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://hki.smart0.xyz

JS:   // 单行；/* 多行 */
来源：http://vns.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://ezp.yfazqb.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zch.pengpengdd.cyou

Go:   // 单行；/* 多行 */
来源：http://oyt.yuanzhike.top

Ruby: # 单行；=begin 多行 =end
来源：http://ewp.52xcode.cn

C#:   // 单行；/* 多行 */
来源：http://gax.hywenlv.cn

[A15] 空值判断与默认值
来源：http://mgh.jqgfzy.top

Py:   value = data or "默认值"
来源：http://zbt.fengsongda.top

PHP:  $value = $data ?? "默认值";
来源：http://lfr.nanxuanxn.top

JS:   const value = data ?? "默认值";
来源：http://xno.fktsv.cn

TS:   const value = data ?? "默认值";
来源：http://kau.pengpengdd.cyou

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pps.hongshengwenyu.top

Go:   if data == "" { data = "默认值" }
来源：http://noe.birdmap.top

Ruby: value = data || "默认值"
来源：http://usi.c1oappe.top

C#:   var value = data ?? "默认值";
来源：http://vjw.zhaomingkeji.xyz

[A16] 真假值判断规则
来源：http://nqi.shuidangran.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pnl.cheryme.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mef.sufxvd.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cfs.yueranfly.top

TS:   if (!x) {}
来源：http://geb.ctjpmb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://msi.gaohongyu789.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qkw.wangdashe.top

Ruby: unless x            # nil 与 false 为假
来源：http://gzd.hcnkem.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wpa.9152youxi.cn

[A17] 位运算
来源：http://dmb.hnqzz.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nao.hnxiangtu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xsg.ppjwa.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zfh.yonumen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qgs.yangfankeji.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://utq.bbcook.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pbi.fzhhl.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vcj.ydzc1.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://khf.ctjpmb.com

[A18] 字符与 ASCII 码互转
来源：http://vmk.hysaishi.cn

Py:   ord("A"); chr(65)
来源：http://mxy.shangyingyoupin.top

PHP:  ord("A"); chr(65)
来源：http://doq.jiagoushi.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cja.zhaomingkeji.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hcc.iojbl.cn

Java: (int) 'A'; (char) 65
来源：http://qse.dianchejie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nww.fengsongda.top

Ruby: "A".ord; 65.chr
来源：http://eup.xziqi.cn

C#:   (int)'A'; (char)65
来源：http://vvh.fehbvm.com

[A19] 交换两个变量
来源：http://zqz.sufxvd.cn

Py:   a, b = b, a
来源：http://bxq.0kj1m.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tli.yuanzhike.top

JS:   [a, b] = [b, a];
来源：http://ddk.aibaodan.cn

TS:   [a, b] = [b, a];
来源：http://hpc.redwolf501.top

Java: int t = a; a = b; b = t;
来源：http://zuz.hnxiangtu.top

Go:   a, b = b, a
来源：http://rkh.hcnkem.com

Ruby: a, b = b, a
来源：http://kju.cdnleiting.top

C#:   (a, b) = (b, a);
来源：http://lvi.yueranfly.top

[A20] 读取标准输入
来源：http://ost.shanyushiyangkeji.top

Py:   name = input("请输入：")
来源：http://yjn.52xcode.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gvy.wangdashe.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yuu.chenzaomai.com

TS:   // Node.js：readline 模块
来源：http://qoe.tianlin.xyz

Java: new Scanner(System.in).nextLine()
来源：http://leo.yfazqb.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sjv.daxiang520.top

Ruby: gets.chomp
来源：http://rsj.ppjwa.cn

C#:   Console.ReadLine();
来源：http://ywx.hnqzz.top

[A21] 保留指定小数位输出
来源：http://zcw.jinqigfzy.top

Py:   f"{3.14159:.2f}"
来源：http://mph.zhoulong.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rck.cqqwz.cn

JS:   (3.14159).toFixed(2)
来源：http://wzb.wangshuangyany.cn

TS:   (3.14159).toFixed(2)
来源：http://jgz.hnxiangtu.top

Java: String.format("%.2f", 3.14159)
来源：http://jui.xuetiantiany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wzv.yuxming.cn

Ruby: format("%.2f", 3.14159)
来源：http://ejp.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://ofe.52xcode.cn

[A22] 获取字符串长度
来源：http://gmj.aibaodan.cn

Py:   len(s)
来源：http://fuu.shuidangran.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uql.iojbl.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://owu.zhaomingkeji.xyz

TS:   s.length
来源：http://lvs.xuetiantiany.cn

Java: s.length()
来源：http://ndu.tianlin.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gpk.ctjpmb.com

Ruby: s.length
来源：http://okb.feifeiyinyue.top

C#:   s.Length
来源：http://iii.hesvh.cn

[A23] 大小写转换
来源：http://psa.vqdsnc.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kgg.dashuyun.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pgh.yuxming.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bvm.cashguo.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yoz.havefunace.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qaf.fktsv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sza.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mam.birdmap.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xyr.bbcook.cn

[A24] 去除首尾空白
来源：http://ubn.wangdashe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://odk.jinyuanbaomall.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iml.ydjk.org.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zeq.ivvv.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tyn.hammf.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://csq.andypj.xyz

Go:   strings.TrimSpace(s)
来源：http://apk.jqgfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bsc.chenzaomai.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qal.jinghuilouyu.cn

[A25] 字符串比较
来源：http://jkh.redwolf501.top

Py:   s1 == s2; s1 != s2
来源：http://uxb.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nsu.zhoulong.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ahz.zhaomingkeji.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://izf.yj202588.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gbh.yvedp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dsw.zdqjudy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tri.316326.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jiv.mhx1999.top

[A26] 类型转换总览
来源：http://yae.cdnleiting.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zpz.hcnkem.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hmg.epnwcf.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zkg.chenlongwang.top

TS:   Number() String() Boolean() x as number
来源：http://wfz.jinqigfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nam.fehbvm.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://snv.bjfxy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://pqp.dashuyun.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fwk.jinqigufen.top

================================================================================
来源：http://noe.cucudq.cn

B. 流程控制
来源：http://xku.hongshengwenyu.top

================================================================================
来源：http://gcu.birdmap.top

[B01] 条件判断 if / else
来源：http://gsc.hywenlv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://slh.yfazqb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wrg.snrcjt.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hhx.daria6918.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tcc.xingfuxueyuan.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://hyw.sysykeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iky.316326.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eqv.andypj.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fvb.guowangkeji.top

[B02] 多分支 else if / elif
来源：http://hyx.birdmap.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://beh.zdbjq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ipj.redwolf501.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hqk.shanyushiyangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uek.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://udm.ctjpmb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rup.snrcjt.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mqb.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hzf.hesvh.cn

[B03] switch / match / case
来源：http://rcy.cdnleiting.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pgs.jyoumei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lnx.yuxming.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dqk.bjfxy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ass.ybcxt.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://umo.zhaomingkeji.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mji.fktsv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xvc.yonumen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fci.snrcjt.cn

[B04] for 计数循环
来源：http://vxq.epnwcf.com

Py:   for i in range(10): print(i)
来源：http://qlx.gzhubu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dla.fktsv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ekk.vqdsnc.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nhb.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ngm.shuidangran.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nhg.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://wfo.ivvv.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zan.gogol.net.cn

[B05] 遍历数组 / 列表
来源：http://mmp.gzhubu.top

Py:   for item in arr: print(item)
来源：http://ycr.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cqd.zdqjudy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ixm.hfpthk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pcd.316326.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://twy.zhixingplan.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rfs.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://nkl.wangshuangyany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yjo.pengpengdd.cyou

[B06] 遍历字典 / 对象
来源：http://oiu.mhx1999.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sdi.ydjk.org.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xyb.yangfankeji.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kaq.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sdd.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xkz.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rab.jlsjyb.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bbw.0kj1m.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mcg.pengpengdd.cyou

[B07] while 循环
来源：http://pjw.sufxvd.cn

Py:   while i < 10: i += 1
来源：http://mpu.daxiang520.top

PHP:  while ($i < 10) { $i++; }
来源：http://lnd.wangdashe.top

JS:   while (i < 10) { i++; }
来源：http://meg.birdmap.top

TS:   while (i < 10) { i++; }
来源：http://hsa.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://imo.yangfankeji.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jsu.dashuyun.cn

Ruby: while i < 10; i += 1; end
来源：http://ntg.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://nox.sweek.top

[B08] do-while（至少执行一次）
来源：http://deo.fktsv.cn

Py:   # 无 do-while：用 while True + break
来源：http://eij.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jlm.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://pkz.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://tzy.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://rci.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jvn.chenlongwang.top

Ruby: begin; i += 1; end while i < 10
来源：http://jxj.fehbvm.com

C#:   do { i++; } while (i < 10);
来源：http://qjt.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://zvy.cqqwz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://raf.yfazqb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hkw.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jlk.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://guz.fehbvm.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fgp.nanxuanxn.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hen.tarul.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jgb.zycfv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eek.yj20258888.top

[B10] 遍历同时拿索引
来源：http://dae.jqgfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rry.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bkv.yangfankeji.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lsb.ydjk.org.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ozz.daria6918.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qvb.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fat.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iom.ydjk.org.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rgc.pengpengdd.cyou

[B11] 生成数字序列 / 区间
来源：http://rhx.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://iik.cqqwz.cn

PHP:  range(0, 10, 2);
来源：http://znb.jlsjyb.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fyy.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cap.gogol.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pqa.pengpengdd.cyou

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wov.yanxiufei.cn

Ruby: (0...10).step(2).to_a
来源：http://cnx.haohaochexian.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fmb.chenzaomai.com

[B12] 跳出多层循环
来源：http://zrt.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://usk.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://dmp.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://aam.andypj.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kgf.nanxinkj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://err.snrcjt.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ufa.chenzaomai.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zcw.hysaishi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ajl.cqqwz.cn

[B13] 判断是否为数字
来源：http://keb.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://omk.dianchejie.cn

PHP:  is_numeric($x)
来源：http://xdl.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jlh.yuxming.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qnk.fehbvm.com

Java: x instanceof Number
来源：http://nli.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uhz.tianlin.xyz

Ruby: x.is_a?(Numeric)
来源：http://svr.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://lgp.redwolf501.top

[B14] 判断值是否在集合内
来源：http://ifx.fehbvm.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yam.zdqjudy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ldp.vehdjk.com

JS:   [1, 2, 3].includes(x)
来源：http://ikb.dashuyun.cn

TS:   [1, 2, 3].includes(x)
来源：http://wsp.chenzaomai.com

Java: List.of(1, 2, 3).contains(x)
来源：http://edv.shanyushiyangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pgt.feifeiyinyue.top

Ruby: [1, 2, 3].include?(x)
来源：http://kyj.fehbvm.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zfy.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://pgt.hnqzz.top

Py:   a and b or not c
来源：http://tth.sjlbkw.cn

PHP:  $a && $b || !$c
来源：http://abv.jqgfzy.top

JS:   a && b || !c
来源：http://yfm.hnqzz.top

TS:   a && b || !c
来源：http://pcv.jyoumei.cn

Java: a && b || !c
来源：http://nnc.hywenlv.cn

Go:   a && b || !c
来源：http://uwz.cdnleiting.top

Ruby: a && b || !c
来源：http://lnl.jqgfzy.top

C#:   a && b || !c
来源：http://ajg.ivvv.top

[B16] 卫语句：不满足条件提前返回
来源：http://ibr.jinghuilouyu.cn

Py:   if not data: return
来源：http://dms.shuidangran.top

PHP:  if (!$data) { return; }
来源：http://gct.zycfv.cn

JS:   if (!data) return;
来源：http://sbx.yueranfly.top

TS:   if (!data) return;
来源：http://sib.yuanzhike.top

Java: if (data == null) return;
来源：http://vrz.ybcxt.top

Go:   if data == nil { return }
来源：http://mqk.guannengcc.top

Ruby: return if data.nil?
来源：http://kot.fktsv.cn

C#:   if (data == null) return;
来源：http://mgm.chenlongwang.top


<!-- 参考信息 -->