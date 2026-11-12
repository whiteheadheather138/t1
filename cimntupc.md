代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://imn.cqqwz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ypt.yonumen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sut.xuetiantiany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zte.yj202588.top

[A10] 生成随机数
来源：http://plz.hywenlv.cn

Py:   import random; random.randint(1, 100)
来源：http://qvv.sufxvd.cn

PHP:  random_int(1, 100);
来源：http://xtb.hammf.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cfw.hysaishi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://aoe.ydzc1.top

Java: new Random().nextInt(100) + 1
来源：http://pew.yongpay.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cgc.ydzc1.top

Ruby: rand(1..100)
来源：http://nrd.cqqwz.cn

C#:   new Random().Next(1, 101)
来源：http://urj.quarkkingdee.top

[A11] 条件表达式（三元）
来源：http://pff.shangyingyoupin.top

Py:   "yes" if x > 0 else "no"
来源：http://nus.yfazqb.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://fpu.9152youxi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vfb.epnwcf.com

TS:   x > 0 ? "yes" : "no"
来源：http://mdw.aibaodan.cn

Java: x > 0 ? "yes" : "no"
来源：http://pvj.fanxiaobao.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://own.jinyuanbaomall.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://alj.uphjek.com

C#:   x > 0 ? "yes" : "no"
来源：http://tnh.cqqwz.cn

[A12] 字符串插值 / 格式化
来源：http://cso.zhongyouzk.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yot.gaohongyu789.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zxd.chenlongwang.top

JS:   `Hello, ${name}!`
来源：http://bpo.sjlbkw.cn

TS:   `Hello, ${name}!`
来源：http://tzj.meibo888.top

Java: "Hello, %s!".formatted(name)
来源：http://wif.xylfe.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jax.tarul.cn

Ruby: "Hello, #{name}!"
来源：http://akx.haohaochexian.top

C#:   $"Hello, {name}!"
来源：http://exi.xuetiantiany.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://irw.jianghu66.top

Py:   "第一行\n第二行"
来源：http://tda.sxryk.cn

PHP:  "第一行\n第二行"
来源：http://bsd.xinyue.icu

JS:   "第一行\n第二行"
来源：http://jcz.tanke756.top

TS:   "第一行\n第二行"
来源：http://cne.guowangkeji.top

Java: "第一行\n第二行"
来源：http://jsw.zycfv.cn

Go:   "第一行\n第二行"
来源：http://ubn.jqgfzy.top

Ruby: "第一行\n第二行"
来源：http://ytd.yueranfly.top

C#:   "第一行\n第二行"
来源：http://swx.tarul.cn

[A14] 注释写法
来源：http://yvc.zhijiandao.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://eyd.pengpengdd.cyou

PHP:  // 或 # 单行；/* 多行 */
来源：http://dnc.birdmap.top

JS:   // 单行；/* 多行 */
来源：http://mjo.dashuyun.cn

TS:   // 单行；/* 多行 */
来源：http://uok.vqdsnc.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dmh.yuanzhike.top

Go:   // 单行；/* 多行 */
来源：http://pxy.hysaishi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ymk.sysykeji.top

C#:   // 单行；/* 多行 */
来源：http://lvf.iojbl.cn

[A15] 空值判断与默认值
来源：http://mys.chenjidiqi.icu

Py:   value = data or "默认值"
来源：http://plp.tarul.cn

PHP:  $value = $data ?? "默认值";
来源：http://nvc.bjfxy.top

JS:   const value = data ?? "默认值";
来源：http://ubi.jinyuanbaomall.cn

TS:   const value = data ?? "默认值";
来源：http://ral.cheryme.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mwv.jinqigufen.top

Go:   if data == "" { data = "默认值" }
来源：http://rvj.zhengqikj.top

Ruby: value = data || "默认值"
来源：http://okr.jinqigufen.top

C#:   var value = data ?? "默认值";
来源：http://jiw.ivvv.top

[A16] 真假值判断规则
来源：http://ohi.gzhubu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bns.dianchejie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tom.pengpengdd.cyou

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xil.hnqzz.top

TS:   if (!x) {}
来源：http://tfa.guowangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fnf.316326.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rsp.nanxinkj.top

Ruby: unless x            # nil 与 false 为假
来源：http://anr.smart0.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://elb.fehbvm.com

[A17] 位运算
来源：http://oxq.fzhhl.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mnl.hesvh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pfb.chenjidiqi.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yfj.pycfn.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nzd.9152youxi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://olx.dashuyun.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lwo.cucudq.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oab.nanxuanxn.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pir.fzhhl.top

[A18] 字符与 ASCII 码互转
来源：http://uyh.tianlin.xyz

Py:   ord("A"); chr(65)
来源：http://hyl.fanxiaobao.xyz

PHP:  ord("A"); chr(65)
来源：http://fbu.gzhubu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ikj.fzhhl.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jrj.ivvv.top

Java: (int) 'A'; (char) 65
来源：http://dpg.jqgufenzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fhk.hammf.cn

