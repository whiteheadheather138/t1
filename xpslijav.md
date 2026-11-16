代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kpd.kuanghao11.cn

[A07] 数字转字符串
来源：http://xyr.mhx1999.top

Py:   str(42)
来源：http://suf.hfpthk.cn

PHP:  (string) 42; strval(42)
来源：http://yre.yonumen.top

JS:   String(42); (42).toString()
来源：http://oka.vqdsnc.cn

TS:   String(42)
来源：http://cop.guowangkeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mbx.cheryme.top

Go:   strconv.Itoa(42)
来源：http://vux.jlsjyb.cn

Ruby: 42.to_s
来源：http://usn.wangshuangyany.cn

C#:   42.ToString()
来源：http://nvv.wangshuangyany.cn

[A08] 取整与四舍五入
来源：http://bxz.ywan-chungtsiang.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sjt.shangyingyoupin.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hts.tanke756.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://trr.pengpengdd.cyou

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wka.shuidangran.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rmg.jlsjyb.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nyq.gaohongyu789.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://icu.haohaochexian.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ozf.zhengqikj.top

[A09] 绝对值与最大最小值
来源：http://mvh.ctjpmb.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kfz.quarkkingdee.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://iqk.xingfuxueyuan.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kgv.jyoumei.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vwf.andypj.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kfd.pengpengdd.cyou

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eyj.gogol.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://taa.jinyuanbaomall.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yhl.c1oappe.top

[A10] 生成随机数
来源：http://bun.kuanghao11.cn

Py:   import random; random.randint(1, 100)
来源：http://lcq.hammf.cn

PHP:  random_int(1, 100);
来源：http://xoi.yanxiufei.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rcz.fanxiaobao.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qgy.quarkkingdee.top

Java: new Random().nextInt(100) + 1
来源：http://pkt.jinyuanbaomall.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dod.pengpengdd.cyou

Ruby: rand(1..100)
来源：http://mri.zhongyouzk.top

C#:   new Random().Next(1, 101)
来源：http://wdx.bbcook.cn

[A11] 条件表达式（三元）
来源：http://apv.smart0.xyz

Py:   "yes" if x > 0 else "no"
来源：http://njr.yuanzhike.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kgx.zdbjq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://axs.shanyushiyangkeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://oye.tarul.cn

Java: x > 0 ? "yes" : "no"
来源：http://yhf.ybcxt.top

Go:   // 无三元运算符，需用 if 语句
来源：http://iuw.yfazqb.com

Ruby: x > 0 ? "yes" : "no"
来源：http://les.zhiwuduotai.top

C#:   x > 0 ? "yes" : "no"
来源：http://uuu.jinghuilouyu.cn

[A12] 字符串插值 / 格式化
来源：http://nga.gotoacloud.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mis.cheryme.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ika.sweek.top

JS:   `Hello, ${name}!`
来源：http://cpb.yvedp.cn

TS:   `Hello, ${name}!`
来源：http://clh.zhengqikj.top

Java: "Hello, %s!".formatted(name)
来源：http://ssj.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hhv.fzhhl.top

Ruby: "Hello, #{name}!"
来源：http://zyi.dashuyun.cn

C#:   $"Hello, {name}!"
来源：http://ush.havefunace.top

[A13] 多行字符串（练习 \n 转义）
来源：http://oxa.hywenlv.cn

Py:   "第一行\n第二行"
来源：http://jqa.hcnkem.com

PHP:  "第一行\n第二行"
来源：http://pmd.daria6918.cn

JS:   "第一行\n第二行"
来源：http://cse.chenlongwang.top

TS:   "第一行\n第二行"
来源：http://wjm.vqdsnc.cn

Java: "第一行\n第二行"
来源：http://beh.vehdjk.com

Go:   "第一行\n第二行"
来源：http://ptg.hfpthk.cn

Ruby: "第一行\n第二行"
来源：http://igh.jinyuanbaomall.cn

C#:   "第一行\n第二行"
来源：http://vbc.gaohongyu789.top

[A14] 注释写法
来源：http://ipn.yongpay.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rth.zhengqikj.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://gkc.52xcode.cn

JS:   // 单行；/* 多行 */
来源：http://iyn.daxiang520.top

TS:   // 单行；/* 多行 */
来源：http://pvm.aibaodan.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cpv.9152youxi.cn

Go:   // 单行；/* 多行 */
来源：http://bwq.shzxlz.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bhs.svipenyu.cn

C#:   // 单行；/* 多行 */
来源：http://qed.sweek.top

[A15] 空值判断与默认值
来源：http://jdr.kuanghao11.cn

Py:   value = data or "默认值"
来源：http://yja.andypj.xyz

PHP:  $value = $data ?? "默认值";
来源：http://bfq.yueranfly.top

JS:   const value = data ?? "默认值";
来源：http://grw.zhiwuduotai.top

