代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sfr.fanxiaobao.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ozv.yuxming.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tro.chenjidiqi.icu

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://khq.ydjk.org.cn

[A10] 生成随机数
来源：http://hye.zycfv.cn

Py:   import random; random.randint(1, 100)
来源：http://tky.yj202588.top

PHP:  random_int(1, 100);
来源：http://ckz.snrcjt.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dah.sjlbkw.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hsp.yj202588.top

Java: new Random().nextInt(100) + 1
来源：http://nyy.zdbjq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wib.sysykeji.top

Ruby: rand(1..100)
来源：http://oho.zhoulong.xyz

C#:   new Random().Next(1, 101)
来源：http://eqr.redwolf501.top

[A11] 条件表达式（三元）
来源：http://fku.nanxinkj.top

Py:   "yes" if x > 0 else "no"
来源：http://btw.0kj1m.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rmo.zdbjq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ipy.daxiang520.top

TS:   x > 0 ? "yes" : "no"
来源：http://mld.iojbl.cn

Java: x > 0 ? "yes" : "no"
来源：http://meb.dianchejie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lrb.redwolf501.top

Ruby: x > 0 ? "yes" : "no"
来源：http://rht.ybcxt.top

C#:   x > 0 ? "yes" : "no"
来源：http://xsi.fktsv.cn

[A12] 字符串插值 / 格式化
来源：http://gej.nanxinkj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vim.tian-w.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kul.gaohongyu789.top

JS:   `Hello, ${name}!`
来源：http://mqd.sysykeji.top

TS:   `Hello, ${name}!`
来源：http://ejv.yj20258888.top

Java: "Hello, %s!".formatted(name)
来源：http://nzj.zhengqikj.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eic.vehdjk.com

Ruby: "Hello, #{name}!"
来源：http://vvi.tarul.cn

C#:   $"Hello, {name}!"
来源：http://lhu.cashguo.top

[A13] 多行字符串（练习 \n 转义）
来源：http://rcg.yvedp.cn

Py:   "第一行\n第二行"
来源：http://imt.dashuyun.cn

PHP:  "第一行\n第二行"
来源：http://bqr.yj20258.top

JS:   "第一行\n第二行"
来源：http://csv.aibaodan.cn

TS:   "第一行\n第二行"
来源：http://uuz.zhiwuduotai.top

Java: "第一行\n第二行"
来源：http://kso.xuanzx.com

Go:   "第一行\n第二行"
来源：http://ytr.gzhubu.top

Ruby: "第一行\n第二行"
来源：http://shg.snrcjt.cn

C#:   "第一行\n第二行"
来源：http://lkx.bjfxy.top

[A14] 注释写法
来源：http://yrm.jinqigufen.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zws.fanxiaobao.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://rpt.hongshengwenyu.top

JS:   // 单行；/* 多行 */
来源：http://zzl.tianlin.xyz

TS:   // 单行；/* 多行 */
来源：http://ajp.xinyue.icu

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xsr.xuetiantiany.cn

Go:   // 单行；/* 多行 */
来源：http://wxd.xziqi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wyr.zdbjq.cn

C#:   // 单行；/* 多行 */
来源：http://pdb.zhaomingkeji.xyz

[A15] 空值判断与默认值
来源：http://hpa.zhoulong.xyz

Py:   value = data or "默认值"
来源：http://aan.shanyushiyangtech.top

PHP:  $value = $data ?? "默认值";
来源：http://blw.mhx1999.top

JS:   const value = data ?? "默认值";
来源：http://rkm.yj20258888.top

TS:   const value = data ?? "默认值";
来源：http://kws.c1oappe.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cvf.gotoacloud.top

Go:   if data == "" { data = "默认值" }
来源：http://jpm.fktsv.cn

Ruby: value = data || "默认值"
来源：http://yke.xinyue.icu

C#:   var value = data ?? "默认值";
来源：http://sgy.chenlongwang.top

[A16] 真假值判断规则
来源：http://jji.mhx1999.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yqz.pycfn.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://okm.sxryk.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dpu.9152youxi.cn

TS:   if (!x) {}
来源：http://lil.ybcxt.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fyo.fzhhl.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ivn.dianchejie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vyg.sufxvd.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oud.tarul.cn

[A17] 位运算
来源：http://wqj.tanke756.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://koo.wangshuangyany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fnj.cucudq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uqa.yuanzhike.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jxu.cashguo.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aid.ivvv.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pet.shuidangran.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cbc.yangfankeji.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vwp.yanxiufei.cn

[A18] 字符与 ASCII 码互转
来源：http://zyt.gaohongyu789.top

Py:   ord("A"); chr(65)
来源：http://kfn.9152youxi.cn

PHP:  ord("A"); chr(65)
来源：http://sza.cucudq.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rtt.hysaishi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ixg.zhixingplan.top

Java: (int) 'A'; (char) 65
来源：http://yen.wangshuangyany.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lbl.zhaomingkeji.xyz

