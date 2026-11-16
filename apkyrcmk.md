代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lxj.meibo888.top

[A07] 数字转字符串
来源：http://gbx.yfazqb.com

Py:   str(42)
来源：http://tuf.meibo888.top

PHP:  (string) 42; strval(42)
来源：http://hmx.xinyue.icu

JS:   String(42); (42).toString()
来源：http://cix.yj20258888.top

TS:   String(42)
来源：http://dnm.xylfe.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vwr.bbcook.cn

Go:   strconv.Itoa(42)
来源：http://zly.tian-w.cn

Ruby: 42.to_s
来源：http://qyf.hnxiangtu.top

C#:   42.ToString()
来源：http://psp.9152youxi.cn

[A08] 取整与四舍五入
来源：http://oul.fzhhl.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jla.yfazqb.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wgh.xingfuxueyuan.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jax.yuxming.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://svg.hnqzz.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://eka.zhongyouzk.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pjc.kuanghao11.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tdr.hammf.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yhl.xuanzx.com

[A09] 绝对值与最大最小值
来源：http://emn.shuidangran.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hob.vehdjk.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dom.wangdashe.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://czw.dianchejie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oya.nanxuanxn.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mux.sufxvd.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lox.zhixingplan.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nmy.xuanzx.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xyo.xuanzx.com

[A10] 生成随机数
来源：http://mvr.tianlin.xyz

Py:   import random; random.randint(1, 100)
来源：http://vhv.hongshengwenyu.top

PHP:  random_int(1, 100);
来源：http://wkk.yongpay.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tih.nanxinkj.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kej.hysaishi.cn

Java: new Random().nextInt(100) + 1
来源：http://gym.aizwys.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sqf.birdmap.top

Ruby: rand(1..100)
来源：http://omc.xingfuxueyuan.xyz

C#:   new Random().Next(1, 101)
来源：http://zah.sysykeji.top

[A11] 条件表达式（三元）
来源：http://lnb.yuanzhike.top

Py:   "yes" if x > 0 else "no"
来源：http://efz.aizwys.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://axq.xylfe.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tey.fktsv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dkc.bbcook.cn

Java: x > 0 ? "yes" : "no"
来源：http://cql.wangshuangyany.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://guy.cashguo.top

Ruby: x > 0 ? "yes" : "no"
来源：http://wuw.zhijiandao.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uyv.0kj1m.cn

[A12] 字符串插值 / 格式化
来源：http://snn.52xcode.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://erv.gzhubu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dwp.ybcxt.top

JS:   `Hello, ${name}!`
来源：http://qbo.zycfv.cn

TS:   `Hello, ${name}!`
来源：http://rpq.bjfxy.top

Java: "Hello, %s!".formatted(name)
来源：http://tlw.zdbjq.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ers.xinyue.icu

Ruby: "Hello, #{name}!"
来源：http://kqz.zycfv.cn

C#:   $"Hello, {name}!"
来源：http://atd.fehbvm.com

[A13] 多行字符串（练习 \n 转义）
来源：http://qbl.fzhhl.top

Py:   "第一行\n第二行"
来源：http://rhn.fktsv.cn

PHP:  "第一行\n第二行"
来源：http://myn.vqdsnc.cn

JS:   "第一行\n第二行"
来源：http://qvg.jyoumei.cn

TS:   "第一行\n第二行"
来源：http://iyk.zhiwuduotai.top

Java: "第一行\n第二行"
来源：http://gyi.jinyuanbaomall.cn

Go:   "第一行\n第二行"
来源：http://nub.52xcode.cn

Ruby: "第一行\n第二行"
来源：http://urm.zdqjudy.top

C#:   "第一行\n第二行"
来源：http://vef.jinqigfzy.top

[A14] 注释写法
来源：http://zpa.sweek.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://vkc.zdbjq.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hnc.shanyushiyangkeji.top

JS:   // 单行；/* 多行 */
来源：http://cwu.yj20258888.top

TS:   // 单行；/* 多行 */
来源：http://vmk.nanxuanxn.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://stm.hongshengwenyu.top

Go:   // 单行；/* 多行 */
来源：http://mwx.9152youxi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xgw.zhiwuduotai.top

C#:   // 单行；/* 多行 */
来源：http://baq.zhijiandao.cn

[A15] 空值判断与默认值
来源：http://eee.hammf.cn

Py:   value = data or "默认值"
来源：http://pdn.wangdashe.top

PHP:  $value = $data ?? "默认值";
来源：http://cba.zdbjq.cn

JS:   const value = data ?? "默认值";
来源：http://nrt.cashguo.top

TS:   const value = data ?? "默认值";
来源：http://qwm.sysykeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rwf.xingfuxueyuan.xyz

Go:   if data == "" { data = "默认值" }
来源：http://aif.redwolf501.top

Ruby: value = data || "默认值"
来源：http://vea.ywan-chungtsiang.top

