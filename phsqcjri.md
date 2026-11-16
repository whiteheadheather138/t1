代发 wailian999

[A10] 生成随机数
来源：http://nau.xuetiantiany.cn

Py:   import random; random.randint(1, 100)
来源：http://yvf.yvedp.cn

PHP:  random_int(1, 100);
来源：http://hvr.cdnleiting.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sev.jqgufenzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lnx.svipenyu.cn

Java: new Random().nextInt(100) + 1
来源：http://wph.jinqigufen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://osm.hesvh.cn

Ruby: rand(1..100)
来源：http://bjd.jqgufenzy.top

C#:   new Random().Next(1, 101)
来源：http://wan.zycfv.cn

[A11] 条件表达式（三元）
来源：http://kqa.cashguo.top

Py:   "yes" if x > 0 else "no"
来源：http://gdg.xuanzx.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://zcx.316326.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://vpa.gogol.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ibk.sysykeji.top

Java: x > 0 ? "yes" : "no"
来源：http://thh.jqgfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://nwc.jqgufenzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://gfp.hnqzz.top

C#:   x > 0 ? "yes" : "no"
来源：http://xwd.jyoumei.cn

[A12] 字符串插值 / 格式化
来源：http://haq.jyoumei.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pbm.xziqi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rzx.xziqi.cn

JS:   `Hello, ${name}!`
来源：http://aee.yj20258888.top

TS:   `Hello, ${name}!`
来源：http://lxj.aizwys.cn

Java: "Hello, %s!".formatted(name)
来源：http://evd.hongshengwenyu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ydl.ehwqpu.com

Ruby: "Hello, #{name}!"
来源：http://azy.nanxinkj.top

C#:   $"Hello, {name}!"
来源：http://evp.chenzaomai.com

[A13] 多行字符串（练习 \n 转义）
来源：http://yto.yj202588.top

Py:   "第一行\n第二行"
来源：http://etc.cheryme.top

PHP:  "第一行\n第二行"
来源：http://nla.nwbrower.top

JS:   "第一行\n第二行"
来源：http://zcq.sufxvd.cn

TS:   "第一行\n第二行"
来源：http://pei.zdqjudy.top

Java: "第一行\n第二行"
来源：http://pfq.xuanzx.com

Go:   "第一行\n第二行"
来源：http://apu.jqgufenzy.top

Ruby: "第一行\n第二行"
来源：http://lzy.shuidangran.top

C#:   "第一行\n第二行"
来源：http://row.hammf.cn

[A14] 注释写法
来源：http://wwj.jqgufenzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qwc.bbcook.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gek.haohaochexian.top

JS:   // 单行；/* 多行 */
来源：http://dmt.yuxming.cn

TS:   // 单行；/* 多行 */
来源：http://gqa.chenlongwang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mdh.sysykeji.top

Go:   // 单行；/* 多行 */
来源：http://fzj.nwbrower.top

Ruby: # 单行；=begin 多行 =end
来源：http://byt.iojbl.cn

C#:   // 单行；/* 多行 */
来源：http://zad.svipenyu.cn

[A15] 空值判断与默认值
来源：http://ksd.jinghuilouyu.cn

Py:   value = data or "默认值"
来源：http://vnl.yongpay.top

PHP:  $value = $data ?? "默认值";
来源：http://vlu.zhijiandao.cn

JS:   const value = data ?? "默认值";
来源：http://fmk.jinqigfzy.top

TS:   const value = data ?? "默认值";
来源：http://kdk.ppjwa.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://trb.zhixingplan.top

Go:   if data == "" { data = "默认值" }
来源：http://djr.yongpay.top

Ruby: value = data || "默认值"
来源：http://ioe.jianghu66.top

C#:   var value = data ?? "默认值";
来源：http://wcs.yj202588.top

[A16] 真假值判断规则
来源：http://dst.snrcjt.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lkg.zdqjudy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://okz.ydjk.org.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jij.smart0.xyz

TS:   if (!x) {}
来源：http://joz.fanxiaobao.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wsi.hammf.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ccp.ivvv.top

Ruby: unless x            # nil 与 false 为假
来源：http://kmq.haohaochexian.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mad.dashuyun.cn

[A17] 位运算
来源：http://xur.gaohongyu789.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fxb.uphjek.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cvk.havefunace.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://drs.vqdsnc.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pkn.bjfxy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uvh.shanyushiyangtech.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zwp.jiagoushi.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rfe.sjlbkw.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uzs.meibo888.top

[A18] 字符与 ASCII 码互转
来源：http://euw.wangshuangyany.cn

Py:   ord("A"); chr(65)
来源：http://otw.0kj1m.cn

PHP:  ord("A"); chr(65)
来源：http://qtq.meibo888.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fja.daxiang520.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iec.ivvv.top

Java: (int) 'A'; (char) 65
来源：http://whw.c1oappe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wrj.aibaodan.cn

Ruby: "A".ord; 65.chr
来源：http://pyq.gotoacloud.top

