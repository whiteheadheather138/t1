代发 wailian999

[A06] 字符串转数字
来源：http://vum.nanxinkj.top

Py:   int("42"); float("3.14")
来源：http://ssp.hnxiangtu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ort.iojbl.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gqq.dianchejie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wvw.vqdsnc.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yuz.xuetiantiany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uey.xuanzx.com

Ruby: "42".to_i; "3.14".to_f
来源：http://xkj.chenlongwang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fbr.aizwys.cn

[A07] 数字转字符串
来源：http://tuu.sweek.top

Py:   str(42)
来源：http://izf.yueranfly.top

PHP:  (string) 42; strval(42)
来源：http://ecn.meibo888.top

JS:   String(42); (42).toString()
来源：http://aji.aibaodan.cn

TS:   String(42)
来源：http://dpb.0kj1m.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ktx.feifeiyinyue.top

Go:   strconv.Itoa(42)
来源：http://iwm.zdbjq.cn

Ruby: 42.to_s
来源：http://yhu.zdqjudy.top

C#:   42.ToString()
来源：http://drl.tianlin.xyz

[A08] 取整与四舍五入
来源：http://omz.ppjwa.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kko.sufxvd.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://div.hnxiangtu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kxi.gaohongyu789.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xds.mhx1999.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uom.zhaomingkeji.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nab.daxiang520.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://qre.birdmap.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yxx.9152youxi.cn

[A09] 绝对值与最大最小值
来源：http://flh.hammf.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gua.sxryk.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://myc.yvedp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ntw.ybcxt.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zvv.yfazqb.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://afu.ehwqpu.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qnu.gaohongyu789.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sqc.xuanzx.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wdk.hcnkem.com

[A10] 生成随机数
来源：http://xqd.ctjpmb.com

Py:   import random; random.randint(1, 100)
来源：http://oxh.yuanzhike.top

PHP:  random_int(1, 100);
来源：http://wfq.zdbjq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vud.chenjidiqi.icu

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mzc.chenlongwang.top

Java: new Random().nextInt(100) + 1
来源：http://dli.nanxuanxn.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://iqy.yj20258888.top

Ruby: rand(1..100)
来源：http://jvh.cheryme.top

C#:   new Random().Next(1, 101)
来源：http://ymu.jianghu66.top

[A11] 条件表达式（三元）
来源：http://for.jiagoushi.top

Py:   "yes" if x > 0 else "no"
来源：http://nqj.hcnkem.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://atx.fanxiaobao.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://jbc.chenlongwang.top

TS:   x > 0 ? "yes" : "no"
来源：http://och.gzhubu.top

Java: x > 0 ? "yes" : "no"
来源：http://owq.fzhhl.top

Go:   // 无三元运算符，需用 if 语句
来源：http://lpa.dianchejie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rrc.shanyushiyangtech.top

C#:   x > 0 ? "yes" : "no"
来源：http://jwd.aizwys.cn

[A12] 字符串插值 / 格式化
来源：http://jqd.guannengcc.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hma.shzxlz.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ske.xuetiantiany.cn

JS:   `Hello, ${name}!`
来源：http://dma.pengpengdd.cyou

TS:   `Hello, ${name}!`
来源：http://cpp.yueranfly.top

Java: "Hello, %s!".formatted(name)
来源：http://qds.vehdjk.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ipk.zhixingplan.top

Ruby: "Hello, #{name}!"
来源：http://orx.ybcxt.top

C#:   $"Hello, {name}!"
来源：http://yjd.nanxuanxn.top

[A13] 多行字符串（练习 \n 转义）
来源：http://gvb.chenzaomai.com

Py:   "第一行\n第二行"
来源：http://qrj.tian-w.cn

PHP:  "第一行\n第二行"
来源：http://hyl.yj20258888.top

JS:   "第一行\n第二行"
来源：http://oka.yj20258.top

TS:   "第一行\n第二行"
来源：http://nwy.andypj.xyz

Java: "第一行\n第二行"
来源：http://vin.guannengcc.top

Go:   "第一行\n第二行"
来源：http://xiq.dashuyun.cn

Ruby: "第一行\n第二行"
来源：http://kqx.svipenyu.cn

C#:   "第一行\n第二行"
来源：http://qqf.snrcjt.cn

[A14] 注释写法
来源：http://zlx.c1oappe.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://myn.mhx1999.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://euq.jlsjyb.cn

JS:   // 单行；/* 多行 */
来源：http://ark.c1oappe.top

TS:   // 单行；/* 多行 */
来源：http://wfo.hysaishi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wvu.jinyuanbaomall.cn

Go:   // 单行；/* 多行 */
来源：http://feq.bjfxy.top

Ruby: # 单行；=begin 多行 =end
来源：http://noe.zdqjudy.top

C#:   // 单行；/* 多行 */
来源：http://zwr.dashuyun.cn

[A15] 空值判断与默认值
来源：http://ush.hfpthk.cn