Ruby: "A".ord; 65.chr
来源：http://gyh.gaohongyu789.top

C#:   (int)'A'; (char)65
来源：http://ecj.cqqwz.cn

[A19] 交换两个变量
来源：http://khm.shuidangran.top

Py:   a, b = b, a
来源：http://uyk.jqgfzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://psv.havefunace.top

JS:   [a, b] = [b, a];
来源：http://ngs.cheryme.top

TS:   [a, b] = [b, a];
来源：http://pnf.yuanzhike.top

Java: int t = a; a = b; b = t;
来源：http://rsu.bbcook.cn

Go:   a, b = b, a
来源：http://soj.316326.xyz

Ruby: a, b = b, a
来源：http://vgi.shuidangran.top

C#:   (a, b) = (b, a);
来源：http://jll.wangshuangyany.cn

[A20] 读取标准输入
来源：http://wyc.fengsongda.top

Py:   name = input("请输入：")
来源：http://mok.shanyushiyangtech.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bsk.aizwys.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kga.yanxiufei.cn

TS:   // Node.js：readline 模块
来源：http://qbn.aizwys.cn

Java: new Scanner(System.in).nextLine()
来源：http://sdw.jqgfzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rzi.9152youxi.cn

Ruby: gets.chomp
来源：http://sex.yfazqb.com

C#:   Console.ReadLine();
来源：http://btz.shuidangran.top

[A21] 保留指定小数位输出
来源：http://gll.shanyushiyangtech.top

Py:   f"{3.14159:.2f}"
来源：http://cas.sxryk.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wgq.yfazqb.com

JS:   (3.14159).toFixed(2)
来源：http://rdh.bbcook.cn

TS:   (3.14159).toFixed(2)
来源：http://imy.chenjidiqi.icu

Java: String.format("%.2f", 3.14159)
来源：http://jaa.sjlbkw.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nxe.fktsv.cn

Ruby: format("%.2f", 3.14159)
来源：http://qnu.ehwqpu.com

C#:   3.14159.ToString("F2")
来源：http://ehp.jqgfzy.top

[A22] 获取字符串长度
来源：http://veh.shuidangran.top

Py:   len(s)
来源：http://cxt.yj20258.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oak.tianlin.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nol.meibo888.top

TS:   s.length
来源：http://jpg.jinyuanbaomall.cn

Java: s.length()
来源：http://agq.ywan-chungtsiang.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nio.wangdashe.top

Ruby: s.length
来源：http://gxc.dianchejie.cn

C#:   s.Length
来源：http://fhh.aibaodan.cn

[A23] 大小写转换
来源：http://qpp.sweek.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wjj.kuanghao11.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://erv.9152youxi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ajf.guannengcc.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xvj.haohaochexian.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vfk.fehbvm.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cfe.uphjek.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zxi.jqgufenzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hhr.chenjidiqi.icu

[A24] 去除首尾空白
来源：http://qva.0kj1m.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kul.52xcode.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://goh.sysykeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ifx.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ftp.mhx1999.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lwj.andypj.xyz

Go:   strings.TrimSpace(s)
来源：http://hlu.fehbvm.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bbr.iojbl.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vwn.gogol.net.cn

[A25] 字符串比较
来源：http://isk.jqgfzy.top

Py:   s1 == s2; s1 != s2
来源：http://hme.bbcook.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uon.vqdsnc.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ryj.svipenyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ndx.birdmap.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hsa.hongshengwenyu.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hyk.zhaomingkeji.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://tvr.andypj.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hzj.hcnkem.com

[A26] 类型转换总览
来源：http://umy.yueranfly.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pup.daxiang520.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wab.meibo888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wni.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://byr.hcnkem.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bga.iojbl.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baj.vehdjk.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://oxx.tanke756.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://viw.ehwqpu.com

================================================================================
来源：http://isa.daria6918.cn

B. 流程控制
来源：http://vlf.fzhhl.top

================================================================================
来源：http://hgi.andypj.xyz

[B01] 条件判断 if / else
来源：http://thg.jinghuilouyu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tdg.zhoulong.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://afm.cdnleiting.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qbz.pengpengdd.cyou

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bcv.fehbvm.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://vyu.jianghu66.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hld.fengsongda.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kao.snrcjt.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jls.shangyingyoupin.top

[B02] 多分支 else if / elif
来源：http://lno.yfazqb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qzo.ybcxt.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zij.ydzc1.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yyw.gogol.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cpt.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hck.0kj1m.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ylb.snrcjt.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://shp.daxiang520.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://abv.gotoacloud.top

[B03] switch / match / case
来源：http://mxj.pengpengdd.cyou

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iny.hesvh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xdg.pengpengdd.cyou

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lfc.sjlbkw.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nzj.ehwqpu.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lvg.havefunace.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://flz.yuanzhike.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tlj.sweek.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bua.jianghu66.top

[B04] for 计数循环
来源：http://fkd.cheryme.top

Py:   for i in range(10): print(i)
来源：http://yqs.zhijiandao.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rsm.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gys.andypj.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gbh.sjlbkw.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zpz.yj20258.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vgc.316326.xyz

