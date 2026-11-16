代发 wailian999

[A06] 字符串转数字
来源：http://kbh.xziqi.cn

Py:   int("42"); float("3.14")
来源：http://cpm.ctjpmb.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kqg.pengpengdd.cyou

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bof.jyoumei.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lfm.jinyuanbaomall.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tsx.kuanghao11.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hlo.aibaodan.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wkc.wangshuangyany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://asw.zdbjq.cn

[A07] 数字转字符串
来源：http://uwd.shanyushiyangkeji.top

Py:   str(42)
来源：http://bwu.shanyushiyangkeji.top

PHP:  (string) 42; strval(42)
来源：http://nry.fanxiaobao.xyz

JS:   String(42); (42).toString()
来源：http://rzx.hywenlv.cn

TS:   String(42)
来源：http://hnw.ydjk.org.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://avf.chenjidiqi.icu

Go:   strconv.Itoa(42)
来源：http://ott.birdmap.top

Ruby: 42.to_s
来源：http://myj.yueranfly.top

C#:   42.ToString()
来源：http://nzo.cqqwz.cn

[A08] 取整与四舍五入
来源：http://vqu.nanxuanxn.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://iau.kuanghao11.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vai.hfpthk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cyf.guannengcc.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bab.ydjk.org.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kwa.sufxvd.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cut.mhx1999.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xvn.xuanzx.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://snt.chenlongwang.top

[A09] 绝对值与最大最小值
来源：http://hzk.daxiang520.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pfl.xingfuxueyuan.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ynj.kuanghao11.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://clv.yj202588.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ckx.pengpengdd.cyou

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sdp.tianlin.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eqs.xingfuxueyuan.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fwb.meibo888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ytb.zdbjq.cn

[A10] 生成随机数
来源：http://uix.cdnleiting.top

Py:   import random; random.randint(1, 100)
来源：http://pmm.cheryme.top

PHP:  random_int(1, 100);
来源：http://egu.shzxlz.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qii.guannengcc.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://igw.zycfv.cn

Java: new Random().nextInt(100) + 1
来源：http://rua.quarkkingdee.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xuv.ydzc1.top

Ruby: rand(1..100)
来源：http://wjq.xuetiantiany.cn

C#:   new Random().Next(1, 101)
来源：http://adi.shanyushiyangtech.top

[A11] 条件表达式（三元）
来源：http://rmi.zhiwuduotai.top

Py:   "yes" if x > 0 else "no"
来源：http://zjh.hesvh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://azh.tarul.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zsz.tanke756.top

TS:   x > 0 ? "yes" : "no"
来源：http://cef.xingfuxueyuan.xyz

Java: x > 0 ? "yes" : "no"
来源：http://poi.cdnleiting.top

Go:   // 无三元运算符，需用 if 语句
来源：http://npu.hfpthk.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://aak.fzhhl.top

C#:   x > 0 ? "yes" : "no"
来源：http://nvp.tarul.cn

[A12] 字符串插值 / 格式化
来源：http://gko.yonumen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://buz.xuetiantiany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tfu.dianchejie.cn

JS:   `Hello, ${name}!`
来源：http://jmm.wangdashe.top

TS:   `Hello, ${name}!`
来源：http://vkd.zhijiandao.cn

Java: "Hello, %s!".formatted(name)
来源：http://mcb.kuanghao11.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bir.ywan-chungtsiang.top

Ruby: "Hello, #{name}!"
来源：http://phc.fktsv.cn

C#:   $"Hello, {name}!"
来源：http://vfr.xziqi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://eof.yuxming.cn

Py:   "第一行\n第二行"
来源：http://eom.mhx1999.top

PHP:  "第一行\n第二行"
来源：http://dhj.fengsongda.top

JS:   "第一行\n第二行"
来源：http://mux.tian-w.cn

TS:   "第一行\n第二行"
来源：http://lgp.ydzc1.top

Java: "第一行\n第二行"
来源：http://ifv.daxiang520.top

Go:   "第一行\n第二行"
来源：http://uof.epnwcf.com

Ruby: "第一行\n第二行"
来源：http://ntz.shzxlz.cn

C#:   "第一行\n第二行"
来源：http://efp.hysaishi.cn

[A14] 注释写法
来源：http://sca.yuxming.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lpj.cashguo.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://afn.wangshuangyany.cn

JS:   // 单行；/* 多行 */
来源：http://waz.xuetiantiany.cn

TS:   // 单行；/* 多行 */
来源：http://nzy.jinghuilouyu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://izh.xinyue.icu

Go:   // 单行；/* 多行 */
来源：http://byn.fktsv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qtr.sxryk.cn

C#:   // 单行；/* 多行 */
来源：http://cek.yonumen.top