C#:   var value = data ?? "默认值";
来源：http://ndt.tian-w.cn

[A16] 真假值判断规则
来源：http://djv.havefunace.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mkk.wangdashe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lzb.gzhubu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qis.ybcxt.top

TS:   if (!x) {}
来源：http://qxg.jyoumei.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fgd.gaohongyu789.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sfs.aibaodan.cn

Ruby: unless x            # nil 与 false 为假
来源：http://roi.jqgfzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lio.jinqigfzy.top

[A17] 位运算
来源：http://bny.hcnkem.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sjo.yangfankeji.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dof.guannengcc.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cku.9152youxi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yae.zhoulong.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eae.0kj1m.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lvc.ehwqpu.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dhw.xingfuxueyuan.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ots.quarkkingdee.top

[A18] 字符与 ASCII 码互转
来源：http://jtb.tarul.cn

Py:   ord("A"); chr(65)
来源：http://eap.hcnkem.com

PHP:  ord("A"); chr(65)
来源：http://hrz.ywan-chungtsiang.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eyd.xuetiantiany.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://elq.hnqzz.top

Java: (int) 'A'; (char) 65
来源：http://cxv.hammf.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mai.ctjpmb.com

Ruby: "A".ord; 65.chr
来源：http://jmp.shzxlz.cn

C#:   (int)'A'; (char)65
来源：http://ble.zhiwuduotai.top

[A19] 交换两个变量
来源：http://fsb.hesvh.cn

Py:   a, b = b, a
来源：http://ubg.jqgufenzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ybj.pycfn.com

JS:   [a, b] = [b, a];
来源：http://uke.tian-w.cn

TS:   [a, b] = [b, a];
来源：http://eeu.hysaishi.cn

Java: int t = a; a = b; b = t;
来源：http://ptt.aibaodan.cn

Go:   a, b = b, a
来源：http://azc.sjlbkw.cn

Ruby: a, b = b, a
来源：http://adu.hnxiangtu.top

C#:   (a, b) = (b, a);
来源：http://hnl.shangyingyoupin.top

[A20] 读取标准输入
来源：http://tej.ydjk.org.cn

Py:   name = input("请输入：")
来源：http://fip.hnxiangtu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://yql.zhengqikj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mdw.zdqjudy.top

TS:   // Node.js：readline 模块
来源：http://vxf.tanke756.top

Java: new Scanner(System.in).nextLine()
来源：http://lxf.bjfxy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lxg.jlsjyb.cn

Ruby: gets.chomp
来源：http://hph.xinyue.icu

C#:   Console.ReadLine();
来源：http://ifi.hfpthk.cn

[A21] 保留指定小数位输出
来源：http://jte.yvedp.cn

Py:   f"{3.14159:.2f}"
来源：http://fvn.cheryme.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tcs.gaohongyu789.top

JS:   (3.14159).toFixed(2)
来源：http://hih.nanxuanxn.top

TS:   (3.14159).toFixed(2)
来源：http://avi.wangshuangyany.cn

Java: String.format("%.2f", 3.14159)
来源：http://cuv.sjlbkw.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uzh.dianchejie.cn

Ruby: format("%.2f", 3.14159)
来源：http://bbu.9152youxi.cn

C#:   3.14159.ToString("F2")
来源：http://lhl.dianchejie.cn

[A22] 获取字符串长度
来源：http://hmf.shanyushiyangkeji.top

Py:   len(s)
来源：http://pxy.hnqzz.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yto.jlsjyb.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wqp.shuidangran.top

TS:   s.length
来源：http://oar.birdmap.top

Java: s.length()
来源：http://mdn.hfpthk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kxq.tarul.cn

Ruby: s.length
来源：http://req.dashuyun.cn

C#:   s.Length
来源：http://efj.9152youxi.cn

[A23] 大小写转换
来源：http://sfl.jinqigufen.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xbp.xziqi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://roo.xylfe.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tot.ybcxt.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://huw.daria6918.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://brx.gogol.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ifx.cashguo.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yjf.bjfxy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://zec.hcnkem.com

[A24] 去除首尾空白
来源：http://tcd.xuetiantiany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qai.xziqi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lqo.zdbjq.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vnz.hongshengwenyu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://win.yueranfly.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kqa.cqqwz.cn

Go:   strings.TrimSpace(s)
来源：http://kyi.smart0.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qzy.dianchejie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zei.shangyingyoupin.top

[A25] 字符串比较
来源：http://xrj.c1oappe.top

Py:   s1 == s2; s1 != s2
来源：http://zul.quarkkingdee.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://psw.fzhhl.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kvm.316326.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nok.nanxuanxn.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pzq.bbcook.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qes.jinghuilouyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jas.hesvh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gly.yongpay.top

[A26] 类型转换总览
来源：http://nix.c1oappe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bnp.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ole.daria6918.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wwg.xuanzx.com

