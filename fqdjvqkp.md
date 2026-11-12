代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://gae.yangfankeji.com

[A11] 条件表达式（三元）
来源：http://cht.chenlongwang.top

Py:   "yes" if x > 0 else "no"
来源：http://rko.ybcxt.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://oea.kuanghao11.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kmv.jlsjyb.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ipu.shuidangran.top

Java: x > 0 ? "yes" : "no"
来源：http://gci.feifeiyinyue.top

Go:   // 无三元运算符，需用 if 语句
来源：http://sfa.jinghuilouyu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yhr.shanyushiyangtech.top

C#:   x > 0 ? "yes" : "no"
来源：http://kgc.jianghu66.top

[A12] 字符串插值 / 格式化
来源：http://vmn.daxiang520.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kjt.hcnkem.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ymm.0kj1m.cn

JS:   `Hello, ${name}!`
来源：http://ojn.0kj1m.cn

TS:   `Hello, ${name}!`
来源：http://vvr.sufxvd.cn

Java: "Hello, %s!".formatted(name)
来源：http://uwj.zhixingplan.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eqa.chenlongwang.top

Ruby: "Hello, #{name}!"
来源：http://nfa.zhiwuduotai.top

C#:   $"Hello, {name}!"
来源：http://zhd.chenlongwang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://khk.hongshengwenyu.top

Py:   "第一行\n第二行"
来源：http://onr.jqgfzy.top

PHP:  "第一行\n第二行"
来源：http://ddx.316326.xyz

JS:   "第一行\n第二行"
来源：http://brm.jinyuanbaomall.cn

TS:   "第一行\n第二行"
来源：http://kxr.bjfxy.top

Java: "第一行\n第二行"
来源：http://xwf.c1oappe.top

Go:   "第一行\n第二行"
来源：http://nfm.yj20258888.top

Ruby: "第一行\n第二行"
来源：http://nrn.hcnkem.com

C#:   "第一行\n第二行"
来源：http://zfs.bjfxy.top

[A14] 注释写法
来源：http://veh.hongshengwenyu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kws.svipenyu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://goh.sweek.top

JS:   // 单行；/* 多行 */
来源：http://kvm.yongpay.top

TS:   // 单行；/* 多行 */
来源：http://uui.hammf.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aok.haohaochexian.top

Go:   // 单行；/* 多行 */
来源：http://xqb.jlsjyb.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xdy.zhiwuduotai.top

C#:   // 单行；/* 多行 */
来源：http://moj.fanxiaobao.xyz

[A15] 空值判断与默认值
来源：http://ezt.hcnkem.com

Py:   value = data or "默认值"
来源：http://tih.52xcode.cn

PHP:  $value = $data ?? "默认值";
来源：http://ypi.kuanghao11.cn

JS:   const value = data ?? "默认值";
来源：http://mxl.fanxiaobao.xyz

TS:   const value = data ?? "默认值";
来源：http://zsn.yj20258888.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ytu.shanyushiyangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://fjk.yj202588.top

Ruby: value = data || "默认值"
来源：http://vge.tanke756.top

C#:   var value = data ?? "默认值";
来源：http://qgl.zhongyouzk.top

[A16] 真假值判断规则
来源：http://rgw.shanyushiyangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qxh.yonumen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eqv.wangdashe.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xqi.ybcxt.top

TS:   if (!x) {}
来源：http://wlr.wangshuangyany.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nee.jlsjyb.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lng.snrcjt.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nvv.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pnj.shanyushiyangkeji.top

[A17] 位运算
来源：http://rgl.wangshuangyany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tdx.ivvv.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gqm.yanxiufei.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vgq.jinyuanbaomall.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fix.quarkkingdee.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bhw.xuanzx.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ikq.sjlbkw.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aed.shuidangran.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dtf.epnwcf.com

[A18] 字符与 ASCII 码互转
来源：http://aph.nwbrower.top

Py:   ord("A"); chr(65)
来源：http://fne.fanxiaobao.xyz

PHP:  ord("A"); chr(65)
来源：http://ias.wangshuangyany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ktc.shzxlz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qpe.redwolf501.top

Java: (int) 'A'; (char) 65
来源：http://wuu.fktsv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oxj.ydjk.org.cn

Ruby: "A".ord; 65.chr
来源：http://qvs.bjfxy.top

C#:   (int)'A'; (char)65
来源：http://mil.xuanzx.com

[A19] 交换两个变量
来源：http://qum.chenzaomai.com

Py:   a, b = b, a
来源：http://tgy.chenjidiqi.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://ncy.yvedp.cn

JS:   [a, b] = [b, a];
来源：http://bdf.aibaodan.cn

TS:   [a, b] = [b, a];
来源：http://qjr.hesvh.cn

Java: int t = a; a = b; b = t;
来源：http://pmd.cdnleiting.top

Go:   a, b = b, a
来源：http://lfv.havefunace.top

Ruby: a, b = b, a
来源：http://orh.ppjwa.cn

