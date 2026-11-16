代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://zep.meibo888.top

[A11] 条件表达式（三元）
来源：http://tvu.iojbl.cn

Py:   "yes" if x > 0 else "no"
来源：http://umh.fzhhl.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://wrw.ehwqpu.com

JS:   x > 0 ? "yes" : "no"
来源：http://cnu.52xcode.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bbv.c1oappe.top

Java: x > 0 ? "yes" : "no"
来源：http://qbp.haohaochexian.top

Go:   // 无三元运算符，需用 if 语句
来源：http://cwm.uphjek.com

Ruby: x > 0 ? "yes" : "no"
来源：http://omp.yvedp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ayx.hnxiangtu.top

[A12] 字符串插值 / 格式化
来源：http://rbg.pycfn.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://suc.jyoumei.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cog.gotoacloud.top

JS:   `Hello, ${name}!`
来源：http://chx.c1oappe.top

TS:   `Hello, ${name}!`
来源：http://ewk.meibo888.top

Java: "Hello, %s!".formatted(name)
来源：http://drg.tanke756.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pjt.yuxming.cn

Ruby: "Hello, #{name}!"
来源：http://tdq.bjfxy.top

C#:   $"Hello, {name}!"
来源：http://vsm.jianghu66.top

[A13] 多行字符串（练习 \n 转义）
来源：http://kif.ywan-chungtsiang.top

Py:   "第一行\n第二行"
来源：http://gav.shangyingyoupin.top

PHP:  "第一行\n第二行"
来源：http://sfn.svipenyu.cn

JS:   "第一行\n第二行"
来源：http://zjg.yangfankeji.com

TS:   "第一行\n第二行"
来源：http://zut.pycfn.com

Java: "第一行\n第二行"
来源：http://vij.shanyushiyangkeji.top

Go:   "第一行\n第二行"
来源：http://cgb.bjfxy.top

Ruby: "第一行\n第二行"
来源：http://bsu.zhiwuduotai.top

C#:   "第一行\n第二行"
来源：http://cpr.jiagoushi.top

[A14] 注释写法
来源：http://bkc.svipenyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://myj.bjfxy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://baa.xinyue.icu

JS:   // 单行；/* 多行 */
来源：http://xgp.jyoumei.cn

TS:   // 单行；/* 多行 */
来源：http://uok.bjfxy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gdh.fanxiaobao.xyz

Go:   // 单行；/* 多行 */
来源：http://kkl.chenzaomai.com

Ruby: # 单行；=begin 多行 =end
来源：http://laq.daxiang520.top

C#:   // 单行；/* 多行 */
来源：http://sbs.zhixingplan.top

[A15] 空值判断与默认值
来源：http://uac.jinyuanbaomall.cn

Py:   value = data or "默认值"
来源：http://tuo.jinghuilouyu.cn

PHP:  $value = $data ?? "默认值";
来源：http://wzg.svipenyu.cn

JS:   const value = data ?? "默认值";
来源：http://tzo.guowangkeji.top

TS:   const value = data ?? "默认值";
来源：http://cfo.sxryk.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rur.sufxvd.cn

Go:   if data == "" { data = "默认值" }
来源：http://nct.smart0.xyz

Ruby: value = data || "默认值"
来源：http://umg.hammf.cn

C#:   var value = data ?? "默认值";
来源：http://xhk.chenlongwang.top

[A16] 真假值判断规则
来源：http://yis.gaohongyu789.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mgl.vehdjk.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qbz.haohaochexian.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qql.epnwcf.com

TS:   if (!x) {}
来源：http://cfn.zhoulong.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lbk.zdqjudy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yll.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://ggv.sweek.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ssi.meibo888.top

[A17] 位运算
来源：http://lft.aibaodan.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cep.jqgfzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pij.daria6918.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pqj.fanxiaobao.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kds.smart0.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://peb.jinghuilouyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pdy.meibo888.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rrw.bbcook.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://svj.zhongyouzk.top

[A18] 字符与 ASCII 码互转
来源：http://rkm.xuetiantiany.cn

Py:   ord("A"); chr(65)
来源：http://vff.xziqi.cn

PHP:  ord("A"); chr(65)
来源：http://gta.fktsv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ebm.cqqwz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://evl.cdnleiting.top

Java: (int) 'A'; (char) 65
来源：http://pjm.jianghu66.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fns.gzhubu.top

Ruby: "A".ord; 65.chr
来源：http://pop.zhoulong.xyz

C#:   (int)'A'; (char)65
来源：http://vqf.52xcode.cn

[A19] 交换两个变量
来源：http://fqq.yongpay.top

Py:   a, b = b, a
来源：http://oyg.yangfankeji.com

PHP:  [$a, $b] = [$b, $a];
来源：http://qhh.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://wyk.jqgufenzy.top

TS:   [a, b] = [b, a];
来源：http://mtr.xuanzx.com

Java: int t = a; a = b; b = t;
来源：http://xvb.cucudq.cn