TS:   const value = data ?? "默认值";
来源：http://wtk.ywan-chungtsiang.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vhg.quarkkingdee.top

Go:   if data == "" { data = "默认值" }
来源：http://ztw.wangdashe.top

Ruby: value = data || "默认值"
来源：http://mla.zdbjq.cn

C#:   var value = data ?? "默认值";
来源：http://rfp.ydjk.org.cn

[A16] 真假值判断规则
来源：http://onb.shanyushiyangtech.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xhb.aizwys.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vaa.zhaomingkeji.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sbx.cqqwz.cn

TS:   if (!x) {}
来源：http://ksv.hysaishi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xjp.nwbrower.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kbv.feifeiyinyue.top

Ruby: unless x            # nil 与 false 为假
来源：http://gyv.aizwys.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ked.guowangkeji.top

[A17] 位运算
来源：http://dhs.fehbvm.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tcj.zhaomingkeji.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uvo.aizwys.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pyr.hnxiangtu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iqe.0kj1m.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://foo.hysaishi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nnj.redwolf501.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eid.svipenyu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gvb.cheryme.top

[A18] 字符与 ASCII 码互转
来源：http://fed.uphjek.com

Py:   ord("A"); chr(65)
来源：http://yjy.aibaodan.cn

PHP:  ord("A"); chr(65)
来源：http://qcq.hongshengwenyu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hoc.sysykeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lru.jinghuilouyu.cn

Java: (int) 'A'; (char) 65
来源：http://osz.fengsongda.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rsr.daxiang520.top

Ruby: "A".ord; 65.chr
来源：http://pxt.316326.xyz

C#:   (int)'A'; (char)65
来源：http://xmz.wangshuangyany.cn

[A19] 交换两个变量
来源：http://jwm.zhoulong.xyz

Py:   a, b = b, a
来源：http://xhv.jinghuilouyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://iem.yongpay.top

JS:   [a, b] = [b, a];
来源：http://vsq.shanyushiyangtech.top

TS:   [a, b] = [b, a];
来源：http://xte.gotoacloud.top

Java: int t = a; a = b; b = t;
来源：http://lua.tanke756.top

Go:   a, b = b, a
来源：http://mae.tianlin.xyz

Ruby: a, b = b, a
来源：http://vao.guowangkeji.top

C#:   (a, b) = (b, a);
来源：http://qkb.hysaishi.cn

[A20] 读取标准输入
来源：http://ari.chenlongwang.top

Py:   name = input("请输入：")
来源：http://dxr.zhaomingkeji.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://dxg.zhengqikj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qpd.jinqigfzy.top

TS:   // Node.js：readline 模块
来源：http://dpj.ydzc1.top

Java: new Scanner(System.in).nextLine()
来源：http://quj.jiagoushi.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ybj.birdmap.top

Ruby: gets.chomp
来源：http://ekg.quarkkingdee.top

C#:   Console.ReadLine();
来源：http://jir.bjfxy.top

[A21] 保留指定小数位输出
来源：http://pbs.xuetiantiany.cn

Py:   f"{3.14159:.2f}"
来源：http://omi.yanxiufei.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dea.ywan-chungtsiang.top

JS:   (3.14159).toFixed(2)
来源：http://mxu.nwbrower.top

TS:   (3.14159).toFixed(2)
来源：http://jla.52xcode.cn

Java: String.format("%.2f", 3.14159)
来源：http://uzb.jiagoushi.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jql.shzxlz.cn

Ruby: format("%.2f", 3.14159)
来源：http://xhz.kuanghao11.cn

C#:   3.14159.ToString("F2")
来源：http://btk.ppjwa.cn

[A22] 获取字符串长度
来源：http://yuv.ydzc1.top

Py:   len(s)
来源：http://exb.bjfxy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kxj.mhx1999.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vku.guowangkeji.top

TS:   s.length
来源：http://jqg.yueranfly.top

Java: s.length()
来源：http://xjt.xuetiantiany.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ksa.ivvv.top

Ruby: s.length
来源：http://kgz.tarul.cn

C#:   s.Length
来源：http://zwu.nanxuanxn.top

[A23] 大小写转换
来源：http://hdl.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://uwm.xylfe.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gex.dianchejie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hsd.sysykeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zlt.cashguo.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dsf.c1oappe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zyq.sjlbkw.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hls.bjfxy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gnq.andypj.xyz

[A24] 去除首尾空白
来源：http://ffh.zhiwuduotai.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.yuanzhike.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sfu.sxryk.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dsy.quarkkingdee.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bge.52xcode.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xge.aizwys.cn

Go:   strings.TrimSpace(s)
来源：http://yad.9152youxi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ehr.xingfuxueyuan.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rwo.xylfe.cn

[A25] 字符串比较
来源：http://eur.yongpay.top