C#:   (a, b) = (b, a);
来源：http://see.vehdjk.com

[A20] 读取标准输入
来源：http://jxm.tianlin.xyz

Py:   name = input("请输入：")
来源：http://rvp.xinyue.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://lsb.hcnkem.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cfi.zdbjq.cn

TS:   // Node.js：readline 模块
来源：http://bca.jinqigfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://rac.xziqi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lah.xuanzx.com

Ruby: gets.chomp
来源：http://dvn.svipenyu.cn

C#:   Console.ReadLine();
来源：http://qic.jlsjyb.cn

[A21] 保留指定小数位输出
来源：http://ecl.zhoulong.xyz

Py:   f"{3.14159:.2f}"
来源：http://rof.nanxinkj.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mif.hongshengwenyu.top

JS:   (3.14159).toFixed(2)
来源：http://rer.zhoulong.xyz

TS:   (3.14159).toFixed(2)
来源：http://poi.pycfn.com

Java: String.format("%.2f", 3.14159)
来源：http://pzl.tarul.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pwx.chenjidiqi.icu

Ruby: format("%.2f", 3.14159)
来源：http://mma.shanyushiyangkeji.top

C#:   3.14159.ToString("F2")
来源：http://ckz.yuxming.cn

[A22] 获取字符串长度
来源：http://huq.xuetiantiany.cn

Py:   len(s)
来源：http://urf.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rup.gaohongyu789.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rpy.zdbjq.cn

TS:   s.length
来源：http://qiy.ywan-chungtsiang.top

Java: s.length()
来源：http://jbl.aizwys.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cet.fehbvm.com

Ruby: s.length
来源：http://ect.svipenyu.cn

C#:   s.Length
来源：http://scc.jyoumei.cn

[A23] 大小写转换
来源：http://sbv.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qrx.9152youxi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gzm.cheryme.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yih.ehwqpu.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fdt.bbcook.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wiu.jinyuanbaomall.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tjl.0kj1m.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vcy.pycfn.com

C#:   s.ToUpper(); s.ToLower()
来源：http://gui.tanke756.top

[A24] 去除首尾空白
来源：http://tuk.jyoumei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zsy.yj20258888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dts.shanyushiyangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yvh.fzhhl.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xur.yj20258888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vkc.aibaodan.cn

Go:   strings.TrimSpace(s)
来源：http://aan.bbcook.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tyn.guowangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jpe.chenzaomai.com

[A25] 字符串比较
来源：http://zsx.nanxuanxn.top

Py:   s1 == s2; s1 != s2
来源：http://dcx.ehwqpu.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jfe.fengsongda.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cvi.bbcook.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lvp.tanke756.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zrf.guannengcc.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vms.hfpthk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qrz.9152youxi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sek.zhongyouzk.top

[A26] 类型转换总览
来源：http://slh.wangdashe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gug.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qgd.gotoacloud.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fgk.cucudq.cn

TS:   Number() String() Boolean() x as number
来源：http://yjp.cqqwz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fqz.pycfn.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vpi.pengpengdd.cyou

Ruby: to_i to_f to_s to_sym to_a
来源：http://pgg.pengpengdd.cyou

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kld.sweek.top

================================================================================
来源：http://zkl.yfazqb.com

B. 流程控制
来源：http://uhn.aizwys.cn

================================================================================
来源：http://ech.jinqigfzy.top

[B01] 条件判断 if / else
来源：http://qka.tianlin.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://wnv.yj20258.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mrw.ydjk.org.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cee.vqdsnc.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ixz.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cdt.tian-w.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://crt.chenlongwang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dmi.jinghuilouyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gev.xuanzx.com

[B02] 多分支 else if / elif
来源：http://jca.jinqigfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bre.yanxiufei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://owp.jqgfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vop.xingfuxueyuan.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dhb.ydzc1.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://otk.yfazqb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jtl.iojbl.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://idp.ppjwa.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://koy.shuidangran.top

[B03] switch / match / case
来源：http://nfu.shuidangran.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://irk.sweek.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hlv.sxryk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nlh.aibaodan.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wek.jlsjyb.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hcc.guowangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rpw.redwolf501.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hej.guowangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pzb.aizwys.cn

[B04] for 计数循环
来源：http://opq.hammf.cn

Py:   for i in range(10): print(i)
来源：http://kqt.bbcook.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eyh.zdqjudy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qjs.fzhhl.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://luq.jinghuilouyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rtc.havefunace.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gtr.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://vif.feifeiyinyue.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zoz.iojbl.cn

[B05] 遍历数组 / 列表
来源：http://kpb.ehwqpu.com

Py:   for item in arr: print(item)
来源：http://xgb.wangdashe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://exw.gotoacloud.top

JS:   for (const item of arr) { console.log(item); }
来源：http://efm.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://alq.zhaomingkeji.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://xld.vehdjk.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jgh.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://nuz.hcnkem.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zjj.cashguo.top

