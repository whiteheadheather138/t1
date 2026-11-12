代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://fzk.shzxlz.cn

[A11] 条件表达式（三元）
来源：http://mkm.yueranfly.top

Py:   "yes" if x > 0 else "no"
来源：http://lbe.shangyingyoupin.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nqr.hnxiangtu.top

JS:   x > 0 ? "yes" : "no"
来源：http://twy.xuetiantiany.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dqr.xziqi.cn

Java: x > 0 ? "yes" : "no"
来源：http://uhz.smart0.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://ukn.mhx1999.top

Ruby: x > 0 ? "yes" : "no"
来源：http://xqq.yuxming.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mur.fanxiaobao.xyz

[A12] 字符串插值 / 格式化
来源：http://tjs.snrcjt.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ufm.zhiwuduotai.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://scs.shanyushiyangtech.top

JS:   `Hello, ${name}!`
来源：http://fqo.snrcjt.cn

TS:   `Hello, ${name}!`
来源：http://moz.mhx1999.top

Java: "Hello, %s!".formatted(name)
来源：http://kqb.iojbl.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hgh.xuetiantiany.cn

Ruby: "Hello, #{name}!"
来源：http://dxb.ywan-chungtsiang.top

C#:   $"Hello, {name}!"
来源：http://jry.ybcxt.top

[A13] 多行字符串（练习 \n 转义）
来源：http://pxw.0kj1m.cn

Py:   "第一行\n第二行"
来源：http://fko.daxiang520.top

PHP:  "第一行\n第二行"
来源：http://ain.9152youxi.cn

JS:   "第一行\n第二行"
来源：http://tht.havefunace.top

TS:   "第一行\n第二行"
来源：http://oqr.nanxinkj.top

Java: "第一行\n第二行"
来源：http://rsx.jiagoushi.top

Go:   "第一行\n第二行"
来源：http://bnf.tarul.cn

Ruby: "第一行\n第二行"
来源：http://hpm.tian-w.cn

C#:   "第一行\n第二行"
来源：http://rmj.birdmap.top

[A14] 注释写法
来源：http://umb.haohaochexian.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kfc.52xcode.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hia.guowangkeji.top

JS:   // 单行；/* 多行 */
来源：http://nnl.vqdsnc.cn

TS:   // 单行；/* 多行 */
来源：http://dce.aibaodan.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uoi.dianchejie.cn

Go:   // 单行；/* 多行 */
来源：http://ttp.yuxming.cn

Ruby: # 单行；=begin 多行 =end
来源：http://oqo.fehbvm.com

C#:   // 单行；/* 多行 */
来源：http://fce.ydzc1.top

[A15] 空值判断与默认值
来源：http://oxk.xylfe.cn

Py:   value = data or "默认值"
来源：http://rkl.zhiwuduotai.top

PHP:  $value = $data ?? "默认值";
来源：http://nft.smart0.xyz

JS:   const value = data ?? "默认值";
来源：http://htf.fktsv.cn

TS:   const value = data ?? "默认值";
来源：http://uha.9152youxi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://obw.guannengcc.top

Go:   if data == "" { data = "默认值" }
来源：http://pbg.zhixingplan.top

Ruby: value = data || "默认值"
来源：http://eet.xinyue.icu

C#:   var value = data ?? "默认值";
来源：http://fvn.shanyushiyangtech.top

[A16] 真假值判断规则
来源：http://zvh.c1oappe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kmz.smart0.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qwt.guowangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://caf.aibaodan.cn

TS:   if (!x) {}
来源：http://bde.jinqigufen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ian.cashguo.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wvh.chenlongwang.top

Ruby: unless x            # nil 与 false 为假
来源：http://ijx.daxiang520.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://svy.yfazqb.com

[A17] 位运算
来源：http://ylb.xziqi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gng.cdnleiting.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hxq.bbcook.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lsh.xinyue.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zea.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ccx.meibo888.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://eqk.jinqigfzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ltt.zycfv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qkd.ivvv.top

[A18] 字符与 ASCII 码互转
来源：http://gec.jqgufenzy.top

Py:   ord("A"); chr(65)
来源：http://suq.gotoacloud.top

PHP:  ord("A"); chr(65)
来源：http://tur.epnwcf.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dbg.sxryk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mex.sweek.top

Java: (int) 'A'; (char) 65
来源：http://icp.dashuyun.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yxa.chenjidiqi.icu

Ruby: "A".ord; 65.chr
来源：http://qvc.guannengcc.top

C#:   (int)'A'; (char)65
来源：http://dol.yj20258.top

[A19] 交换两个变量
来源：http://ihl.vqdsnc.cn

Py:   a, b = b, a
来源：http://oiz.bjfxy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qyu.ppjwa.cn

JS:   [a, b] = [b, a];
来源：http://ppf.chenjidiqi.icu

TS:   [a, b] = [b, a];
来源：http://hxq.kuanghao11.cn

Java: int t = a; a = b; b = t;
来源：http://ihf.jinghuilouyu.cn

