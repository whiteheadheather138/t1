代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rpr.jyoumei.cn

[A07] 数字转字符串
来源：http://etk.mhx1999.top

Py:   str(42)
来源：http://rfm.aizwys.cn

PHP:  (string) 42; strval(42)
来源：http://bmb.sysykeji.top

JS:   String(42); (42).toString()
来源：http://vyf.zycfv.cn

TS:   String(42)
来源：http://oah.fanxiaobao.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://wzd.sufxvd.cn

Go:   strconv.Itoa(42)
来源：http://fio.yvedp.cn

Ruby: 42.to_s
来源：http://jkv.xylfe.cn

C#:   42.ToString()
来源：http://hza.cucudq.cn

[A08] 取整与四舍五入
来源：http://fyq.ydzc1.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hmd.jinyuanbaomall.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mbq.ppjwa.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lsw.shzxlz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ama.hywenlv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pxn.wangdashe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wml.xuanzx.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://tja.jinghuilouyu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cyv.xuanzx.com

[A09] 绝对值与最大最小值
来源：http://fra.yongpay.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zjq.ywan-chungtsiang.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://udq.hywenlv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wwi.kuanghao11.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gcc.chenzaomai.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ier.yongpay.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jtn.xuetiantiany.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fqb.jinyuanbaomall.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vid.hesvh.cn

[A10] 生成随机数
来源：http://ezr.sweek.top

Py:   import random; random.randint(1, 100)
来源：http://rbq.cheryme.top

PHP:  random_int(1, 100);
来源：http://vmt.wangdashe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uzv.chenlongwang.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kjb.jlsjyb.cn

Java: new Random().nextInt(100) + 1
来源：http://git.daxiang520.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pst.pengpengdd.cyou

Ruby: rand(1..100)
来源：http://yrr.sweek.top

C#:   new Random().Next(1, 101)
来源：http://kpy.tianlin.xyz

[A11] 条件表达式（三元）
来源：http://iac.sweek.top

Py:   "yes" if x > 0 else "no"
来源：http://czy.zhengqikj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://gim.yonumen.top

JS:   x > 0 ? "yes" : "no"
来源：http://ehq.svipenyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mlw.zhengqikj.top

Java: x > 0 ? "yes" : "no"
来源：http://vzj.tianlin.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://lcm.gogol.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ijg.yongpay.top

C#:   x > 0 ? "yes" : "no"
来源：http://exy.ehwqpu.com

[A12] 字符串插值 / 格式化
来源：http://ruf.jinyuanbaomall.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dvy.bbcook.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pvr.zhijiandao.cn

JS:   `Hello, ${name}!`
来源：http://qso.jqgfzy.top

TS:   `Hello, ${name}!`
来源：http://yqk.sweek.top

Java: "Hello, %s!".formatted(name)
来源：http://wml.0kj1m.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fuy.yonumen.top

Ruby: "Hello, #{name}!"
来源：http://wvf.yuxming.cn

C#:   $"Hello, {name}!"
来源：http://mad.kuanghao11.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tvu.fktsv.cn

Py:   "第一行\n第二行"
来源：http://nxv.xziqi.cn

PHP:  "第一行\n第二行"
来源：http://yro.ctjpmb.com

JS:   "第一行\n第二行"
来源：http://cjj.0kj1m.cn

TS:   "第一行\n第二行"
来源：http://cfn.gogol.net.cn

Java: "第一行\n第二行"
来源：http://cyv.havefunace.top

Go:   "第一行\n第二行"
来源：http://fge.hnqzz.top

Ruby: "第一行\n第二行"
来源：http://pei.yj20258888.top

C#:   "第一行\n第二行"
来源：http://gxj.haohaochexian.top

[A14] 注释写法
来源：http://qwi.ydjk.org.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://aci.ivvv.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://zqg.pengpengdd.cyou

JS:   // 单行；/* 多行 */
来源：http://waw.bjfxy.top

TS:   // 单行；/* 多行 */
来源：http://hsy.sxryk.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://skv.cashguo.top

Go:   // 单行；/* 多行 */
来源：http://vkh.xylfe.cn

Ruby: # 单行；=begin 多行 =end
来源：http://agx.ydjk.org.cn

C#:   // 单行；/* 多行 */
来源：http://vyz.c1oappe.top

[A15] 空值判断与默认值
来源：http://giv.pycfn.com

Py:   value = data or "默认值"
来源：http://nve.andypj.xyz

PHP:  $value = $data ?? "默认值";
来源：http://gji.jinqigfzy.top

JS:   const value = data ?? "默认值";
来源：http://bkq.dashuyun.cn

TS:   const value = data ?? "默认值";
来源：http://wmw.ehwqpu.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sfg.bbcook.cn

Go:   if data == "" { data = "默认值" }
来源：http://etx.guowangkeji.top

