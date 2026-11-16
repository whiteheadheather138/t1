代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://feo.tarul.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pfu.gzhubu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zqv.gaohongyu789.top

Ruby: "42".to_i; "3.14".to_f
来源：http://tmj.nanxinkj.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mev.epnwcf.com

[A07] 数字转字符串
来源：http://miu.9152youxi.cn

Py:   str(42)
来源：http://ylc.ybcxt.top

PHP:  (string) 42; strval(42)
来源：http://ift.zhixingplan.top

JS:   String(42); (42).toString()
来源：http://zzp.shanyushiyangkeji.top

TS:   String(42)
来源：http://nsi.shzxlz.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ajn.birdmap.top

Go:   strconv.Itoa(42)
来源：http://yok.hnqzz.top

Ruby: 42.to_s
来源：http://ugn.wangdashe.top

C#:   42.ToString()
来源：http://wwa.jlsjyb.cn

[A08] 取整与四舍五入
来源：http://kyr.epnwcf.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qjj.aibaodan.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vtg.iojbl.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gxf.guowangkeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hje.xziqi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bvo.yuanzhike.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://amy.zhengqikj.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xqy.zycfv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lqb.hywenlv.cn

[A09] 绝对值与最大最小值
来源：http://kof.nanxinkj.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jdu.cucudq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sep.yvedp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ukg.snrcjt.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nmg.sweek.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wjz.sjlbkw.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lak.yuxming.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tpb.nanxinkj.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://koj.tian-w.cn

[A10] 生成随机数
来源：http://jfh.cashguo.top

Py:   import random; random.randint(1, 100)
来源：http://dxi.redwolf501.top

PHP:  random_int(1, 100);
来源：http://iij.hysaishi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nfk.hcnkem.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://krr.zhiwuduotai.top

Java: new Random().nextInt(100) + 1
来源：http://atg.cashguo.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ioa.316326.xyz

Ruby: rand(1..100)
来源：http://hht.zhengqikj.top

C#:   new Random().Next(1, 101)
来源：http://cql.daxiang520.top

[A11] 条件表达式（三元）
来源：http://wma.zhoulong.xyz

Py:   "yes" if x > 0 else "no"
来源：http://mtx.daria6918.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rsh.dashuyun.cn

JS:   x > 0 ? "yes" : "no"
来源：http://esn.hysaishi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tqb.yj20258.top

Java: x > 0 ? "yes" : "no"
来源：http://xbk.meibo888.top

Go:   // 无三元运算符，需用 if 语句
来源：http://kyr.cdnleiting.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tqy.zhaomingkeji.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://ssg.haohaochexian.top

[A12] 字符串插值 / 格式化
来源：http://mec.bjfxy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xnh.cashguo.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ium.sufxvd.cn

JS:   `Hello, ${name}!`
来源：http://jbv.gaohongyu789.top

TS:   `Hello, ${name}!`
来源：http://eqa.ppjwa.cn

Java: "Hello, %s!".formatted(name)
来源：http://azp.0kj1m.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://grq.epnwcf.com

Ruby: "Hello, #{name}!"
来源：http://vpb.fehbvm.com

C#:   $"Hello, {name}!"
来源：http://wuh.zdbjq.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zus.hywenlv.cn

Py:   "第一行\n第二行"
来源：http://qgh.zhiwuduotai.top

PHP:  "第一行\n第二行"
来源：http://kay.yvedp.cn

JS:   "第一行\n第二行"
来源：http://dfr.bbcook.cn

TS:   "第一行\n第二行"
来源：http://wxr.yueranfly.top

Java: "第一行\n第二行"
来源：http://zww.hcnkem.com

Go:   "第一行\n第二行"
来源：http://ccj.sweek.top

Ruby: "第一行\n第二行"
来源：http://kut.cdnleiting.top

C#:   "第一行\n第二行"
来源：http://itf.chenjidiqi.icu

[A14] 注释写法
来源：http://ubq.jianghu66.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://dex.haohaochexian.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://cub.ctjpmb.com

JS:   // 单行；/* 多行 */
来源：http://cqm.hfpthk.cn

TS:   // 单行；/* 多行 */
来源：http://eom.gogol.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cqw.sufxvd.cn

Go:   // 单行；/* 多行 */
来源：http://kew.feifeiyinyue.top

Ruby: # 单行；=begin 多行 =end
来源：http://hhx.ydzc1.top

C#:   // 单行；/* 多行 */
来源：http://txr.shuidangran.top

[A15] 空值判断与默认值
来源：http://kmt.bjfxy.top

Py:   value = data or "默认值"
来源：http://qnb.tianlin.xyz

PHP:  $value = $data ?? "默认值";
来源：http://hvk.fzhhl.top

JS:   const value = data ?? "默认值";
来源：http://syl.pengpengdd.cyou