Go:   a, b = b, a
来源：http://hsr.hcnkem.com

Ruby: a, b = b, a
来源：http://sth.fanxiaobao.xyz

C#:   (a, b) = (b, a);
来源：http://trx.jianghu66.top

[A20] 读取标准输入
来源：http://gon.zdbjq.cn

Py:   name = input("请输入：")
来源：http://vwf.sysykeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bbx.guannengcc.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://imi.guannengcc.top

TS:   // Node.js：readline 模块
来源：http://rej.chenzaomai.com

Java: new Scanner(System.in).nextLine()
来源：http://qej.zhijiandao.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://peq.haohaochexian.top

Ruby: gets.chomp
来源：http://nkm.xuetiantiany.cn

C#:   Console.ReadLine();
来源：http://qsb.xylfe.cn

[A21] 保留指定小数位输出
来源：http://nud.zhaomingkeji.xyz

Py:   f"{3.14159:.2f}"
来源：http://hhw.shanyushiyangkeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oti.chenlongwang.top

JS:   (3.14159).toFixed(2)
来源：http://zas.hnxiangtu.top

TS:   (3.14159).toFixed(2)
来源：http://kto.52xcode.cn

Java: String.format("%.2f", 3.14159)
来源：http://iiq.zhixingplan.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vlp.jinyuanbaomall.cn

Ruby: format("%.2f", 3.14159)
来源：http://vyg.yj20258.top

C#:   3.14159.ToString("F2")
来源：http://tfa.xinyue.icu

[A22] 获取字符串长度
来源：http://ztj.wangshuangyany.cn

Py:   len(s)
来源：http://xin.guannengcc.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hiw.hesvh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nii.hongshengwenyu.top

TS:   s.length
来源：http://ufu.aizwys.cn

Java: s.length()
来源：http://kic.ppjwa.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jua.jinyuanbaomall.cn

Ruby: s.length
来源：http://vkm.hnqzz.top

C#:   s.Length
来源：http://qwa.tanke756.top

[A23] 大小写转换
来源：http://kra.jlsjyb.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ivg.ywan-chungtsiang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fvm.yj20258.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rmg.xziqi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qvs.zhiwuduotai.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cbf.ctjpmb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gfr.jinqigfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ald.vehdjk.com

C#:   s.ToUpper(); s.ToLower()
来源：http://gth.shangyingyoupin.top

[A24] 去除首尾空白
来源：http://lvh.hammf.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wuo.zhoulong.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jiv.jinqigufen.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tts.bjfxy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://idm.yfazqb.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uys.daxiang520.top

Go:   strings.TrimSpace(s)
来源：http://ioi.aibaodan.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ady.fktsv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cin.fengsongda.top

[A25] 字符串比较
来源：http://ofh.daria6918.cn

Py:   s1 == s2; s1 != s2
来源：http://qla.jinqigufen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lco.xuanzx.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xdm.yfazqb.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zip.316326.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pmu.guannengcc.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hkj.cdnleiting.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ara.sjlbkw.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rgj.fzhhl.top

[A26] 类型转换总览
来源：http://pnk.zhoulong.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://snh.nanxinkj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://act.havefunace.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fzy.gotoacloud.top

TS:   Number() String() Boolean() x as number
来源：http://jrk.shanyushiyangtech.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://geb.fengsongda.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vjz.gotoacloud.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qzl.guannengcc.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ogr.yj20258888.top

================================================================================
来源：http://eus.hesvh.cn

B. 流程控制
来源：http://dhp.zhengqikj.top

================================================================================
来源：http://sob.jqgfzy.top

[B01] 条件判断 if / else
来源：http://suf.sjlbkw.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ybh.daria6918.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ihk.bjfxy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rso.epnwcf.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bpy.tianlin.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://qlo.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gvw.ybcxt.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jdi.zdbjq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pnb.gzhubu.top

[B02] 多分支 else if / elif
来源：http://gia.bjfxy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xxv.xinyue.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qls.nanxinkj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zna.zdbjq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sdt.yanxiufei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kbd.yueranfly.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eyb.hnxiangtu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tgf.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xun.zhaomingkeji.xyz

[B03] switch / match / case
来源：http://fft.nanxuanxn.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ixz.cdnleiting.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hea.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://phr.meibo888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nfp.cheryme.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ipc.aizwys.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pec.xuetiantiany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sfh.hesvh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ahr.fanxiaobao.xyz

[B04] for 计数循环
来源：http://nia.hnqzz.top

Py:   for i in range(10): print(i)
来源：http://tbg.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dji.chenlongwang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dfc.yangfankeji.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://swq.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rsn.xuetiantiany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fib.ctjpmb.com

Ruby: 10.times { |i| puts i }
来源：http://hwr.shuidangran.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tfy.haohaochexian.top

[B05] 遍历数组 / 列表
来源：http://mbc.yfazqb.com

Py:   for item in arr: print(item)
来源：http://tcn.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ruo.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://mnq.dashuyun.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cqd.kuanghao11.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://exb.pycfn.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kvp.haohaochexian.top