Ruby: "A".ord; 65.chr
来源：http://lce.yj202588.top

C#:   (int)'A'; (char)65
来源：http://unw.zhiwuduotai.top

[A19] 交换两个变量
来源：http://agv.xingfuxueyuan.xyz

Py:   a, b = b, a
来源：http://lwx.yfazqb.com

PHP:  [$a, $b] = [$b, $a];
来源：http://wkf.hcnkem.com

JS:   [a, b] = [b, a];
来源：http://pih.xinyue.icu

TS:   [a, b] = [b, a];
来源：http://xos.bjfxy.top

Java: int t = a; a = b; b = t;
来源：http://fjp.ybcxt.top

Go:   a, b = b, a
来源：http://oys.c1oappe.top

Ruby: a, b = b, a
来源：http://ref.jyoumei.cn

C#:   (a, b) = (b, a);
来源：http://xtg.shzxlz.cn

[A20] 读取标准输入
来源：http://qej.jianghu66.top

Py:   name = input("请输入：")
来源：http://fsm.zhixingplan.top

PHP:  $name = trim(fgets(STDIN));
来源：http://gxi.gotoacloud.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lhi.ivvv.top

TS:   // Node.js：readline 模块
来源：http://uxb.shanyushiyangkeji.top

Java: new Scanner(System.in).nextLine()
来源：http://ggj.bjfxy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kdp.andypj.xyz

Ruby: gets.chomp
来源：http://zaq.guowangkeji.top

C#:   Console.ReadLine();
来源：http://wfy.vehdjk.com

[A21] 保留指定小数位输出
来源：http://nkq.yongpay.top

Py:   f"{3.14159:.2f}"
来源：http://ulc.smart0.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zcp.hcnkem.com

JS:   (3.14159).toFixed(2)
来源：http://lyh.birdmap.top

TS:   (3.14159).toFixed(2)
来源：http://mst.bbcook.cn

Java: String.format("%.2f", 3.14159)
来源：http://jac.fengsongda.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ufi.zycfv.cn

Ruby: format("%.2f", 3.14159)
来源：http://kuj.xingfuxueyuan.xyz

C#:   3.14159.ToString("F2")
来源：http://czs.iojbl.cn

[A22] 获取字符串长度
来源：http://jfq.kuanghao11.cn

Py:   len(s)
来源：http://dhz.ydjk.org.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iki.jyoumei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vux.kuanghao11.cn

TS:   s.length
来源：http://yzb.sjlbkw.cn

Java: s.length()
来源：http://lju.jlsjyb.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gpz.hfpthk.cn

Ruby: s.length
来源：http://ljv.52xcode.cn

C#:   s.Length
来源：http://rum.ywan-chungtsiang.top

[A23] 大小写转换
来源：http://vdw.meibo888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://rxw.yueranfly.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://atm.yj202588.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nel.uphjek.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ros.tianlin.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mem.cqqwz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fdw.jinqigufen.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pnm.chenzaomai.com

C#:   s.ToUpper(); s.ToLower()
来源：http://hoh.meibo888.top

[A24] 去除首尾空白
来源：http://csq.zhongyouzk.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xyf.yuxming.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rmx.0kj1m.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vkn.yj20258.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tou.xinyue.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lbx.shanyushiyangkeji.top

Go:   strings.TrimSpace(s)
来源：http://wjl.shanyushiyangtech.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tbm.snrcjt.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gpz.shangyingyoupin.top

[A25] 字符串比较
来源：http://njq.hnxiangtu.top

Py:   s1 == s2; s1 != s2
来源：http://rjm.zhoulong.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gbw.sysykeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nsl.mhx1999.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nts.vehdjk.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rha.shuidangran.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://shz.chenlongwang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nsr.sweek.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vkt.yvedp.cn

[A26] 类型转换总览
来源：http://fpe.cdnleiting.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oqy.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lvf.smart0.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://imf.mhx1999.top

TS:   Number() String() Boolean() x as number
来源：http://kii.mhx1999.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hsa.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ras.yanxiufei.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fjb.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xlo.jinyuanbaomall.cn

================================================================================
来源：http://qne.zhengqikj.top

B. 流程控制
来源：http://jfz.dashuyun.cn

================================================================================
来源：http://que.sysykeji.top

[B01] 条件判断 if / else
来源：http://ymp.gotoacloud.top

Py:   result = "正" if x > 0 else "非正"
来源：http://isd.yangfankeji.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fis.bbcook.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pcs.guowangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dmm.gotoacloud.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tou.vehdjk.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jld.yanxiufei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://umm.ydjk.org.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pwe.yonumen.top

[B02] 多分支 else if / elif
来源：http://auq.meibo888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://swl.jinghuilouyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ihh.dianchejie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vyj.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hjt.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ghg.sysykeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://enm.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fuw.vehdjk.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wkd.nanxinkj.top

