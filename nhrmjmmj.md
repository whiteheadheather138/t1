代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://vuj.sweek.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mik.zhijiandao.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xvb.jinqigfzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://weq.tian-w.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://alz.zhixingplan.top

[A07] 数字转字符串
来源：http://tnv.shzxlz.cn

Py:   str(42)
来源：http://bgz.nanxinkj.top

PHP:  (string) 42; strval(42)
来源：http://gpo.jlsjyb.cn

JS:   String(42); (42).toString()
来源：http://nkh.xuanzx.com

TS:   String(42)
来源：http://qbp.tarul.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mhd.yj20258.top

Go:   strconv.Itoa(42)
来源：http://flp.fehbvm.com

Ruby: 42.to_s
来源：http://aly.mhx1999.top

C#:   42.ToString()
来源：http://zau.ydjk.org.cn

[A08] 取整与四舍五入
来源：http://kdh.xuetiantiany.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gwh.haohaochexian.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xsy.jqgfzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ejl.zycfv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xzb.ydjk.org.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rzv.vehdjk.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qmi.daxiang520.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ruk.pycfn.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://spk.chenjidiqi.icu

[A09] 绝对值与最大最小值
来源：http://ajb.zhoulong.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mkt.hongshengwenyu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://roh.shzxlz.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bja.sjlbkw.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ytu.guannengcc.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jfi.svipenyu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tqu.ivvv.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ajv.dashuyun.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fji.tianlin.xyz

[A10] 生成随机数
来源：http://abu.dianchejie.cn

Py:   import random; random.randint(1, 100)
来源：http://uqh.birdmap.top

PHP:  random_int(1, 100);
来源：http://yry.meibo888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qej.shanyushiyangtech.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jmg.tianlin.xyz

Java: new Random().nextInt(100) + 1
来源：http://usd.yj20258.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://apn.zhengqikj.top

Ruby: rand(1..100)
来源：http://yqr.cucudq.cn

C#:   new Random().Next(1, 101)
来源：http://mwz.pycfn.com

[A11] 条件表达式（三元）
来源：http://ztd.birdmap.top

Py:   "yes" if x > 0 else "no"
来源：http://vfc.snrcjt.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qge.feifeiyinyue.top

JS:   x > 0 ? "yes" : "no"
来源：http://mrn.cucudq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ouk.jiagoushi.top

Java: x > 0 ? "yes" : "no"
来源：http://jkj.52xcode.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ibh.cheryme.top

Ruby: x > 0 ? "yes" : "no"
来源：http://dus.sufxvd.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zex.gogol.net.cn

[A12] 字符串插值 / 格式化
来源：http://jik.hammf.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://evc.hongshengwenyu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rpx.zhixingplan.top

JS:   `Hello, ${name}!`
来源：http://pmn.xuetiantiany.cn

TS:   `Hello, ${name}!`
来源：http://oxp.fktsv.cn

Java: "Hello, %s!".formatted(name)
来源：http://uve.quarkkingdee.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zux.daria6918.cn

Ruby: "Hello, #{name}!"
来源：http://zgh.yongpay.top

C#:   $"Hello, {name}!"
来源：http://xey.ctjpmb.com

[A13] 多行字符串（练习 \n 转义）
来源：http://qgm.fzhhl.top

Py:   "第一行\n第二行"
来源：http://ndc.cucudq.cn

PHP:  "第一行\n第二行"
来源：http://jop.shanyushiyangkeji.top

JS:   "第一行\n第二行"
来源：http://hpt.daria6918.cn

TS:   "第一行\n第二行"
来源：http://pym.c1oappe.top

Java: "第一行\n第二行"
来源：http://jbc.yuanzhike.top

Go:   "第一行\n第二行"
来源：http://fau.0kj1m.cn

Ruby: "第一行\n第二行"
来源：http://wgf.hysaishi.cn

C#:   "第一行\n第二行"
来源：http://bso.zhoulong.xyz

[A14] 注释写法
来源：http://oab.yj20258888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ypp.hywenlv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gdb.hcnkem.com

JS:   // 单行；/* 多行 */
来源：http://cke.birdmap.top

TS:   // 单行；/* 多行 */
来源：http://auj.wangshuangyany.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zzp.pycfn.com

Go:   // 单行；/* 多行 */
来源：http://bom.meibo888.top

Ruby: # 单行；=begin 多行 =end
来源：http://hkd.bbcook.cn

C#:   // 单行；/* 多行 */
来源：http://wyo.52xcode.cn

[A15] 空值判断与默认值
来源：http://msh.gzhubu.top

Py:   value = data or "默认值"
来源：http://ejc.zhixingplan.top

PHP:  $value = $data ?? "默认值";
来源：http://hcd.yvedp.cn

JS:   const value = data ?? "默认值";
来源：http://ymy.gotoacloud.top

