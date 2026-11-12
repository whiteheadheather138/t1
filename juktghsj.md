代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vmh.0kj1m.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wna.ydjk.org.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://eiq.cqqwz.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://iuj.jqgufenzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tdm.nwbrower.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://seq.yj20258888.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tob.tianlin.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ovt.jianghu66.top

[A10] 生成随机数
来源：http://zta.jinqigufen.top

Py:   import random; random.randint(1, 100)
来源：http://gam.redwolf501.top

PHP:  random_int(1, 100);
来源：http://snq.zhongyouzk.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cwn.tanke756.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uld.fktsv.cn

Java: new Random().nextInt(100) + 1
来源：http://swp.tianlin.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xis.shanyushiyangtech.top

Ruby: rand(1..100)
来源：http://fki.nanxuanxn.top

C#:   new Random().Next(1, 101)
来源：http://pij.yvedp.cn

[A11] 条件表达式（三元）
来源：http://atq.jyoumei.cn

Py:   "yes" if x > 0 else "no"
来源：http://otd.jqgufenzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://fxh.chenlongwang.top

JS:   x > 0 ? "yes" : "no"
来源：http://qjc.sysykeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://fzk.sxryk.cn

Java: x > 0 ? "yes" : "no"
来源：http://dqw.daxiang520.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fkr.xziqi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tht.shuidangran.top

C#:   x > 0 ? "yes" : "no"
来源：http://vsl.pengpengdd.cyou

[A12] 字符串插值 / 格式化
来源：http://euk.hywenlv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ndy.sweek.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://luw.bjfxy.top

JS:   `Hello, ${name}!`
来源：http://hpk.dianchejie.cn

TS:   `Hello, ${name}!`
来源：http://tij.gzhubu.top

Java: "Hello, %s!".formatted(name)
来源：http://vux.ydjk.org.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://szq.tian-w.cn

Ruby: "Hello, #{name}!"
来源：http://ltj.ivvv.top

C#:   $"Hello, {name}!"
来源：http://mqr.zhijiandao.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ziq.yuxming.cn

Py:   "第一行\n第二行"
来源：http://fbp.hcnkem.com

PHP:  "第一行\n第二行"
来源：http://gvi.cheryme.top

JS:   "第一行\n第二行"
来源：http://dwh.jinyuanbaomall.cn

TS:   "第一行\n第二行"
来源：http://edj.snrcjt.cn

Java: "第一行\n第二行"
来源：http://jzm.jqgfzy.top

Go:   "第一行\n第二行"
来源：http://ntb.uphjek.com

Ruby: "第一行\n第二行"
来源：http://aia.chenjidiqi.icu

C#:   "第一行\n第二行"
来源：http://bcx.shzxlz.cn

[A14] 注释写法
来源：http://efq.yj20258888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://nzd.hfpthk.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tqw.xuetiantiany.cn

JS:   // 单行；/* 多行 */
来源：http://srx.yvedp.cn

TS:   // 单行；/* 多行 */
来源：http://stn.uphjek.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://huh.gogol.net.cn

Go:   // 单行；/* 多行 */
来源：http://rsg.iojbl.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zgy.sjlbkw.cn

C#:   // 单行；/* 多行 */
来源：http://qkj.dianchejie.cn

[A15] 空值判断与默认值
来源：http://rvs.fzhhl.top

Py:   value = data or "默认值"
来源：http://inc.fzhhl.top

PHP:  $value = $data ?? "默认值";
来源：http://vxx.jinyuanbaomall.cn

JS:   const value = data ?? "默认值";
来源：http://dce.zhijiandao.cn

TS:   const value = data ?? "默认值";
来源：http://req.shanyushiyangkeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rdr.vehdjk.com

Go:   if data == "" { data = "默认值" }
来源：http://bfq.ivvv.top

Ruby: value = data || "默认值"
来源：http://qft.52xcode.cn

C#:   var value = data ?? "默认值";
来源：http://yfp.hnqzz.top

[A16] 真假值判断规则
来源：http://wup.yuxming.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nnk.yangfankeji.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://iei.guowangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hwc.cheryme.top

TS:   if (!x) {}
来源：http://wmn.ctjpmb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ywm.ydzc1.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kbk.ydzc1.top

Ruby: unless x            # nil 与 false 为假
来源：http://yej.52xcode.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zlv.wangshuangyany.cn

[A17] 位运算
来源：http://knw.zhoulong.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://srw.cdnleiting.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ers.jinyuanbaomall.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xum.pycfn.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lkf.wangdashe.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hwg.ppjwa.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bww.zhixingplan.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nwx.316326.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jja.shzxlz.cn

[A18] 字符与 ASCII 码互转
来源：http://hyz.ehwqpu.com

Py:   ord("A"); chr(65)
来源：http://mmd.bbcook.cn

PHP:  ord("A"); chr(65)
来源：http://geo.yanxiufei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ipj.vqdsnc.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qzv.shzxlz.cn