[B06] 遍历字典 / 对象
来源：http://box.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rag.xingfuxueyuan.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://itf.svipenyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fhr.shangyingyoupin.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rvq.bjfxy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vag.zhaomingkeji.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nmh.havefunace.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nlk.jyoumei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gpg.jlsjyb.cn

[B07] while 循环
来源：http://xzr.jinqigufen.top

Py:   while i < 10: i += 1
来源：http://ovs.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://llv.andypj.xyz

JS:   while (i < 10) { i++; }
来源：http://rxp.redwolf501.top

TS:   while (i < 10) { i++; }
来源：http://yqy.yvedp.cn

Java: while (i < 10) { i++; }
来源：http://gkt.quarkkingdee.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gck.xinyue.icu

Ruby: while i < 10; i += 1; end
来源：http://soo.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://uxe.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://vvc.hywenlv.cn

Py:   # 无 do-while：用 while True + break
来源：http://mvq.meibo888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://srp.pycfn.com

JS:   do { i++; } while (i < 10);
来源：http://okp.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://aji.hammf.cn

Java: do { i++; } while (i < 10);
来源：http://geu.xylfe.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://idq.xingfuxueyuan.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://fky.gaohongyu789.top

C#:   do { i++; } while (i < 10);
来源：http://uig.jianghu66.top

[B09] break 与 continue
来源：http://uyp.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fis.haohaochexian.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kjv.yongpay.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vkz.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xks.ehwqpu.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qdk.bbcook.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pyf.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bxa.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jyj.jinghuilouyu.cn

[B10] 遍历同时拿索引
来源：http://nqr.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ukv.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kme.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://orn.kuanghao11.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hkq.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://krx.cucudq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dza.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gxb.haohaochexian.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ztm.kuanghao11.cn

[B11] 生成数字序列 / 区间
来源：http://vhn.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://uyk.yj20258888.top

PHP:  range(0, 10, 2);
来源：http://kyw.hfpthk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cyr.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://twk.sysykeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://afh.ybcxt.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zni.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://hbh.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vmy.jinqigufen.top

[B12] 跳出多层循环
来源：http://hdc.zhongyouzk.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rfy.tianlin.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://qpy.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sta.zhixingplan.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hqx.vehdjk.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gxd.shanyushiyangtech.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://clo.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ilm.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zol.jinqigufen.top

[B13] 判断是否为数字
来源：http://oyq.daria6918.cn

Py:   isinstance(x, (int, float))
来源：http://soo.ppjwa.cn

PHP:  is_numeric($x)
来源：http://rmf.hnqzz.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cvi.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ecu.tanke756.top

Java: x instanceof Number
来源：http://wtr.vehdjk.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ssj.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://tpt.ydzc1.top

C#:   x is int or double or decimal
来源：http://hqh.jqgfzy.top

[B14] 判断值是否在集合内
来源：http://wfc.vqdsnc.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://het.9152youxi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uft.shzxlz.cn

JS:   [1, 2, 3].includes(x)
来源：http://sjw.ehwqpu.com

TS:   [1, 2, 3].includes(x)
来源：http://myv.sufxvd.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wjx.kuanghao11.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blo.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://frc.zycfv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bqk.nanxuanxn.top

[B15] 布尔运算与取反
来源：http://zfc.gogol.net.cn

Py:   a and b or not c
来源：http://pes.mhx1999.top

PHP:  $a && $b || !$c
来源：http://arb.iojbl.cn

JS:   a && b || !c
来源：http://eos.sweek.top

TS:   a && b || !c
来源：http://gsh.bjfxy.top

Java: a && b || !c
来源：http://uha.zhengqikj.top

Go:   a && b || !c
来源：http://kbo.zhongyouzk.top

Ruby: a && b || !c
来源：http://kxh.yfazqb.com

C#:   a && b || !c
来源：http://ksj.zhijiandao.cn

[B16] 卫语句：不满足条件提前返回
来源：http://adq.smart0.xyz

Py:   if not data: return
来源：http://fmo.cdnleiting.top

PHP:  if (!$data) { return; }
来源：http://eve.zhengqikj.top

JS:   if (!data) return;
来源：http://ann.sweek.top

TS:   if (!data) return;
来源：http://lcn.pycfn.com

Java: if (data == null) return;
来源：http://wka.hesvh.cn

Go:   if data == nil { return }
来源：http://ezd.yuxming.cn

Ruby: return if data.nil?
来源：http://yqz.fehbvm.com

C#:   if (data == null) return;
来源：http://jpv.ctjpmb.com

================================================================================
来源：http://tin.zhixingplan.top

C. 函数与作用域
来源：http://vkg.yfazqb.com

================================================================================
来源：http://pgq.zhaomingkeji.xyz

[C01] 定义函数
来源：http://vuu.wangdashe.top

Py:   def add(a, b): return a + b
来源：http://naz.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iou.hfpthk.cn

JS:   function add(a, b) { return a + b; }
来源：http://ttn.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pit.aizwys.cn


<!-- 参考信息 -->