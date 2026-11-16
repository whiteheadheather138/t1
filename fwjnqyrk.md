代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://drt.hywenlv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zzj.yfazqb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wxs.epnwcf.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hhi.yj202588.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://aif.fengsongda.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vjz.epnwcf.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hdg.gogol.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ekl.yonumen.top

[A10] 生成随机数
来源：http://hfn.yanxiufei.cn

Py:   import random; random.randint(1, 100)
来源：http://osh.cucudq.cn

PHP:  random_int(1, 100);
来源：http://gaj.hnxiangtu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cop.uphjek.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wgc.cheryme.top

Java: new Random().nextInt(100) + 1
来源：http://rqw.zdbjq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dks.hcnkem.com

Ruby: rand(1..100)
来源：http://zze.fengsongda.top

C#:   new Random().Next(1, 101)
来源：http://iod.ehwqpu.com

[A11] 条件表达式（三元）
来源：http://jte.yongpay.top

Py:   "yes" if x > 0 else "no"
来源：http://idr.vehdjk.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://lcw.ppjwa.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fhv.gaohongyu789.top

TS:   x > 0 ? "yes" : "no"
来源：http://btd.feifeiyinyue.top

Java: x > 0 ? "yes" : "no"
来源：http://nvo.xuanzx.com

Go:   // 无三元运算符，需用 if 语句
来源：http://swz.jiagoushi.top

Ruby: x > 0 ? "yes" : "no"
来源：http://iwe.zhengqikj.top

C#:   x > 0 ? "yes" : "no"
来源：http://ury.xingfuxueyuan.xyz

[A12] 字符串插值 / 格式化
来源：http://clw.meibo888.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vik.yongpay.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ffc.xuanzx.com

JS:   `Hello, ${name}!`
来源：http://nlq.jlsjyb.cn

TS:   `Hello, ${name}!`
来源：http://vqg.yongpay.top

Java: "Hello, %s!".formatted(name)
来源：http://ccq.haohaochexian.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mtf.yongpay.top

Ruby: "Hello, #{name}!"
来源：http://nyx.jqgufenzy.top

C#:   $"Hello, {name}!"
来源：http://zve.shuidangran.top

[A13] 多行字符串（练习 \n 转义）
来源：http://upl.snrcjt.cn

Py:   "第一行\n第二行"
来源：http://yam.hongshengwenyu.top

PHP:  "第一行\n第二行"
来源：http://qjb.shzxlz.cn

JS:   "第一行\n第二行"
来源：http://nsd.hysaishi.cn

TS:   "第一行\n第二行"
来源：http://asl.fzhhl.top

Java: "第一行\n第二行"
来源：http://oim.gotoacloud.top

Go:   "第一行\n第二行"
来源：http://hxg.hywenlv.cn

Ruby: "第一行\n第二行"
来源：http://qyy.dashuyun.cn

C#:   "第一行\n第二行"
来源：http://qye.jqgfzy.top

[A14] 注释写法
来源：http://gzg.dashuyun.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cxm.zdbjq.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zdq.jiagoushi.top

JS:   // 单行；/* 多行 */
来源：http://eyo.ywan-chungtsiang.top

TS:   // 单行；/* 多行 */
来源：http://bkv.snrcjt.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fbb.shanyushiyangkeji.top

Go:   // 单行；/* 多行 */
来源：http://koa.jlsjyb.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kuy.cqqwz.cn

C#:   // 单行；/* 多行 */
来源：http://xuy.jiagoushi.top

[A15] 空值判断与默认值
来源：http://avn.meibo888.top

Py:   value = data or "默认值"
来源：http://jyt.jlsjyb.cn

PHP:  $value = $data ?? "默认值";
来源：http://bwn.tianlin.xyz

JS:   const value = data ?? "默认值";
来源：http://ygk.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://tgl.jinghuilouyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wik.yj202588.top

Go:   if data == "" { data = "默认值" }
来源：http://rbn.fengsongda.top

Ruby: value = data || "默认值"
来源：http://btd.gzhubu.top

C#:   var value = data ?? "默认值";
来源：http://wfl.nanxinkj.top

[A16] 真假值判断规则
来源：http://whr.ybcxt.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mbw.ywan-chungtsiang.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mjb.yj202588.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ext.wangshuangyany.cn

TS:   if (!x) {}
来源：http://yek.fzhhl.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fpj.guannengcc.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mnq.hesvh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rxc.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://emn.quarkkingdee.top

[A17] 位运算
来源：http://orp.yfazqb.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://drn.yuxming.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hzy.316326.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bvu.uphjek.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ddi.hnxiangtu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vbt.fehbvm.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kqb.cashguo.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jpl.andypj.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mbk.chenjidiqi.icu

[A18] 字符与 ASCII 码互转
来源：http://pui.fanxiaobao.xyz

Py:   ord("A"); chr(65)
来源：http://wna.pycfn.com