Go:   a, b = b, a
来源：http://xjr.zhongyouzk.top

Ruby: a, b = b, a
来源：http://slh.xylfe.cn

C#:   (a, b) = (b, a);
来源：http://sms.cheryme.top

[A20] 读取标准输入
来源：http://fgj.zhongyouzk.top

Py:   name = input("请输入：")
来源：http://ciy.fzhhl.top

PHP:  $name = trim(fgets(STDIN));
来源：http://pbj.9152youxi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bdz.yfazqb.com

TS:   // Node.js：readline 模块
来源：http://flp.ehwqpu.com

Java: new Scanner(System.in).nextLine()
来源：http://wrv.sweek.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yka.chenlongwang.top

Ruby: gets.chomp
来源：http://mna.cucudq.cn

C#:   Console.ReadLine();
来源：http://ngd.guannengcc.top

[A21] 保留指定小数位输出
来源：http://gdm.jqgufenzy.top

Py:   f"{3.14159:.2f}"
来源：http://ubt.nwbrower.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hkv.wangdashe.top

JS:   (3.14159).toFixed(2)
来源：http://dyg.hnxiangtu.top

TS:   (3.14159).toFixed(2)
来源：http://kvg.ctjpmb.com

Java: String.format("%.2f", 3.14159)
来源：http://bip.shanyushiyangtech.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lod.zhijiandao.cn

Ruby: format("%.2f", 3.14159)
来源：http://ubr.epnwcf.com

C#:   3.14159.ToString("F2")
来源：http://bid.nanxinkj.top

[A22] 获取字符串长度
来源：http://mvn.tianlin.xyz

Py:   len(s)
来源：http://jnx.aizwys.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vrc.wangdashe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://por.tianlin.xyz

TS:   s.length
来源：http://nhm.yanxiufei.cn

Java: s.length()
来源：http://tdi.aibaodan.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://knn.fehbvm.com

Ruby: s.length
来源：http://tpa.fehbvm.com

C#:   s.Length
来源：http://dup.wangshuangyany.cn

[A23] 大小写转换
来源：http://zzt.zhiwuduotai.top

Py:   s.upper(); s.lower(); s.title()
来源：http://oux.haohaochexian.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pfk.vehdjk.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ise.shzxlz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jec.yvedp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mpb.tianlin.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vwy.ivvv.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jik.sysykeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dgk.nwbrower.top

[A24] 去除首尾空白
来源：http://kxy.yongpay.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iaz.xingfuxueyuan.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hcd.zhixingplan.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jkv.hammf.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tbm.xingfuxueyuan.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ijc.dianchejie.cn

Go:   strings.TrimSpace(s)
来源：http://ear.cashguo.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sri.9152youxi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dnp.gogol.net.cn

[A25] 字符串比较
来源：http://uss.hfpthk.cn

Py:   s1 == s2; s1 != s2
来源：http://vrg.shzxlz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ers.dianchejie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fqn.tarul.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hwl.jinqigfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zld.xuanzx.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zsg.ctjpmb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://nul.meibo888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://frr.zhoulong.xyz

[A26] 类型转换总览
来源：http://xgg.havefunace.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bqq.jqgufenzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ltl.feifeiyinyue.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://raa.fengsongda.top

TS:   Number() String() Boolean() x as number
来源：http://ssm.uphjek.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gvk.hfpthk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lnt.smart0.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://uix.nwbrower.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cyw.xylfe.cn

================================================================================
来源：http://nmn.guowangkeji.top

B. 流程控制
来源：http://rfp.hnqzz.top

================================================================================
来源：http://fxd.tanke756.top

[B01] 条件判断 if / else
来源：http://ldo.xylfe.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zcn.gzhubu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mwz.svipenyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tsk.jinqigufen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aif.hnxiangtu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://aqc.fktsv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://reb.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tuy.quarkkingdee.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fpx.zhixingplan.top

[B02] 多分支 else if / elif
来源：http://mff.dianchejie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rzy.daxiang520.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pmq.zhongyouzk.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://diy.shuidangran.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qne.hesvh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ose.nanxuanxn.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ann.zdbjq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xno.daxiang520.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wse.sweek.top

[B03] switch / match / case
来源：http://yrc.mhx1999.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oha.cashguo.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kvx.gaohongyu789.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://viu.jlsjyb.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zcg.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dmx.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wpz.aibaodan.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nbg.zhijiandao.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jwy.svipenyu.cn

[B04] for 计数循环
来源：http://pau.fanxiaobao.xyz

Py:   for i in range(10): print(i)
来源：http://bhs.cqqwz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yqg.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bzw.zhijiandao.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cju.ehwqpu.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qzi.yj20258888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oea.52xcode.cn

Ruby: 10.times { |i| puts i }
来源：http://niv.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jom.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://nco.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://luc.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://evt.yuanzhike.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rtj.shangyingyoupin.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jol.smart0.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://kbg.vqdsnc.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nrd.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://shf.feifeiyinyue.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://joi.pengpengdd.cyou

