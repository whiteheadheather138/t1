代发 wailian999

[A06] 字符串转数字
来源：http://hqw.chenlongwang.top

Py:   int("42"); float("3.14")
来源：http://uch.zdqjudy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://smm.fanxiaobao.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://npm.haohaochexian.top

TS:   parseInt("42", 10); Number("42")
来源：http://fep.jyoumei.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zzs.hcnkem.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zua.gzhubu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://fwk.iojbl.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mim.xuetiantiany.cn

[A07] 数字转字符串
来源：http://wbr.guowangkeji.top

Py:   str(42)
来源：http://jns.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://kft.jqgfzy.top

JS:   String(42); (42).toString()
来源：http://pdj.fzhhl.top

TS:   String(42)
来源：http://kzr.jinqigfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://eyt.zhoulong.xyz

Go:   strconv.Itoa(42)
来源：http://hql.birdmap.top

Ruby: 42.to_s
来源：http://pqo.ybcxt.top

C#:   42.ToString()
来源：http://clp.gotoacloud.top

[A08] 取整与四舍五入
来源：http://gkt.yuxming.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jox.epnwcf.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zwc.hnqzz.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cro.ivvv.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zda.chenlongwang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hew.pengpengdd.cyou

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://axk.fengsongda.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://jbv.xuanzx.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tln.fanxiaobao.xyz

[A09] 绝对值与最大最小值
来源：http://zlh.ydzc1.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jha.tianlin.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sjz.chenlongwang.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kqe.ydzc1.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://obm.sufxvd.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bmh.zhoulong.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pgj.jqgfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://aep.jqgufenzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dlt.pycfn.com

[A10] 生成随机数
来源：http://khe.zhengqikj.top

Py:   import random; random.randint(1, 100)
来源：http://jlu.zdbjq.cn

PHP:  random_int(1, 100);
来源：http://jkc.shzxlz.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kii.shzxlz.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vfw.xziqi.cn

Java: new Random().nextInt(100) + 1
来源：http://xwn.sufxvd.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oqf.tianlin.xyz

Ruby: rand(1..100)
来源：http://axr.guannengcc.top

C#:   new Random().Next(1, 101)
来源：http://drk.jlsjyb.cn

[A11] 条件表达式（三元）
来源：http://dlk.xuetiantiany.cn

Py:   "yes" if x > 0 else "no"
来源：http://oyu.epnwcf.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://hdq.svipenyu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mpq.sjlbkw.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rem.pengpengdd.cyou

Java: x > 0 ? "yes" : "no"
来源：http://qiu.gaohongyu789.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pzr.uphjek.com

Ruby: x > 0 ? "yes" : "no"
来源：http://igc.fanxiaobao.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://esh.tianlin.xyz

[A12] 字符串插值 / 格式化
来源：http://tui.zhengqikj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kxj.xinyue.icu

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tzw.birdmap.top

JS:   `Hello, ${name}!`
来源：http://zem.vqdsnc.cn

TS:   `Hello, ${name}!`
来源：http://emh.nwbrower.top

Java: "Hello, %s!".formatted(name)
来源：http://aun.hongshengwenyu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ota.zhijiandao.cn

Ruby: "Hello, #{name}!"
来源：http://yyd.0kj1m.cn

C#:   $"Hello, {name}!"
来源：http://pjg.chenjidiqi.icu

[A13] 多行字符串（练习 \n 转义）
来源：http://hau.dashuyun.cn

Py:   "第一行\n第二行"
来源：http://cqf.hywenlv.cn

PHP:  "第一行\n第二行"
来源：http://wba.xziqi.cn

JS:   "第一行\n第二行"
来源：http://win.wangdashe.top

TS:   "第一行\n第二行"
来源：http://oqs.bbcook.cn

Java: "第一行\n第二行"
来源：http://lxs.kuanghao11.cn

Go:   "第一行\n第二行"
来源：http://fbp.sweek.top

Ruby: "第一行\n第二行"
来源：http://nyz.xuetiantiany.cn

C#:   "第一行\n第二行"
来源：http://saf.nwbrower.top

[A14] 注释写法
来源：http://lqe.hfpthk.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ycv.yj202588.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://sdk.iojbl.cn

JS:   // 单行；/* 多行 */
来源：http://dxt.gotoacloud.top

TS:   // 单行；/* 多行 */
来源：http://zqz.jqgufenzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zsc.uphjek.com

Go:   // 单行；/* 多行 */
来源：http://qyr.zdbjq.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fkv.ctjpmb.com

C#:   // 单行；/* 多行 */
来源：http://jrq.tarul.cn

[A15] 空值判断与默认值
来源：http://zpo.zhongyouzk.top

Py:   value = data or "默认值"
来源：http://svw.birdmap.top

PHP:  $value = $data ?? "默认值";
来源：http://ugp.tianlin.xyz