TS:   const value = data ?? "默认值";
来源：http://ept.shangyingyoupin.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jjq.uphjek.com

Go:   if data == "" { data = "默认值" }
来源：http://wnk.316326.xyz

Ruby: value = data || "默认值"
来源：http://zjv.zhixingplan.top

C#:   var value = data ?? "默认值";
来源：http://jkn.quarkkingdee.top

[A16] 真假值判断规则
来源：http://xnk.jyoumei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fqm.aibaodan.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xau.jyoumei.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jek.fanxiaobao.xyz

TS:   if (!x) {}
来源：http://ajj.quarkkingdee.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sob.cashguo.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zcn.jinqigfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://nhs.gogol.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ogs.yj20258888.top

[A17] 位运算
来源：http://cwb.yangfankeji.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vwj.meibo888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wuk.ydjk.org.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gnm.0kj1m.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://khu.ppjwa.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aff.9152youxi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bcm.jiagoushi.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pza.xingfuxueyuan.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://old.bjfxy.top

[A18] 字符与 ASCII 码互转
来源：http://xsc.chenlongwang.top

Py:   ord("A"); chr(65)
来源：http://hfw.chenzaomai.com

PHP:  ord("A"); chr(65)
来源：http://wnm.ydzc1.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wpe.andypj.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oek.havefunace.top

Java: (int) 'A'; (char) 65
来源：http://jpo.pengpengdd.cyou

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jhh.aibaodan.cn

Ruby: "A".ord; 65.chr
来源：http://rjm.daxiang520.top

C#:   (int)'A'; (char)65
来源：http://spe.dashuyun.cn

[A19] 交换两个变量
来源：http://vjx.yuxming.cn

Py:   a, b = b, a
来源：http://daq.cashguo.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hna.ywan-chungtsiang.top

JS:   [a, b] = [b, a];
来源：http://jyc.gogol.net.cn

TS:   [a, b] = [b, a];
来源：http://mjd.daxiang520.top

Java: int t = a; a = b; b = t;
来源：http://oiw.xylfe.cn

Go:   a, b = b, a
来源：http://syo.guowangkeji.top

Ruby: a, b = b, a
来源：http://huk.gotoacloud.top

C#:   (a, b) = (b, a);
来源：http://ydc.jyoumei.cn

[A20] 读取标准输入
来源：http://bjq.jianghu66.top

Py:   name = input("请输入：")
来源：http://mxi.dashuyun.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oou.zhengqikj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ntb.tianlin.xyz

TS:   // Node.js：readline 模块
来源：http://quq.hcnkem.com

Java: new Scanner(System.in).nextLine()
来源：http://uih.smart0.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gwg.uphjek.com

Ruby: gets.chomp
来源：http://gjh.dianchejie.cn

C#:   Console.ReadLine();
来源：http://iro.sxryk.cn

[A21] 保留指定小数位输出
来源：http://ash.cheryme.top

Py:   f"{3.14159:.2f}"
来源：http://ddk.meibo888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kgc.gzhubu.top

JS:   (3.14159).toFixed(2)
来源：http://fsn.ppjwa.cn

TS:   (3.14159).toFixed(2)
来源：http://vvk.aizwys.cn

Java: String.format("%.2f", 3.14159)
来源：http://gft.dashuyun.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vph.feifeiyinyue.top

Ruby: format("%.2f", 3.14159)
来源：http://bnd.ehwqpu.com

C#:   3.14159.ToString("F2")
来源：http://mrr.jinqigfzy.top

[A22] 获取字符串长度
来源：http://ify.fzhhl.top

Py:   len(s)
来源：http://tua.yj20258.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://axa.yj202588.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gne.xinyue.icu

TS:   s.length
来源：http://isn.pengpengdd.cyou

Java: s.length()
来源：http://dov.jinghuilouyu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nqm.epnwcf.com

Ruby: s.length
来源：http://hey.wangshuangyany.cn

C#:   s.Length
来源：http://exa.ppjwa.cn

[A23] 大小写转换
来源：http://kom.zhongyouzk.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ago.gzhubu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ehy.xylfe.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aqj.fktsv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rgh.meibo888.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mkc.sysykeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gwc.sjlbkw.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rul.chenjidiqi.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://owx.fanxiaobao.xyz

[A24] 去除首尾空白
来源：http://jzy.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://usr.sysykeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hci.ydjk.org.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sfc.jianghu66.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gpr.9152youxi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xby.yj20258888.top

Go:   strings.TrimSpace(s)
来源：http://qyb.yvedp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://npn.sxryk.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xsf.zhongyouzk.top

[A25] 字符串比较
来源：http://xoy.hammf.cn

