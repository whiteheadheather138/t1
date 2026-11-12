代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hxt.xziqi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://trk.fzhhl.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cop.yj202588.top

[A09] 绝对值与最大最小值
来源：http://cvl.uphjek.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hgf.ivvv.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wrf.snrcjt.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bfv.hongshengwenyu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cyu.yangfankeji.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uvy.hesvh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mro.yonumen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ceo.aizwys.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tik.chenzaomai.com

[A10] 生成随机数
来源：http://jhp.guowangkeji.top

Py:   import random; random.randint(1, 100)
来源：http://rgt.gogol.net.cn

PHP:  random_int(1, 100);
来源：http://ovi.xziqi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dzc.jqgfzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jgt.cqqwz.cn

Java: new Random().nextInt(100) + 1
来源：http://fci.shanyushiyangkeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gls.zhoulong.xyz

Ruby: rand(1..100)
来源：http://jui.hongshengwenyu.top

C#:   new Random().Next(1, 101)
来源：http://kyy.yuanzhike.top

[A11] 条件表达式（三元）
来源：http://wes.shuidangran.top

Py:   "yes" if x > 0 else "no"
来源：http://hyr.andypj.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://ecj.ivvv.top

JS:   x > 0 ? "yes" : "no"
来源：http://pij.ydzc1.top

TS:   x > 0 ? "yes" : "no"
来源：http://vsf.jyoumei.cn

Java: x > 0 ? "yes" : "no"
来源：http://zpq.jqgufenzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ndq.ybcxt.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ylv.gotoacloud.top

C#:   x > 0 ? "yes" : "no"
来源：http://wbf.jiagoushi.top

[A12] 字符串插值 / 格式化
来源：http://sib.jyoumei.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://byo.fzhhl.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cvf.tarul.cn

JS:   `Hello, ${name}!`
来源：http://efy.feifeiyinyue.top

TS:   `Hello, ${name}!`
来源：http://etu.cqqwz.cn

Java: "Hello, %s!".formatted(name)
来源：http://npq.hfpthk.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://snf.ehwqpu.com

Ruby: "Hello, #{name}!"
来源：http://xwd.cashguo.top

C#:   $"Hello, {name}!"
来源：http://zyz.snrcjt.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tmv.chenjidiqi.icu

Py:   "第一行\n第二行"
来源：http://bpx.yonumen.top

PHP:  "第一行\n第二行"
来源：http://qif.xziqi.cn

JS:   "第一行\n第二行"
来源：http://stp.nanxinkj.top

TS:   "第一行\n第二行"
来源：http://kzb.jinqigufen.top

Java: "第一行\n第二行"
来源：http://pvw.hnxiangtu.top

Go:   "第一行\n第二行"
来源：http://cmh.chenzaomai.com

Ruby: "第一行\n第二行"
来源：http://dwu.haohaochexian.top

C#:   "第一行\n第二行"
来源：http://pba.aibaodan.cn

[A14] 注释写法
来源：http://gez.dianchejie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gyi.ydzc1.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pkq.shangyingyoupin.top

JS:   // 单行；/* 多行 */
来源：http://dmq.smart0.xyz

TS:   // 单行；/* 多行 */
来源：http://nnw.hywenlv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gcm.mhx1999.top

Go:   // 单行；/* 多行 */
来源：http://gbd.svipenyu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cad.zhengqikj.top

C#:   // 单行；/* 多行 */
来源：http://fbv.birdmap.top

[A15] 空值判断与默认值
来源：http://uyb.yuxming.cn

Py:   value = data or "默认值"
来源：http://lgg.ctjpmb.com

PHP:  $value = $data ?? "默认值";
来源：http://wvv.redwolf501.top

JS:   const value = data ?? "默认值";
来源：http://uhp.zhengqikj.top

TS:   const value = data ?? "默认值";
来源：http://dxj.meibo888.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bnn.birdmap.top

Go:   if data == "" { data = "默认值" }
来源：http://iou.sufxvd.cn

Ruby: value = data || "默认值"
来源：http://knv.ybcxt.top

C#:   var value = data ?? "默认值";
来源：http://rjg.ybcxt.top

[A16] 真假值判断规则
来源：http://hat.aibaodan.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xwi.yuanzhike.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xxy.jinyuanbaomall.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://spj.hongshengwenyu.top

TS:   if (!x) {}
来源：http://aeq.ybcxt.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ubp.52xcode.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zli.hnqzz.top

Ruby: unless x            # nil 与 false 为假
来源：http://blj.zdqjudy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ntq.yj202588.top

[A17] 位运算
来源：http://opo.nanxuanxn.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cca.zhiwuduotai.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vrv.mhx1999.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cqb.9152youxi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qbm.yueranfly.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rri.jqgufenzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://igs.feifeiyinyue.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qlk.fktsv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ntz.iojbl.cn