JS:   const value = data ?? "默认值";
来源：http://bnd.hongshengwenyu.top

TS:   const value = data ?? "默认值";
来源：http://rmi.52xcode.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uwv.chenjidiqi.icu

Go:   if data == "" { data = "默认值" }
来源：http://maz.shuidangran.top

Ruby: value = data || "默认值"
来源：http://zcj.0kj1m.cn

C#:   var value = data ?? "默认值";
来源：http://qqe.daxiang520.top

[A16] 真假值判断规则
来源：http://nly.shanyushiyangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://znm.dashuyun.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dgb.sweek.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gcw.gotoacloud.top

TS:   if (!x) {}
来源：http://bxk.xuanzx.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://msx.gogol.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xnh.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://rji.0kj1m.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uto.yj202588.top

[A17] 位运算
来源：http://jvo.hammf.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fqr.hysaishi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ict.ydjk.org.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ogj.ppjwa.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ijd.dashuyun.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tgd.fzhhl.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ltn.hfpthk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dhl.xziqi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fdd.gotoacloud.top

[A18] 字符与 ASCII 码互转
来源：http://bhq.fktsv.cn

Py:   ord("A"); chr(65)
来源：http://odk.vqdsnc.cn

PHP:  ord("A"); chr(65)
来源：http://rio.xziqi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://edb.jyoumei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mir.ivvv.top

Java: (int) 'A'; (char) 65
来源：http://tpv.cdnleiting.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dlz.9152youxi.cn

Ruby: "A".ord; 65.chr
来源：http://vnu.hnqzz.top

C#:   (int)'A'; (char)65
来源：http://qqj.yj20258888.top

[A19] 交换两个变量
来源：http://qbr.xziqi.cn

Py:   a, b = b, a
来源：http://ney.hcnkem.com

PHP:  [$a, $b] = [$b, $a];
来源：http://cyn.ehwqpu.com

JS:   [a, b] = [b, a];
来源：http://ffe.zdbjq.cn

TS:   [a, b] = [b, a];
来源：http://lkn.nwbrower.top

Java: int t = a; a = b; b = t;
来源：http://wnf.uphjek.com

Go:   a, b = b, a
来源：http://okf.hysaishi.cn

Ruby: a, b = b, a
来源：http://bvu.sjlbkw.cn

C#:   (a, b) = (b, a);
来源：http://zhw.yonumen.top

[A20] 读取标准输入
来源：http://dgb.chenjidiqi.icu

Py:   name = input("请输入：")
来源：http://eog.sjlbkw.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zyq.tian-w.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hgg.xinyue.icu

TS:   // Node.js：readline 模块
来源：http://jtl.yj20258888.top

Java: new Scanner(System.in).nextLine()
来源：http://nic.cqqwz.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zwm.yuanzhike.top

Ruby: gets.chomp
来源：http://uts.zhijiandao.cn

C#:   Console.ReadLine();
来源：http://axe.mhx1999.top

[A21] 保留指定小数位输出
来源：http://zbk.kuanghao11.cn

Py:   f"{3.14159:.2f}"
来源：http://gyq.xingfuxueyuan.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jdb.dianchejie.cn

JS:   (3.14159).toFixed(2)
来源：http://iqa.zhiwuduotai.top

TS:   (3.14159).toFixed(2)
来源：http://wkv.sjlbkw.cn

Java: String.format("%.2f", 3.14159)
来源：http://nap.jinqigfzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://swx.yuxming.cn

Ruby: format("%.2f", 3.14159)
来源：http://vxh.tian-w.cn

C#:   3.14159.ToString("F2")
来源：http://wrv.ywan-chungtsiang.top

[A22] 获取字符串长度
来源：http://pkz.ctjpmb.com

Py:   len(s)
来源：http://ozd.sufxvd.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hua.nwbrower.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xsw.ivvv.top

TS:   s.length
来源：http://mbf.yanxiufei.cn

Java: s.length()
来源：http://gxl.sufxvd.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://clr.yanxiufei.cn

Ruby: s.length
来源：http://cmd.wangdashe.top

C#:   s.Length
来源：http://jhx.sjlbkw.cn

[A23] 大小写转换
来源：http://oup.zycfv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zpn.xuanzx.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kgq.sysykeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rzr.gzhubu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fus.nwbrower.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://trz.bjfxy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ekc.yj20258.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zbt.tanke756.top

C#:   s.ToUpper(); s.ToLower()
来源：http://idf.xziqi.cn

[A24] 去除首尾空白
来源：http://tit.andypj.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://evk.sxryk.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qqr.mhx1999.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vvc.hfpthk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mvg.yanxiufei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rtu.0kj1m.cn

Go:   strings.TrimSpace(s)
来源：http://yjs.chenzaomai.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mcm.cqqwz.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://usm.guannengcc.top

[A25] 字符串比较
来源：http://lpq.nwbrower.top