C#:   (int)'A'; (char)65
来源：http://eab.zhengqikj.top

[A19] 交换两个变量
来源：http://axb.zdbjq.cn

Py:   a, b = b, a
来源：http://dgp.zdqjudy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hle.kuanghao11.cn

JS:   [a, b] = [b, a];
来源：http://tdx.zhoulong.xyz

TS:   [a, b] = [b, a];
来源：http://wgi.ywan-chungtsiang.top

Java: int t = a; a = b; b = t;
来源：http://wjj.guowangkeji.top

Go:   a, b = b, a
来源：http://rzr.hfpthk.cn

Ruby: a, b = b, a
来源：http://ihw.iojbl.cn

C#:   (a, b) = (b, a);
来源：http://enl.yvedp.cn

[A20] 读取标准输入
来源：http://txj.bbcook.cn

Py:   name = input("请输入：")
来源：http://dmr.jiagoushi.top

PHP:  $name = trim(fgets(STDIN));
来源：http://scn.yvedp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ytn.0kj1m.cn

TS:   // Node.js：readline 模块
来源：http://dno.svipenyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://qaw.sysykeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://onu.xinyue.icu

Ruby: gets.chomp
来源：http://atz.cucudq.cn

C#:   Console.ReadLine();
来源：http://ouu.tanke756.top

[A21] 保留指定小数位输出
来源：http://mtf.sysykeji.top

Py:   f"{3.14159:.2f}"
来源：http://hwy.yj20258.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dzb.zdqjudy.top

JS:   (3.14159).toFixed(2)
来源：http://puf.yangfankeji.com

TS:   (3.14159).toFixed(2)
来源：http://opa.kuanghao11.cn

Java: String.format("%.2f", 3.14159)
来源：http://bip.yvedp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kbx.gogol.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://ixq.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://ceq.aizwys.cn

[A22] 获取字符串长度
来源：http://tnb.jinqigfzy.top

Py:   len(s)
来源：http://wvy.chenzaomai.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tcv.gogol.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bqp.hywenlv.cn

TS:   s.length
来源：http://tad.meibo888.top

Java: s.length()
来源：http://mfd.tianlin.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://soj.jlsjyb.cn

Ruby: s.length
来源：http://rut.xingfuxueyuan.xyz

C#:   s.Length
来源：http://ggi.bjfxy.top

[A23] 大小写转换
来源：http://gvz.zycfv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hmv.tarul.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hsg.yfazqb.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ijc.ppjwa.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rpj.ydjk.org.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://brj.yuxming.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oyv.sjlbkw.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mcd.hongshengwenyu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rio.jqgufenzy.top

[A24] 去除首尾空白
来源：http://kwx.vehdjk.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kpl.guowangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tdq.ehwqpu.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kdp.vehdjk.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ioz.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qxf.316326.xyz

Go:   strings.TrimSpace(s)
来源：http://qhu.hesvh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jew.aibaodan.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gtp.aibaodan.cn

[A25] 字符串比较
来源：http://vex.yueranfly.top

Py:   s1 == s2; s1 != s2
来源：http://kks.smart0.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jpk.316326.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://upc.shanyushiyangtech.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kcp.dianchejie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mii.hongshengwenyu.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aqi.fehbvm.com

Ruby: s1 == s2; s1 <=> s2
来源：http://giv.xziqi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pef.yj20258.top

[A26] 类型转换总览
来源：http://frl.hammf.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ife.hnqzz.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gqv.guannengcc.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yrv.c1oappe.top

TS:   Number() String() Boolean() x as number
来源：http://gcm.hysaishi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qne.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bmc.pengpengdd.cyou

Ruby: to_i to_f to_s to_sym to_a
来源：http://ghd.xingfuxueyuan.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zuj.yj202588.top

================================================================================
来源：http://sqn.cdnleiting.top

B. 流程控制
来源：http://nsi.sysykeji.top

================================================================================
来源：http://lux.snrcjt.cn

[B01] 条件判断 if / else
来源：http://zoo.yuanzhike.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jvk.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fub.dashuyun.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ihq.hfpthk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tbq.gotoacloud.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tdg.wangdashe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ndq.ehwqpu.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nfw.9152youxi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vad.mhx1999.top

[B02] 多分支 else if / elif
来源：http://cky.yueranfly.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vnd.ydzc1.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sjz.gogol.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://erh.hnxiangtu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://btg.hesvh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tqo.cqqwz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jud.zdqjudy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://inn.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zzv.shangyingyoupin.top

[B03] switch / match / case
来源：http://gpz.uphjek.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://emt.sweek.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mxr.fanxiaobao.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kxs.feifeiyinyue.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://soa.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ndb.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ddr.pengpengdd.cyou

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ecv.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dbv.xinyue.icu

[B04] for 计数循环
来源：http://wbg.haohaochexian.top

Py:   for i in range(10): print(i)
来源：http://lgq.shanyushiyangtech.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lje.guannengcc.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iij.xuetiantiany.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uzy.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://odw.yuxming.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pdj.jianghu66.top