Ruby: arr.each { |item| puts item }
来源：http://vbf.daria6918.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rvd.vqdsnc.cn

[B06] 遍历字典 / 对象
来源：http://dnp.ywan-chungtsiang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ssm.chenlongwang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yge.shzxlz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sto.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://phd.yueranfly.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nni.sufxvd.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dff.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jhk.kuanghao11.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qjv.nwbrower.top

[B07] while 循环
来源：http://xpw.zhongyouzk.top

Py:   while i < 10: i += 1
来源：http://hud.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qxq.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://iqz.epnwcf.com

TS:   while (i < 10) { i++; }
来源：http://kwm.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://oxg.ywan-chungtsiang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://apf.zhaomingkeji.xyz

Ruby: while i < 10; i += 1; end
来源：http://dek.zhaomingkeji.xyz

C#:   while (i < 10) { i++; }
来源：http://juf.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://cyv.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://tdu.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kfp.cdnleiting.top

JS:   do { i++; } while (i < 10);
来源：http://eeq.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://mhu.sjlbkw.cn

Java: do { i++; } while (i < 10);
来源：http://eju.52xcode.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rxf.vehdjk.com

Ruby: begin; i += 1; end while i < 10
来源：http://ihh.xinyue.icu

C#:   do { i++; } while (i < 10);
来源：http://dof.bjfxy.top

[B09] break 与 continue
来源：http://had.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gkx.zhixingplan.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oyj.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kwd.yfazqb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://whg.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fzr.jiagoushi.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nak.zycfv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ime.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hrh.zhaomingkeji.xyz

[B10] 遍历同时拿索引
来源：http://pte.zhiwuduotai.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mrl.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hgv.hnqzz.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nmu.hcnkem.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mvn.sweek.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://inc.dashuyun.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wll.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dtv.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jfg.iojbl.cn

[B11] 生成数字序列 / 区间
来源：http://xoo.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://ccm.gaohongyu789.top

PHP:  range(0, 10, 2);
来源：http://yot.ehwqpu.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qlh.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mwp.yueranfly.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blp.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vym.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://ajp.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bzq.gogol.net.cn

[B12] 跳出多层循环
来源：http://nxs.daxiang520.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yki.zhengqikj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rvm.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jgp.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kty.quarkkingdee.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wem.yanxiufei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bgk.cdnleiting.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fur.hnqzz.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kyx.gogol.net.cn

[B13] 判断是否为数字
来源：http://wvy.hcnkem.com

Py:   isinstance(x, (int, float))
来源：http://lad.gzhubu.top

PHP:  is_numeric($x)
来源：http://cdr.fktsv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://akb.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ets.tarul.cn

Java: x instanceof Number
来源：http://dlc.fzhhl.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oiy.0kj1m.cn

Ruby: x.is_a?(Numeric)
来源：http://bsd.yvedp.cn

C#:   x is int or double or decimal
来源：http://dvk.fanxiaobao.xyz

[B14] 判断值是否在集合内
来源：http://nfk.cashguo.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wjz.chenjidiqi.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uat.zhengqikj.top

JS:   [1, 2, 3].includes(x)
来源：http://srx.mhx1999.top

TS:   [1, 2, 3].includes(x)
来源：http://hgo.yanxiufei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://geh.xinyue.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dwf.shzxlz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wfb.cucudq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://deo.zycfv.cn

[B15] 布尔运算与取反
来源：http://nkx.uphjek.com

Py:   a and b or not c
来源：http://nfs.jqgufenzy.top

PHP:  $a && $b || !$c
来源：http://lvi.sufxvd.cn

JS:   a && b || !c
来源：http://fbi.fanxiaobao.xyz

TS:   a && b || !c
来源：http://bin.vehdjk.com

Java: a && b || !c
来源：http://ekr.yangfankeji.com

Go:   a && b || !c
来源：http://xcw.kuanghao11.cn

Ruby: a && b || !c
来源：http://wxf.kuanghao11.cn

C#:   a && b || !c
来源：http://qce.redwolf501.top

[B16] 卫语句：不满足条件提前返回
来源：http://sbz.chenlongwang.top

Py:   if not data: return
来源：http://kbh.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://vzg.sufxvd.cn

JS:   if (!data) return;
来源：http://qel.ppjwa.cn

TS:   if (!data) return;
来源：http://scs.jlsjyb.cn

Java: if (data == null) return;
来源：http://acz.ybcxt.top

Go:   if data == nil { return }
来源：http://apm.sjlbkw.cn

Ruby: return if data.nil?
来源：http://iwg.yvedp.cn

C#:   if (data == null) return;
来源：http://jma.xinyue.icu

================================================================================
来源：http://lwa.zdqjudy.top

C. 函数与作用域
来源：http://dqq.jinqigufen.top

================================================================================
来源：http://hxt.yvedp.cn

[C01] 定义函数
来源：http://aep.yongpay.top

Py:   def add(a, b): return a + b
来源：http://gpm.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tsc.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://agd.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kxx.zhongyouzk.top


<!-- 参考信息 -->