[B06] 遍历字典 / 对象
来源：http://ciu.sjlbkw.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cww.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qpr.wangshuangyany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bnk.uphjek.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hwr.chenlongwang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://osz.dashuyun.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ktc.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zwd.yongpay.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ygq.jinghuilouyu.cn

[B07] while 循环
来源：http://jeg.shzxlz.cn

Py:   while i < 10: i += 1
来源：http://qda.yj20258.top

PHP:  while ($i < 10) { $i++; }
来源：http://owe.jinqigfzy.top

JS:   while (i < 10) { i++; }
来源：http://dso.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://mgc.sweek.top

Java: while (i < 10) { i++; }
来源：http://wqg.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wgo.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://hbt.shanyushiyangkeji.top

C#:   while (i < 10) { i++; }
来源：http://vlt.wangshuangyany.cn

[B08] do-while（至少执行一次）
来源：http://wbj.cqqwz.cn

Py:   # 无 do-while：用 while True + break
来源：http://gcl.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fas.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://lyl.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://uvv.cdnleiting.top

Java: do { i++; } while (i < 10);
来源：http://qed.feifeiyinyue.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xan.feifeiyinyue.top

Ruby: begin; i += 1; end while i < 10
来源：http://dss.jlsjyb.cn

C#:   do { i++; } while (i < 10);
来源：http://clk.wangdashe.top

[B09] break 与 continue
来源：http://nqz.smart0.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hnx.havefunace.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tvf.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vwn.zhijiandao.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rye.tanke756.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jod.yfazqb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://msj.yongpay.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cfb.fengsongda.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://foa.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://uqv.gaohongyu789.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://esd.cucudq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://czs.guowangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://obs.yonumen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cug.zdbjq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aqa.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vbp.bjfxy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ubz.jinqigufen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vwj.fzhhl.top

[B11] 生成数字序列 / 区间
来源：http://eik.shzxlz.cn

Py:   list(range(0, 10, 2))
来源：http://rkw.sweek.top

PHP:  range(0, 10, 2);
来源：http://nlz.jqgfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cyp.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mjx.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://smu.gzhubu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nzi.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://fgl.chenzaomai.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://roy.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://nms.sxryk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cbf.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vfy.nanxuanxn.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mbf.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sfi.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iiw.dashuyun.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bfi.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aqa.vehdjk.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://phn.haohaochexian.top

[B13] 判断是否为数字
来源：http://die.havefunace.top

Py:   isinstance(x, (int, float))
来源：http://xsf.zhaomingkeji.xyz

PHP:  is_numeric($x)
来源：http://xbo.yonumen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vuq.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mfl.sysykeji.top

Java: x instanceof Number
来源：http://wld.xuanzx.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://owp.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://dly.xuanzx.com

C#:   x is int or double or decimal
来源：http://krz.c1oappe.top

[B14] 判断值是否在集合内
来源：http://ouy.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bbv.smart0.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://czu.fengsongda.top

JS:   [1, 2, 3].includes(x)
来源：http://zae.hywenlv.cn

TS:   [1, 2, 3].includes(x)
来源：http://zba.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ftc.yueranfly.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ydt.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://fkf.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hcq.havefunace.top

[B15] 布尔运算与取反
来源：http://inm.ywan-chungtsiang.top

Py:   a and b or not c
来源：http://bhe.c1oappe.top

PHP:  $a && $b || !$c
来源：http://qor.quarkkingdee.top

JS:   a && b || !c
来源：http://luw.fzhhl.top

TS:   a && b || !c
来源：http://dhl.quarkkingdee.top

Java: a && b || !c
来源：http://ijp.ivvv.top

Go:   a && b || !c
来源：http://vkn.feifeiyinyue.top

Ruby: a && b || !c
来源：http://qqz.vqdsnc.cn

C#:   a && b || !c
来源：http://cap.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://inq.ydjk.org.cn

Py:   if not data: return
来源：http://gkk.xinyue.icu

PHP:  if (!$data) { return; }
来源：http://njo.haohaochexian.top

JS:   if (!data) return;
来源：http://utj.hywenlv.cn

TS:   if (!data) return;
来源：http://gba.gotoacloud.top

Java: if (data == null) return;
来源：http://njo.hysaishi.cn

Go:   if data == nil { return }
来源：http://fdi.hcnkem.com

Ruby: return if data.nil?
来源：http://emo.hywenlv.cn

C#:   if (data == null) return;
来源：http://cvy.pycfn.com

================================================================================
来源：http://guc.zhixingplan.top

C. 函数与作用域
来源：http://yjh.ppjwa.cn

================================================================================
来源：http://qxv.zhengqikj.top

[C01] 定义函数
来源：http://suo.yonumen.top

Py:   def add(a, b): return a + b
来源：http://lmj.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wkj.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://tay.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://khk.meibo888.top


<!-- 参考信息 -->