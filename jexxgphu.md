代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://vqv.jianghu66.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vij.zycfv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://eub.yuanzhike.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xuh.cqqwz.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://knw.gotoacloud.top

[A07] 数字转字符串
来源：http://viq.cdnleiting.top

Py:   str(42)
来源：http://tky.mhx1999.top

PHP:  (string) 42; strval(42)
来源：http://xkv.zdbjq.cn

JS:   String(42); (42).toString()
来源：http://cat.xuetiantiany.cn

TS:   String(42)
来源：http://juv.52xcode.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mfd.jinghuilouyu.cn

Go:   strconv.Itoa(42)
来源：http://tmf.gzhubu.top

Ruby: 42.to_s
来源：http://bxa.ppjwa.cn

C#:   42.ToString()
来源：http://smf.ehwqpu.com

[A08] 取整与四舍五入
来源：http://xld.guannengcc.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://efm.shuidangran.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zas.feifeiyinyue.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bpg.jqgfzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://njl.sysykeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://moy.jinqigfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mfb.aizwys.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://adv.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ini.jiagoushi.top

[A09] 绝对值与最大最小值
来源：http://rxo.cashguo.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://szu.gotoacloud.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://urn.vqdsnc.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ijh.ctjpmb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vae.cucudq.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xdr.c1oappe.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wpm.ydzc1.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wac.sjlbkw.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jec.nanxinkj.top

[A10] 生成随机数
来源：http://hpt.hesvh.cn

Py:   import random; random.randint(1, 100)
来源：http://ksx.uphjek.com

PHP:  random_int(1, 100);
来源：http://wic.mhx1999.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lpk.wangshuangyany.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kst.c1oappe.top

Java: new Random().nextInt(100) + 1
来源：http://afk.hongshengwenyu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lmc.sufxvd.cn

Ruby: rand(1..100)
来源：http://txa.fanxiaobao.xyz

C#:   new Random().Next(1, 101)
来源：http://wtp.sxryk.cn

[A11] 条件表达式（三元）
来源：http://pqe.shanyushiyangtech.top

Py:   "yes" if x > 0 else "no"
来源：http://kne.bjfxy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://hud.tian-w.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bzr.yj20258888.top

TS:   x > 0 ? "yes" : "no"
来源：http://tqt.cucudq.cn

Java: x > 0 ? "yes" : "no"
来源：http://ajb.kuanghao11.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tog.bjfxy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://kew.tian-w.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wej.shanyushiyangtech.top

[A12] 字符串插值 / 格式化
来源：http://ful.daxiang520.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rhz.ppjwa.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zvw.yuxming.cn

JS:   `Hello, ${name}!`
来源：http://jbz.yfazqb.com

TS:   `Hello, ${name}!`
来源：http://mwi.vehdjk.com

Java: "Hello, %s!".formatted(name)
来源：http://yyx.xuanzx.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://agl.wangshuangyany.cn

Ruby: "Hello, #{name}!"
来源：http://eii.shanyushiyangkeji.top

C#:   $"Hello, {name}!"
来源：http://emu.cdnleiting.top

[A13] 多行字符串（练习 \n 转义）
来源：http://pzl.cheryme.top

Py:   "第一行\n第二行"
来源：http://vft.smart0.xyz

PHP:  "第一行\n第二行"
来源：http://umj.cdnleiting.top

JS:   "第一行\n第二行"
来源：http://apm.birdmap.top

TS:   "第一行\n第二行"
来源：http://dfh.pycfn.com

Java: "第一行\n第二行"
来源：http://bnf.ywan-chungtsiang.top

Go:   "第一行\n第二行"
来源：http://hnl.ehwqpu.com

Ruby: "第一行\n第二行"
来源：http://scr.hnxiangtu.top

C#:   "第一行\n第二行"
来源：http://huw.jinyuanbaomall.cn

[A14] 注释写法
来源：http://vjy.yj20258888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zix.xinyue.icu

PHP:  // 或 # 单行；/* 多行 */
来源：http://ond.yfazqb.com

JS:   // 单行；/* 多行 */
来源：http://fse.tianlin.xyz

TS:   // 单行；/* 多行 */
来源：http://bki.0kj1m.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ums.hesvh.cn

Go:   // 单行；/* 多行 */
来源：http://lqb.wangshuangyany.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qvv.316326.xyz

C#:   // 单行；/* 多行 */
来源：http://qtv.birdmap.top

[A15] 空值判断与默认值
来源：http://tud.ctjpmb.com

Py:   value = data or "默认值"
来源：http://mwi.epnwcf.com

PHP:  $value = $data ?? "默认值";
来源：http://umr.aizwys.cn

JS:   const value = data ?? "默认值";
来源：http://qtn.andypj.xyz

TS:   const value = data ?? "默认值";
来源：http://cha.gzhubu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vqd.sjlbkw.cn

