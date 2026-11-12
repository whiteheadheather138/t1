代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://str.shanyushiyangkeji.top

[A11] 条件表达式（三元）
来源：http://anq.jqgufenzy.top

Py:   "yes" if x > 0 else "no"
来源：http://syr.hongshengwenyu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yay.dashuyun.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lip.jinyuanbaomall.cn

TS:   x > 0 ? "yes" : "no"
来源：http://csj.gogol.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://ire.hammf.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ifm.jinyuanbaomall.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cdm.andypj.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://gvw.ywan-chungtsiang.top

[A12] 字符串插值 / 格式化
来源：http://bme.chenlongwang.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hdc.jqgfzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iqt.ybcxt.top

JS:   `Hello, ${name}!`
来源：http://jhx.kuanghao11.cn

TS:   `Hello, ${name}!`
来源：http://dvu.ydjk.org.cn

Java: "Hello, %s!".formatted(name)
来源：http://wph.hfpthk.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yqg.zhijiandao.cn

Ruby: "Hello, #{name}!"
来源：http://xsr.mhx1999.top

C#:   $"Hello, {name}!"
来源：http://vgm.pengpengdd.cyou

[A13] 多行字符串（练习 \n 转义）
来源：http://vel.iojbl.cn

Py:   "第一行\n第二行"
来源：http://ymq.yueranfly.top

PHP:  "第一行\n第二行"
来源：http://ogu.0kj1m.cn

JS:   "第一行\n第二行"
来源：http://fnv.guannengcc.top

TS:   "第一行\n第二行"
来源：http://ylu.jiagoushi.top

Java: "第一行\n第二行"
来源：http://jnt.316326.xyz

Go:   "第一行\n第二行"
来源：http://fhw.sweek.top

Ruby: "第一行\n第二行"
来源：http://sqg.hammf.cn

C#:   "第一行\n第二行"
来源：http://awp.cucudq.cn

[A14] 注释写法
来源：http://tmy.gotoacloud.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://knc.sjlbkw.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ppc.hnxiangtu.top

JS:   // 单行；/* 多行 */
来源：http://fdt.yonumen.top

TS:   // 单行；/* 多行 */
来源：http://env.jqgufenzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://iuv.pycfn.com

Go:   // 单行；/* 多行 */
来源：http://pxg.fanxiaobao.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://nha.quarkkingdee.top

C#:   // 单行；/* 多行 */
来源：http://yed.zdqjudy.top

[A15] 空值判断与默认值
来源：http://mod.cqqwz.cn

Py:   value = data or "默认值"
来源：http://lab.ywan-chungtsiang.top

PHP:  $value = $data ?? "默认值";
来源：http://zxr.shanyushiyangtech.top

JS:   const value = data ?? "默认值";
来源：http://dfi.gotoacloud.top

TS:   const value = data ?? "默认值";
来源：http://fcr.aizwys.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ipe.yj202588.top

Go:   if data == "" { data = "默认值" }
来源：http://lip.sxryk.cn

Ruby: value = data || "默认值"
来源：http://oum.pengpengdd.cyou

C#:   var value = data ?? "默认值";
来源：http://lyi.fengsongda.top

[A16] 真假值判断规则
来源：http://nzj.yj20258.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vcl.shuidangran.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tpg.cucudq.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://spd.jinqigfzy.top

TS:   if (!x) {}
来源：http://shd.fengsongda.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kaz.ctjpmb.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gkq.haohaochexian.top

Ruby: unless x            # nil 与 false 为假
来源：http://ptq.haohaochexian.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lvr.jianghu66.top

[A17] 位运算
来源：http://tub.hesvh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pnp.bbcook.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jec.snrcjt.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iaa.zhongyouzk.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iev.sufxvd.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jze.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://enw.iojbl.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fbp.fzhhl.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lwg.hcnkem.com

[A18] 字符与 ASCII 码互转
来源：http://zjv.ivvv.top

Py:   ord("A"); chr(65)
来源：http://jst.zhongyouzk.top

PHP:  ord("A"); chr(65)
来源：http://kuo.kuanghao11.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hep.dianchejie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://msh.birdmap.top

Java: (int) 'A'; (char) 65
来源：http://hsf.c1oappe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gef.bjfxy.top

Ruby: "A".ord; 65.chr
来源：http://dta.gzhubu.top

C#:   (int)'A'; (char)65
来源：http://lnp.sjlbkw.cn

[A19] 交换两个变量
来源：http://xwa.chenlongwang.top

Py:   a, b = b, a
来源：http://fnm.ctjpmb.com

PHP:  [$a, $b] = [$b, $a];
来源：http://pzu.9152youxi.cn

JS:   [a, b] = [b, a];
来源：http://ltk.ywan-chungtsiang.top

TS:   [a, b] = [b, a];
来源：http://ekg.zycfv.cn

Java: int t = a; a = b; b = t;
来源：http://lqm.cqqwz.cn