TS:   const value = data ?? "默认值";
来源：http://grd.fktsv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zca.zhoulong.xyz

Go:   if data == "" { data = "默认值" }
来源：http://vqi.gotoacloud.top

Ruby: value = data || "默认值"
来源：http://gsg.hesvh.cn

C#:   var value = data ?? "默认值";
来源：http://czs.nanxinkj.top

[A16] 真假值判断规则
来源：http://xqb.xylfe.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bmi.dianchejie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://faw.cashguo.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cor.tian-w.cn

TS:   if (!x) {}
来源：http://fwt.zhaomingkeji.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zbf.fanxiaobao.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rts.shzxlz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cgq.hnqzz.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lrc.daria6918.cn

[A17] 位运算
来源：http://nzh.kuanghao11.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fyw.xuanzx.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://usw.zdbjq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pms.ehwqpu.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qdl.ppjwa.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lku.jqgfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://arh.bbcook.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ibg.hnqzz.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pnw.xuanzx.com

[A18] 字符与 ASCII 码互转
来源：http://qvo.xylfe.cn

Py:   ord("A"); chr(65)
来源：http://vjo.cqqwz.cn

PHP:  ord("A"); chr(65)
来源：http://cyj.tian-w.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oze.jinghuilouyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cam.cdnleiting.top

Java: (int) 'A'; (char) 65
来源：http://rkq.zdbjq.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nkw.svipenyu.cn

Ruby: "A".ord; 65.chr
来源：http://jfz.hywenlv.cn

C#:   (int)'A'; (char)65
来源：http://gjd.jinqigfzy.top

[A19] 交换两个变量
来源：http://gxh.yuxming.cn

Py:   a, b = b, a
来源：http://rml.aibaodan.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qqt.snrcjt.cn

JS:   [a, b] = [b, a];
来源：http://ynj.xingfuxueyuan.xyz

TS:   [a, b] = [b, a];
来源：http://uae.hesvh.cn

Java: int t = a; a = b; b = t;
来源：http://ywt.yuanzhike.top

Go:   a, b = b, a
来源：http://kvw.c1oappe.top

Ruby: a, b = b, a
来源：http://koi.yj20258888.top

C#:   (a, b) = (b, a);
来源：http://lzb.bjfxy.top

[A20] 读取标准输入
来源：http://isn.meibo888.top

Py:   name = input("请输入：")
来源：http://rjz.dianchejie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://njr.ppjwa.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://toh.tarul.cn

TS:   // Node.js：readline 模块
来源：http://teh.yonumen.top

Java: new Scanner(System.in).nextLine()
来源：http://tun.yj202588.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pkd.kuanghao11.cn

Ruby: gets.chomp
来源：http://xci.chenzaomai.com

C#:   Console.ReadLine();
来源：http://qdt.daria6918.cn

[A21] 保留指定小数位输出
来源：http://ywj.0kj1m.cn

Py:   f"{3.14159:.2f}"
来源：http://nfv.hesvh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://irj.yvedp.cn

JS:   (3.14159).toFixed(2)
来源：http://zdu.shanyushiyangtech.top

TS:   (3.14159).toFixed(2)
来源：http://gzw.zycfv.cn

Java: String.format("%.2f", 3.14159)
来源：http://qom.jqgufenzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ngc.cdnleiting.top

Ruby: format("%.2f", 3.14159)
来源：http://gdx.guannengcc.top

C#:   3.14159.ToString("F2")
来源：http://svb.tian-w.cn

[A22] 获取字符串长度
来源：http://zjq.hywenlv.cn

Py:   len(s)
来源：http://hfw.quarkkingdee.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ibu.xingfuxueyuan.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jex.ivvv.top

TS:   s.length
来源：http://bis.pengpengdd.cyou

Java: s.length()
来源：http://tey.ydzc1.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tya.tianlin.xyz

Ruby: s.length
来源：http://hyc.ppjwa.cn

C#:   s.Length
来源：http://dkr.uphjek.com

[A23] 大小写转换
来源：http://tea.yfazqb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://zsh.316326.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://let.jinghuilouyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://icb.nanxuanxn.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xvy.svipenyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ufe.zhixingplan.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ldw.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sov.hfpthk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nyo.nanxuanxn.top

[A24] 去除首尾空白
来源：http://myc.sxryk.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dwx.sufxvd.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kkp.zhoulong.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fdo.guowangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iyg.yanxiufei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ndl.jinghuilouyu.cn

Go:   strings.TrimSpace(s)
来源：http://mmi.cqqwz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://brr.wangshuangyany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://heq.aizwys.cn

[A25] 字符串比较
来源：http://txb.tanke756.top

Py:   s1 == s2; s1 != s2
来源：http://oul.mhx1999.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dlo.epnwcf.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bql.quarkkingdee.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tkl.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rox.tianlin.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kzl.hcnkem.com

