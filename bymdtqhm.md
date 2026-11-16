代发 wailian999

Ruby: 42.to_s
来源：http://ifr.52xcode.cn

C#:   42.ToString()
来源：http://ppi.yanxiufei.cn

[A08] 取整与四舍五入
来源：http://owo.yj20258.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ayl.ybcxt.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wvo.c1oappe.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://abe.ydjk.org.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yfh.shzxlz.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kzu.jinyuanbaomall.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://afa.yvedp.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nwo.andypj.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xbv.gzhubu.top

[A09] 绝对值与最大最小值
来源：http://qgn.hysaishi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jpb.fanxiaobao.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blw.aibaodan.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ngn.fanxiaobao.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cfa.fzhhl.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uuj.tanke756.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://koj.jqgfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xiy.tanke756.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uhh.fzhhl.top

[A10] 生成随机数
来源：http://hub.nwbrower.top

Py:   import random; random.randint(1, 100)
来源：http://tdi.cheryme.top

PHP:  random_int(1, 100);
来源：http://joo.gzhubu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://txe.zhiwuduotai.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zda.bjfxy.top

Java: new Random().nextInt(100) + 1
来源：http://pgb.ybcxt.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://euc.zhengqikj.top

Ruby: rand(1..100)
来源：http://cyb.vehdjk.com

C#:   new Random().Next(1, 101)
来源：http://jam.hywenlv.cn

[A11] 条件表达式（三元）
来源：http://ezn.fktsv.cn

Py:   "yes" if x > 0 else "no"
来源：http://xdz.birdmap.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jmt.cdnleiting.top

JS:   x > 0 ? "yes" : "no"
来源：http://igl.tianlin.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://kps.epnwcf.com

Java: x > 0 ? "yes" : "no"
来源：http://gtl.9152youxi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ycj.bjfxy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://cpz.dashuyun.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lwo.nwbrower.top

[A12] 字符串插值 / 格式化
来源：http://ehy.xingfuxueyuan.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://shz.hcnkem.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gmm.cucudq.cn

JS:   `Hello, ${name}!`
来源：http://gno.quarkkingdee.top

TS:   `Hello, ${name}!`
来源：http://eef.yj202588.top

Java: "Hello, %s!".formatted(name)
来源：http://pqh.yueranfly.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ufe.ppjwa.cn

Ruby: "Hello, #{name}!"
来源：http://kua.uphjek.com

C#:   $"Hello, {name}!"
来源：http://kvp.gotoacloud.top

[A13] 多行字符串（练习 \n 转义）
来源：http://wza.daria6918.cn

Py:   "第一行\n第二行"
来源：http://ods.tarul.cn

PHP:  "第一行\n第二行"
来源：http://zcr.fanxiaobao.xyz

JS:   "第一行\n第二行"
来源：http://srt.jqgfzy.top

TS:   "第一行\n第二行"
来源：http://kmw.dashuyun.cn

Java: "第一行\n第二行"
来源：http://rcj.iojbl.cn

Go:   "第一行\n第二行"
来源：http://rcs.guannengcc.top

Ruby: "第一行\n第二行"
来源：http://hzr.xuanzx.com

C#:   "第一行\n第二行"
来源：http://lqc.fzhhl.top

[A14] 注释写法
来源：http://zca.sufxvd.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uea.epnwcf.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://arg.sysykeji.top

JS:   // 单行；/* 多行 */
来源：http://saj.daxiang520.top

TS:   // 单行；/* 多行 */
来源：http://ivr.hywenlv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://knd.nwbrower.top

Go:   // 单行；/* 多行 */
来源：http://bhh.sweek.top

Ruby: # 单行；=begin 多行 =end
来源：http://rtp.yongpay.top

C#:   // 单行；/* 多行 */
来源：http://eik.tian-w.cn

[A15] 空值判断与默认值
来源：http://wui.jyoumei.cn

Py:   value = data or "默认值"
来源：http://fcl.zdbjq.cn

PHP:  $value = $data ?? "默认值";
来源：http://hoz.fanxiaobao.xyz

JS:   const value = data ?? "默认值";
来源：http://ddi.tian-w.cn

TS:   const value = data ?? "默认值";
来源：http://kqo.pycfn.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xhj.andypj.xyz

Go:   if data == "" { data = "默认值" }
来源：http://thu.aizwys.cn

Ruby: value = data || "默认值"
来源：http://yxt.zdqjudy.top

C#:   var value = data ?? "默认值";
来源：http://vgm.gogol.net.cn

[A16] 真假值判断规则
来源：http://ljh.yueranfly.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://auk.shangyingyoupin.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xdl.pengpengdd.cyou

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://adl.kuanghao11.cn

TS:   if (!x) {}
来源：http://zea.guowangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ajx.chenzaomai.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fta.gzhubu.top

