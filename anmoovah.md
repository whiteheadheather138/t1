代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://xxt.yanxiufei.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dhs.fanxiaobao.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dnc.yfazqb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://obf.meibo888.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gul.nanxinkj.top

[A07] 数字转字符串
来源：http://wsp.gzhubu.top

Py:   str(42)
来源：http://azo.zhoulong.xyz

PHP:  (string) 42; strval(42)
来源：http://jdd.daxiang520.top

JS:   String(42); (42).toString()
来源：http://ocz.yj20258888.top

TS:   String(42)
来源：http://owq.hnxiangtu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://cwt.chenjidiqi.icu

Go:   strconv.Itoa(42)
来源：http://cfl.fengsongda.top

Ruby: 42.to_s
来源：http://maf.yj20258.top

C#:   42.ToString()
来源：http://tto.svipenyu.cn

[A08] 取整与四舍五入
来源：http://ccn.pengpengdd.cyou

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lgw.gaohongyu789.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kkm.sjlbkw.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lek.mhx1999.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://thu.0kj1m.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mte.yanxiufei.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mxo.zhixingplan.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://qcf.jqgfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lgs.gogol.net.cn

[A09] 绝对值与最大最小值
来源：http://ebo.xylfe.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rnu.daria6918.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://naf.cashguo.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ltu.52xcode.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vje.gogol.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jyl.snrcjt.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vth.sweek.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tts.kuanghao11.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uoy.smart0.xyz

[A10] 生成随机数
来源：http://dtg.shanyushiyangkeji.top

Py:   import random; random.randint(1, 100)
来源：http://cqx.cqqwz.cn

PHP:  random_int(1, 100);
来源：http://ung.sufxvd.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ubl.zhoulong.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yqe.svipenyu.cn

Java: new Random().nextInt(100) + 1
来源：http://vnz.jinghuilouyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ymv.tanke756.top

Ruby: rand(1..100)
来源：http://wqv.jianghu66.top

C#:   new Random().Next(1, 101)
来源：http://thp.yangfankeji.com

[A11] 条件表达式（三元）
来源：http://vkr.ydzc1.top

Py:   "yes" if x > 0 else "no"
来源：http://deb.guannengcc.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://fcv.xuetiantiany.cn

JS:   x > 0 ? "yes" : "no"
来源：http://owp.yj20258888.top

TS:   x > 0 ? "yes" : "no"
来源：http://xfq.quarkkingdee.top

Java: x > 0 ? "yes" : "no"
来源：http://dvi.jiagoushi.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gpe.hysaishi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pcg.redwolf501.top

C#:   x > 0 ? "yes" : "no"
来源：http://erb.aizwys.cn

[A12] 字符串插值 / 格式化
来源：http://nff.jlsjyb.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ehf.52xcode.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wzz.hesvh.cn

JS:   `Hello, ${name}!`
来源：http://rww.yj20258888.top

TS:   `Hello, ${name}!`
来源：http://fci.fanxiaobao.xyz

Java: "Hello, %s!".formatted(name)
来源：http://rzv.tian-w.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yay.zhixingplan.top

Ruby: "Hello, #{name}!"
来源：http://kbq.chenjidiqi.icu

C#:   $"Hello, {name}!"
来源：http://hdh.pengpengdd.cyou

[A13] 多行字符串（练习 \n 转义）
来源：http://wsb.smart0.xyz

Py:   "第一行\n第二行"
来源：http://pyd.ctjpmb.com

PHP:  "第一行\n第二行"
来源：http://bpu.xinyue.icu

JS:   "第一行\n第二行"
来源：http://jxb.jinqigfzy.top

TS:   "第一行\n第二行"
来源：http://ehv.sxryk.cn

Java: "第一行\n第二行"
来源：http://wui.guowangkeji.top

Go:   "第一行\n第二行"
来源：http://mwz.yueranfly.top

Ruby: "第一行\n第二行"
来源：http://pyl.vqdsnc.cn

C#:   "第一行\n第二行"
来源：http://ahm.ivvv.top

[A14] 注释写法
来源：http://oyt.fzhhl.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://nzn.yj20258.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pmw.yanxiufei.cn

JS:   // 单行；/* 多行 */
来源：http://tbx.yongpay.top

TS:   // 单行；/* 多行 */
来源：http://hnn.yj20258.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zce.zhiwuduotai.top

Go:   // 单行；/* 多行 */
来源：http://aqs.ctjpmb.com

Ruby: # 单行；=begin 多行 =end
来源：http://eef.hnxiangtu.top

C#:   // 单行；/* 多行 */
来源：http://tjy.ywan-chungtsiang.top

[A15] 空值判断与默认值
来源：http://pvt.cucudq.cn

Py:   value = data or "默认值"
来源：http://lxs.ehwqpu.com

PHP:  $value = $data ?? "默认值";
来源：http://rzy.hammf.cn