[A18] 字符与 ASCII 码互转
来源：http://qfd.pycfn.com

Py:   ord("A"); chr(65)
来源：http://jwx.jinghuilouyu.cn

PHP:  ord("A"); chr(65)
来源：http://odo.cqqwz.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://klq.pycfn.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ned.hnqzz.top

Java: (int) 'A'; (char) 65
来源：http://zct.hesvh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hsg.bjfxy.top

Ruby: "A".ord; 65.chr
来源：http://jvp.yangfankeji.com

C#:   (int)'A'; (char)65
来源：http://avu.jiagoushi.top

[A19] 交换两个变量
来源：http://qrj.jinqigfzy.top

Py:   a, b = b, a
来源：http://nww.epnwcf.com

PHP:  [$a, $b] = [$b, $a];
来源：http://snu.shangyingyoupin.top

JS:   [a, b] = [b, a];
来源：http://yeq.shanyushiyangtech.top

TS:   [a, b] = [b, a];
来源：http://epa.ybcxt.top

Java: int t = a; a = b; b = t;
来源：http://myy.vqdsnc.cn

Go:   a, b = b, a
来源：http://ucg.dianchejie.cn

Ruby: a, b = b, a
来源：http://cmo.redwolf501.top

C#:   (a, b) = (b, a);
来源：http://rjd.jinqigufen.top

[A20] 读取标准输入
来源：http://olj.yj202588.top

Py:   name = input("请输入：")
来源：http://vjl.fanxiaobao.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://iqy.pengpengdd.cyou

JS:   // Node.js：readline 模块或 process.stdin
来源：http://awo.ybcxt.top

TS:   // Node.js：readline 模块
来源：http://mdi.gogol.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://ffg.xylfe.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wju.tianlin.xyz

Ruby: gets.chomp
来源：http://ekz.cdnleiting.top

C#:   Console.ReadLine();
来源：http://ppv.zdbjq.cn

[A21] 保留指定小数位输出
来源：http://waz.gotoacloud.top

Py:   f"{3.14159:.2f}"
来源：http://cug.nwbrower.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pzd.ydzc1.top

JS:   (3.14159).toFixed(2)
来源：http://mas.uphjek.com

TS:   (3.14159).toFixed(2)
来源：http://qlf.jianghu66.top

Java: String.format("%.2f", 3.14159)
来源：http://vys.sxryk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wwp.xinyue.icu

Ruby: format("%.2f", 3.14159)
来源：http://snu.zhengqikj.top

C#:   3.14159.ToString("F2")
来源：http://jvw.xylfe.cn

[A22] 获取字符串长度
来源：http://xrr.zhiwuduotai.top

Py:   len(s)
来源：http://jsm.ywan-chungtsiang.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xvh.yfazqb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xcg.redwolf501.top

TS:   s.length
来源：http://qcf.zhongyouzk.top

Java: s.length()
来源：http://ycl.hysaishi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sxc.yueranfly.top

Ruby: s.length
来源：http://ydc.shuidangran.top

C#:   s.Length
来源：http://wzf.gogol.net.cn

[A23] 大小写转换
来源：http://kvh.c1oappe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://yfh.sufxvd.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zrj.wangshuangyany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xbl.ydzc1.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://anq.cqqwz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mhv.wangdashe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jmb.zdqjudy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ijj.gaohongyu789.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nqi.zdqjudy.top

[A24] 去除首尾空白
来源：http://ure.yangfankeji.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ohy.uphjek.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ehz.zhaomingkeji.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gdy.9152youxi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nyb.c1oappe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dbs.vehdjk.com

Go:   strings.TrimSpace(s)
来源：http://jvq.dianchejie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zur.sysykeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dtb.jinqigfzy.top

[A25] 字符串比较
来源：http://xie.tanke756.top

Py:   s1 == s2; s1 != s2
来源：http://cxy.quarkkingdee.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xzw.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hwx.zhixingplan.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xfv.hnxiangtu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bex.kuanghao11.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qfo.daxiang520.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jho.9152youxi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cly.nanxinkj.top

[A26] 类型转换总览
来源：http://aru.ivvv.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lon.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ccn.svipenyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://unk.zhoulong.xyz

TS:   Number() String() Boolean() x as number
来源：http://cvp.pycfn.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mpf.nanxuanxn.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bjx.redwolf501.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://thh.shanyushiyangkeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ydq.gogol.net.cn

================================================================================
来源：http://kyu.zdqjudy.top

B. 流程控制
来源：http://zob.redwolf501.top

================================================================================
来源：http://dqr.zhixingplan.top

[B01] 条件判断 if / else
来源：http://njn.zhiwuduotai.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zbk.fktsv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://flf.jiagoushi.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bri.quarkkingdee.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kxn.sjlbkw.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rbp.ybcxt.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cfg.yueranfly.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://imz.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mro.cdnleiting.top

