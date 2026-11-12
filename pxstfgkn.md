代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://uip.havefunace.top

[A11] 条件表达式（三元）
来源：http://sqo.vqdsnc.cn

Py:   "yes" if x > 0 else "no"
来源：http://riz.ybcxt.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://hem.yongpay.top

JS:   x > 0 ? "yes" : "no"
来源：http://nkk.havefunace.top

TS:   x > 0 ? "yes" : "no"
来源：http://xur.meibo888.top

Java: x > 0 ? "yes" : "no"
来源：http://utk.52xcode.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://snv.xuanzx.com

Ruby: x > 0 ? "yes" : "no"
来源：http://qhl.chenlongwang.top

C#:   x > 0 ? "yes" : "no"
来源：http://lhi.uphjek.com

[A12] 字符串插值 / 格式化
来源：http://ofg.sxryk.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mpv.birdmap.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lab.fehbvm.com

JS:   `Hello, ${name}!`
来源：http://vcz.epnwcf.com

TS:   `Hello, ${name}!`
来源：http://kbg.yongpay.top

Java: "Hello, %s!".formatted(name)
来源：http://sxb.havefunace.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qik.sweek.top

Ruby: "Hello, #{name}!"
来源：http://xrz.jinghuilouyu.cn

C#:   $"Hello, {name}!"
来源：http://ndx.ydjk.org.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zse.fanxiaobao.xyz

Py:   "第一行\n第二行"
来源：http://epv.zhijiandao.cn

PHP:  "第一行\n第二行"
来源：http://otf.9152youxi.cn

JS:   "第一行\n第二行"
来源：http://vxh.pycfn.com

TS:   "第一行\n第二行"
来源：http://ahc.aizwys.cn

Java: "第一行\n第二行"
来源：http://wbq.fehbvm.com

Go:   "第一行\n第二行"
来源：http://tlu.dashuyun.cn

Ruby: "第一行\n第二行"
来源：http://pah.wangshuangyany.cn

C#:   "第一行\n第二行"
来源：http://yed.zhixingplan.top

[A14] 注释写法
来源：http://pzm.yj20258888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zer.zdqjudy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://sqz.ctjpmb.com

JS:   // 单行；/* 多行 */
来源：http://yhk.xziqi.cn

TS:   // 单行；/* 多行 */
来源：http://pid.sysykeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lqd.ppjwa.cn

Go:   // 单行；/* 多行 */
来源：http://wrw.yanxiufei.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dlh.cqqwz.cn

C#:   // 单行；/* 多行 */
来源：http://iju.shanyushiyangtech.top

[A15] 空值判断与默认值
来源：http://fzk.daxiang520.top

Py:   value = data or "默认值"
来源：http://dcf.yangfankeji.com

PHP:  $value = $data ?? "默认值";
来源：http://xgq.cdnleiting.top

JS:   const value = data ?? "默认值";
来源：http://kem.haohaochexian.top

TS:   const value = data ?? "默认值";
来源：http://uvu.zhengqikj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tlh.yangfankeji.com

Go:   if data == "" { data = "默认值" }
来源：http://smj.vqdsnc.cn

Ruby: value = data || "默认值"
来源：http://jmy.zhaomingkeji.xyz

C#:   var value = data ?? "默认值";
来源：http://qbf.shanyushiyangtech.top

[A16] 真假值判断规则
来源：http://pjh.0kj1m.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vsj.ywan-chungtsiang.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lnw.hongshengwenyu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nuu.dianchejie.cn

TS:   if (!x) {}
来源：http://hpm.jqgufenzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rle.haohaochexian.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ltd.yj20258.top

Ruby: unless x            # nil 与 false 为假
来源：http://izn.zdqjudy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rss.316326.xyz

[A17] 位运算
来源：http://qly.tianlin.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mug.yonumen.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xgf.jiagoushi.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hzy.sxryk.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pqy.yongpay.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oqw.fengsongda.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bpf.meibo888.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tqy.uphjek.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fyy.hysaishi.cn

[A18] 字符与 ASCII 码互转
来源：http://bxk.zhixingplan.top

Py:   ord("A"); chr(65)
来源：http://qbt.xylfe.cn

PHP:  ord("A"); chr(65)
来源：http://sgl.yj202588.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zqs.tanke756.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dhe.dianchejie.cn

Java: (int) 'A'; (char) 65
来源：http://ogl.yj20258888.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://akx.shangyingyoupin.top

Ruby: "A".ord; 65.chr
来源：http://vbv.xinyue.icu

C#:   (int)'A'; (char)65
来源：http://bfm.yvedp.cn

[A19] 交换两个变量
来源：http://scg.chenlongwang.top

Py:   a, b = b, a
来源：http://auh.gogol.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vfx.birdmap.top

JS:   [a, b] = [b, a];
来源：http://kwq.gogol.net.cn

TS:   [a, b] = [b, a];
来源：http://iwz.sjlbkw.cn

Java: int t = a; a = b; b = t;
来源：http://usn.redwolf501.top