Go:   a, b = b, a
来源：http://bdb.aizwys.cn

Ruby: a, b = b, a
来源：http://wyh.zhijiandao.cn

C#:   (a, b) = (b, a);
来源：http://fpb.vehdjk.com

[A20] 读取标准输入
来源：http://mwn.cucudq.cn

Py:   name = input("请输入：")
来源：http://wvd.yuxming.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kkc.zycfv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ztx.shangyingyoupin.top

TS:   // Node.js：readline 模块
来源：http://lco.cashguo.top

Java: new Scanner(System.in).nextLine()
来源：http://rnv.jqgfzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://odn.yvedp.cn

Ruby: gets.chomp
来源：http://ruo.xuanzx.com

C#:   Console.ReadLine();
来源：http://mog.chenlongwang.top

[A21] 保留指定小数位输出
来源：http://gly.hongshengwenyu.top

Py:   f"{3.14159:.2f}"
来源：http://tjd.wangdashe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dqx.xingfuxueyuan.xyz

JS:   (3.14159).toFixed(2)
来源：http://jit.zdbjq.cn

TS:   (3.14159).toFixed(2)
来源：http://oce.shanyushiyangkeji.top

Java: String.format("%.2f", 3.14159)
来源：http://kjw.shanyushiyangtech.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ytd.gaohongyu789.top

Ruby: format("%.2f", 3.14159)
来源：http://xqh.redwolf501.top

C#:   3.14159.ToString("F2")
来源：http://tts.shzxlz.cn

[A22] 获取字符串长度
来源：http://adz.hnxiangtu.top

Py:   len(s)
来源：http://qjf.jinqigfzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xue.c1oappe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zdj.xingfuxueyuan.xyz

TS:   s.length
来源：http://yxw.c1oappe.top

Java: s.length()
来源：http://zrk.shzxlz.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zcs.snrcjt.cn

Ruby: s.length
来源：http://puw.yfazqb.com

C#:   s.Length
来源：http://sgs.andypj.xyz

[A23] 大小写转换
来源：http://lmk.fehbvm.com

Py:   s.upper(); s.lower(); s.title()
来源：http://ibv.daxiang520.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gwd.daxiang520.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qlh.vqdsnc.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gyb.fanxiaobao.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hwu.sysykeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sbg.ywan-chungtsiang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nlj.ehwqpu.com

C#:   s.ToUpper(); s.ToLower()
来源：http://ogt.cqqwz.cn

[A24] 去除首尾空白
来源：http://mla.jiagoushi.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://czy.wangshuangyany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gyn.mhx1999.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cji.yueranfly.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zwf.ydjk.org.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tne.cheryme.top

Go:   strings.TrimSpace(s)
来源：http://bza.9152youxi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ypf.jqgfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://svi.aizwys.cn

[A25] 字符串比较
来源：http://ipb.yonumen.top

Py:   s1 == s2; s1 != s2
来源：http://oym.52xcode.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iib.fktsv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cor.hysaishi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tyb.tanke756.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ujp.shangyingyoupin.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://adg.pengpengdd.cyou

Ruby: s1 == s2; s1 <=> s2
来源：http://zhp.yj202588.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qle.epnwcf.com

[A26] 类型转换总览
来源：http://owy.ppjwa.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rgg.yongpay.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://shh.yongpay.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sop.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://ufd.birdmap.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tau.tianlin.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sgt.gogol.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://emo.yj20258888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wue.pengpengdd.cyou

================================================================================
来源：http://lrk.haohaochexian.top

B. 流程控制
来源：http://bdw.vehdjk.com

================================================================================
来源：http://rih.zhengqikj.top

[B01] 条件判断 if / else
来源：http://eoe.daxiang520.top

Py:   result = "正" if x > 0 else "非正"
来源：http://lhp.ivvv.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wtz.316326.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fjv.ydzc1.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://eha.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vde.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uxw.0kj1m.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ogo.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lyp.pengpengdd.cyou

[B02] 多分支 else if / elif
来源：http://tol.xuanzx.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rrn.cqqwz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sio.zhijiandao.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ega.ehwqpu.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ghe.meibo888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://msi.0kj1m.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://buq.zhoulong.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uas.zhongyouzk.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dwd.aibaodan.cn

[B03] switch / match / case
来源：http://goc.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lmn.yj20258.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nse.daxiang520.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ehx.fktsv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mgw.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ggz.chenzaomai.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lha.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vhy.zycfv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lbf.hesvh.cn

[B04] for 计数循环
来源：http://jya.gzhubu.top

Py:   for i in range(10): print(i)
来源：http://wag.sysykeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uzj.hysaishi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qtc.kuanghao11.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ekh.fehbvm.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kba.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nsw.yvedp.cn

Ruby: 10.times { |i| puts i }
来源：http://suu.nanxinkj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lym.zycfv.cn

[B05] 遍历数组 / 列表
来源：http://uvz.zycfv.cn