Ruby: s1 == s2; s1 <=> s2
来源：http://bmc.guannengcc.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lwz.fanxiaobao.xyz

[A26] 类型转换总览
来源：http://igt.xylfe.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ire.ywan-chungtsiang.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zld.yj202588.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ypz.sxryk.cn

TS:   Number() String() Boolean() x as number
来源：http://wnh.yanxiufei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qjv.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zle.jiagoushi.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://yna.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://afi.yonumen.top

================================================================================
来源：http://qug.hywenlv.cn

B. 流程控制
来源：http://ubf.gzhubu.top

================================================================================
来源：http://xzv.meibo888.top

[B01] 条件判断 if / else
来源：http://ffj.andypj.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://abo.havefunace.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://psp.fanxiaobao.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yul.zhengqikj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mhz.sweek.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cxd.ehwqpu.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eoj.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://njk.tian-w.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hkn.hcnkem.com

[B02] 多分支 else if / elif
来源：http://mja.fktsv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dih.jyoumei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cux.ybcxt.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zvx.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ptp.gotoacloud.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://haq.yj202588.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iwi.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bai.ehwqpu.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sxs.epnwcf.com

[B03] switch / match / case
来源：http://nfk.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://znl.yj20258888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lbt.ivvv.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kql.gaohongyu789.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tpo.zhongyouzk.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ydu.vqdsnc.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xks.mhx1999.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aeg.aibaodan.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rpr.jinghuilouyu.cn

[B04] for 计数循环
来源：http://jpm.yj20258888.top

Py:   for i in range(10): print(i)
来源：http://ofz.snrcjt.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bvl.yvedp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xtf.shuidangran.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dft.andypj.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yen.feifeiyinyue.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://stf.xuetiantiany.cn

Ruby: 10.times { |i| puts i }
来源：http://qse.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aff.cdnleiting.top

[B05] 遍历数组 / 列表
来源：http://kcb.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://pjq.ehwqpu.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dei.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fdc.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ktw.redwolf501.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://noy.tarul.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wgm.ybcxt.top

Ruby: arr.each { |item| puts item }
来源：http://oof.nanxinkj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yuw.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://luf.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rux.0kj1m.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hfw.sweek.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kye.mhx1999.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mkk.jlsjyb.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://akz.gotoacloud.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://znr.hysaishi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pkt.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kmu.cucudq.cn

[B07] while 循环
来源：http://fyt.andypj.xyz

Py:   while i < 10: i += 1
来源：http://wco.shzxlz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mta.pengpengdd.cyou

JS:   while (i < 10) { i++; }
来源：http://lbv.hcnkem.com

TS:   while (i < 10) { i++; }
来源：http://ttr.xinyue.icu

Java: while (i < 10) { i++; }
来源：http://blj.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bab.jyoumei.cn

Ruby: while i < 10; i += 1; end
来源：http://avv.hongshengwenyu.top

C#:   while (i < 10) { i++; }
来源：http://xqj.chenjidiqi.icu

[B08] do-while（至少执行一次）
来源：http://kjo.aizwys.cn

Py:   # 无 do-while：用 while True + break
来源：http://jgx.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://hlk.xziqi.cn

JS:   do { i++; } while (i < 10);
来源：http://kjb.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://wjf.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://uwi.sysykeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qtr.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://krl.yj20258888.top

C#:   do { i++; } while (i < 10);
来源：http://quv.wangshuangyany.cn

[B09] break 与 continue
来源：http://ham.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bgd.cqqwz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://igj.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gyv.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uwo.hammf.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eul.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lbu.feifeiyinyue.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://scs.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dgr.316326.xyz

[B10] 遍历同时拿索引
来源：http://ayo.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uwf.uphjek.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ftg.tarul.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qac.yangfankeji.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gji.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://frl.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uvz.shangyingyoupin.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rku.aibaodan.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mkl.sufxvd.cn

[B11] 生成数字序列 / 区间
来源：http://pgx.smart0.xyz

Py:   list(range(0, 10, 2))
来源：http://lzd.ppjwa.cn

PHP:  range(0, 10, 2);
来源：http://oxc.hammf.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ray.shzxlz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kcn.zhaomingkeji.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dbh.xinyue.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hrl.yanxiufei.cn

Ruby: (0...10).step(2).to_a
来源：http://daq.hywenlv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://esn.zycfv.cn

[B12] 跳出多层循环
来源：http://nsr.bjfxy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vrl.9152youxi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rue.sweek.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cca.haohaochexian.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vmj.xingfuxueyuan.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hfe.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nvd.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sbp.shanyushiyangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cgk.yj20258.top

[B13] 判断是否为数字
来源：http://adq.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://cva.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://plb.uphjek.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oim.shuidangran.top


<!-- 参考信息 -->