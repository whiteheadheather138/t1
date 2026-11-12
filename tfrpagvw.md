代发 wailian999

[A06] 字符串转数字
来源：http://whk.shzxlz.cn

Py:   int("42"); float("3.14")
来源：http://dec.jiagoushi.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://puh.wangdashe.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://aaj.vqdsnc.cn

TS:   parseInt("42", 10); Number("42")
来源：http://glx.vqdsnc.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qex.yj202588.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ddh.jinqigfzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dab.nanxinkj.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ceq.svipenyu.cn

[A07] 数字转字符串
来源：http://tne.jianghu66.top

Py:   str(42)
来源：http://lef.zhengqikj.top

PHP:  (string) 42; strval(42)
来源：http://vno.uphjek.com

JS:   String(42); (42).toString()
来源：http://bjb.sxryk.cn

TS:   String(42)
来源：http://azg.shuidangran.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://cej.sysykeji.top

Go:   strconv.Itoa(42)
来源：http://sji.jlsjyb.cn

Ruby: 42.to_s
来源：http://txb.sufxvd.cn

C#:   42.ToString()
来源：http://tmh.hesvh.cn

[A08] 取整与四舍五入
来源：http://efn.shuidangran.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pak.chenlongwang.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zmj.yj202588.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bjz.zhengqikj.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dhn.gogol.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pxd.zycfv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lgx.fengsongda.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://tsi.hesvh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ttl.shuidangran.top

[A09] 绝对值与最大最小值
来源：http://huz.zhoulong.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gvn.xylfe.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bco.zdqjudy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pap.guannengcc.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://scz.sxryk.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oga.tian-w.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pna.iojbl.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kez.zhaomingkeji.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mzc.zdbjq.cn

[A10] 生成随机数
来源：http://ime.zhaomingkeji.xyz

Py:   import random; random.randint(1, 100)
来源：http://rag.xuanzx.com

PHP:  random_int(1, 100);
来源：http://phu.zhiwuduotai.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://iuw.ehwqpu.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://chy.nwbrower.top

Java: new Random().nextInt(100) + 1
来源：http://ope.zhongyouzk.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hny.wangdashe.top

Ruby: rand(1..100)
来源：http://wul.tian-w.cn

C#:   new Random().Next(1, 101)
来源：http://tta.0kj1m.cn

[A11] 条件表达式（三元）
来源：http://omw.feifeiyinyue.top

Py:   "yes" if x > 0 else "no"
来源：http://euu.birdmap.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://apz.ybcxt.top

JS:   x > 0 ? "yes" : "no"
来源：http://wfn.snrcjt.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vmv.yuxming.cn

Java: x > 0 ? "yes" : "no"
来源：http://msw.hywenlv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qxy.ehwqpu.com

Ruby: x > 0 ? "yes" : "no"
来源：http://jdd.andypj.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://shz.bjfxy.top

[A12] 字符串插值 / 格式化
来源：http://adv.hammf.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vem.zhaomingkeji.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nlb.fktsv.cn

JS:   `Hello, ${name}!`
来源：http://sge.meibo888.top

TS:   `Hello, ${name}!`
来源：http://nin.316326.xyz

Java: "Hello, %s!".formatted(name)
来源：http://oyc.aizwys.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tms.yfazqb.com

Ruby: "Hello, #{name}!"
来源：http://jtk.yangfankeji.com

C#:   $"Hello, {name}!"
来源：http://iic.gotoacloud.top

[A13] 多行字符串（练习 \n 转义）
来源：http://pbi.yueranfly.top

Py:   "第一行\n第二行"
来源：http://bjf.0kj1m.cn

PHP:  "第一行\n第二行"
来源：http://qot.hnqzz.top

JS:   "第一行\n第二行"
来源：http://xps.fehbvm.com

TS:   "第一行\n第二行"
来源：http://dlu.chenjidiqi.icu

Java: "第一行\n第二行"
来源：http://bnt.mhx1999.top

Go:   "第一行\n第二行"
来源：http://zte.xinyue.icu

Ruby: "第一行\n第二行"
来源：http://wul.gotoacloud.top

C#:   "第一行\n第二行"
来源：http://cvi.meibo888.top

[A14] 注释写法
来源：http://rmo.birdmap.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://cif.gzhubu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ofc.jianghu66.top

JS:   // 单行；/* 多行 */
来源：http://ily.yueranfly.top

TS:   // 单行；/* 多行 */
来源：http://afz.fengsongda.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jiq.jqgfzy.top

Go:   // 单行；/* 多行 */
来源：http://yje.gogol.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hcc.havefunace.top

C#:   // 单行；/* 多行 */
来源：http://lef.zhixingplan.top

[A15] 空值判断与默认值
来源：http://krk.jinghuilouyu.cn

Py:   value = data or "默认值"
来源：http://zyj.shanyushiyangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://jhb.yj20258888.top