Go:   a, b = b, a
来源：http://yyu.jinyuanbaomall.cn

Ruby: a, b = b, a
来源：http://fua.pycfn.com

C#:   (a, b) = (b, a);
来源：http://tab.wangshuangyany.cn

[A20] 读取标准输入
来源：http://dls.jinqigufen.top

Py:   name = input("请输入：")
来源：http://ncj.zhengqikj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://dgo.cashguo.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://grs.ivvv.top

TS:   // Node.js：readline 模块
来源：http://arz.iojbl.cn

Java: new Scanner(System.in).nextLine()
来源：http://ytd.c1oappe.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hkj.yonumen.top

Ruby: gets.chomp
来源：http://yny.nwbrower.top

C#:   Console.ReadLine();
来源：http://qpl.ydjk.org.cn

[A21] 保留指定小数位输出
来源：http://uuw.pycfn.com

Py:   f"{3.14159:.2f}"
来源：http://aqs.gzhubu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wrv.hongshengwenyu.top

JS:   (3.14159).toFixed(2)
来源：http://xna.wangshuangyany.cn

TS:   (3.14159).toFixed(2)
来源：http://ftm.shuidangran.top

Java: String.format("%.2f", 3.14159)
来源：http://tcy.pycfn.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xmi.zhengqikj.top

Ruby: format("%.2f", 3.14159)
来源：http://yik.hnxiangtu.top

C#:   3.14159.ToString("F2")
来源：http://kbm.fehbvm.com

[A22] 获取字符串长度
来源：http://wae.fktsv.cn

Py:   len(s)
来源：http://uml.cdnleiting.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qrq.shanyushiyangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cnr.bjfxy.top

TS:   s.length
来源：http://cgg.yongpay.top

Java: s.length()
来源：http://dou.mhx1999.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zlz.sxryk.cn

Ruby: s.length
来源：http://drb.ydzc1.top

C#:   s.Length
来源：http://crv.guannengcc.top

[A23] 大小写转换
来源：http://dyz.cqqwz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mxw.gotoacloud.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sfa.9152youxi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wfx.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cqv.nwbrower.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vxs.tarul.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xjn.fzhhl.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://egd.jinghuilouyu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ojj.bbcook.cn

[A24] 去除首尾空白
来源：http://kyr.cdnleiting.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://end.hfpthk.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nht.uphjek.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mto.quarkkingdee.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fyq.zycfv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://div.sysykeji.top

Go:   strings.TrimSpace(s)
来源：http://xwr.quarkkingdee.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bnt.sjlbkw.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ubc.fktsv.cn

[A25] 字符串比较
来源：http://idx.fengsongda.top

Py:   s1 == s2; s1 != s2
来源：http://arc.xuanzx.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eml.yfazqb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tho.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://psa.yonumen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vag.sjlbkw.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xwm.smart0.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://dgs.xuanzx.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://agn.xuetiantiany.cn

[A26] 类型转换总览
来源：http://vot.chenlongwang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ioz.fanxiaobao.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mix.yanxiufei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dhm.jqgufenzy.top

TS:   Number() String() Boolean() x as number
来源：http://ndf.jinyuanbaomall.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://abt.yuanzhike.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ijh.shanyushiyangtech.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://iev.wangdashe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ias.ivvv.top

================================================================================
来源：http://vyk.zhijiandao.cn

B. 流程控制
来源：http://frq.uphjek.com

================================================================================
来源：http://wde.jyoumei.cn

[B01] 条件判断 if / else
来源：http://jtn.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tvk.hammf.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zas.jinqigufen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ufb.nanxinkj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oft.hysaishi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ays.jinyuanbaomall.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qnd.cashguo.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rqn.guowangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://urw.xuanzx.com

[B02] 多分支 else if / elif
来源：http://apr.nwbrower.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://div.sufxvd.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://afg.andypj.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vxm.ctjpmb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://udf.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://len.yangfankeji.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jew.yongpay.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kuz.guowangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fcv.316326.xyz

[B03] switch / match / case
来源：http://rxj.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zwe.nanxinkj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iiu.tianlin.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ufj.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pnx.yuanzhike.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jdn.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wnk.ivvv.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://udu.tian-w.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ziq.hammf.cn

[B04] for 计数循环
来源：http://ddf.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://ukf.zdqjudy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kmf.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uax.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ucg.jinghuilouyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mpc.cdnleiting.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://plk.tianlin.xyz

Ruby: 10.times { |i| puts i }
来源：http://hix.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dlt.meibo888.top

[B05] 遍历数组 / 列表
来源：http://fhh.sweek.top

Py:   for item in arr: print(item)
来源：http://xsl.xylfe.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ydn.shanyushiyangtech.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xmx.jinyuanbaomall.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://exy.fanxiaobao.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://fqy.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ysd.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://wlt.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fex.nanxinkj.top

[B06] 遍历字典 / 对象
来源：http://wym.pengpengdd.cyou