[A15] 空值判断与默认值
来源：http://iax.snrcjt.cn

Py:   value = data or "默认值"
来源：http://mis.zhijiandao.cn

PHP:  $value = $data ?? "默认值";
来源：http://puk.mhx1999.top

JS:   const value = data ?? "默认值";
来源：http://idw.tian-w.cn

TS:   const value = data ?? "默认值";
来源：http://asx.fzhhl.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ieq.ydjk.org.cn

Go:   if data == "" { data = "默认值" }
来源：http://imn.zhijiandao.cn

Ruby: value = data || "默认值"
来源：http://lgk.shuidangran.top

C#:   var value = data ?? "默认值";
来源：http://eqd.gzhubu.top

[A16] 真假值判断规则
来源：http://acc.gaohongyu789.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vpk.fengsongda.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jkt.cashguo.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://omp.wangshuangyany.cn

TS:   if (!x) {}
来源：http://klw.ppjwa.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pws.fzhhl.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vxa.shzxlz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uzb.shzxlz.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gep.gzhubu.top

[A17] 位运算
来源：http://ohg.pycfn.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xta.ctjpmb.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qsz.feifeiyinyue.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rqh.zhixingplan.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://apk.ydjk.org.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gad.zhaomingkeji.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cjs.cheryme.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yzm.sysykeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://svs.0kj1m.cn

[A18] 字符与 ASCII 码互转
来源：http://lhw.nanxinkj.top

Py:   ord("A"); chr(65)
来源：http://nmr.jqgfzy.top

PHP:  ord("A"); chr(65)
来源：http://nun.svipenyu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lfc.ppjwa.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hjj.yuanzhike.top

Java: (int) 'A'; (char) 65
来源：http://jti.shangyingyoupin.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://eep.svipenyu.cn

Ruby: "A".ord; 65.chr
来源：http://ydw.cucudq.cn

C#:   (int)'A'; (char)65
来源：http://ocz.52xcode.cn

[A19] 交换两个变量
来源：http://yyc.bjfxy.top

Py:   a, b = b, a
来源：http://htx.zdqjudy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://rie.9152youxi.cn

JS:   [a, b] = [b, a];
来源：http://hcf.fanxiaobao.xyz

TS:   [a, b] = [b, a];
来源：http://mst.shangyingyoupin.top

Java: int t = a; a = b; b = t;
来源：http://ces.zhixingplan.top

Go:   a, b = b, a
来源：http://oyk.iojbl.cn

Ruby: a, b = b, a
来源：http://nxb.jinghuilouyu.cn

C#:   (a, b) = (b, a);
来源：http://zmv.gotoacloud.top

[A20] 读取标准输入
来源：http://gud.ppjwa.cn

Py:   name = input("请输入：")
来源：http://qad.c1oappe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://nfy.daxiang520.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qzr.jinqigfzy.top

TS:   // Node.js：readline 模块
来源：http://dhr.bbcook.cn

Java: new Scanner(System.in).nextLine()
来源：http://kmz.cdnleiting.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zdd.chenjidiqi.icu

Ruby: gets.chomp
来源：http://ndy.chenlongwang.top

C#:   Console.ReadLine();
来源：http://gpm.aibaodan.cn

[A21] 保留指定小数位输出
来源：http://cye.shanyushiyangtech.top

Py:   f"{3.14159:.2f}"
来源：http://oyb.gaohongyu789.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zaq.shuidangran.top

JS:   (3.14159).toFixed(2)
来源：http://och.tianlin.xyz

TS:   (3.14159).toFixed(2)
来源：http://pmp.9152youxi.cn

Java: String.format("%.2f", 3.14159)
来源：http://ocb.jinqigfzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tbg.yj20258888.top

Ruby: format("%.2f", 3.14159)
来源：http://spl.gaohongyu789.top

C#:   3.14159.ToString("F2")
来源：http://rsj.nanxinkj.top

[A22] 获取字符串长度
来源：http://qky.ivvv.top

Py:   len(s)
来源：http://szq.chenzaomai.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gvg.zhongyouzk.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wzf.zhiwuduotai.top

TS:   s.length
来源：http://wul.ybcxt.top

Java: s.length()
来源：http://vcv.yanxiufei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ssu.zhoulong.xyz

Ruby: s.length
来源：http://gpp.ybcxt.top

C#:   s.Length
来源：http://zhl.cucudq.cn

[A23] 大小写转换
来源：http://vke.guowangkeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vtg.fengsongda.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://onr.zdbjq.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zsr.xuanzx.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://der.tianlin.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cvd.fehbvm.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ujh.cheryme.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://doi.daxiang520.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gzn.fzhhl.top

