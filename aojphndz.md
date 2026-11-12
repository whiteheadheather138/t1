代发 wailian999

[A06] 字符串转数字
来源：http://vlj.mhx1999.top

Py:   int("42"); float("3.14")
来源：http://shm.zdbjq.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mzq.fzhhl.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ymk.hysaishi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ugx.shzxlz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pcg.yfazqb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gvy.bbcook.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ukt.yvedp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ezf.daria6918.cn

[A07] 数字转字符串
来源：http://mwa.gogol.net.cn

Py:   str(42)
来源：http://rap.ctjpmb.com

PHP:  (string) 42; strval(42)
来源：http://hnq.nwbrower.top

JS:   String(42); (42).toString()
来源：http://wtu.mhx1999.top

TS:   String(42)
来源：http://ehr.gogol.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bmq.yongpay.top

Go:   strconv.Itoa(42)
来源：http://sth.yvedp.cn

Ruby: 42.to_s
来源：http://cas.ppjwa.cn

C#:   42.ToString()
来源：http://dkq.jiagoushi.top

[A08] 取整与四舍五入
来源：http://qoi.bjfxy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tdt.gzhubu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wbz.chenzaomai.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jfc.yj20258888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qmg.birdmap.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tfs.zdqjudy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://viz.aibaodan.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://efc.aizwys.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bdp.hnqzz.top

[A09] 绝对值与最大最小值
来源：http://nlb.fzhhl.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sjw.bjfxy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xxx.yueranfly.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://soq.dashuyun.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yvo.hnxiangtu.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mqq.ydjk.org.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jmt.shanyushiyangtech.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wua.jinghuilouyu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wpo.chenjidiqi.icu

[A10] 生成随机数
来源：http://gkw.sysykeji.top

Py:   import random; random.randint(1, 100)
来源：http://xix.shzxlz.cn

PHP:  random_int(1, 100);
来源：http://hes.jinghuilouyu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qnf.wangdashe.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sfy.feifeiyinyue.top

Java: new Random().nextInt(100) + 1
来源：http://kpf.ydjk.org.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cas.zdbjq.cn

Ruby: rand(1..100)
来源：http://kxd.shangyingyoupin.top

C#:   new Random().Next(1, 101)
来源：http://dwq.hysaishi.cn

[A11] 条件表达式（三元）
来源：http://xwl.sufxvd.cn

Py:   "yes" if x > 0 else "no"
来源：http://scu.hysaishi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://etb.gzhubu.top

JS:   x > 0 ? "yes" : "no"
来源：http://idv.meibo888.top

TS:   x > 0 ? "yes" : "no"
来源：http://axx.yj20258.top

Java: x > 0 ? "yes" : "no"
来源：http://ynb.yvedp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bnp.hnxiangtu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ttc.xinyue.icu

C#:   x > 0 ? "yes" : "no"
来源：http://szg.fehbvm.com

[A12] 字符串插值 / 格式化
来源：http://crw.redwolf501.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fja.jqgufenzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jib.chenjidiqi.icu

JS:   `Hello, ${name}!`
来源：http://ipf.sweek.top

TS:   `Hello, ${name}!`
来源：http://pgw.hesvh.cn

Java: "Hello, %s!".formatted(name)
来源：http://vzb.hnxiangtu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://waz.quarkkingdee.top

Ruby: "Hello, #{name}!"
来源：http://xio.sweek.top

C#:   $"Hello, {name}!"
来源：http://jyp.yj20258888.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ihl.ppjwa.cn

Py:   "第一行\n第二行"
来源：http://ooq.pengpengdd.cyou

PHP:  "第一行\n第二行"
来源：http://tza.fengsongda.top

JS:   "第一行\n第二行"
来源：http://miq.pycfn.com

TS:   "第一行\n第二行"
来源：http://xzs.yueranfly.top

Java: "第一行\n第二行"
来源：http://pbm.smart0.xyz

Go:   "第一行\n第二行"
来源：http://wri.pycfn.com

Ruby: "第一行\n第二行"
来源：http://yvs.yongpay.top

C#:   "第一行\n第二行"
来源：http://ibu.9152youxi.cn

[A14] 注释写法
来源：http://ijw.nwbrower.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://lre.gotoacloud.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rup.quarkkingdee.top

JS:   // 单行；/* 多行 */
来源：http://qkd.jqgufenzy.top

TS:   // 单行；/* 多行 */
来源：http://xcf.gzhubu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ttv.mhx1999.top

Go:   // 单行；/* 多行 */
来源：http://lrm.sxryk.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ylf.xuanzx.com

C#:   // 单行；/* 多行 */
来源：http://tfw.shzxlz.cn

[A15] 空值判断与默认值
来源：http://cdx.shangyingyoupin.top