TS:   Number() String() Boolean() x as number
来源：http://fcj.dianchejie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mwh.jqgfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://svt.jiagoushi.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bls.fktsv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vek.yanxiufei.cn

================================================================================
来源：http://xyw.birdmap.top

B. 流程控制
来源：http://oea.316326.xyz

================================================================================
来源：http://bad.shangyingyoupin.top

[B01] 条件判断 if / else
来源：http://aji.xylfe.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wye.316326.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oqk.yanxiufei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ysz.hongshengwenyu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ufr.quarkkingdee.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ybz.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mlu.zhoulong.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dkd.pengpengdd.cyou

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ibn.hesvh.cn

[B02] 多分支 else if / elif
来源：http://czr.daria6918.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rfu.hysaishi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xjs.ybcxt.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wdj.sufxvd.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zfq.andypj.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fab.gotoacloud.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://quw.nwbrower.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uum.52xcode.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gdg.jqgfzy.top

[B03] switch / match / case
来源：http://sfr.dashuyun.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rzo.zhaomingkeji.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://apn.haohaochexian.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ntz.cdnleiting.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zas.yangfankeji.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iwl.yvedp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://out.fengsongda.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zrj.feifeiyinyue.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lro.zhengqikj.top

[B04] for 计数循环
来源：http://wgt.316326.xyz

Py:   for i in range(10): print(i)
来源：http://mvg.xingfuxueyuan.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lxo.shangyingyoupin.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://guv.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kyt.ydzc1.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://efm.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ape.yueranfly.top

Ruby: 10.times { |i| puts i }
来源：http://sgd.jinghuilouyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vvi.xingfuxueyuan.xyz

[B05] 遍历数组 / 列表
来源：http://aoo.quarkkingdee.top

Py:   for item in arr: print(item)
来源：http://xjy.sxryk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vhh.sxryk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://myr.hywenlv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mxl.kuanghao11.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://djk.iojbl.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://etq.uphjek.com

Ruby: arr.each { |item| puts item }
来源：http://ril.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bmv.uphjek.com

[B06] 遍历字典 / 对象
来源：http://mif.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://rtb.zhixingplan.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lxg.zhijiandao.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ajg.xziqi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mah.ydjk.org.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mht.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nkj.yuanzhike.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xcx.zdqjudy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://udf.jinyuanbaomall.cn

[B07] while 循环
来源：http://urh.zhongyouzk.top

Py:   while i < 10: i += 1
来源：http://ciq.iojbl.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kly.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://xrx.sysykeji.top

TS:   while (i < 10) { i++; }
来源：http://ikn.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://gso.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nhf.bbcook.cn

Ruby: while i < 10; i += 1; end
来源：http://mid.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://iqf.shuidangran.top

[B08] do-while（至少执行一次）
来源：http://oas.smart0.xyz

Py:   # 无 do-while：用 while True + break
来源：http://ivr.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zer.ctjpmb.com

JS:   do { i++; } while (i < 10);
来源：http://sik.ctjpmb.com

TS:   do { i++; } while (i < 10);
来源：http://xfv.svipenyu.cn

Java: do { i++; } while (i < 10);
来源：http://xxe.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ojs.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://psm.guannengcc.top

C#:   do { i++; } while (i < 10);
来源：http://hmc.sysykeji.top

[B09] break 与 continue
来源：http://ixf.mhx1999.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ooq.xylfe.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kns.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fnm.andypj.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dih.yj202588.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bkv.shanyushiyangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dov.pycfn.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vuz.0kj1m.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://plm.hywenlv.cn

[B10] 遍历同时拿索引
来源：http://ujh.wangdashe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dyk.sysykeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ljk.ybcxt.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vbh.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ukd.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://imf.fzhhl.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oyx.sufxvd.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nsz.gzhubu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rms.gzhubu.top

[B11] 生成数字序列 / 区间
来源：http://cfk.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://nht.snrcjt.cn

PHP:  range(0, 10, 2);
来源：http://vbx.gogol.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yka.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jsx.feifeiyinyue.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vrn.zhoulong.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jqi.ydjk.org.cn

Ruby: (0...10).step(2).to_a
来源：http://vpc.bbcook.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://get.yueranfly.top

[B12] 跳出多层循环
来源：http://zbe.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://alm.cashguo.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://thu.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uns.sysykeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kjr.xylfe.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://shv.jyoumei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ubb.9152youxi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ibq.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pxj.cashguo.top

[B13] 判断是否为数字
来源：http://rpy.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://yvw.cucudq.cn

PHP:  is_numeric($x)
来源：http://npd.kuanghao11.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xmi.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gtg.cdnleiting.top

Java: x instanceof Number
来源：http://pin.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lls.nanxuanxn.top

Ruby: x.is_a?(Numeric)
来源：http://nvy.jqgufenzy.top


<!-- 参考信息 -->