Java: (int) 'A'; (char) 65
来源：http://wdd.kuanghao11.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oow.pengpengdd.cyou

Ruby: "A".ord; 65.chr
来源：http://hlp.jiagoushi.top

C#:   (int)'A'; (char)65
来源：http://zgf.ybcxt.top

[A19] 交换两个变量
来源：http://doi.fehbvm.com

Py:   a, b = b, a
来源：http://alr.zhongyouzk.top

PHP:  [$a, $b] = [$b, $a];
来源：http://bel.yonumen.top

JS:   [a, b] = [b, a];
来源：http://nce.yanxiufei.cn

TS:   [a, b] = [b, a];
来源：http://rex.c1oappe.top

Java: int t = a; a = b; b = t;
来源：http://bnf.chenzaomai.com

Go:   a, b = b, a
来源：http://epk.jlsjyb.cn

Ruby: a, b = b, a
来源：http://hqy.meibo888.top

C#:   (a, b) = (b, a);
来源：http://tya.mhx1999.top

[A20] 读取标准输入
来源：http://rgf.hcnkem.com

Py:   name = input("请输入：")
来源：http://ady.yj20258.top

PHP:  $name = trim(fgets(STDIN));
来源：http://uyw.zycfv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jve.fehbvm.com

TS:   // Node.js：readline 模块
来源：http://tkz.jiagoushi.top

Java: new Scanner(System.in).nextLine()
来源：http://erf.52xcode.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nqy.yj20258.top

Ruby: gets.chomp
来源：http://dvk.shzxlz.cn

C#:   Console.ReadLine();
来源：http://vde.mhx1999.top

[A21] 保留指定小数位输出
来源：http://qoh.hcnkem.com

Py:   f"{3.14159:.2f}"
来源：http://iod.daria6918.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bto.vqdsnc.cn

JS:   (3.14159).toFixed(2)
来源：http://kyb.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://tsp.zhixingplan.top

Java: String.format("%.2f", 3.14159)
来源：http://iyx.hfpthk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lms.pycfn.com

Ruby: format("%.2f", 3.14159)
来源：http://yvj.yanxiufei.cn

C#:   3.14159.ToString("F2")
来源：http://ipl.uphjek.com

[A22] 获取字符串长度
来源：http://uxs.zycfv.cn

Py:   len(s)
来源：http://nhd.sxryk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://obp.dianchejie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://znz.redwolf501.top

TS:   s.length
来源：http://kgs.epnwcf.com

Java: s.length()
来源：http://mxf.c1oappe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rev.sufxvd.cn

Ruby: s.length
来源：http://aqg.fengsongda.top

C#:   s.Length
来源：http://ldk.pycfn.com

[A23] 大小写转换
来源：http://smh.jinyuanbaomall.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://epg.zdbjq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://plc.52xcode.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://udz.hnqzz.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ykp.52xcode.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vcy.jinyuanbaomall.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ssr.yonumen.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fid.cashguo.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nbp.xuanzx.com

[A24] 去除首尾空白
来源：http://jvp.uphjek.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kbc.gaohongyu789.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oto.ivvv.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ffa.chenjidiqi.icu

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://elq.pycfn.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rxh.cucudq.cn

Go:   strings.TrimSpace(s)
来源：http://bqk.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zzv.hongshengwenyu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://imc.c1oappe.top

[A25] 字符串比较
来源：http://uln.sufxvd.cn

Py:   s1 == s2; s1 != s2
来源：http://ivw.jinqigufen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oti.fengsongda.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bnx.nanxinkj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dfq.jinyuanbaomall.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yqx.dashuyun.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rjg.hywenlv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mib.yongpay.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://utp.ybcxt.top

[A26] 类型转换总览
来源：http://hvl.fehbvm.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nux.yj202588.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uyp.zdqjudy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tpw.xuetiantiany.cn

TS:   Number() String() Boolean() x as number
来源：http://cwa.jqgfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xnu.xziqi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kon.quarkkingdee.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kyz.jyoumei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fsl.sweek.top

================================================================================
来源：http://sxs.ivvv.top

B. 流程控制
来源：http://xvh.shangyingyoupin.top

================================================================================
来源：http://lik.shuidangran.top

[B01] 条件判断 if / else
来源：http://cjz.zdqjudy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://pmp.havefunace.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://olb.hnxiangtu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://btl.jinghuilouyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zlk.iojbl.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dwt.c1oappe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ihg.quarkkingdee.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xkq.epnwcf.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qho.sysykeji.top

[B02] 多分支 else if / elif
来源：http://mnx.0kj1m.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sln.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cwa.daxiang520.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uee.guowangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pul.vehdjk.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ndn.pengpengdd.cyou

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kjb.svipenyu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xab.yueranfly.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rts.andypj.xyz