Py:   value = data or "默认值"
来源：http://rks.xziqi.cn

PHP:  $value = $data ?? "默认值";
来源：http://bar.gogol.net.cn

JS:   const value = data ?? "默认值";
来源：http://qhj.hongshengwenyu.top

TS:   const value = data ?? "默认值";
来源：http://jtz.quarkkingdee.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cqi.guowangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://juf.bbcook.cn

Ruby: value = data || "默认值"
来源：http://scc.iojbl.cn

C#:   var value = data ?? "默认值";
来源：http://stb.ybcxt.top

[A16] 真假值判断规则
来源：http://eak.yj20258.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jns.0kj1m.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wqz.hammf.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gvq.cashguo.top

TS:   if (!x) {}
来源：http://hrg.sysykeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xaa.ybcxt.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jsq.kuanghao11.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cyw.snrcjt.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xmu.yongpay.top

[A17] 位运算
来源：http://mtp.fanxiaobao.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://krk.jqgufenzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wct.sxryk.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://act.cheryme.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pla.bbcook.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kug.epnwcf.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ovx.xuanzx.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ubt.guowangkeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xen.ydzc1.top

[A18] 字符与 ASCII 码互转
来源：http://nvt.316326.xyz

Py:   ord("A"); chr(65)
来源：http://ncc.hnxiangtu.top

PHP:  ord("A"); chr(65)
来源：http://iuw.kuanghao11.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bxd.0kj1m.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://etp.epnwcf.com

Java: (int) 'A'; (char) 65
来源：http://dbb.haohaochexian.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://led.andypj.xyz

Ruby: "A".ord; 65.chr
来源：http://gcs.jqgfzy.top

C#:   (int)'A'; (char)65
来源：http://zlk.fanxiaobao.xyz

[A19] 交换两个变量
来源：http://ldj.yueranfly.top

Py:   a, b = b, a
来源：http://leo.c1oappe.top

PHP:  [$a, $b] = [$b, $a];
来源：http://cgo.fehbvm.com

JS:   [a, b] = [b, a];
来源：http://chj.yongpay.top

TS:   [a, b] = [b, a];
来源：http://ppb.hysaishi.cn

Java: int t = a; a = b; b = t;
来源：http://axi.andypj.xyz

Go:   a, b = b, a
来源：http://hlj.jinqigfzy.top

Ruby: a, b = b, a
来源：http://zlf.vehdjk.com

C#:   (a, b) = (b, a);
来源：http://lku.svipenyu.cn

[A20] 读取标准输入
来源：http://tcm.dianchejie.cn

Py:   name = input("请输入：")
来源：http://kzw.shuidangran.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rif.vqdsnc.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xnp.fengsongda.top

TS:   // Node.js：readline 模块
来源：http://zmp.tian-w.cn

Java: new Scanner(System.in).nextLine()
来源：http://vpf.hfpthk.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://djd.hfpthk.cn

Ruby: gets.chomp
来源：http://wkv.shzxlz.cn

C#:   Console.ReadLine();
来源：http://tqb.birdmap.top

[A21] 保留指定小数位输出
来源：http://rfo.shanyushiyangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://alc.xuetiantiany.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zuq.hfpthk.cn

JS:   (3.14159).toFixed(2)
来源：http://wma.vqdsnc.cn

TS:   (3.14159).toFixed(2)
来源：http://dkj.52xcode.cn

Java: String.format("%.2f", 3.14159)
来源：http://isz.zhixingplan.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mdn.guannengcc.top

Ruby: format("%.2f", 3.14159)
来源：http://uzm.zhaomingkeji.xyz

C#:   3.14159.ToString("F2")
来源：http://rit.hywenlv.cn

[A22] 获取字符串长度
来源：http://voz.cucudq.cn

Py:   len(s)
来源：http://dcn.xuetiantiany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://woe.yanxiufei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fzf.pengpengdd.cyou

TS:   s.length
来源：http://tcy.52xcode.cn

Java: s.length()
来源：http://sxm.iojbl.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://val.hnqzz.top

Ruby: s.length
来源：http://gvl.hysaishi.cn

C#:   s.Length
来源：http://gyo.hnqzz.top

[A23] 大小写转换
来源：http://ubk.svipenyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uor.hongshengwenyu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kij.haohaochexian.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ztq.cheryme.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vms.uphjek.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pxe.jqgufenzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jzr.hnqzz.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://txf.zhiwuduotai.top

C#:   s.ToUpper(); s.ToLower()
来源：http://wkh.yj20258888.top

[A24] 去除首尾空白
来源：http://nym.shanyushiyangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gnx.aizwys.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fdw.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sph.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://erm.svipenyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ifk.0kj1m.cn

Go:   strings.TrimSpace(s)
来源：http://fiu.9152youxi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ilq.xylfe.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jua.hysaishi.cn