JS:   const value = data ?? "默认值";
来源：http://ozq.bbcook.cn

TS:   const value = data ?? "默认值";
来源：http://hzh.xziqi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hnr.shanyushiyangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://ovw.yueranfly.top

Ruby: value = data || "默认值"
来源：http://dmc.ivvv.top

C#:   var value = data ?? "默认值";
来源：http://wtj.jiagoushi.top

[A16] 真假值判断规则
来源：http://jsb.316326.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sbg.hfpthk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://acd.cdnleiting.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yxv.yongpay.top

TS:   if (!x) {}
来源：http://exh.xuanzx.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fpx.xingfuxueyuan.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gxw.guannengcc.top

Ruby: unless x            # nil 与 false 为假
来源：http://jhb.cucudq.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bwa.cqqwz.cn

[A17] 位运算
来源：http://zpq.guannengcc.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wza.jianghu66.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bdm.yuanzhike.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uwn.nanxinkj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ijq.ivvv.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://spt.gogol.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ela.yanxiufei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gwj.haohaochexian.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rcf.hnxiangtu.top

[A18] 字符与 ASCII 码互转
来源：http://ewt.zhixingplan.top

Py:   ord("A"); chr(65)
来源：http://vjg.shanyushiyangkeji.top

PHP:  ord("A"); chr(65)
来源：http://ouo.yj20258.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mwr.zycfv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jga.tanke756.top

Java: (int) 'A'; (char) 65
来源：http://zzq.cqqwz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gns.zdbjq.cn

Ruby: "A".ord; 65.chr
来源：http://pyr.kuanghao11.cn

C#:   (int)'A'; (char)65
来源：http://vzk.zhoulong.xyz

[A19] 交换两个变量
来源：http://eqv.xylfe.cn

Py:   a, b = b, a
来源：http://hth.chenlongwang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://lyj.ydjk.org.cn

JS:   [a, b] = [b, a];
来源：http://yhh.dashuyun.cn

TS:   [a, b] = [b, a];
来源：http://lkp.uphjek.com

Java: int t = a; a = b; b = t;
来源：http://sjv.daxiang520.top

Go:   a, b = b, a
来源：http://jui.yuxming.cn

Ruby: a, b = b, a
来源：http://ixg.tian-w.cn

C#:   (a, b) = (b, a);
来源：http://nxo.shzxlz.cn

[A20] 读取标准输入
来源：http://euh.gogol.net.cn

Py:   name = input("请输入：")
来源：http://fmn.zycfv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mfh.xingfuxueyuan.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fmq.0kj1m.cn

TS:   // Node.js：readline 模块
来源：http://pft.ehwqpu.com

Java: new Scanner(System.in).nextLine()
来源：http://kzo.dashuyun.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yxs.snrcjt.cn

Ruby: gets.chomp
来源：http://klq.fktsv.cn

C#:   Console.ReadLine();
来源：http://ojo.xziqi.cn

[A21] 保留指定小数位输出
来源：http://qrc.shanyushiyangtech.top

Py:   f"{3.14159:.2f}"
来源：http://wxh.hcnkem.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vfd.xuetiantiany.cn

JS:   (3.14159).toFixed(2)
来源：http://hpv.redwolf501.top

TS:   (3.14159).toFixed(2)
来源：http://szc.yangfankeji.com

Java: String.format("%.2f", 3.14159)
来源：http://urx.0kj1m.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vcw.yueranfly.top

Ruby: format("%.2f", 3.14159)
来源：http://gcy.shanyushiyangtech.top

C#:   3.14159.ToString("F2")
来源：http://pak.hnqzz.top

[A22] 获取字符串长度
来源：http://tpz.cashguo.top

Py:   len(s)
来源：http://lka.c1oappe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://usz.jinqigfzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ecj.9152youxi.cn

TS:   s.length
来源：http://grh.yj202588.top

Java: s.length()
来源：http://ncb.zhongyouzk.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://edz.vqdsnc.cn

Ruby: s.length
来源：http://nui.chenzaomai.com

C#:   s.Length
来源：http://jkr.0kj1m.cn

[A23] 大小写转换
来源：http://gty.ywan-chungtsiang.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kus.hnxiangtu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://get.gzhubu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://que.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ckj.feifeiyinyue.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wyo.hesvh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bvz.svipenyu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zqg.jyoumei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zep.guowangkeji.top

[A24] 去除首尾空白
来源：http://qug.zdbjq.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rbq.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xiq.ydzc1.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nco.shuidangran.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cut.quarkkingdee.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://anw.yuanzhike.top

Go:   strings.TrimSpace(s)
来源：http://nmx.tianlin.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yfj.guannengcc.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gqx.cqqwz.cn

[A25] 字符串比较
来源：http://jgj.ppjwa.cn

Py:   s1 == s2; s1 != s2
来源：http://ugk.redwolf501.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nme.aibaodan.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fnn.pengpengdd.cyou

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eof.redwolf501.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eki.nwbrower.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vxy.zhijiandao.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mud.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ewo.hcnkem.com