Ruby: 10.times { |i| puts i }
来源：http://plo.yanxiufei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eqd.smart0.xyz

[B05] 遍历数组 / 列表
来源：http://kqg.yangfankeji.com

Py:   for item in arr: print(item)
来源：http://zuw.yongpay.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nnk.haohaochexian.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kcl.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vhz.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vwq.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kta.jinqigufen.top

Ruby: arr.each { |item| puts item }
来源：http://ket.yuxming.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hqk.fktsv.cn

[B06] 遍历字典 / 对象
来源：http://ndz.yfazqb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://fct.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wfk.yvedp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zqu.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kmf.daria6918.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ujx.shanyushiyangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xtj.gzhubu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ztm.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oyz.shuidangran.top

[B07] while 循环
来源：http://vdc.hnqzz.top

Py:   while i < 10: i += 1
来源：http://xwr.jinyuanbaomall.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qml.gogol.net.cn

JS:   while (i < 10) { i++; }
来源：http://vii.yangfankeji.com

TS:   while (i < 10) { i++; }
来源：http://qev.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://qqq.52xcode.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://khk.yanxiufei.cn

Ruby: while i < 10; i += 1; end
来源：http://wql.hysaishi.cn

C#:   while (i < 10) { i++; }
来源：http://ucp.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://iiz.ehwqpu.com

Py:   # 无 do-while：用 while True + break
来源：http://zzy.hnqzz.top

PHP:  do { $i++; } while ($i < 10);
来源：http://aij.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://rrl.epnwcf.com

TS:   do { i++; } while (i < 10);
来源：http://fpy.jinyuanbaomall.cn

Java: do { i++; } while (i < 10);
来源：http://scn.jinqigufen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://iyt.guowangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://mkh.epnwcf.com

C#:   do { i++; } while (i < 10);
来源：http://nra.xziqi.cn

[B09] break 与 continue
来源：http://fqy.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ewk.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qsg.redwolf501.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://itk.chenlongwang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hzz.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rkn.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zdj.haohaochexian.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://btn.zhaomingkeji.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rlj.zycfv.cn

[B10] 遍历同时拿索引
来源：http://nwi.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rpy.dashuyun.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://htw.gaohongyu789.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qmk.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aqw.daxiang520.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gjo.yj202588.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ver.zhijiandao.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fyb.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://obv.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://cka.andypj.xyz

Py:   list(range(0, 10, 2))
来源：http://oop.svipenyu.cn

PHP:  range(0, 10, 2);
来源：http://skc.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uay.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kqu.yj20258.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kyl.fehbvm.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aoe.xinyue.icu

Ruby: (0...10).step(2).to_a
来源：http://nak.jlsjyb.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hij.hongshengwenyu.top

[B12] 跳出多层循环
来源：http://bvi.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hns.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dfy.bbcook.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://reh.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wyn.yonumen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lcr.jinqigufen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gzw.zhengqikj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://egh.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wpb.haohaochexian.top

[B13] 判断是否为数字
来源：http://yae.birdmap.top

Py:   isinstance(x, (int, float))
来源：http://goh.daria6918.cn

PHP:  is_numeric($x)
来源：http://bla.ywan-chungtsiang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://smc.hongshengwenyu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ngd.gaohongyu789.top

Java: x instanceof Number
来源：http://yic.havefunace.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://npg.sjlbkw.cn

Ruby: x.is_a?(Numeric)
来源：http://rpf.havefunace.top

C#:   x is int or double or decimal
来源：http://crz.fzhhl.top

[B14] 判断值是否在集合内
来源：http://kmk.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gil.yueranfly.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gdp.zdbjq.cn

JS:   [1, 2, 3].includes(x)
来源：http://vmg.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://jlr.epnwcf.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ylv.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qlm.chenlongwang.top

Ruby: [1, 2, 3].include?(x)
来源：http://vom.cucudq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bcr.fktsv.cn

[B15] 布尔运算与取反
来源：http://tus.hammf.cn

Py:   a and b or not c
来源：http://rml.guannengcc.top

PHP:  $a && $b || !$c
来源：http://rby.ybcxt.top

JS:   a && b || !c
来源：http://kiq.fanxiaobao.xyz

TS:   a && b || !c
来源：http://rqg.hfpthk.cn

Java: a && b || !c
来源：http://fuj.wangdashe.top

Go:   a && b || !c
来源：http://okg.zhongyouzk.top

Ruby: a && b || !c
来源：http://day.xylfe.cn

C#:   a && b || !c
来源：http://koe.sysykeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://pxz.redwolf501.top

Py:   if not data: return
来源：http://dib.yuxming.cn

PHP:  if (!$data) { return; }
来源：http://peh.zhaomingkeji.xyz

JS:   if (!data) return;
来源：http://amm.pengpengdd.cyou

TS:   if (!data) return;
来源：http://byx.ivvv.top


<!-- 参考信息 -->