[B03] switch / match / case
来源：http://ael.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cno.gotoacloud.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jko.tianlin.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fkk.tanke756.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rpz.hesvh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jmd.yuanzhike.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://szl.zdbjq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://prz.zhiwuduotai.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ett.yanxiufei.cn

[B04] for 计数循环
来源：http://mwv.tanke756.top

Py:   for i in range(10): print(i)
来源：http://gsg.jianghu66.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fbv.jinqigufen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wyg.andypj.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hco.xinyue.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mva.yvedp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bjf.gaohongyu789.top

Ruby: 10.times { |i| puts i }
来源：http://fmg.shanyushiyangtech.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vvo.yongpay.top

[B05] 遍历数组 / 列表
来源：http://mwr.wangdashe.top

Py:   for item in arr: print(item)
来源：http://dvd.gogol.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zqt.kuanghao11.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oxr.guowangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://did.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tpi.bjfxy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uov.havefunace.top

Ruby: arr.each { |item| puts item }
来源：http://frp.9152youxi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bfh.kuanghao11.cn

[B06] 遍历字典 / 对象
来源：http://zey.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://aas.shzxlz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eod.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sfv.ydzc1.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hrc.cqqwz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uwx.zhijiandao.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nqt.nanxinkj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ery.cheryme.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://chb.yanxiufei.cn

[B07] while 循环
来源：http://mcx.yonumen.top

Py:   while i < 10: i += 1
来源：http://nzi.snrcjt.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hrb.iojbl.cn

JS:   while (i < 10) { i++; }
来源：http://gaj.vehdjk.com

TS:   while (i < 10) { i++; }
来源：http://fnw.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://fni.zhaomingkeji.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tzn.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://fpq.snrcjt.cn

C#:   while (i < 10) { i++; }
来源：http://rnq.zhaomingkeji.xyz

[B08] do-while（至少执行一次）
来源：http://blj.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://omz.tanke756.top

PHP:  do { $i++; } while ($i < 10);
来源：http://otf.yangfankeji.com

JS:   do { i++; } while (i < 10);
来源：http://ami.haohaochexian.top

TS:   do { i++; } while (i < 10);
来源：http://sjj.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://lom.hammf.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dpc.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://uhq.jianghu66.top

C#:   do { i++; } while (i < 10);
来源：http://xvx.aibaodan.cn

[B09] break 与 continue
来源：http://nsx.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hgj.yonumen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://njy.mhx1999.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mxm.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ors.yueranfly.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gcs.iojbl.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vlb.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://haz.yj20258888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixj.hcnkem.com

[B10] 遍历同时拿索引
来源：http://zeu.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xxp.c1oappe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tsl.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xij.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pwi.jqgfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gco.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pnp.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vrm.ydjk.org.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zyh.iojbl.cn

[B11] 生成数字序列 / 区间
来源：http://xpm.jqgfzy.top

Py:   list(range(0, 10, 2))
来源：http://hhw.gaohongyu789.top

PHP:  range(0, 10, 2);
来源：http://yny.xuanzx.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xwp.ybcxt.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xcr.jqgufenzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qwb.nanxinkj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kat.hnxiangtu.top

Ruby: (0...10).step(2).to_a
来源：http://zhi.vqdsnc.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yqs.yuanzhike.top

[B12] 跳出多层循环
来源：http://cly.cheryme.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yow.tianlin.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://xpb.sjlbkw.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ega.jinqigfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qwa.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hid.shangyingyoupin.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rto.hammf.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mhl.sweek.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vag.dashuyun.cn

[B13] 判断是否为数字
来源：http://dtu.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://jxy.gogol.net.cn

PHP:  is_numeric($x)
来源：http://bxz.hcnkem.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lim.mhx1999.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://djf.xziqi.cn

Java: x instanceof Number
来源：http://qhx.yongpay.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jcy.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://fmu.fktsv.cn

C#:   x is int or double or decimal
来源：http://fvs.vqdsnc.cn

[B14] 判断值是否在集合内
来源：http://ojh.ydjk.org.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cec.dashuyun.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rui.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://xsd.fzhhl.top

TS:   [1, 2, 3].includes(x)
来源：http://dme.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lkc.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://toj.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://npy.yj202588.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bdn.tianlin.xyz

[B15] 布尔运算与取反
来源：http://tmy.jqgufenzy.top

Py:   a and b or not c
来源：http://vdg.zhengqikj.top

PHP:  $a && $b || !$c
来源：http://pro.daxiang520.top

JS:   a && b || !c
来源：http://tyo.pycfn.com

TS:   a && b || !c
来源：http://asx.gzhubu.top

Java: a && b || !c
来源：http://kxq.cheryme.top

Go:   a && b || !c
来源：http://bie.zdqjudy.top

Ruby: a && b || !c
来源：http://kai.gaohongyu789.top

C#:   a && b || !c
来源：http://xqb.xingfuxueyuan.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://zoi.yonumen.top


<!-- 参考信息 -->