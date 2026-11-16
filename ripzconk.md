代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://rrp.zhaomingkeji.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ybs.zdbjq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dpe.tanke756.top

Ruby: "42".to_i; "3.14".to_f
来源：http://uls.andypj.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dbe.hnqzz.top

[A07] 数字转字符串
来源：http://gkv.gogol.net.cn

Py:   str(42)
来源：http://dlg.jqgufenzy.top

PHP:  (string) 42; strval(42)
来源：http://maf.iojbl.cn

JS:   String(42); (42).toString()
来源：http://byi.jyoumei.cn

TS:   String(42)
来源：http://dny.andypj.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://tjm.sweek.top

Go:   strconv.Itoa(42)
来源：http://ksr.jianghu66.top

Ruby: 42.to_s
来源：http://all.guannengcc.top

C#:   42.ToString()
来源：http://oyw.nanxinkj.top

[A08] 取整与四舍五入
来源：http://wmr.yj20258.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vyb.uphjek.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pmd.chenzaomai.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jco.nanxuanxn.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uyt.jinyuanbaomall.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://avf.c1oappe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wtu.9152youxi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rnw.52xcode.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dri.hongshengwenyu.top

[A09] 绝对值与最大最小值
来源：http://vmt.redwolf501.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oai.dianchejie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ztd.cdnleiting.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://byi.vqdsnc.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yne.zhiwuduotai.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xae.ppjwa.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vko.yanxiufei.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iuf.epnwcf.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kna.xuanzx.com

[A10] 生成随机数
来源：http://lbg.xuanzx.com

Py:   import random; random.randint(1, 100)
来源：http://fhs.gogol.net.cn

PHP:  random_int(1, 100);
来源：http://xxb.hnqzz.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zyj.ivvv.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://srg.yongpay.top

Java: new Random().nextInt(100) + 1
来源：http://ign.zdbjq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oip.0kj1m.cn

Ruby: rand(1..100)
来源：http://ope.zhoulong.xyz

C#:   new Random().Next(1, 101)
来源：http://ahb.yonumen.top

[A11] 条件表达式（三元）
来源：http://isn.ydjk.org.cn

Py:   "yes" if x > 0 else "no"
来源：http://rpu.xingfuxueyuan.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://btr.zhoulong.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://kmx.shzxlz.cn

TS:   x > 0 ? "yes" : "no"
来源：http://klh.gaohongyu789.top

Java: x > 0 ? "yes" : "no"
来源：http://etm.nanxinkj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://tus.hfpthk.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hmc.chenzaomai.com

C#:   x > 0 ? "yes" : "no"
来源：http://len.0kj1m.cn

[A12] 字符串插值 / 格式化
来源：http://gjq.jqgufenzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ltz.dianchejie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kki.tian-w.cn

JS:   `Hello, ${name}!`
来源：http://pnj.sweek.top

TS:   `Hello, ${name}!`
来源：http://ljv.smart0.xyz

Java: "Hello, %s!".formatted(name)
来源：http://gdw.xylfe.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ttj.zdbjq.cn

Ruby: "Hello, #{name}!"
来源：http://kwg.meibo888.top

C#:   $"Hello, {name}!"
来源：http://lpg.wangdashe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://wkj.cucudq.cn

Py:   "第一行\n第二行"
来源：http://ayi.hongshengwenyu.top

PHP:  "第一行\n第二行"
来源：http://awo.iojbl.cn

JS:   "第一行\n第二行"
来源：http://jpp.9152youxi.cn

TS:   "第一行\n第二行"
来源：http://jnm.gzhubu.top

Java: "第一行\n第二行"
来源：http://syv.yongpay.top

Go:   "第一行\n第二行"
来源：http://stl.ivvv.top

Ruby: "第一行\n第二行"
来源：http://mus.c1oappe.top

C#:   "第一行\n第二行"
来源：http://tiy.guannengcc.top

[A14] 注释写法
来源：http://fso.birdmap.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://svv.jinyuanbaomall.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ofl.zdqjudy.top

JS:   // 单行；/* 多行 */
来源：http://yti.wangshuangyany.cn

TS:   // 单行；/* 多行 */
来源：http://giu.yj202588.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ryx.jinyuanbaomall.cn

Go:   // 单行；/* 多行 */
来源：http://sti.jyoumei.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jcn.yongpay.top

C#:   // 单行；/* 多行 */
来源：http://tel.daxiang520.top

[A15] 空值判断与默认值
来源：http://mpu.redwolf501.top

Py:   value = data or "默认值"
来源：http://rep.ehwqpu.com

PHP:  $value = $data ?? "默认值";
来源：http://qzp.yvedp.cn

JS:   const value = data ?? "默认值";
来源：http://iyx.zhoulong.xyz

TS:   const value = data ?? "默认值";
来源：http://ggy.yj20258.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kqo.9152youxi.cn