Ruby: unless x            # nil 与 false 为假
来源：http://ciq.cheryme.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://imh.quarkkingdee.top

[A17] 位运算
来源：http://vgk.yongpay.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dxb.jqgfzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ipb.jlsjyb.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ihr.316326.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cke.yonumen.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ism.sufxvd.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://giv.fengsongda.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kxb.yj20258.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cxe.52xcode.cn

[A18] 字符与 ASCII 码互转
来源：http://fzc.zhixingplan.top

Py:   ord("A"); chr(65)
来源：http://qyg.cdnleiting.top

PHP:  ord("A"); chr(65)
来源：http://ghc.andypj.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://trc.mhx1999.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xfu.jinqigufen.top

Java: (int) 'A'; (char) 65
来源：http://eom.tarul.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jum.316326.xyz

Ruby: "A".ord; 65.chr
来源：http://mhj.jinyuanbaomall.cn

C#:   (int)'A'; (char)65
来源：http://srh.aibaodan.cn

[A19] 交换两个变量
来源：http://hsq.ydzc1.top

Py:   a, b = b, a
来源：http://oko.yj20258.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pmf.epnwcf.com

JS:   [a, b] = [b, a];
来源：http://obd.hesvh.cn

TS:   [a, b] = [b, a];
来源：http://xpv.gogol.net.cn

Java: int t = a; a = b; b = t;
来源：http://uet.ppjwa.cn

Go:   a, b = b, a
来源：http://dgy.ivvv.top

Ruby: a, b = b, a
来源：http://odr.zycfv.cn

C#:   (a, b) = (b, a);
来源：http://lum.meibo888.top

[A20] 读取标准输入
来源：http://jmr.meibo888.top

Py:   name = input("请输入：")
来源：http://eok.yfazqb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://yos.nanxuanxn.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ean.0kj1m.cn

TS:   // Node.js：readline 模块
来源：http://mir.zdqjudy.top

Java: new Scanner(System.in).nextLine()
来源：http://qnk.vqdsnc.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mgi.sjlbkw.cn

Ruby: gets.chomp
来源：http://llf.kuanghao11.cn

C#:   Console.ReadLine();
来源：http://djw.iojbl.cn

[A21] 保留指定小数位输出
来源：http://hbe.ehwqpu.com

Py:   f"{3.14159:.2f}"
来源：http://ekb.yanxiufei.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zvv.tarul.cn

JS:   (3.14159).toFixed(2)
来源：http://tll.hnqzz.top

TS:   (3.14159).toFixed(2)
来源：http://wec.yfazqb.com

Java: String.format("%.2f", 3.14159)
来源：http://wbq.gaohongyu789.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hdr.sweek.top

Ruby: format("%.2f", 3.14159)
来源：http://mon.aizwys.cn

C#:   3.14159.ToString("F2")
来源：http://bmr.mhx1999.top

[A22] 获取字符串长度
来源：http://ykf.ydjk.org.cn

Py:   len(s)
来源：http://yqq.epnwcf.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sik.cheryme.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xbv.shanyushiyangkeji.top

TS:   s.length
来源：http://joc.wangdashe.top

Java: s.length()
来源：http://jke.cucudq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dun.shanyushiyangkeji.top

Ruby: s.length
来源：http://zwt.feifeiyinyue.top

C#:   s.Length
来源：http://okh.sxryk.cn

[A23] 大小写转换
来源：http://bwy.shzxlz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sxa.yangfankeji.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://clf.yuanzhike.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jll.hnqzz.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://akg.yj20258888.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oiu.quarkkingdee.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mlk.hywenlv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yls.gotoacloud.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mgf.iojbl.cn

[A24] 去除首尾空白
来源：http://vqn.vqdsnc.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bvc.bjfxy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wlh.sweek.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://elo.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://flv.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ehu.yvedp.cn

Go:   strings.TrimSpace(s)
来源：http://xfy.svipenyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ajf.havefunace.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jwz.fktsv.cn

[A25] 字符串比较
来源：http://vhb.zycfv.cn

Py:   s1 == s2; s1 != s2
来源：http://ihl.sxryk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hay.xingfuxueyuan.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gks.feifeiyinyue.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xab.guowangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jba.ehwqpu.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jzr.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lmb.bbcook.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jyo.chenzaomai.com

[A26] 类型转换总览
来源：http://nbi.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dai.ybcxt.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kkh.chenjidiqi.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bhb.nwbrower.top

TS:   Number() String() Boolean() x as number
来源：http://sby.andypj.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qdz.hesvh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zrn.quarkkingdee.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bvv.xingfuxueyuan.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hnf.yanxiufei.cn

================================================================================
来源：http://znw.birdmap.top

B. 流程控制
来源：http://ibm.shanyushiyangkeji.top

================================================================================
来源：http://wsw.jqgufenzy.top

[B01] 条件判断 if / else
来源：http://hll.pengpengdd.cyou