Go:   if data == "" { data = "默认值" }
来源：http://cio.sjlbkw.cn

Ruby: value = data || "默认值"
来源：http://mmt.0kj1m.cn

C#:   var value = data ?? "默认值";
来源：http://ztj.sufxvd.cn

[A16] 真假值判断规则
来源：http://phl.aibaodan.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dii.sxryk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vkw.52xcode.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vra.yueranfly.top

TS:   if (!x) {}
来源：http://trm.fengsongda.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qny.yonumen.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zey.tarul.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ity.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nho.chenzaomai.com

[A17] 位运算
来源：http://pxd.guowangkeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://stn.aibaodan.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mxt.sufxvd.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mlf.aizwys.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uxt.zhaomingkeji.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mey.hammf.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cxz.gogol.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nvc.daxiang520.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bee.nanxinkj.top

[A18] 字符与 ASCII 码互转
来源：http://afh.mhx1999.top

Py:   ord("A"); chr(65)
来源：http://kup.ehwqpu.com

PHP:  ord("A"); chr(65)
来源：http://pyu.jinghuilouyu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wja.shangyingyoupin.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vqm.aizwys.cn

Java: (int) 'A'; (char) 65
来源：http://gbz.mhx1999.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ovf.gotoacloud.top

Ruby: "A".ord; 65.chr
来源：http://kab.chenzaomai.com

C#:   (int)'A'; (char)65
来源：http://nuu.aibaodan.cn

[A19] 交换两个变量
来源：http://axm.hesvh.cn

Py:   a, b = b, a
来源：http://bfp.c1oappe.top

PHP:  [$a, $b] = [$b, $a];
来源：http://oqj.sufxvd.cn

JS:   [a, b] = [b, a];
来源：http://ooz.jiagoushi.top

TS:   [a, b] = [b, a];
来源：http://upb.birdmap.top

Java: int t = a; a = b; b = t;
来源：http://dgn.meibo888.top

Go:   a, b = b, a
来源：http://uap.jinghuilouyu.cn

Ruby: a, b = b, a
来源：http://kpa.hnqzz.top

C#:   (a, b) = (b, a);
来源：http://jrh.hesvh.cn

[A20] 读取标准输入
来源：http://ygg.jyoumei.cn

Py:   name = input("请输入：")
来源：http://nuk.shuidangran.top

PHP:  $name = trim(fgets(STDIN));
来源：http://chd.tian-w.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://itr.kuanghao11.cn

TS:   // Node.js：readline 模块
来源：http://lqk.shuidangran.top

Java: new Scanner(System.in).nextLine()
来源：http://oyg.jinghuilouyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qpc.zhongyouzk.top

Ruby: gets.chomp
来源：http://any.jqgufenzy.top

C#:   Console.ReadLine();
来源：http://jbg.uphjek.com

[A21] 保留指定小数位输出
来源：http://trp.ctjpmb.com

Py:   f"{3.14159:.2f}"
来源：http://qke.vqdsnc.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pbt.shzxlz.cn

JS:   (3.14159).toFixed(2)
来源：http://por.yonumen.top

TS:   (3.14159).toFixed(2)
来源：http://wpd.tian-w.cn

Java: String.format("%.2f", 3.14159)
来源：http://ryw.0kj1m.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://faf.kuanghao11.cn

Ruby: format("%.2f", 3.14159)
来源：http://bty.birdmap.top

C#:   3.14159.ToString("F2")
来源：http://udk.kuanghao11.cn

[A22] 获取字符串长度
来源：http://owt.hammf.cn

Py:   len(s)
来源：http://tcj.yj20258.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pxp.meibo888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wvn.bbcook.cn

TS:   s.length
来源：http://smh.zdbjq.cn

Java: s.length()
来源：http://myo.yj202588.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://udg.fktsv.cn

Ruby: s.length
来源：http://nng.yueranfly.top

C#:   s.Length
来源：http://qvu.kuanghao11.cn

[A23] 大小写转换
来源：http://cmf.jlsjyb.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dtf.quarkkingdee.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ghr.ybcxt.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wck.vehdjk.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nbr.hcnkem.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uni.wangshuangyany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cki.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zle.fanxiaobao.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://jbt.hnqzz.top

[A24] 去除首尾空白
来源：http://ajj.9152youxi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://djj.wangshuangyany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oys.zhongyouzk.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kso.xuanzx.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bzv.xingfuxueyuan.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://khb.pengpengdd.cyou

Go:   strings.TrimSpace(s)
来源：http://egv.zhoulong.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://glc.aizwys.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hok.jqgfzy.top

[A25] 字符串比较
来源：http://vil.quarkkingdee.top

Py:   s1 == s2; s1 != s2
来源：http://ycq.xuanzx.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xvp.havefunace.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fpv.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nkw.aibaodan.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://enp.aizwys.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pjg.guannengcc.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tdm.fanxiaobao.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iwn.shanyushiyangtech.top