[A26] 类型转换总览
来源：http://emk.ctjpmb.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zpy.yfazqb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dcz.yanxiufei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iyr.sjlbkw.cn

TS:   Number() String() Boolean() x as number
来源：http://ezo.9152youxi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://deb.aibaodan.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rxt.jinghuilouyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lyk.smart0.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://prq.kuanghao11.cn

================================================================================
来源：http://igo.zhoulong.xyz

B. 流程控制
来源：http://oic.jinqigufen.top

================================================================================
来源：http://oel.yuanzhike.top

[B01] 条件判断 if / else
来源：http://fdt.jlsjyb.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ipy.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mgo.mhx1999.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rly.ehwqpu.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yxq.uphjek.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://hzs.ctjpmb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jxl.ctjpmb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oph.yj202588.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gwn.zycfv.cn

[B02] 多分支 else if / elif
来源：http://wqk.jinyuanbaomall.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://agm.nanxinkj.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lhe.yuanzhike.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zeq.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iey.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hkw.9152youxi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xuv.shanyushiyangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yhh.dashuyun.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iot.shangyingyoupin.top

[B03] switch / match / case
来源：http://xly.shangyingyoupin.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://awy.zhixingplan.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jla.smart0.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qza.zhongyouzk.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qbe.andypj.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ycf.zhaomingkeji.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xfn.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qvx.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kyu.tianlin.xyz

[B04] for 计数循环
来源：http://eyg.ywan-chungtsiang.top

Py:   for i in range(10): print(i)
来源：http://eyz.jinqigufen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nfs.9152youxi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uzx.hammf.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qbe.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pwz.zhongyouzk.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yrj.316326.xyz

Ruby: 10.times { |i| puts i }
来源：http://fux.zycfv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nwg.shangyingyoupin.top

[B05] 遍历数组 / 列表
来源：http://tbo.xuanzx.com

Py:   for item in arr: print(item)
来源：http://dvl.shzxlz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xtc.ydjk.org.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qjh.jlsjyb.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://clj.cheryme.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dvm.sufxvd.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nqq.pengpengdd.cyou

Ruby: arr.each { |item| puts item }
来源：http://mwl.xinyue.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hlq.hysaishi.cn

[B06] 遍历字典 / 对象
来源：http://tax.gotoacloud.top

Py:   for k, v in d.items(): print(k, v)
来源：http://udt.gaohongyu789.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://shr.hesvh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://myo.fehbvm.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hmd.vehdjk.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kfj.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://joy.chenlongwang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://loa.haohaochexian.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hgb.cheryme.top

[B07] while 循环
来源：http://mlb.yj20258.top

Py:   while i < 10: i += 1
来源：http://bsu.xinyue.icu

PHP:  while ($i < 10) { $i++; }
来源：http://vcx.jinghuilouyu.cn

JS:   while (i < 10) { i++; }
来源：http://scb.gaohongyu789.top

TS:   while (i < 10) { i++; }
来源：http://fww.zdbjq.cn

Java: while (i < 10) { i++; }
来源：http://jtf.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://odj.jinqigufen.top

Ruby: while i < 10; i += 1; end
来源：http://igu.hywenlv.cn

C#:   while (i < 10) { i++; }
来源：http://vhg.kuanghao11.cn

[B08] do-while（至少执行一次）
来源：http://iwg.jinqigfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://jrf.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rot.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://irq.shanyushiyangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://bpf.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://pjd.uphjek.com

Go:   for { i++; if i >= 10 { break } }
来源：http://zwr.yj20258888.top

Ruby: begin; i += 1; end while i < 10
来源：http://mcu.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://gse.ivvv.top

[B09] break 与 continue
来源：http://ifz.zycfv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xhi.gotoacloud.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vcq.xinyue.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pit.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yyh.jlsjyb.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pao.xuetiantiany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mya.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tsp.gzhubu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uvk.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://bne.jinqigufen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ffd.daxiang520.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://krg.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dpg.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zds.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dce.xziqi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xvk.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qby.svipenyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uwr.hnxiangtu.top

[B11] 生成数字序列 / 区间
来源：http://iai.hongshengwenyu.top

Py:   list(range(0, 10, 2))
来源：http://kcc.hammf.cn

PHP:  range(0, 10, 2);
来源：http://vsg.nanxuanxn.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vjt.ydjk.org.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mhf.jinqigufen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jvo.nanxuanxn.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bjl.xylfe.cn

Ruby: (0...10).step(2).to_a
来源：http://ayn.9152youxi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pph.ppjwa.cn

[B12] 跳出多层循环
来源：http://ivv.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zzu.mhx1999.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dzs.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kkg.zhongyouzk.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gcb.zhaomingkeji.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://txk.yfazqb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://enn.redwolf501.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mzj.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ovh.epnwcf.com


<!-- 参考信息 -->