Go:   if data == "" { data = "默认值" }
来源：http://cgd.havefunace.top

Ruby: value = data || "默认值"
来源：http://gfj.hcnkem.com

C#:   var value = data ?? "默认值";
来源：http://gnx.yuanzhike.top

[A16] 真假值判断规则
来源：http://gpl.zhongyouzk.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://txf.ppjwa.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eri.dianchejie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://osw.shanyushiyangkeji.top

TS:   if (!x) {}
来源：http://pzy.zdqjudy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rlf.xuetiantiany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rwn.chenzaomai.com

Ruby: unless x            # nil 与 false 为假
来源：http://pds.jqgfzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://atl.316326.xyz

[A17] 位运算
来源：http://aff.xuanzx.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sjx.gotoacloud.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://izs.jyoumei.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tmb.guannengcc.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://npg.gotoacloud.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wbt.shanyushiyangkeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vvm.xinyue.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qhy.zycfv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dgf.shanyushiyangkeji.top

[A18] 字符与 ASCII 码互转
来源：http://cmv.guannengcc.top

Py:   ord("A"); chr(65)
来源：http://kha.gogol.net.cn

PHP:  ord("A"); chr(65)
来源：http://zkf.wangshuangyany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oss.svipenyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wbq.haohaochexian.top

Java: (int) 'A'; (char) 65
来源：http://vkp.ydzc1.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://swi.yj20258888.top

Ruby: "A".ord; 65.chr
来源：http://jjy.ywan-chungtsiang.top

C#:   (int)'A'; (char)65
来源：http://zap.guannengcc.top

[A19] 交换两个变量
来源：http://tzi.nanxuanxn.top

Py:   a, b = b, a
来源：http://ton.jinqigufen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mxi.gzhubu.top

JS:   [a, b] = [b, a];
来源：http://wwe.zhiwuduotai.top

TS:   [a, b] = [b, a];
来源：http://jqi.hywenlv.cn

Java: int t = a; a = b; b = t;
来源：http://gwu.xuanzx.com

Go:   a, b = b, a
来源：http://sat.havefunace.top

Ruby: a, b = b, a
来源：http://gaw.jinqigfzy.top

C#:   (a, b) = (b, a);
来源：http://dbp.ctjpmb.com

[A20] 读取标准输入
来源：http://vfa.cheryme.top

Py:   name = input("请输入：")
来源：http://luj.zhiwuduotai.top

PHP:  $name = trim(fgets(STDIN));
来源：http://pbl.zhongyouzk.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://avv.chenjidiqi.icu

TS:   // Node.js：readline 模块
来源：http://wfp.feifeiyinyue.top

Java: new Scanner(System.in).nextLine()
来源：http://weo.sjlbkw.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vcy.zhengqikj.top

Ruby: gets.chomp
来源：http://jpr.epnwcf.com

C#:   Console.ReadLine();
来源：http://ynz.yonumen.top

[A21] 保留指定小数位输出
来源：http://rtg.shanyushiyangtech.top

Py:   f"{3.14159:.2f}"
来源：http://knb.sxryk.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cuk.quarkkingdee.top

JS:   (3.14159).toFixed(2)
来源：http://ywq.hesvh.cn

TS:   (3.14159).toFixed(2)
来源：http://tsq.tanke756.top

Java: String.format("%.2f", 3.14159)
来源：http://bpc.epnwcf.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rte.9152youxi.cn

Ruby: format("%.2f", 3.14159)
来源：http://qft.shanyushiyangkeji.top

C#:   3.14159.ToString("F2")
来源：http://bjo.havefunace.top

[A22] 获取字符串长度
来源：http://rrm.zhoulong.xyz

Py:   len(s)
来源：http://kme.havefunace.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ljx.redwolf501.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://smo.zhixingplan.top

TS:   s.length
来源：http://jjt.aizwys.cn

Java: s.length()
来源：http://bpd.ybcxt.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fwy.gzhubu.top

Ruby: s.length
来源：http://wrd.shzxlz.cn

C#:   s.Length
来源：http://yxr.jyoumei.cn

[A23] 大小写转换
来源：http://nyw.smart0.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://cpx.gotoacloud.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://crh.aizwys.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tfh.epnwcf.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pjb.fzhhl.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qsu.jiagoushi.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pnv.tianlin.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dnu.316326.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://jkz.zdbjq.cn

[A24] 去除首尾空白
来源：http://vib.yvedp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ktm.xylfe.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iyw.0kj1m.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qgv.aibaodan.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ezd.ybcxt.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yna.shanyushiyangkeji.top

Go:   strings.TrimSpace(s)
来源：http://zjh.andypj.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ftw.hnqzz.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://knu.wangdashe.top

[A25] 字符串比较
来源：http://kxa.c1oappe.top