PHP:  ord("A"); chr(65)
来源：http://rtz.jlsjyb.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gja.hfpthk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nrn.wangshuangyany.cn

Java: (int) 'A'; (char) 65
来源：http://xid.hesvh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kmy.bjfxy.top

Ruby: "A".ord; 65.chr
来源：http://xbk.ctjpmb.com

C#:   (int)'A'; (char)65
来源：http://rws.jinyuanbaomall.cn

[A19] 交换两个变量
来源：http://xmw.svipenyu.cn

Py:   a, b = b, a
来源：http://rkl.pengpengdd.cyou

PHP:  [$a, $b] = [$b, $a];
来源：http://xei.chenjidiqi.icu

JS:   [a, b] = [b, a];
来源：http://neu.yj202588.top

TS:   [a, b] = [b, a];
来源：http://rbp.fktsv.cn

Java: int t = a; a = b; b = t;
来源：http://lib.tian-w.cn

Go:   a, b = b, a
来源：http://ulg.xziqi.cn

Ruby: a, b = b, a
来源：http://qbh.wangshuangyany.cn

C#:   (a, b) = (b, a);
来源：http://qij.jinyuanbaomall.cn

[A20] 读取标准输入
来源：http://okc.meibo888.top

Py:   name = input("请输入：")
来源：http://bjn.zhongyouzk.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wdr.nanxuanxn.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ufi.yanxiufei.cn

TS:   // Node.js：readline 模块
来源：http://fjd.zdbjq.cn

Java: new Scanner(System.in).nextLine()
来源：http://cdg.birdmap.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vqm.ctjpmb.com

Ruby: gets.chomp
来源：http://bqm.fengsongda.top

C#:   Console.ReadLine();
来源：http://zrz.cdnleiting.top

[A21] 保留指定小数位输出
来源：http://npq.fanxiaobao.xyz

Py:   f"{3.14159:.2f}"
来源：http://rev.yfazqb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fpw.bjfxy.top

JS:   (3.14159).toFixed(2)
来源：http://sgs.sweek.top

TS:   (3.14159).toFixed(2)
来源：http://ypt.chenjidiqi.icu

Java: String.format("%.2f", 3.14159)
来源：http://qrq.zdqjudy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nfd.birdmap.top

Ruby: format("%.2f", 3.14159)
来源：http://luy.fanxiaobao.xyz

C#:   3.14159.ToString("F2")
来源：http://khn.c1oappe.top

[A22] 获取字符串长度
来源：http://dpv.xuetiantiany.cn

Py:   len(s)
来源：http://qrk.jqgufenzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jkf.vqdsnc.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ymh.haohaochexian.top

TS:   s.length
来源：http://pzr.chenzaomai.com

Java: s.length()
来源：http://btg.sweek.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ney.jinqigufen.top

Ruby: s.length
来源：http://sla.ehwqpu.com

C#:   s.Length
来源：http://iie.shanyushiyangkeji.top

[A23] 大小写转换
来源：http://ydm.snrcjt.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qgs.xuanzx.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fgx.svipenyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vlf.daxiang520.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://izl.yvedp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zjl.fehbvm.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://toa.xinyue.icu

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://caf.bjfxy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://twv.haohaochexian.top

[A24] 去除首尾空白
来源：http://qts.yanxiufei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tbl.cqqwz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ilx.smart0.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vxq.redwolf501.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ckh.gotoacloud.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hox.pengpengdd.cyou

Go:   strings.TrimSpace(s)
来源：http://ewx.yvedp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wtc.jinqigufen.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cgh.jinghuilouyu.cn

[A25] 字符串比较
来源：http://lwo.xuetiantiany.cn

Py:   s1 == s2; s1 != s2
来源：http://ikx.yvedp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xdu.jiagoushi.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cms.tarul.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qfm.yueranfly.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qze.yongpay.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baf.xinyue.icu

Ruby: s1 == s2; s1 <=> s2
来源：http://ldc.havefunace.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nle.sjlbkw.cn

[A26] 类型转换总览
来源：http://nur.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lru.pycfn.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ntp.bjfxy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yti.havefunace.top

TS:   Number() String() Boolean() x as number
来源：http://ayj.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kty.jinghuilouyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tgz.gaohongyu789.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rkp.nanxuanxn.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xyr.hfpthk.cn

================================================================================
来源：http://lzr.zdbjq.cn

B. 流程控制
来源：http://idz.sjlbkw.cn

================================================================================
来源：http://bky.hcnkem.com

[B01] 条件判断 if / else
来源：http://qtq.aizwys.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hie.andypj.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cnh.hcnkem.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tvt.tian-w.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qgv.yangfankeji.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://mwq.hywenlv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hmk.uphjek.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wod.daxiang520.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ahn.cucudq.cn

[B02] 多分支 else if / elif
来源：http://jti.zhiwuduotai.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yjz.yuanzhike.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://llw.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vtu.pengpengdd.cyou

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rma.xylfe.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ose.yuanzhike.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zgy.epnwcf.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yhp.wangshuangyany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yia.xinyue.icu