Py:   s1 == s2; s1 != s2
来源：http://kua.zdqjudy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ksr.jinqigufen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tzq.yj20258.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hmo.nanxuanxn.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ceq.daria6918.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iwe.chenlongwang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qgo.zhiwuduotai.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kxm.nanxuanxn.top

[A26] 类型转换总览
来源：http://zlw.nwbrower.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qdr.ydjk.org.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yhh.hysaishi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pkj.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://frk.xuanzx.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eqc.hcnkem.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rzx.sufxvd.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mwe.0kj1m.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dox.jinqigufen.top

================================================================================
来源：http://ejh.jiagoushi.top

B. 流程控制
来源：http://hks.hesvh.cn

================================================================================
来源：http://fhg.jinyuanbaomall.cn

[B01] 条件判断 if / else
来源：http://vpe.316326.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://hfj.hammf.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vyg.redwolf501.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kii.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qcw.daria6918.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tvk.pycfn.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ual.xinyue.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ltt.sjlbkw.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wdi.feifeiyinyue.top

[B02] 多分支 else if / elif
来源：http://xxx.cheryme.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fhm.cdnleiting.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mhk.yanxiufei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iol.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ggq.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mdf.yanxiufei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://npd.yonumen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tey.fktsv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jwu.dianchejie.cn

[B03] switch / match / case
来源：http://wgi.hcnkem.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://liv.meibo888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://von.daxiang520.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dis.sjlbkw.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aqz.gaohongyu789.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://chm.yueranfly.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nwk.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rzy.bbcook.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vwy.shangyingyoupin.top

[B04] for 计数循环
来源：http://yrb.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://eab.hesvh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mix.guowangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lxa.cheryme.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dvw.hnxiangtu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xhd.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gkx.cdnleiting.top

Ruby: 10.times { |i| puts i }
来源：http://vuj.shzxlz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ykx.wangdashe.top

[B05] 遍历数组 / 列表
来源：http://vks.nwbrower.top

Py:   for item in arr: print(item)
来源：http://qjl.zhoulong.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ggq.haohaochexian.top

JS:   for (const item of arr) { console.log(item); }
来源：http://pug.aibaodan.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gww.daxiang520.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://maj.zhongyouzk.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iiv.daria6918.cn

Ruby: arr.each { |item| puts item }
来源：http://ofo.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lel.gogol.net.cn

[B06] 遍历字典 / 对象
来源：http://neh.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://unb.redwolf501.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jab.aizwys.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qfv.shuidangran.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://chw.nwbrower.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gfh.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lol.ehwqpu.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rym.yanxiufei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ygx.jinghuilouyu.cn

[B07] while 循环
来源：http://keg.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://qom.shuidangran.top

PHP:  while ($i < 10) { $i++; }
来源：http://kbo.c1oappe.top

JS:   while (i < 10) { i++; }
来源：http://mil.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://uiz.yj202588.top

Java: while (i < 10) { i++; }
来源：http://moa.quarkkingdee.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://auc.epnwcf.com

Ruby: while i < 10; i += 1; end
来源：http://dwv.jqgufenzy.top

C#:   while (i < 10) { i++; }
来源：http://gor.daxiang520.top

[B08] do-while（至少执行一次）
来源：http://yna.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://rcd.daxiang520.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wqn.zhoulong.xyz

JS:   do { i++; } while (i < 10);
来源：http://onm.zdqjudy.top

TS:   do { i++; } while (i < 10);
来源：http://ikb.svipenyu.cn

Java: do { i++; } while (i < 10);
来源：http://dma.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hdy.zdbjq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vlp.pengpengdd.cyou

C#:   do { i++; } while (i < 10);
来源：http://got.gaohongyu789.top

[B09] break 与 continue
来源：http://shd.fanxiaobao.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nqm.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jql.bjfxy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cba.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yxe.tanke756.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ftg.yangfankeji.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aep.dianchejie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ayx.jqgufenzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nbd.c1oappe.top

[B10] 遍历同时拿索引
来源：http://acn.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eaj.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jni.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hce.fktsv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xxs.aibaodan.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://psb.cdnleiting.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yec.yangfankeji.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jsw.jinyuanbaomall.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dfe.sweek.top

[B11] 生成数字序列 / 区间
来源：http://ymp.yueranfly.top

Py:   list(range(0, 10, 2))
来源：http://umv.yonumen.top

PHP:  range(0, 10, 2);
来源：http://afu.jinqigfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gmt.zhongyouzk.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ffc.jinqigfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qze.xuanzx.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yez.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://krk.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://crw.yanxiufei.cn

[B12] 跳出多层循环
来源：http://ozp.cqqwz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cmv.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://tib.cdnleiting.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cce.dianchejie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xkp.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kls.havefunace.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ofz.jianghu66.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://okk.zhongyouzk.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gss.zdbjq.cn


<!-- 参考信息 -->