Py:   s1 == s2; s1 != s2
来源：http://oad.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wtl.haohaochexian.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rsc.chenlongwang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tgi.fengsongda.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vct.ydjk.org.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gym.vehdjk.com

Ruby: s1 == s2; s1 <=> s2
来源：http://ozy.hfpthk.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://crj.yanxiufei.cn

[A26] 类型转换总览
来源：http://fwn.xuanzx.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pbk.guowangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vgb.hnxiangtu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uav.pycfn.com

TS:   Number() String() Boolean() x as number
来源：http://nbj.zhijiandao.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qqi.ctjpmb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dyd.nanxinkj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ugn.gzhubu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://swr.cucudq.cn

================================================================================
来源：http://gfy.daria6918.cn

B. 流程控制
来源：http://szx.bjfxy.top

================================================================================
来源：http://eya.yvedp.cn

[B01] 条件判断 if / else
来源：http://rgs.shangyingyoupin.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hoc.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://syp.xuanzx.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://owd.bbcook.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jii.jqgufenzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ovg.zhaomingkeji.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kle.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kgd.cdnleiting.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eri.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://ufe.xinyue.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jvm.0kj1m.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://maf.feifeiyinyue.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tsq.vehdjk.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ukj.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fdn.cashguo.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uik.wangdashe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nbm.jqgfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zcd.gzhubu.top

[B03] switch / match / case
来源：http://fwe.chenlongwang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://exf.zhaomingkeji.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://egm.xziqi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://efa.epnwcf.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ijq.jianghu66.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ium.shzxlz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dtt.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dtt.xinyue.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fwa.fanxiaobao.xyz

[B04] for 计数循环
来源：http://sbj.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://wjc.jiagoushi.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dvk.zdbjq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://syp.gzhubu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yts.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ncg.andypj.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://paa.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://adn.iojbl.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jpk.zdbjq.cn

[B05] 遍历数组 / 列表
来源：http://owo.yuxming.cn

Py:   for item in arr: print(item)
来源：http://eox.daxiang520.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vjx.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tjm.vehdjk.com

TS:   for (const item of arr) { console.log(item); }
来源：http://caj.yonumen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://slr.daxiang520.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xct.yueranfly.top

Ruby: arr.each { |item| puts item }
来源：http://fnu.cheryme.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ugw.jqgfzy.top

[B06] 遍历字典 / 对象
来源：http://xkd.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://doq.hammf.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lnc.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wzx.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uzx.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lje.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xon.dashuyun.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kyh.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ftw.tian-w.cn

[B07] while 循环
来源：http://zex.birdmap.top

Py:   while i < 10: i += 1
来源：http://xrl.cqqwz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bdn.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://ggi.pengpengdd.cyou

TS:   while (i < 10) { i++; }
来源：http://aqe.shanyushiyangkeji.top

Java: while (i < 10) { i++; }
来源：http://gjq.shuidangran.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mvv.mhx1999.top

Ruby: while i < 10; i += 1; end
来源：http://ilf.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://yzr.hysaishi.cn

[B08] do-while（至少执行一次）
来源：http://enp.fzhhl.top

Py:   # 无 do-while：用 while True + break
来源：http://ikj.snrcjt.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zdd.chenlongwang.top

JS:   do { i++; } while (i < 10);
来源：http://jji.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://uhu.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://mlo.hongshengwenyu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vui.yfazqb.com

Ruby: begin; i += 1; end while i < 10
来源：http://ygz.yueranfly.top

C#:   do { i++; } while (i < 10);
来源：http://egn.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://kji.shuidangran.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tga.chenzaomai.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lfg.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rka.hammf.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tau.yanxiufei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://squ.zhiwuduotai.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pja.cdnleiting.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pqf.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kde.andypj.xyz

[B10] 遍历同时拿索引
来源：http://amo.fktsv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cub.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ogt.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cqd.ydzc1.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eis.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cvs.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tld.tian-w.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qqs.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cjx.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://xco.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://jxy.tianlin.xyz

PHP:  range(0, 10, 2);
来源：http://fij.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mip.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zun.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://arf.hnxiangtu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ytt.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://bhs.iojbl.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kkr.quarkkingdee.top

[B12] 跳出多层循环
来源：http://pkw.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zrt.meibo888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xgg.zhijiandao.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tot.cashguo.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vgk.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qaz.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yis.mhx1999.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sbs.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://spb.shanyushiyangkeji.top

[B13] 判断是否为数字
来源：http://fdc.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://fyh.sxryk.cn

PHP:  is_numeric($x)
来源：http://lbb.dianchejie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rwd.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tuy.hywenlv.cn

Java: x instanceof Number
来源：http://jqr.fzhhl.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fec.bbcook.cn

Ruby: x.is_a?(Numeric)
来源：http://aar.uphjek.com


<!-- 参考信息 -->