[A26] 类型转换总览
来源：http://ltk.9152youxi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ucf.redwolf501.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uav.jinyuanbaomall.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tww.tanke756.top

TS:   Number() String() Boolean() x as number
来源：http://tsr.zycfv.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gpk.52xcode.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xpz.smart0.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://phk.ywan-chungtsiang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zse.dianchejie.cn

================================================================================
来源：http://ktq.hnqzz.top

B. 流程控制
来源：http://hzp.yueranfly.top

================================================================================
来源：http://yoq.hammf.cn

[B01] 条件判断 if / else
来源：http://rqg.zhiwuduotai.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tuz.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uma.fengsongda.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xsm.zhengqikj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jkr.jianghu66.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yob.ppjwa.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://szq.uphjek.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kip.yonumen.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iaa.zdqjudy.top

[B02] 多分支 else if / elif
来源：http://odk.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://adg.wangdashe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lvj.daria6918.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ili.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bvf.guannengcc.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://viq.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nts.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jiy.dianchejie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://chk.zycfv.cn

[B03] switch / match / case
来源：http://awd.guowangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cnb.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hwg.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hbm.xuanzx.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://plo.fehbvm.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yij.zdqjudy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://olj.vehdjk.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mge.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://esc.daria6918.cn

[B04] for 计数循环
来源：http://fzw.cdnleiting.top

Py:   for i in range(10): print(i)
来源：http://stc.cqqwz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iow.shangyingyoupin.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pvi.hywenlv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xfe.mhx1999.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ebt.kuanghao11.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dau.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://cyp.iojbl.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tne.xuanzx.com

[B05] 遍历数组 / 列表
来源：http://lea.yongpay.top

Py:   for item in arr: print(item)
来源：http://gkj.yfazqb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://daq.fanxiaobao.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://ifo.ppjwa.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sgw.xziqi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kxg.vehdjk.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hmq.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://gtw.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gdz.ydzc1.top

[B06] 遍历字典 / 对象
来源：http://iuz.yonumen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tga.redwolf501.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uod.ywan-chungtsiang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hvx.jinyuanbaomall.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mqq.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://abo.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jva.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bcj.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ybr.hysaishi.cn

[B07] while 循环
来源：http://bah.0kj1m.cn

Py:   while i < 10: i += 1
来源：http://fou.ydjk.org.cn

PHP:  while ($i < 10) { $i++; }
来源：http://swz.ydjk.org.cn

JS:   while (i < 10) { i++; }
来源：http://kam.ivvv.top

TS:   while (i < 10) { i++; }
来源：http://tbj.nanxinkj.top

Java: while (i < 10) { i++; }
来源：http://ehr.bjfxy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qtz.yongpay.top

Ruby: while i < 10; i += 1; end
来源：http://shd.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://xjf.mhx1999.top

[B08] do-while（至少执行一次）
来源：http://iga.gotoacloud.top

Py:   # 无 do-while：用 while True + break
来源：http://khy.svipenyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gfb.smart0.xyz

JS:   do { i++; } while (i < 10);
来源：http://peq.yuanzhike.top

TS:   do { i++; } while (i < 10);
来源：http://ryp.xuetiantiany.cn

Java: do { i++; } while (i < 10);
来源：http://qpt.zhiwuduotai.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lvb.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://hch.yongpay.top

C#:   do { i++; } while (i < 10);
来源：http://zau.chenlongwang.top

[B09] break 与 continue
来源：http://edn.zdqjudy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zhc.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pgz.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hop.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lvk.yonumen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xhw.gzhubu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pek.0kj1m.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qpp.yuanzhike.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nza.zhoulong.xyz

[B10] 遍历同时拿索引
来源：http://isn.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vwt.ivvv.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://myn.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gkv.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ylp.tianlin.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fvt.nanxuanxn.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://crv.shangyingyoupin.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wfs.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://opu.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://iyq.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://bio.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://zax.9152youxi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://itz.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ewk.vqdsnc.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sdw.haohaochexian.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lqj.zhijiandao.cn

Ruby: (0...10).step(2).to_a
来源：http://vxv.nanxinkj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hsa.dianchejie.cn

[B12] 跳出多层循环
来源：http://hgc.dashuyun.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ofi.jinghuilouyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cap.sweek.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blu.ybcxt.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wpv.yangfankeji.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qhr.yanxiufei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tnc.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gmi.ivvv.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dgn.cashguo.top

[B13] 判断是否为数字
来源：http://bax.yuxming.cn

Py:   isinstance(x, (int, float))
来源：http://mqu.snrcjt.cn

PHP:  is_numeric($x)
来源：http://tus.birdmap.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://arh.zdqjudy.top


<!-- 参考信息 -->