Py:   for k, v in d.items(): print(k, v)
来源：http://yqp.xingfuxueyuan.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kzu.yj20258.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nsv.fzhhl.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://njh.jianghu66.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ngo.birdmap.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hcf.xylfe.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zgw.jianghu66.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nhs.hnqzz.top

[B07] while 循环
来源：http://tny.zhijiandao.cn

Py:   while i < 10: i += 1
来源：http://iif.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://tjf.hnqzz.top

JS:   while (i < 10) { i++; }
来源：http://zxc.dashuyun.cn

TS:   while (i < 10) { i++; }
来源：http://xgx.daria6918.cn

Java: while (i < 10) { i++; }
来源：http://suh.yongpay.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fnt.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://eti.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://tff.ppjwa.cn

[B08] do-while（至少执行一次）
来源：http://bwi.jlsjyb.cn

Py:   # 无 do-while：用 while True + break
来源：http://uqd.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ajt.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://uhi.ybcxt.top

TS:   do { i++; } while (i < 10);
来源：http://nrx.nanxinkj.top

Java: do { i++; } while (i < 10);
来源：http://tmn.xziqi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xzi.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://dpu.gotoacloud.top

C#:   do { i++; } while (i < 10);
来源：http://oox.zdqjudy.top

[B09] break 与 continue
来源：http://vjt.snrcjt.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eck.gaohongyu789.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baw.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vnk.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dwy.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://opi.shanyushiyangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jiz.hongshengwenyu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dnj.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vub.hywenlv.cn

[B10] 遍历同时拿索引
来源：http://txo.jiagoushi.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eej.yuanzhike.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xef.c1oappe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nmt.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gei.ybcxt.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mrx.ppjwa.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mtx.vqdsnc.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nnt.hfpthk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tlw.xylfe.cn

[B11] 生成数字序列 / 区间
来源：http://jnu.gogol.net.cn

Py:   list(range(0, 10, 2))
来源：http://bjt.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://rju.tarul.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wzn.hcnkem.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pob.yanxiufei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ong.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hbg.shuidangran.top

Ruby: (0...10).step(2).to_a
来源：http://vhy.yj20258888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aaf.ivvv.top

[B12] 跳出多层循环
来源：http://ufw.haohaochexian.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mlg.yfazqb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://kes.316326.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://voj.hnxiangtu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fvf.hysaishi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://noi.nanxuanxn.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iyp.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jet.zhaomingkeji.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ovz.yuxming.cn

[B13] 判断是否为数字
来源：http://pxv.zhongyouzk.top

Py:   isinstance(x, (int, float))
来源：http://ghg.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://ntt.shuidangran.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vby.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xui.aizwys.cn

Java: x instanceof Number
来源：http://isl.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pnf.cqqwz.cn

Ruby: x.is_a?(Numeric)
来源：http://aez.jianghu66.top

C#:   x is int or double or decimal
来源：http://vus.0kj1m.cn

[B14] 判断值是否在集合内
来源：http://dcg.birdmap.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uni.ehwqpu.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qdh.yuxming.cn

JS:   [1, 2, 3].includes(x)
来源：http://rbi.smart0.xyz

TS:   [1, 2, 3].includes(x)
来源：http://evx.tianlin.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://zrl.shzxlz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oij.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://whx.fanxiaobao.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tzo.yj20258888.top

[B15] 布尔运算与取反
来源：http://pkw.52xcode.cn

Py:   a and b or not c
来源：http://uoh.tarul.cn

PHP:  $a && $b || !$c
来源：http://yjj.tianlin.xyz

JS:   a && b || !c
来源：http://ywb.0kj1m.cn

TS:   a && b || !c
来源：http://okl.jinqigufen.top

Java: a && b || !c
来源：http://yge.nwbrower.top

Go:   a && b || !c
来源：http://jzb.quarkkingdee.top

Ruby: a && b || !c
来源：http://zeq.zhaomingkeji.xyz

C#:   a && b || !c
来源：http://kon.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://dka.shzxlz.cn

Py:   if not data: return
来源：http://aqb.9152youxi.cn

PHP:  if (!$data) { return; }
来源：http://ovg.cdnleiting.top

JS:   if (!data) return;
来源：http://fpq.hnqzz.top

TS:   if (!data) return;
来源：http://jsf.yueranfly.top

Java: if (data == null) return;
来源：http://jlm.shanyushiyangkeji.top

Go:   if data == nil { return }
来源：http://ezk.snrcjt.cn

Ruby: return if data.nil?
来源：http://hyq.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://gtd.xylfe.cn

================================================================================
来源：http://big.jinqigufen.top

C. 函数与作用域
来源：http://wvg.dianchejie.cn

================================================================================
来源：http://vrv.pycfn.com

[C01] 定义函数
来源：http://wcd.jyoumei.cn

Py:   def add(a, b): return a + b
来源：http://mum.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hxl.fehbvm.com

JS:   function add(a, b) { return a + b; }
来源：http://dlq.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pgt.cashguo.top


<!-- 参考信息 -->