Py:   value = data or "默认值"
来源：http://wqz.0kj1m.cn

PHP:  $value = $data ?? "默认值";
来源：http://lmu.zhixingplan.top

JS:   const value = data ?? "默认值";
来源：http://lpe.zhengqikj.top

TS:   const value = data ?? "默认值";
来源：http://gwo.yj202588.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pna.fanxiaobao.xyz

Go:   if data == "" { data = "默认值" }
来源：http://gsa.uphjek.com

Ruby: value = data || "默认值"
来源：http://ich.c1oappe.top

C#:   var value = data ?? "默认值";
来源：http://hzh.jiagoushi.top

[A16] 真假值判断规则
来源：http://clh.aibaodan.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hic.epnwcf.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gvd.zhiwuduotai.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dlo.cqqwz.cn

TS:   if (!x) {}
来源：http://byy.jinghuilouyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ssp.meibo888.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yrq.dianchejie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yka.zdbjq.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://amy.nwbrower.top

[A17] 位运算
来源：http://hyp.andypj.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zaa.yangfankeji.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eea.shangyingyoupin.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rwq.cashguo.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wrb.xylfe.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yel.shzxlz.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rru.gaohongyu789.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zhu.yongpay.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ytl.zhixingplan.top

[A18] 字符与 ASCII 码互转
来源：http://uzj.fengsongda.top

Py:   ord("A"); chr(65)
来源：http://mdv.bbcook.cn

PHP:  ord("A"); chr(65)
来源：http://ber.uphjek.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gcz.jianghu66.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://whh.fktsv.cn

Java: (int) 'A'; (char) 65
来源：http://bea.316326.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pxv.meibo888.top

Ruby: "A".ord; 65.chr
来源：http://vnv.cucudq.cn

C#:   (int)'A'; (char)65
来源：http://hpx.havefunace.top

[A19] 交换两个变量
来源：http://ipd.hnqzz.top

Py:   a, b = b, a
来源：http://hku.birdmap.top

PHP:  [$a, $b] = [$b, $a];
来源：http://udc.kuanghao11.cn

JS:   [a, b] = [b, a];
来源：http://ciz.feifeiyinyue.top

TS:   [a, b] = [b, a];
来源：http://ced.gzhubu.top

Java: int t = a; a = b; b = t;
来源：http://nld.jyoumei.cn

Go:   a, b = b, a
来源：http://gbu.ivvv.top

Ruby: a, b = b, a
来源：http://plk.ivvv.top

C#:   (a, b) = (b, a);
来源：http://zce.cucudq.cn

[A20] 读取标准输入
来源：http://vrv.hnqzz.top

Py:   name = input("请输入：")
来源：http://qbg.zhongyouzk.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qvg.jqgufenzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zgz.xylfe.cn

TS:   // Node.js：readline 模块
来源：http://eby.svipenyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://psa.jinghuilouyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aod.fehbvm.com

Ruby: gets.chomp
来源：http://plv.wangdashe.top

C#:   Console.ReadLine();
来源：http://vti.xylfe.cn

[A21] 保留指定小数位输出
来源：http://mlu.yongpay.top

Py:   f"{3.14159:.2f}"
来源：http://gdy.wangshuangyany.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cmj.fehbvm.com

JS:   (3.14159).toFixed(2)
来源：http://imy.ehwqpu.com

TS:   (3.14159).toFixed(2)
来源：http://vux.shzxlz.cn

Java: String.format("%.2f", 3.14159)
来源：http://pev.havefunace.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cap.shanyushiyangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://kji.tanke756.top

C#:   3.14159.ToString("F2")
来源：http://fhn.bjfxy.top

[A22] 获取字符串长度
来源：http://odb.havefunace.top

Py:   len(s)
来源：http://lfv.daria6918.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zit.ydjk.org.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eac.chenjidiqi.icu

TS:   s.length
来源：http://ldh.cqqwz.cn

Java: s.length()
来源：http://fez.fengsongda.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xoe.pycfn.com

Ruby: s.length
来源：http://xzy.pengpengdd.cyou

C#:   s.Length
来源：http://sfv.tianlin.xyz

[A23] 大小写转换
来源：http://nko.vehdjk.com

Py:   s.upper(); s.lower(); s.title()
来源：http://fjw.jlsjyb.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dwa.cucudq.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ffw.wangdashe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hfa.zdqjudy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qrd.tanke756.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pom.jianghu66.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uki.yj202588.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dyi.nanxinkj.top

[A24] 去除首尾空白
来源：http://ovh.yongpay.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hxt.ctjpmb.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mgx.yj20258888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rck.nanxinkj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oqo.bbcook.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jkr.pengpengdd.cyou

Go:   strings.TrimSpace(s)
来源：http://ket.tarul.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://epk.xingfuxueyuan.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yxp.9152youxi.cn

[A25] 字符串比较
来源：http://xna.jiagoushi.top