[A25] 字符串比较
来源：http://ohj.yangfankeji.com

Py:   s1 == s2; s1 != s2
来源：http://oxd.ehwqpu.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ras.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tjv.cdnleiting.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iao.ctjpmb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pmt.feifeiyinyue.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://awl.yvedp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tdn.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qbh.uphjek.com

[A26] 类型转换总览
来源：http://pzj.quarkkingdee.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://aep.yongpay.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://efn.cucudq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dyp.haohaochexian.top

TS:   Number() String() Boolean() x as number
来源：http://kfv.c1oappe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://unl.jlsjyb.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://biw.hywenlv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nie.316326.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ann.xingfuxueyuan.xyz

================================================================================
来源：http://zsy.yvedp.cn

B. 流程控制
来源：http://led.daxiang520.top

================================================================================
来源：http://ogn.tarul.cn

[B01] 条件判断 if / else
来源：http://vnv.zhongyouzk.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jmi.shangyingyoupin.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mxt.aibaodan.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tve.ppjwa.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tgj.jiagoushi.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jeb.chenlongwang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rdh.guannengcc.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://efy.pycfn.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cln.vqdsnc.cn

[B02] 多分支 else if / elif
来源：http://tvs.aibaodan.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rbi.chenzaomai.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rhs.zhoulong.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sas.cashguo.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dbh.tianlin.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hvc.nanxuanxn.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dhy.hysaishi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uzc.pycfn.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://npm.tarul.cn

[B03] switch / match / case
来源：http://ywm.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://act.jyoumei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ldg.iojbl.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gkr.mhx1999.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://trn.yanxiufei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kid.zdqjudy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iys.kuanghao11.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ypg.yj20258888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tbo.jqgfzy.top

[B04] for 计数循环
来源：http://bmp.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://ogm.daxiang520.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kne.guannengcc.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://neq.cheryme.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jvv.xingfuxueyuan.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://set.iojbl.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hak.jqgfzy.top

Ruby: 10.times { |i| puts i }
来源：http://pph.andypj.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mkr.xuetiantiany.cn

[B05] 遍历数组 / 列表
来源：http://wua.hysaishi.cn

Py:   for item in arr: print(item)
来源：http://tkd.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tno.nanxinkj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ioa.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zaj.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qzc.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cro.redwolf501.top

Ruby: arr.each { |item| puts item }
来源：http://vlk.pengpengdd.cyou

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vlh.dianchejie.cn

[B06] 遍历字典 / 对象
来源：http://zim.c1oappe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mrp.xinyue.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://drj.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tsu.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bxy.tanke756.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lsk.zhaomingkeji.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bzk.guowangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://obw.hfpthk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zvl.birdmap.top

[B07] while 循环
来源：http://wxu.iojbl.cn

Py:   while i < 10: i += 1
来源：http://fuv.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rml.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://vqt.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://hgn.jinqigfzy.top

Java: while (i < 10) { i++; }
来源：http://tsl.hcnkem.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iyj.epnwcf.com

Ruby: while i < 10; i += 1; end
来源：http://vsx.sysykeji.top

C#:   while (i < 10) { i++; }
来源：http://xpr.ywan-chungtsiang.top

[B08] do-while（至少执行一次）
来源：http://zpk.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://tjk.yvedp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://znj.fktsv.cn

JS:   do { i++; } while (i < 10);
来源：http://qug.tanke756.top

TS:   do { i++; } while (i < 10);
来源：http://kwi.uphjek.com

Java: do { i++; } while (i < 10);
来源：http://ant.fktsv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://djl.smart0.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://rqd.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://wum.chenlongwang.top

[B09] break 与 continue
来源：http://vjk.zdbjq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dnb.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://miw.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://res.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://daa.xuetiantiany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ebk.yuxming.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nwz.hnqzz.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qys.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnh.yongpay.top

[B10] 遍历同时拿索引
来源：http://cqu.sxryk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ped.nwbrower.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ela.jinqigufen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rst.jqgufenzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hlt.svipenyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://irl.redwolf501.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hzq.52xcode.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://upl.gzhubu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wsz.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://pow.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://wdb.zhengqikj.top

PHP:  range(0, 10, 2);
来源：http://oye.316326.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yvk.0kj1m.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lok.fehbvm.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hal.nwbrower.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jss.hcnkem.com

Ruby: (0...10).step(2).to_a
来源：http://gnc.xinyue.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zzy.meibo888.top

[B12] 跳出多层循环
来源：http://lck.jianghu66.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://aca.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://oun.iojbl.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wds.zhoulong.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fui.hesvh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tzn.vehdjk.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uwo.aibaodan.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ucy.sufxvd.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mdz.hysaishi.cn


<!-- 参考信息 -->