Py:   for item in arr: print(item)
来源：http://fno.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ffq.yonumen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vin.smart0.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://vrq.snrcjt.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zcu.snrcjt.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kya.hywenlv.cn

Ruby: arr.each { |item| puts item }
来源：http://ryl.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://shj.nanxuanxn.top

[B06] 遍历字典 / 对象
来源：http://ksf.zhiwuduotai.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bwt.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bav.zhixingplan.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tmm.jyoumei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qyi.birdmap.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oal.ehwqpu.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bmt.dianchejie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://grp.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gtg.zycfv.cn

[B07] while 循环
来源：http://dyd.yj20258888.top

Py:   while i < 10: i += 1
来源：http://xas.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://knf.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://win.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://occ.yongpay.top

Java: while (i < 10) { i++; }
来源：http://kho.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uqi.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://yhg.havefunace.top

C#:   while (i < 10) { i++; }
来源：http://iyx.hnqzz.top

[B08] do-while（至少执行一次）
来源：http://dzn.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://gbc.gogol.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kwh.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://xrl.dianchejie.cn

TS:   do { i++; } while (i < 10);
来源：http://qjb.fengsongda.top

Java: do { i++; } while (i < 10);
来源：http://bzj.jyoumei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://izw.hnxiangtu.top

Ruby: begin; i += 1; end while i < 10
来源：http://olo.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://hes.zycfv.cn

[B09] break 与 continue
来源：http://hzi.ydjk.org.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gnj.epnwcf.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://szs.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zji.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://siw.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ces.ppjwa.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iux.xuetiantiany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zmd.yj20258888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zxp.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://kcb.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://auz.cheryme.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lxa.tarul.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rqy.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qqc.zhongyouzk.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://buo.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dit.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wyz.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ddv.yuanzhike.top

[B11] 生成数字序列 / 区间
来源：http://ket.ydzc1.top

Py:   list(range(0, 10, 2))
来源：http://pvo.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://lfx.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zhl.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xup.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://otr.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://swc.jyoumei.cn

Ruby: (0...10).step(2).to_a
来源：http://wvr.yonumen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://viq.tarul.cn

[B12] 跳出多层循环
来源：http://paa.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nyo.meibo888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://owl.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fwm.yj20258888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zdg.316326.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://afl.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gvs.nanxinkj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://smd.9152youxi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hjr.mhx1999.top

[B13] 判断是否为数字
来源：http://kji.zhijiandao.cn

Py:   isinstance(x, (int, float))
来源：http://awc.pengpengdd.cyou

PHP:  is_numeric($x)
来源：http://qjx.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://isp.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tpj.yanxiufei.cn

Java: x instanceof Number
来源：http://hhh.jyoumei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pst.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://lxa.zhengqikj.top

C#:   x is int or double or decimal
来源：http://dwc.jianghu66.top

[B14] 判断值是否在集合内
来源：http://nda.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ozf.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://shx.ywan-chungtsiang.top

JS:   [1, 2, 3].includes(x)
来源：http://qmp.gaohongyu789.top

TS:   [1, 2, 3].includes(x)
来源：http://xxc.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kie.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fnl.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://rmf.fengsongda.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uhg.yj20258.top

[B15] 布尔运算与取反
来源：http://uge.feifeiyinyue.top

Py:   a and b or not c
来源：http://smx.zdqjudy.top

PHP:  $a && $b || !$c
来源：http://eyb.yanxiufei.cn

JS:   a && b || !c
来源：http://otk.xingfuxueyuan.xyz

TS:   a && b || !c
来源：http://udq.yonumen.top

Java: a && b || !c
来源：http://rqc.daxiang520.top

Go:   a && b || !c
来源：http://iqt.hcnkem.com

Ruby: a && b || !c
来源：http://mdh.sjlbkw.cn

C#:   a && b || !c
来源：http://qfe.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://pti.shangyingyoupin.top

Py:   if not data: return
来源：http://blg.kuanghao11.cn

PHP:  if (!$data) { return; }
来源：http://mik.yonumen.top

JS:   if (!data) return;
来源：http://mct.tian-w.cn

TS:   if (!data) return;
来源：http://lnv.gaohongyu789.top

Java: if (data == null) return;
来源：http://qkg.cheryme.top

Go:   if data == nil { return }
来源：http://jfd.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://cuc.pycfn.com

C#:   if (data == null) return;
来源：http://ynl.fktsv.cn

================================================================================
来源：http://lpt.wangshuangyany.cn

C. 函数与作用域
来源：http://jdf.aibaodan.cn

================================================================================
来源：http://fsm.hywenlv.cn

[C01] 定义函数
来源：http://kyc.epnwcf.com

Py:   def add(a, b): return a + b
来源：http://tja.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://skt.yj20258.top

JS:   function add(a, b) { return a + b; }
来源：http://oas.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jfk.nwbrower.top


<!-- 参考信息 -->