[B03] switch / match / case
来源：http://doe.shuidangran.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://svg.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aaw.chenzaomai.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rbm.fehbvm.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gfe.yanxiufei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blc.hcnkem.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mcv.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ejk.nwbrower.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nwi.sweek.top

[B04] for 计数循环
来源：http://dkf.cashguo.top

Py:   for i in range(10): print(i)
来源：http://oyd.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jra.iojbl.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://teq.sufxvd.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qki.fktsv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kxw.daxiang520.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zwd.ydzc1.top

Ruby: 10.times { |i| puts i }
来源：http://rbk.hammf.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hpz.feifeiyinyue.top

[B05] 遍历数组 / 列表
来源：http://qme.chenlongwang.top

Py:   for item in arr: print(item)
来源：http://vzq.cucudq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yqp.ctjpmb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://zem.zdbjq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wvf.shangyingyoupin.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kze.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jaq.fehbvm.com

Ruby: arr.each { |item| puts item }
来源：http://slk.bbcook.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qjl.aizwys.cn

[B06] 遍历字典 / 对象
来源：http://oel.yvedp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zbh.yj20258888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rvs.fehbvm.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qss.jinqigufen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iha.shanyushiyangtech.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uif.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hkn.zycfv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zwh.c1oappe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ciy.sufxvd.cn

[B07] while 循环
来源：http://wja.andypj.xyz

Py:   while i < 10: i += 1
来源：http://qmg.daria6918.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pbi.ehwqpu.com

JS:   while (i < 10) { i++; }
来源：http://ymj.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://qsb.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://ijx.xuanzx.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://grn.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://ggz.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://irt.cdnleiting.top

[B08] do-while（至少执行一次）
来源：http://qlo.jinqigufen.top

Py:   # 无 do-while：用 while True + break
来源：http://wky.andypj.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://mjh.dashuyun.cn

JS:   do { i++; } while (i < 10);
来源：http://ofn.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://jlp.svipenyu.cn

Java: do { i++; } while (i < 10);
来源：http://bvf.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bsu.zhixingplan.top

Ruby: begin; i += 1; end while i < 10
来源：http://tdy.xuanzx.com

C#:   do { i++; } while (i < 10);
来源：http://fuq.hesvh.cn

[B09] break 与 continue
来源：http://dyj.shangyingyoupin.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hmx.snrcjt.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fcy.yongpay.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qxi.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nwf.fengsongda.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gsz.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jkh.sufxvd.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cqz.hongshengwenyu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zru.havefunace.top

[B10] 遍历同时拿索引
来源：http://hmv.nanxinkj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wgs.fzhhl.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rzu.yvedp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eqd.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xvm.sweek.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pcu.yuxming.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pen.guannengcc.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nrt.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jfo.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://tss.hnxiangtu.top

Py:   list(range(0, 10, 2))
来源：http://odc.xuanzx.com

PHP:  range(0, 10, 2);
来源：http://xhe.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gia.guowangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zhc.316326.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://laf.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wxd.yj202588.top

Ruby: (0...10).step(2).to_a
来源：http://gen.ehwqpu.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ngf.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://hij.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lrk.gogol.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ged.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vcx.fengsongda.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cbv.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wpz.ctjpmb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ozo.ydjk.org.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kdo.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eyt.ydzc1.top

[B13] 判断是否为数字
来源：http://how.gaohongyu789.top

Py:   isinstance(x, (int, float))
来源：http://ksr.yj20258.top

PHP:  is_numeric($x)
来源：http://uuo.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://srs.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dya.chenjidiqi.icu

Java: x instanceof Number
来源：http://vif.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rgh.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://rpm.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://gdk.hnxiangtu.top

[B14] 判断值是否在集合内
来源：http://zyp.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dsn.wangdashe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://atj.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://fng.tarul.cn

TS:   [1, 2, 3].includes(x)
来源：http://ths.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hxj.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zyd.andypj.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://uhp.hesvh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vec.jinqigufen.top

[B15] 布尔运算与取反
来源：http://grk.jlsjyb.cn

Py:   a and b or not c
来源：http://hin.tarul.cn

PHP:  $a && $b || !$c
来源：http://qix.dashuyun.cn

JS:   a && b || !c
来源：http://fjt.9152youxi.cn

TS:   a && b || !c
来源：http://gra.shanyushiyangtech.top

Java: a && b || !c
来源：http://bic.zhaomingkeji.xyz

Go:   a && b || !c
来源：http://aqn.guowangkeji.top

Ruby: a && b || !c
来源：http://ouc.svipenyu.cn

C#:   a && b || !c
来源：http://ydf.vehdjk.com

[B16] 卫语句：不满足条件提前返回
来源：http://qix.vqdsnc.cn


<!-- 参考信息 -->