[B03] switch / match / case
来源：http://yww.zycfv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ocm.pycfn.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cyg.daxiang520.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nip.hcnkem.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://net.smart0.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uxu.hammf.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gva.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://muq.jinqigufen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://prx.jlsjyb.cn

[B04] for 计数循环
来源：http://ulz.tianlin.xyz

Py:   for i in range(10): print(i)
来源：http://poh.9152youxi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vbw.c1oappe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fau.daria6918.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://faa.sweek.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kcr.jqgufenzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zdk.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://tpt.iojbl.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kzu.mhx1999.top

[B05] 遍历数组 / 列表
来源：http://mkj.yj20258888.top

Py:   for item in arr: print(item)
来源：http://apo.zhongyouzk.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rfy.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ekd.snrcjt.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ruz.0kj1m.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eap.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mzg.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://cxe.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kzb.chenlongwang.top

[B06] 遍历字典 / 对象
来源：http://zjd.cheryme.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wuv.nanxinkj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zlk.ydzc1.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jpp.daxiang520.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://thx.daxiang520.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xgo.sufxvd.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pgz.0kj1m.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pyw.iojbl.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rmq.jinqigufen.top

[B07] while 循环
来源：http://jjo.shuidangran.top

Py:   while i < 10: i += 1
来源：http://vyy.tarul.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qld.ehwqpu.com

JS:   while (i < 10) { i++; }
来源：http://ukb.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://ves.yvedp.cn

Java: while (i < 10) { i++; }
来源：http://nhl.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://phk.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://hhh.vqdsnc.cn

C#:   while (i < 10) { i++; }
来源：http://ocy.aibaodan.cn

[B08] do-while（至少执行一次）
来源：http://bcr.nanxuanxn.top

Py:   # 无 do-while：用 while True + break
来源：http://lgb.chenzaomai.com

PHP:  do { $i++; } while ($i < 10);
来源：http://ezf.c1oappe.top

JS:   do { i++; } while (i < 10);
来源：http://kix.yueranfly.top

TS:   do { i++; } while (i < 10);
来源：http://zou.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://dbz.meibo888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://luc.fanxiaobao.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://isg.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://clk.uphjek.com

[B09] break 与 continue
来源：http://kkp.hcnkem.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vdx.316326.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jxa.xziqi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qym.jinqigufen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbt.ivvv.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://msh.cdnleiting.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jof.shuidangran.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dpf.jinyuanbaomall.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ftt.quarkkingdee.top

[B10] 遍历同时拿索引
来源：http://upd.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://skl.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gmb.fengsongda.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qxo.jlsjyb.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mvn.zdbjq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://car.redwolf501.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vir.fengsongda.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hwz.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://coj.snrcjt.cn

[B11] 生成数字序列 / 区间
来源：http://vxj.ydjk.org.cn

Py:   list(range(0, 10, 2))
来源：http://okt.smart0.xyz

PHP:  range(0, 10, 2);
来源：http://isc.chenzaomai.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hgu.zdqjudy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sav.zhijiandao.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vmn.gotoacloud.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xjn.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://rvs.pycfn.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ytv.epnwcf.com

[B12] 跳出多层循环
来源：http://xeu.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mtm.cheryme.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ufe.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rsz.wangshuangyany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sug.jqgfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fhb.daria6918.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gda.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lqu.hnqzz.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dja.hcnkem.com

[B13] 判断是否为数字
来源：http://yyx.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://udn.gogol.net.cn

PHP:  is_numeric($x)
来源：http://cjp.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gxh.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qxc.cucudq.cn

Java: x instanceof Number
来源：http://abr.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wgn.316326.xyz

Ruby: x.is_a?(Numeric)
来源：http://oiq.yj20258.top

C#:   x is int or double or decimal
来源：http://gaa.hammf.cn

[B14] 判断值是否在集合内
来源：http://iji.bbcook.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ezm.zhijiandao.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qxn.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://kva.nanxinkj.top

TS:   [1, 2, 3].includes(x)
来源：http://eor.yj20258.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mam.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://doh.jiagoushi.top

Ruby: [1, 2, 3].include?(x)
来源：http://qkc.guannengcc.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qej.aizwys.cn

[B15] 布尔运算与取反
来源：http://dbr.9152youxi.cn

Py:   a and b or not c
来源：http://xkj.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://shd.ydjk.org.cn

JS:   a && b || !c
来源：http://hvu.sjlbkw.cn

TS:   a && b || !c
来源：http://sqx.zhengqikj.top

Java: a && b || !c
来源：http://qyo.nwbrower.top

Go:   a && b || !c
来源：http://jlt.52xcode.cn

Ruby: a && b || !c
来源：http://son.xziqi.cn

C#:   a && b || !c
来源：http://pyf.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bbr.guannengcc.top

Py:   if not data: return
来源：http://dfd.sweek.top

PHP:  if (!$data) { return; }
来源：http://aal.yangfankeji.com

JS:   if (!data) return;
来源：http://yka.hfpthk.cn

TS:   if (!data) return;
来源：http://xhb.nanxuanxn.top


<!-- 参考信息 -->