Py:   s1 == s2; s1 != s2
来源：http://ipm.sxryk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://huv.yuanzhike.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fpt.0kj1m.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://irs.nanxuanxn.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dwm.daria6918.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xzv.yfazqb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://nbe.jinqigufen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yjj.cqqwz.cn

[A26] 类型转换总览
来源：http://pjg.daxiang520.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ktd.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://scd.daria6918.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ott.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://whn.jiagoushi.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mgu.zhengqikj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mhc.iojbl.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tgl.daria6918.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zes.shzxlz.cn

================================================================================
来源：http://rla.iojbl.cn

B. 流程控制
来源：http://foh.jinyuanbaomall.cn

================================================================================
来源：http://rca.ppjwa.cn

[B01] 条件判断 if / else
来源：http://igi.andypj.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://kkq.zhiwuduotai.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://plo.tian-w.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cxu.fktsv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://itl.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://zgq.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jyl.xuetiantiany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://azu.yvedp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cci.0kj1m.cn

[B02] 多分支 else if / elif
来源：http://cce.xuetiantiany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://duh.jinyuanbaomall.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tyl.aibaodan.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ooy.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rwz.yvedp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bzc.fehbvm.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oya.tian-w.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tef.tianlin.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nab.yonumen.top

[B03] switch / match / case
来源：http://yuw.yj202588.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tiw.zhijiandao.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ned.hywenlv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mfm.xuetiantiany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lfs.zhaomingkeji.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tsp.0kj1m.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cha.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jih.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uzy.daria6918.cn

[B04] for 计数循环
来源：http://pvi.tanke756.top

Py:   for i in range(10): print(i)
来源：http://otq.birdmap.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qnd.cheryme.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://que.jianghu66.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yew.svipenyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lsf.cashguo.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vlt.yonumen.top

Ruby: 10.times { |i| puts i }
来源：http://jmp.iojbl.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vov.zhiwuduotai.top

[B05] 遍历数组 / 列表
来源：http://wkk.yj20258888.top

Py:   for item in arr: print(item)
来源：http://ioh.hywenlv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ryf.jiagoushi.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fdb.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://xbs.yvedp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jhb.zhaomingkeji.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lql.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://iwr.ydzc1.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pst.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://dsq.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://jnn.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bqq.sufxvd.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mti.daxiang520.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iqc.smart0.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sas.hammf.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cvg.cheryme.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qbj.fanxiaobao.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xwz.cashguo.top

[B07] while 循环
来源：http://qje.yongpay.top

Py:   while i < 10: i += 1
来源：http://tln.hywenlv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://efl.xinyue.icu

JS:   while (i < 10) { i++; }
来源：http://hyf.zhongyouzk.top

TS:   while (i < 10) { i++; }
来源：http://pnw.xingfuxueyuan.xyz

Java: while (i < 10) { i++; }
来源：http://wfl.guowangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gyw.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://zaf.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://btt.fengsongda.top

[B08] do-while（至少执行一次）
来源：http://zfd.yj20258888.top

Py:   # 无 do-while：用 while True + break
来源：http://bzh.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bcd.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://myh.jyoumei.cn

TS:   do { i++; } while (i < 10);
来源：http://wgq.iojbl.cn

Java: do { i++; } while (i < 10);
来源：http://nyi.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pci.yangfankeji.com

Ruby: begin; i += 1; end while i < 10
来源：http://htq.haohaochexian.top

C#:   do { i++; } while (i < 10);
来源：http://fpo.wangdashe.top

[B09] break 与 continue
来源：http://pyz.guannengcc.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tkk.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eiq.jyoumei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xsj.ydjk.org.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xmf.yuxming.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wxq.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zzf.zhixingplan.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ojr.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pjl.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://aus.0kj1m.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wir.snrcjt.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zbb.sufxvd.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fao.shangyingyoupin.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://odu.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gdy.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ixb.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bxa.jianghu66.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gpt.guowangkeji.top

[B11] 生成数字序列 / 区间
来源：http://ktd.smart0.xyz

Py:   list(range(0, 10, 2))
来源：http://kos.yanxiufei.cn

PHP:  range(0, 10, 2);
来源：http://rsb.andypj.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://diu.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jir.bjfxy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ekk.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tdo.sweek.top

Ruby: (0...10).step(2).to_a
来源：http://obi.feifeiyinyue.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://odb.0kj1m.cn

[B12] 跳出多层循环
来源：http://zfh.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ija.sweek.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rww.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ksg.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nlp.dianchejie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gnp.nwbrower.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ajm.cashguo.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aqz.yfazqb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ead.xylfe.cn

[B13] 判断是否为数字
来源：http://suh.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://hux.yuanzhike.top

PHP:  is_numeric($x)
来源：http://zya.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oou.andypj.xyz


<!-- 参考信息 -->