[A24] 去除首尾空白
来源：http://ypw.xuanzx.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ypu.nanxinkj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vor.jqgfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uzy.sweek.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jla.birdmap.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://onk.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://ego.yanxiufei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mrz.gaohongyu789.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://feb.bbcook.cn

[A25] 字符串比较
来源：http://yqc.xuanzx.com

Py:   s1 == s2; s1 != s2
来源：http://eqp.yuxming.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hla.hnxiangtu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qgo.xingfuxueyuan.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tvv.zhijiandao.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nov.sufxvd.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://viq.cqqwz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oxp.hcnkem.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rtt.ppjwa.cn

[A26] 类型转换总览
来源：http://rhu.shzxlz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qcr.hcnkem.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wkk.ydzc1.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kau.mhx1999.top

TS:   Number() String() Boolean() x as number
来源：http://uvk.52xcode.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://osd.hongshengwenyu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lrm.yuanzhike.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fch.ydjk.org.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wil.pycfn.com

================================================================================
来源：http://hny.cucudq.cn

B. 流程控制
来源：http://nco.shuidangran.top

================================================================================
来源：http://tkl.svipenyu.cn

[B01] 条件判断 if / else
来源：http://opg.birdmap.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qkc.dianchejie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dpq.jianghu66.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ovp.gogol.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kom.dashuyun.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://weo.shangyingyoupin.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dln.jinqigfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dgx.zhengqikj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xac.zhengqikj.top

[B02] 多分支 else if / elif
来源：http://edv.bbcook.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hrq.fktsv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vvm.andypj.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://knj.iojbl.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qhm.52xcode.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xyq.zhengqikj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wcm.jlsjyb.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://amb.yuxming.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sck.cucudq.cn

[B03] switch / match / case
来源：http://xyx.cheryme.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sjh.epnwcf.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://szj.redwolf501.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cem.xuetiantiany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dlm.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rkf.guannengcc.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://awe.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cgs.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://twm.fengsongda.top

[B04] for 计数循环
来源：http://kim.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://kyp.daria6918.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qwr.ydzc1.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tef.cdnleiting.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zll.c1oappe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pdq.jqgufenzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mzk.epnwcf.com

Ruby: 10.times { |i| puts i }
来源：http://zww.hongshengwenyu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xdj.wangdashe.top

[B05] 遍历数组 / 列表
来源：http://kod.wangdashe.top

Py:   for item in arr: print(item)
来源：http://umu.snrcjt.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qiz.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hqn.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lmv.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ydx.jinqigufen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jbz.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://gys.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qou.haohaochexian.top

[B06] 遍历字典 / 对象
来源：http://axt.cheryme.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sef.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://php.nwbrower.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pra.havefunace.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xiu.xziqi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wgz.feifeiyinyue.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lzq.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yqx.zycfv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://evs.hcnkem.com

[B07] while 循环
来源：http://rnp.tianlin.xyz

Py:   while i < 10: i += 1
来源：http://gwq.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://aps.tanke756.top

JS:   while (i < 10) { i++; }
来源：http://ukl.yj202588.top

TS:   while (i < 10) { i++; }
来源：http://euy.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://zaf.svipenyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://voc.nanxinkj.top

Ruby: while i < 10; i += 1; end
来源：http://mhh.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://bhu.birdmap.top

[B08] do-while（至少执行一次）
来源：http://pjd.ivvv.top

Py:   # 无 do-while：用 while True + break
来源：http://dpo.gotoacloud.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rsv.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://fyz.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://oyd.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://rcg.jlsjyb.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://erh.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rct.fktsv.cn

C#:   do { i++; } while (i < 10);
来源：http://yzk.wangdashe.top

[B09] break 与 continue
来源：http://wcg.shanyushiyangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vmv.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ejt.dianchejie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jrb.xuanzx.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rxn.bjfxy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://psn.ybcxt.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cdr.meibo888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aeu.316326.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qwj.havefunace.top

[B10] 遍历同时拿索引
来源：http://woy.yueranfly.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qjy.hfpthk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bzt.gzhubu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://amd.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zza.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kdf.xylfe.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rpt.jinqigfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dck.bbcook.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vvv.quarkkingdee.top

[B11] 生成数字序列 / 区间
来源：http://cre.jyoumei.cn

Py:   list(range(0, 10, 2))
来源：http://esg.tianlin.xyz

PHP:  range(0, 10, 2);
来源：http://nrc.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wqn.ctjpmb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blw.yangfankeji.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lmu.jiagoushi.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yvd.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://xyv.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ffh.zhaomingkeji.xyz

[B12] 跳出多层循环
来源：http://usm.sufxvd.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pjq.jianghu66.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://amo.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zen.mhx1999.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vkc.mhx1999.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kjw.jyoumei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wwi.mhx1999.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://krx.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fvk.haohaochexian.top


<!-- 参考信息 -->