[B02] 多分支 else if / elif
来源：http://kuw.shanyushiyangtech.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ucx.shanyushiyangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mem.hnqzz.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ifq.haohaochexian.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rrp.snrcjt.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xri.yuanzhike.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xro.wangshuangyany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://szp.jinqigufen.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xnv.chenlongwang.top

[B03] switch / match / case
来源：http://ikw.hfpthk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qto.nwbrower.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qjx.smart0.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ubi.yangfankeji.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://twp.meibo888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yqq.sufxvd.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mlb.zhoulong.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lzz.hcnkem.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ias.shzxlz.cn

[B04] for 计数循环
来源：http://ddf.fanxiaobao.xyz

Py:   for i in range(10): print(i)
来源：http://ipm.daria6918.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tmf.ydzc1.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bbh.dianchejie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nxv.aizwys.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://npn.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oer.jianghu66.top

Ruby: 10.times { |i| puts i }
来源：http://uhp.hcnkem.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dzb.nanxuanxn.top

[B05] 遍历数组 / 列表
来源：http://pgj.sufxvd.cn

Py:   for item in arr: print(item)
来源：http://yoq.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yyx.nanxinkj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dbq.kuanghao11.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ioe.nanxinkj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uvr.svipenyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mzd.316326.xyz

Ruby: arr.each { |item| puts item }
来源：http://bmy.jinqigufen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rag.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://yiw.mhx1999.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uee.xuanzx.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qaz.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ouj.gotoacloud.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gie.ywan-chungtsiang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wrq.pengpengdd.cyou

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zbj.mhx1999.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://usn.fehbvm.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jcj.guannengcc.top

[B07] while 循环
来源：http://ugr.nwbrower.top

Py:   while i < 10: i += 1
来源：http://mzt.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://psx.chenlongwang.top

JS:   while (i < 10) { i++; }
来源：http://gvr.zhixingplan.top

TS:   while (i < 10) { i++; }
来源：http://chx.epnwcf.com

Java: while (i < 10) { i++; }
来源：http://xer.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ejs.gaohongyu789.top

Ruby: while i < 10; i += 1; end
来源：http://jdt.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://zqa.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://zsf.yuxming.cn

Py:   # 无 do-while：用 while True + break
来源：http://ylv.hcnkem.com

PHP:  do { $i++; } while ($i < 10);
来源：http://pcg.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://lnp.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://nyd.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://czm.hywenlv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wel.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://cnx.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://nfi.gogol.net.cn

[B09] break 与 continue
来源：http://bxi.ydjk.org.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vse.cashguo.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hdn.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bzg.sxryk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nxv.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qvc.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ocm.chenjidiqi.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uuz.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aht.gzhubu.top

[B10] 遍历同时拿索引
来源：http://cre.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rmm.cqqwz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://idp.tarul.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nbn.sufxvd.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qwl.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rgg.feifeiyinyue.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fze.xuetiantiany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ent.tarul.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zxx.gogol.net.cn

[B11] 生成数字序列 / 区间
来源：http://adn.uphjek.com

Py:   list(range(0, 10, 2))
来源：http://hjy.sufxvd.cn

PHP:  range(0, 10, 2);
来源：http://oxp.shanyushiyangtech.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://scm.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yuq.ppjwa.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eip.0kj1m.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bak.fehbvm.com

Ruby: (0...10).step(2).to_a
来源：http://cuh.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ulk.zhengqikj.top

[B12] 跳出多层循环
来源：http://maf.sjlbkw.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ukd.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://zab.c1oappe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://puu.bjfxy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hvm.ctjpmb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fdq.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yxl.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pcm.jinqigfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kcj.jqgufenzy.top

[B13] 判断是否为数字
来源：http://pow.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://vub.jianghu66.top

PHP:  is_numeric($x)
来源：http://zjw.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zvo.hesvh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pek.ctjpmb.com

Java: x instanceof Number
来源：http://pac.bbcook.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gvl.nanxinkj.top

Ruby: x.is_a?(Numeric)
来源：http://rut.mhx1999.top

C#:   x is int or double or decimal
来源：http://otd.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://lwg.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://men.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xnu.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://goe.sxryk.cn

TS:   [1, 2, 3].includes(x)
来源：http://zrc.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://aht.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ije.redwolf501.top

Ruby: [1, 2, 3].include?(x)
来源：http://rmm.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://luj.yueranfly.top

[B15] 布尔运算与取反
来源：http://hqp.hfpthk.cn

Py:   a and b or not c
来源：http://ksr.shuidangran.top

PHP:  $a && $b || !$c
来源：http://pnl.sufxvd.cn

JS:   a && b || !c
来源：http://any.gzhubu.top

TS:   a && b || !c
来源：http://fzf.meibo888.top

Java: a && b || !c
来源：http://lic.jiagoushi.top


<!-- 参考信息 -->