Py:   s1 == s2; s1 != s2
来源：http://mws.redwolf501.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pty.zdbjq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ewr.hcnkem.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cyl.mhx1999.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bcj.316326.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nwr.shangyingyoupin.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qdt.chenlongwang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cqu.sufxvd.cn

[A26] 类型转换总览
来源：http://qns.jinqigfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fii.cheryme.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rxy.guowangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vbf.jyoumei.cn

TS:   Number() String() Boolean() x as number
来源：http://ijk.epnwcf.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uih.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ubk.haohaochexian.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://voz.yanxiufei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hcs.nanxuanxn.top

================================================================================
来源：http://ept.zhixingplan.top

B. 流程控制
来源：http://qtg.shanyushiyangtech.top

================================================================================
来源：http://ipn.cashguo.top

[B01] 条件判断 if / else
来源：http://lrh.jianghu66.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cry.tianlin.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://puj.hfpthk.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dng.cqqwz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://skr.hfpthk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lby.daria6918.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ksd.dashuyun.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rvx.sxryk.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://okg.xuanzx.com

[B02] 多分支 else if / elif
来源：http://tyx.yfazqb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://brv.hywenlv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dim.yongpay.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dfb.jinqigufen.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fki.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zhx.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qaa.xuetiantiany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gbd.snrcjt.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nul.cheryme.top

[B03] switch / match / case
来源：http://mjl.yonumen.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://use.kuanghao11.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ips.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tvr.c1oappe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oge.jiagoushi.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baq.quarkkingdee.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ypj.shzxlz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ncq.pengpengdd.cyou

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ced.iojbl.cn

[B04] for 计数循环
来源：http://myh.yj20258.top

Py:   for i in range(10): print(i)
来源：http://mht.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mfz.shangyingyoupin.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ype.fzhhl.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bbv.gogol.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jwm.jinghuilouyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mgd.bbcook.cn

Ruby: 10.times { |i| puts i }
来源：http://xgq.ybcxt.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lfy.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://fhn.jianghu66.top

Py:   for item in arr: print(item)
来源：http://yiz.ppjwa.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vlo.cdnleiting.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mcq.hammf.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nxa.zhoulong.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://imf.sweek.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ica.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://kqu.pycfn.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lfg.fzhhl.top

[B06] 遍历字典 / 对象
来源：http://qzx.ivvv.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zyi.kuanghao11.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zet.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tqv.ywan-chungtsiang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qxu.bjfxy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cae.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wna.zhengqikj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dvp.kuanghao11.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pak.shanyushiyangtech.top

[B07] while 循环
来源：http://exr.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://rgg.feifeiyinyue.top

PHP:  while ($i < 10) { $i++; }
来源：http://rgh.zhijiandao.cn

JS:   while (i < 10) { i++; }
来源：http://ekb.yangfankeji.com

TS:   while (i < 10) { i++; }
来源：http://bwy.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://jjv.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jak.guannengcc.top

Ruby: while i < 10; i += 1; end
来源：http://rzh.hnxiangtu.top

C#:   while (i < 10) { i++; }
来源：http://sbc.tian-w.cn

[B08] do-while（至少执行一次）
来源：http://axy.svipenyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://era.birdmap.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mqu.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://hlz.xziqi.cn

TS:   do { i++; } while (i < 10);
来源：http://kuo.fzhhl.top

Java: do { i++; } while (i < 10);
来源：http://pfa.c1oappe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uaq.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pzd.zhoulong.xyz

C#:   do { i++; } while (i < 10);
来源：http://duy.vqdsnc.cn

[B09] break 与 continue
来源：http://ukd.daria6918.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uta.sjlbkw.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gmu.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wmq.kuanghao11.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nzu.shangyingyoupin.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ebe.tarul.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://snt.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xfn.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vwb.iojbl.cn

[B10] 遍历同时拿索引
来源：http://ysa.jinyuanbaomall.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dwk.mhx1999.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vtm.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zfr.nanxinkj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ivk.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hnn.hongshengwenyu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ouq.vqdsnc.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wsr.chenlongwang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://igq.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://lpn.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://sbe.birdmap.top

PHP:  range(0, 10, 2);
来源：http://rmk.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jcl.yangfankeji.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yny.hongshengwenyu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rns.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tzk.dianchejie.cn

Ruby: (0...10).step(2).to_a
来源：http://kqb.sxryk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tjj.hnqzz.top

[B12] 跳出多层循环
来源：http://efv.jyoumei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vix.yfazqb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://xiz.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tvb.nanxuanxn.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ego.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://idf.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cej.mhx1999.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xcr.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://snx.mhx1999.top

[B13] 判断是否为数字
来源：http://weg.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://dxh.sysykeji.top

PHP:  is_numeric($x)
来源：http://fmu.yangfankeji.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wpq.hesvh.cn


<!-- 参考信息 -->