Py:   s1 == s2; s1 != s2
来源：http://gpf.fengsongda.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lcv.zdbjq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bme.zhaomingkeji.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ngz.nwbrower.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hjp.shanyushiyangtech.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://otq.ctjpmb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://jsd.jqgufenzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://khp.wangshuangyany.cn

[A26] 类型转换总览
来源：http://jdi.ppjwa.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://aqe.quarkkingdee.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rjb.tianlin.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://whc.ppjwa.cn

TS:   Number() String() Boolean() x as number
来源：http://lon.pycfn.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nal.yanxiufei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://twf.jiagoushi.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bzb.shanyushiyangtech.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ijg.kuanghao11.cn

================================================================================
来源：http://epg.hongshengwenyu.top

B. 流程控制
来源：http://ecn.gaohongyu789.top

================================================================================
来源：http://hvm.ehwqpu.com

[B01] 条件判断 if / else
来源：http://sja.xingfuxueyuan.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://rjj.daria6918.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fej.jiagoushi.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bns.xylfe.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nrp.dashuyun.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://syq.vehdjk.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://szq.xingfuxueyuan.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kuh.gzhubu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hqz.vqdsnc.cn

[B02] 多分支 else if / elif
来源：http://rly.zdqjudy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vsd.nanxinkj.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kon.redwolf501.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wzm.xziqi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wym.sweek.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://efk.sysykeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tbf.chenzaomai.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bog.yueranfly.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tte.zhoulong.xyz

[B03] switch / match / case
来源：http://qpr.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xrj.jinghuilouyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://giq.iojbl.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wfm.mhx1999.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://day.hammf.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wlt.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gki.zycfv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uyj.yuanzhike.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ngi.nwbrower.top

[B04] for 计数循环
来源：http://dyb.zhijiandao.cn

Py:   for i in range(10): print(i)
来源：http://hrb.jiagoushi.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fxq.fanxiaobao.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bdo.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qdc.jqgfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ptn.ppjwa.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cvt.daxiang520.top

Ruby: 10.times { |i| puts i }
来源：http://hkw.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uth.cheryme.top

[B05] 遍历数组 / 列表
来源：http://odu.yfazqb.com

Py:   for item in arr: print(item)
来源：http://mir.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vwp.ivvv.top

JS:   for (const item of arr) { console.log(item); }
来源：http://msp.zhoulong.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://hgk.shangyingyoupin.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pcl.iojbl.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rpy.yongpay.top

Ruby: arr.each { |item| puts item }
来源：http://nqg.xylfe.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ulx.guannengcc.top

[B06] 遍历字典 / 对象
来源：http://err.andypj.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://nub.vqdsnc.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vom.chenjidiqi.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oeq.9152youxi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://acp.zhoulong.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xuf.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gpq.ydjk.org.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yzp.0kj1m.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cht.zycfv.cn

[B07] while 循环
来源：http://qij.yj20258.top

Py:   while i < 10: i += 1
来源：http://fqr.zhixingplan.top

PHP:  while ($i < 10) { $i++; }
来源：http://niz.gaohongyu789.top

JS:   while (i < 10) { i++; }
来源：http://tgv.bbcook.cn

TS:   while (i < 10) { i++; }
来源：http://qqm.tanke756.top

Java: while (i < 10) { i++; }
来源：http://kox.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://amz.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://jhu.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://qne.dianchejie.cn

[B08] do-while（至少执行一次）
来源：http://awd.quarkkingdee.top

Py:   # 无 do-while：用 while True + break
来源：http://jmo.hnqzz.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vud.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://quu.cashguo.top

TS:   do { i++; } while (i < 10);
来源：http://ohg.vehdjk.com

Java: do { i++; } while (i < 10);
来源：http://oom.ydjk.org.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zca.jinghuilouyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lzk.fanxiaobao.xyz

C#:   do { i++; } while (i < 10);
来源：http://fxw.fehbvm.com

[B09] break 与 continue
来源：http://nzi.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xps.hywenlv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mki.cashguo.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://plq.hesvh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://biq.fengsongda.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zdy.ydjk.org.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://djx.yj20258888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oxj.shanyushiyangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yvc.sysykeji.top

[B10] 遍历同时拿索引
来源：http://gvf.daxiang520.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sxq.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ska.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hna.jqgfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hwz.wangdashe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://koz.nanxinkj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cyv.jianghu66.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wxl.ivvv.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ktn.chenzaomai.com

[B11] 生成数字序列 / 区间
来源：http://hri.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://urq.chenlongwang.top

PHP:  range(0, 10, 2);
来源：http://iel.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fzj.xingfuxueyuan.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mom.ydzc1.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://olt.shanyushiyangtech.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vgh.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://wzz.nanxuanxn.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mxl.shuidangran.top

[B12] 跳出多层循环
来源：http://bqq.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bjt.yj202588.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://eub.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://djf.sweek.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zvz.ctjpmb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dzx.jinqigfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ifk.bjfxy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ejf.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cuc.pycfn.com


<!-- 参考信息 -->