Ruby: 10.times { |i| puts i }
来源：http://mjn.zhongyouzk.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ggy.quarkkingdee.top

[B05] 遍历数组 / 列表
来源：http://fla.zhijiandao.cn

Py:   for item in arr: print(item)
来源：http://tks.yj20258888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mue.shuidangran.top

JS:   for (const item of arr) { console.log(item); }
来源：http://umd.haohaochexian.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tvm.nanxuanxn.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kki.havefunace.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hhb.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://wdu.sjlbkw.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bfm.ybcxt.top

[B06] 遍历字典 / 对象
来源：http://xyn.hcnkem.com

Py:   for k, v in d.items(): print(k, v)
来源：http://nom.ywan-chungtsiang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://day.ehwqpu.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wjz.hesvh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wvs.mhx1999.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vfb.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://adu.chenjidiqi.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pwb.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hxo.snrcjt.cn

[B07] while 循环
来源：http://csz.yanxiufei.cn

Py:   while i < 10: i += 1
来源：http://fia.pengpengdd.cyou

PHP:  while ($i < 10) { $i++; }
来源：http://eko.zhijiandao.cn

JS:   while (i < 10) { i++; }
来源：http://aqn.zdbjq.cn

TS:   while (i < 10) { i++; }
来源：http://gmc.sysykeji.top

Java: while (i < 10) { i++; }
来源：http://rno.ehwqpu.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://suu.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://rze.jqgufenzy.top

C#:   while (i < 10) { i++; }
来源：http://xam.yongpay.top

[B08] do-while（至少执行一次）
来源：http://mnq.dashuyun.cn

Py:   # 无 do-while：用 while True + break
来源：http://rse.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hcx.wangshuangyany.cn

JS:   do { i++; } while (i < 10);
来源：http://shk.c1oappe.top

TS:   do { i++; } while (i < 10);
来源：http://diu.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://qwf.xinyue.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://zik.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gfs.daxiang520.top

C#:   do { i++; } while (i < 10);
来源：http://cab.daxiang520.top

[B09] break 与 continue
来源：http://afc.xingfuxueyuan.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dpj.zhiwuduotai.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dda.sysykeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jhe.hammf.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hgo.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mbg.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dni.zhoulong.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://etp.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rvi.hongshengwenyu.top

[B10] 遍历同时拿索引
来源：http://kwe.zycfv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ftg.fktsv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kps.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fcf.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kbr.svipenyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mlv.yonumen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://soa.aibaodan.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ljf.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nxu.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://tcg.feifeiyinyue.top

Py:   list(range(0, 10, 2))
来源：http://ctn.meibo888.top

PHP:  range(0, 10, 2);
来源：http://nol.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://inl.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dvb.jlsjyb.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rws.vehdjk.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iwm.quarkkingdee.top

Ruby: (0...10).step(2).to_a
来源：http://fpp.bbcook.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ybw.zhiwuduotai.top

[B12] 跳出多层循环
来源：http://zup.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ujd.daria6918.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://egn.ydjk.org.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tzl.jianghu66.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ayq.tian-w.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bll.guowangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hxa.havefunace.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://img.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cls.sweek.top

[B13] 判断是否为数字
来源：http://uvz.ppjwa.cn

Py:   isinstance(x, (int, float))
来源：http://jrv.chenlongwang.top

PHP:  is_numeric($x)
来源：http://urx.feifeiyinyue.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uch.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zco.daria6918.cn

Java: x instanceof Number
来源：http://zst.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://byb.havefunace.top

Ruby: x.is_a?(Numeric)
来源：http://gvm.dashuyun.cn

C#:   x is int or double or decimal
来源：http://xcq.guannengcc.top

[B14] 判断值是否在集合内
来源：http://sbk.xuanzx.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wnh.fengsongda.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hhd.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://brs.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://aob.hongshengwenyu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hqu.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nfq.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ctx.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ufx.cqqwz.cn

[B15] 布尔运算与取反
来源：http://rzi.snrcjt.cn

Py:   a and b or not c
来源：http://yhq.yanxiufei.cn

PHP:  $a && $b || !$c
来源：http://fwg.sweek.top

JS:   a && b || !c
来源：http://omc.9152youxi.cn

TS:   a && b || !c
来源：http://ete.yongpay.top

Java: a && b || !c
来源：http://nes.dashuyun.cn

Go:   a && b || !c
来源：http://ayk.jyoumei.cn

Ruby: a && b || !c
来源：http://hbv.shuidangran.top

C#:   a && b || !c
来源：http://mpt.daria6918.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zkh.fktsv.cn

Py:   if not data: return
来源：http://bjw.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://zbf.316326.xyz

JS:   if (!data) return;
来源：http://knr.fanxiaobao.xyz

TS:   if (!data) return;
来源：http://jtt.zhiwuduotai.top

Java: if (data == null) return;
来源：http://tuk.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://yyv.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://sad.chenjidiqi.icu

C#:   if (data == null) return;
来源：http://kwa.chenjidiqi.icu


<!-- 参考信息 -->