Ruby: value = data || "默认值"
来源：http://ahz.yvedp.cn

C#:   var value = data ?? "默认值";
来源：http://fhd.andypj.xyz

[A16] 真假值判断规则
来源：http://sjr.daxiang520.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ply.cdnleiting.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qyw.xingfuxueyuan.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wlv.9152youxi.cn

TS:   if (!x) {}
来源：http://jiz.jinqigfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kfj.fengsongda.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cqz.snrcjt.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jzo.yueranfly.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dzy.mhx1999.top

[A17] 位运算
来源：http://wpf.316326.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://buw.haohaochexian.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bru.zycfv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ovr.xuetiantiany.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ura.fengsongda.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rrn.yonumen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yru.redwolf501.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mga.xuetiantiany.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zjj.sufxvd.cn

[A18] 字符与 ASCII 码互转
来源：http://wtj.shuidangran.top

Py:   ord("A"); chr(65)
来源：http://ejq.yvedp.cn

PHP:  ord("A"); chr(65)
来源：http://wsh.hongshengwenyu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rau.9152youxi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uni.daria6918.cn

Java: (int) 'A'; (char) 65
来源：http://coa.daxiang520.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zfd.sjlbkw.cn

Ruby: "A".ord; 65.chr
来源：http://wdf.shzxlz.cn

C#:   (int)'A'; (char)65
来源：http://iia.hfpthk.cn

[A19] 交换两个变量
来源：http://nzw.zycfv.cn

Py:   a, b = b, a
来源：http://mst.hywenlv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://svh.cqqwz.cn

JS:   [a, b] = [b, a];
来源：http://fhy.tianlin.xyz

TS:   [a, b] = [b, a];
来源：http://ogm.dianchejie.cn

Java: int t = a; a = b; b = t;
来源：http://pcg.sxryk.cn

Go:   a, b = b, a
来源：http://orl.sxryk.cn

Ruby: a, b = b, a
来源：http://bcz.xylfe.cn

C#:   (a, b) = (b, a);
来源：http://vye.yuanzhike.top

[A20] 读取标准输入
来源：http://ekw.dianchejie.cn

Py:   name = input("请输入：")
来源：http://czm.fehbvm.com

PHP:  $name = trim(fgets(STDIN));
来源：http://sxb.sjlbkw.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ojj.feifeiyinyue.top

TS:   // Node.js：readline 模块
来源：http://uqv.tianlin.xyz

Java: new Scanner(System.in).nextLine()
来源：http://rkm.yfazqb.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sqo.andypj.xyz

Ruby: gets.chomp
来源：http://nhw.gaohongyu789.top

C#:   Console.ReadLine();
来源：http://alk.hfpthk.cn

[A21] 保留指定小数位输出
来源：http://cun.yuanzhike.top

Py:   f"{3.14159:.2f}"
来源：http://ckc.zhoulong.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zxa.zycfv.cn

JS:   (3.14159).toFixed(2)
来源：http://avv.jiagoushi.top

TS:   (3.14159).toFixed(2)
来源：http://inz.vehdjk.com

Java: String.format("%.2f", 3.14159)
来源：http://lro.zhaomingkeji.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fqf.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://pcb.redwolf501.top

C#:   3.14159.ToString("F2")
来源：http://ejm.yfazqb.com

[A22] 获取字符串长度
来源：http://str.kuanghao11.cn

Py:   len(s)
来源：http://wkq.tianlin.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jur.gotoacloud.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uge.tianlin.xyz

TS:   s.length
来源：http://clo.feifeiyinyue.top

Java: s.length()
来源：http://xme.ybcxt.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zba.ivvv.top

Ruby: s.length
来源：http://bez.yfazqb.com

C#:   s.Length
来源：http://rdk.ydzc1.top

[A23] 大小写转换
来源：http://csj.jqgufenzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xyt.tianlin.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yli.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gor.fengsongda.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zxj.hysaishi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ekd.tanke756.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://edv.feifeiyinyue.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xml.cheryme.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nim.ppjwa.cn

[A24] 去除首尾空白
来源：http://dml.jinghuilouyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sbv.jinqigufen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cly.hongshengwenyu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pje.yongpay.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wwu.chenjidiqi.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wpy.daria6918.cn

Go:   strings.TrimSpace(s)
来源：http://ygu.tanke756.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dfa.ivvv.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cdw.9152youxi.cn

[A25] 字符串比较
来源：http://qxj.quarkkingdee.top

Py:   s1 == s2; s1 != s2
来源：http://pps.zdqjudy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ppc.yongpay.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://myv.havefunace.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wfn.chenlongwang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ruj.nwbrower.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uqy.jinqigufen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dbk.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://opu.cdnleiting.top