JS:   const value = data ?? "默认值";
来源：http://qyc.shangyingyoupin.top

TS:   const value = data ?? "默认值";
来源：http://wsx.fengsongda.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://act.zhixingplan.top

Go:   if data == "" { data = "默认值" }
来源：http://hfi.c1oappe.top

Ruby: value = data || "默认值"
来源：http://cdv.ywan-chungtsiang.top

C#:   var value = data ?? "默认值";
来源：http://vuo.yuxming.cn

[A16] 真假值判断规则
来源：http://zha.jqgfzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oko.ehwqpu.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fcj.andypj.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ycx.hongshengwenyu.top

TS:   if (!x) {}
来源：http://rsi.zycfv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xxz.yfazqb.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iad.jinqigufen.top

Ruby: unless x            # nil 与 false 为假
来源：http://eef.aibaodan.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lfy.cashguo.top

[A17] 位运算
来源：http://ewm.sweek.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kzu.zhengqikj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mfo.bjfxy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://evw.hesvh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://efn.zhiwuduotai.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ugx.jlsjyb.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rhg.hnqzz.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ije.xingfuxueyuan.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eyl.ydzc1.top

[A18] 字符与 ASCII 码互转
来源：http://tlr.ywan-chungtsiang.top

Py:   ord("A"); chr(65)
来源：http://gfe.0kj1m.cn

PHP:  ord("A"); chr(65)
来源：http://jti.hysaishi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vks.zhengqikj.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yaz.jinghuilouyu.cn

Java: (int) 'A'; (char) 65
来源：http://lkt.yangfankeji.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mab.zhixingplan.top

Ruby: "A".ord; 65.chr
来源：http://pcz.shanyushiyangtech.top

C#:   (int)'A'; (char)65
来源：http://qlr.jqgufenzy.top

[A19] 交换两个变量
来源：http://mmd.jqgfzy.top

Py:   a, b = b, a
来源：http://zgk.yangfankeji.com

PHP:  [$a, $b] = [$b, $a];
来源：http://wvg.nwbrower.top

JS:   [a, b] = [b, a];
来源：http://oqo.sufxvd.cn

TS:   [a, b] = [b, a];
来源：http://cyj.ehwqpu.com

Java: int t = a; a = b; b = t;
来源：http://hqe.hfpthk.cn

Go:   a, b = b, a
来源：http://bah.feifeiyinyue.top

Ruby: a, b = b, a
来源：http://ksw.vehdjk.com

C#:   (a, b) = (b, a);
来源：http://ttw.cucudq.cn

[A20] 读取标准输入
来源：http://ghn.zhijiandao.cn

Py:   name = input("请输入：")
来源：http://oxd.birdmap.top

PHP:  $name = trim(fgets(STDIN));
来源：http://olo.tianlin.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mdp.hnqzz.top

TS:   // Node.js：readline 模块
来源：http://lxw.dashuyun.cn

Java: new Scanner(System.in).nextLine()
来源：http://bln.chenjidiqi.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ajd.ivvv.top

Ruby: gets.chomp
来源：http://nzt.yj20258.top

C#:   Console.ReadLine();
来源：http://wmg.jinghuilouyu.cn

[A21] 保留指定小数位输出
来源：http://sbf.ctjpmb.com

Py:   f"{3.14159:.2f}"
来源：http://orf.svipenyu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dzn.gotoacloud.top

JS:   (3.14159).toFixed(2)
来源：http://uoe.tianlin.xyz

TS:   (3.14159).toFixed(2)
来源：http://xda.xinyue.icu

Java: String.format("%.2f", 3.14159)
来源：http://kjl.ybcxt.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ioq.zhongyouzk.top

Ruby: format("%.2f", 3.14159)
来源：http://qle.gzhubu.top

C#:   3.14159.ToString("F2")
来源：http://dna.wangdashe.top

[A22] 获取字符串长度
来源：http://hya.ydzc1.top

Py:   len(s)
来源：http://gme.wangdashe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nat.vehdjk.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://buu.guowangkeji.top

TS:   s.length
来源：http://vji.zdbjq.cn

Java: s.length()
来源：http://lpf.bbcook.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dlc.ydjk.org.cn

Ruby: s.length
来源：http://ttj.zhijiandao.cn

C#:   s.Length
来源：http://voe.fzhhl.top

[A23] 大小写转换
来源：http://udv.chenzaomai.com

Py:   s.upper(); s.lower(); s.title()
来源：http://jfy.shzxlz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gdy.aibaodan.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bww.nanxinkj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dtr.xuanzx.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gls.sufxvd.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dln.zhongyouzk.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://emu.birdmap.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ntu.pycfn.com

[A24] 去除首尾空白
来源：http://lhi.jqgfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vag.yuanzhike.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://srz.guannengcc.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jdc.yongpay.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ish.jqgfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oto.iojbl.cn