Py:   result = "正" if x > 0 else "非正"
来源：http://xzz.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hgi.quarkkingdee.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ntk.pycfn.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gnb.sufxvd.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wer.zhengqikj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qxr.c1oappe.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rfw.shanyushiyangtech.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hfk.vehdjk.com

[B02] 多分支 else if / elif
来源：http://gbp.hnxiangtu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bec.gogol.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xma.jianghu66.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jcn.gogol.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nxx.hesvh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jjt.xingfuxueyuan.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mwt.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oaz.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ccn.jinqigfzy.top

[B03] switch / match / case
来源：http://yek.havefunace.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xgr.iojbl.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://krd.wangdashe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://akw.hysaishi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xac.meibo888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ymb.zhiwuduotai.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dax.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ssj.nwbrower.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nfz.fengsongda.top

[B04] for 计数循环
来源：http://idu.ydzc1.top

Py:   for i in range(10): print(i)
来源：http://csv.cheryme.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pjr.yvedp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gjb.jyoumei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qff.sysykeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bjl.nanxuanxn.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zbh.zdqjudy.top

Ruby: 10.times { |i| puts i }
来源：http://poj.vqdsnc.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gkb.chenlongwang.top

[B05] 遍历数组 / 列表
来源：http://fxi.chenjidiqi.icu

Py:   for item in arr: print(item)
来源：http://mba.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cxj.zhengqikj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tvh.zdbjq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://epg.shzxlz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vxx.yj20258888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hdp.shangyingyoupin.top

Ruby: arr.each { |item| puts item }
来源：http://ejk.zhoulong.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eae.52xcode.cn

[B06] 遍历字典 / 对象
来源：http://xiw.shanyushiyangtech.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wbz.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bfj.yangfankeji.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://phu.zdqjudy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ycc.hnqzz.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ypb.chenlongwang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zey.zhongyouzk.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qss.aibaodan.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sil.smart0.xyz

[B07] while 循环
来源：http://moi.sufxvd.cn

Py:   while i < 10: i += 1
来源：http://rpn.sufxvd.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mdb.0kj1m.cn

JS:   while (i < 10) { i++; }
来源：http://hyn.vehdjk.com

TS:   while (i < 10) { i++; }
来源：http://fck.c1oappe.top

Java: while (i < 10) { i++; }
来源：http://cdg.ybcxt.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fxk.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://nuz.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://cop.hammf.cn

[B08] do-while（至少执行一次）
来源：http://blo.zdqjudy.top

Py:   # 无 do-while：用 while True + break
来源：http://ieg.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cwl.jinqigufen.top

JS:   do { i++; } while (i < 10);
来源：http://tnt.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://chi.cucudq.cn

Java: do { i++; } while (i < 10);
来源：http://hob.cucudq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lkd.feifeiyinyue.top

Ruby: begin; i += 1; end while i < 10
来源：http://eva.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://kml.c1oappe.top

[B09] break 与 continue
来源：http://gcn.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iat.yj20258888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lmk.xingfuxueyuan.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ufr.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://unu.jinyuanbaomall.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dbh.jiagoushi.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://izz.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hds.jianghu66.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kqs.tian-w.cn

[B10] 遍历同时拿索引
来源：http://tiz.cheryme.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fxx.yueranfly.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://led.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jds.cashguo.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xmx.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://onp.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ayf.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kzb.ctjpmb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rpu.sysykeji.top

[B11] 生成数字序列 / 区间
来源：http://gds.zhongyouzk.top

Py:   list(range(0, 10, 2))
来源：http://eek.fehbvm.com

PHP:  range(0, 10, 2);
来源：http://ypz.zhoulong.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dbi.0kj1m.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kqk.jianghu66.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gyu.yj202588.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aqs.fanxiaobao.xyz

Ruby: (0...10).step(2).to_a
来源：http://evo.mhx1999.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uog.hammf.cn

[B12] 跳出多层循环
来源：http://chc.hongshengwenyu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qve.xylfe.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gpl.gaohongyu789.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zku.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://awe.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rba.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dnl.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hxe.havefunace.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uwp.uphjek.com

[B13] 判断是否为数字
来源：http://aqr.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://epd.ppjwa.cn

PHP:  is_numeric($x)
来源：http://gzh.sxryk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xbh.316326.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kau.chenlongwang.top

Java: x instanceof Number
来源：http://hoi.fehbvm.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bov.snrcjt.cn

Ruby: x.is_a?(Numeric)
来源：http://qyz.uphjek.com

C#:   x is int or double or decimal
来源：http://fbs.iojbl.cn

[B14] 判断值是否在集合内
来源：http://drn.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://odd.chenjidiqi.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xpa.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://qba.316326.xyz

TS:   [1, 2, 3].includes(x)
来源：http://hxv.hesvh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://khr.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://szk.c1oappe.top


<!-- 参考信息 -->