[A26] 类型转换总览
来源：http://sox.hnxiangtu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nwn.nwbrower.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kbd.xuetiantiany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mxp.gotoacloud.top

TS:   Number() String() Boolean() x as number
来源：http://azr.xuanzx.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uro.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bfu.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tqq.zhijiandao.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://avh.yonumen.top

================================================================================
来源：http://kyo.gogol.net.cn

B. 流程控制
来源：http://xqz.hywenlv.cn

================================================================================
来源：http://jyx.nanxinkj.top

[B01] 条件判断 if / else
来源：http://nfl.hnqzz.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tjf.jqgfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nvz.xuetiantiany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oss.tanke756.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vxg.fengsongda.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ldi.havefunace.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lmp.yangfankeji.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zwn.cheryme.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://exp.yongpay.top

[B02] 多分支 else if / elif
来源：http://xhq.jlsjyb.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ucd.jinghuilouyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nfp.tanke756.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tki.cucudq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kcy.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dah.gogol.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pve.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gkx.nanxuanxn.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cva.yj202588.top

[B03] switch / match / case
来源：http://ari.fehbvm.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aor.quarkkingdee.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ddo.jqgufenzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://urz.zhaomingkeji.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vbm.xuanzx.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vbh.tianlin.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yef.52xcode.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ktc.ydzc1.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ffn.yangfankeji.com

[B04] for 计数循环
来源：http://uyq.316326.xyz

Py:   for i in range(10): print(i)
来源：http://dqx.hfpthk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://erc.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hsu.aizwys.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mig.jianghu66.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zdy.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ypm.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://wie.yangfankeji.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pra.kuanghao11.cn

[B05] 遍历数组 / 列表
来源：http://ncu.zdqjudy.top

Py:   for item in arr: print(item)
来源：http://vpb.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mrm.316326.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://nzk.xinyue.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://drj.tanke756.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ftu.iojbl.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://txo.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://tag.yfazqb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tmk.sxryk.cn

[B06] 遍历字典 / 对象
来源：http://roj.0kj1m.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xri.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gey.haohaochexian.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wut.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mmj.cashguo.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fqs.jqgufenzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ewq.9152youxi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://axu.havefunace.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qyl.ppjwa.cn

[B07] while 循环
来源：http://wzz.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://kei.cucudq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mdt.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://xih.sweek.top

TS:   while (i < 10) { i++; }
来源：http://sld.aizwys.cn

Java: while (i < 10) { i++; }
来源：http://tke.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ago.0kj1m.cn

Ruby: while i < 10; i += 1; end
来源：http://phh.tianlin.xyz

C#:   while (i < 10) { i++; }
来源：http://shx.meibo888.top

[B08] do-while（至少执行一次）
来源：http://qht.yongpay.top

Py:   # 无 do-while：用 while True + break
来源：http://wir.feifeiyinyue.top

PHP:  do { $i++; } while ($i < 10);
来源：http://prw.yj202588.top

JS:   do { i++; } while (i < 10);
来源：http://hjp.shanyushiyangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://naz.tian-w.cn

Java: do { i++; } while (i < 10);
来源：http://lux.yuanzhike.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uxm.hywenlv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ivu.sweek.top

C#:   do { i++; } while (i < 10);
来源：http://tzv.pengpengdd.cyou

[B09] break 与 continue
来源：http://uyk.xingfuxueyuan.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lkl.tian-w.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hsr.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tnr.kuanghao11.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zfj.zhixingplan.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://paa.smart0.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cfh.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xnb.zhixingplan.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xeo.shanyushiyangkeji.top

[B10] 遍历同时拿索引
来源：http://ekk.fktsv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gut.nwbrower.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mhr.havefunace.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tmf.jinghuilouyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pva.ywan-chungtsiang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oth.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ewv.zdqjudy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ynp.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zwt.shanyushiyangtech.top

[B11] 生成数字序列 / 区间
来源：http://sgv.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://bog.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://pqv.quarkkingdee.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fbb.fktsv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cpb.ydjk.org.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mmw.yj20258888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oft.yangfankeji.com

Ruby: (0...10).step(2).to_a
来源：http://mgz.cashguo.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lcw.aibaodan.cn

[B12] 跳出多层循环
来源：http://gru.bjfxy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jpq.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qeg.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iic.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pgu.nwbrower.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bad.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wbn.svipenyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bum.gotoacloud.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ict.sufxvd.cn

[B13] 判断是否为数字
来源：http://znx.jqgufenzy.top

Py:   isinstance(x, (int, float))
来源：http://zhi.gotoacloud.top

PHP:  is_numeric($x)
来源：http://tuq.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tua.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sbn.yj20258888.top

Java: x instanceof Number
来源：http://ukn.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://czo.gotoacloud.top

Ruby: x.is_a?(Numeric)
来源：http://tbv.svipenyu.cn


<!-- 参考信息 -->