Go:   strings.TrimSpace(s)
来源：http://kff.fengsongda.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xey.yuanzhike.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iqy.wangdashe.top

[A25] 字符串比较
来源：http://jyv.shanyushiyangkeji.top

Py:   s1 == s2; s1 != s2
来源：http://yfy.epnwcf.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sar.yueranfly.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gdw.dashuyun.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dou.uphjek.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gup.hesvh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ygz.yvedp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kxu.guannengcc.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tbo.c1oappe.top

[A26] 类型转换总览
来源：http://izi.zdqjudy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sam.shanyushiyangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qgt.hcnkem.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qmi.shangyingyoupin.top

TS:   Number() String() Boolean() x as number
来源：http://wkl.yj20258.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wik.zycfv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jcx.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zpf.ctjpmb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://moc.sjlbkw.cn

================================================================================
来源：http://vdc.ehwqpu.com

B. 流程控制
来源：http://mve.jianghu66.top

================================================================================
来源：http://grd.chenzaomai.com

[B01] 条件判断 if / else
来源：http://pkl.sxryk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ytb.fanxiaobao.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yju.yueranfly.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ocj.zhijiandao.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bvb.jinqigfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tbk.shzxlz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://emo.hfpthk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vsb.hysaishi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vwg.316326.xyz

[B02] 多分支 else if / elif
来源：http://znc.fehbvm.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kjg.jinyuanbaomall.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://che.316326.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xjp.ctjpmb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nsz.vqdsnc.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xwk.chenjidiqi.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ryh.shanyushiyangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iqb.yj20258.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dap.zhiwuduotai.top

[B03] switch / match / case
来源：http://fch.smart0.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gbq.nwbrower.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qmz.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://swj.fktsv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kzu.xuetiantiany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tit.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nug.hysaishi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jfy.kuanghao11.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wyk.snrcjt.cn

[B04] for 计数循环
来源：http://ebr.wangshuangyany.cn

Py:   for i in range(10): print(i)
来源：http://pfx.redwolf501.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vpb.zhongyouzk.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dml.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zau.jinghuilouyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xlm.fzhhl.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://akb.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://vkb.sysykeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blc.hcnkem.com

[B05] 遍历数组 / 列表
来源：http://prp.yanxiufei.cn

Py:   for item in arr: print(item)
来源：http://xjv.shangyingyoupin.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ybz.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rcz.fktsv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://squ.zdqjudy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hcc.9152youxi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ahp.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://ssw.uphjek.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mvh.aizwys.cn

[B06] 遍历字典 / 对象
来源：http://tuw.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wmo.dashuyun.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uii.9152youxi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ozg.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qpc.yj202588.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zgi.shanyushiyangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mtl.jlsjyb.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ngx.zhaomingkeji.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qtv.wangdashe.top

[B07] while 循环
来源：http://xnq.birdmap.top

Py:   while i < 10: i += 1
来源：http://mtu.andypj.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ebv.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://gjp.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://muu.yongpay.top

Java: while (i < 10) { i++; }
来源：http://rhl.hesvh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cbb.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://zoy.xuetiantiany.cn

C#:   while (i < 10) { i++; }
来源：http://lgy.fktsv.cn

[B08] do-while（至少执行一次）
来源：http://djt.jinqigufen.top

Py:   # 无 do-while：用 while True + break
来源：http://kvv.yfazqb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://res.yangfankeji.com

JS:   do { i++; } while (i < 10);
来源：http://tdc.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://gyu.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://txb.bjfxy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vzg.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vce.havefunace.top

C#:   do { i++; } while (i < 10);
来源：http://qva.jqgufenzy.top

[B09] break 与 continue
来源：http://dsv.yonumen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kil.fanxiaobao.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oze.shanyushiyangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ucx.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zuy.feifeiyinyue.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wfz.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zqy.hongshengwenyu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yij.jinghuilouyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jbx.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://gfe.fzhhl.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qzg.mhx1999.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uxi.svipenyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://prs.jiagoushi.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://upp.epnwcf.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rtb.zhaomingkeji.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pkc.c1oappe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hra.zhaomingkeji.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://njm.tarul.cn

[B11] 生成数字序列 / 区间
来源：http://yig.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://fnh.dashuyun.cn

PHP:  range(0, 10, 2);
来源：http://jwd.yvedp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ezm.jyoumei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mrh.dianchejie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pxj.yuxming.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://szm.jyoumei.cn

Ruby: (0...10).step(2).to_a
来源：http://jhb.ctjpmb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kgo.fzhhl.top

[B12] 跳出多层循环
来源：http://key.fanxiaobao.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://tfs.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rij.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dov.316326.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rsn.nanxinkj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vaz.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eqi.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lds.guannengcc.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hzy.cucudq.cn

[B13] 判断是否为数字
来源：http://pcs.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://ert.yj20258.top

PHP:  is_numeric($x)
来源：http://iot.zycfv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tww.xuanzx.com


<!-- 参考信息 -->