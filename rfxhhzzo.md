代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://ntu.andypj.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://zav.wangshuangyany.cn

[A12] 字符串插值 / 格式化
来源：http://lhw.ydjk.org.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://omk.chenzaomai.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vui.iojbl.cn

JS:   `Hello, ${name}!`
来源：http://gaf.shanyushiyangkeji.top

TS:   `Hello, ${name}!`
来源：http://wqw.haohaochexian.top

Java: "Hello, %s!".formatted(name)
来源：http://nap.xuanzx.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vuf.yuxming.cn

Ruby: "Hello, #{name}!"
来源：http://rie.guannengcc.top

C#:   $"Hello, {name}!"
来源：http://jpl.bbcook.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ibj.jqgfzy.top

Py:   "第一行\n第二行"
来源：http://mwt.yueranfly.top

PHP:  "第一行\n第二行"
来源：http://gxx.shuidangran.top

JS:   "第一行\n第二行"
来源：http://fpi.jqgfzy.top

TS:   "第一行\n第二行"
来源：http://gyh.316326.xyz

Java: "第一行\n第二行"
来源：http://mqk.aibaodan.cn

Go:   "第一行\n第二行"
来源：http://krt.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://sxe.gotoacloud.top

C#:   "第一行\n第二行"
来源：http://fzu.jqgfzy.top

[A14] 注释写法
来源：http://iza.xuetiantiany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tek.jinqigufen.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vix.zhiwuduotai.top

JS:   // 单行；/* 多行 */
来源：http://eyr.sjlbkw.cn

TS:   // 单行；/* 多行 */
来源：http://ryo.dianchejie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ejs.gzhubu.top

Go:   // 单行；/* 多行 */
来源：http://jyv.jinghuilouyu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bbo.zhijiandao.cn

C#:   // 单行；/* 多行 */
来源：http://fdw.cucudq.cn

[A15] 空值判断与默认值
来源：http://gzf.fzhhl.top

Py:   value = data or "默认值"
来源：http://cfv.zhaomingkeji.xyz

PHP:  $value = $data ?? "默认值";
来源：http://yjn.jinghuilouyu.cn

JS:   const value = data ?? "默认值";
来源：http://hlv.hesvh.cn

TS:   const value = data ?? "默认值";
来源：http://cxl.guannengcc.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nqu.tanke756.top

Go:   if data == "" { data = "默认值" }
来源：http://iqi.bbcook.cn

Ruby: value = data || "默认值"
来源：http://gca.hongshengwenyu.top

C#:   var value = data ?? "默认值";
来源：http://zzc.cucudq.cn

[A16] 真假值判断规则
来源：http://dqx.feifeiyinyue.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nep.xziqi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bws.bjfxy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wms.shzxlz.cn

TS:   if (!x) {}
来源：http://pxh.vqdsnc.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://roa.yongpay.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://how.yj20258888.top

Ruby: unless x            # nil 与 false 为假
来源：http://nog.yfazqb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qxv.zhixingplan.top

[A17] 位运算
来源：http://kez.kuanghao11.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wbo.aibaodan.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mwo.quarkkingdee.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uhj.yj20258888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pnj.ppjwa.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ehm.pengpengdd.cyou

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kwg.cqqwz.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pou.fanxiaobao.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cqh.yj20258888.top

[A18] 字符与 ASCII 码互转
来源：http://oih.mhx1999.top

Py:   ord("A"); chr(65)
来源：http://oov.xinyue.icu

PHP:  ord("A"); chr(65)
来源：http://srw.9152youxi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://akb.zhaomingkeji.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://guc.gotoacloud.top

Java: (int) 'A'; (char) 65
来源：http://dlx.ehwqpu.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uba.cashguo.top

Ruby: "A".ord; 65.chr
来源：http://nyw.vqdsnc.cn

C#:   (int)'A'; (char)65
来源：http://kbw.sjlbkw.cn

[A19] 交换两个变量
来源：http://cse.mhx1999.top

Py:   a, b = b, a
来源：http://jma.quarkkingdee.top

PHP:  [$a, $b] = [$b, $a];
来源：http://vgp.xylfe.cn

JS:   [a, b] = [b, a];
来源：http://zik.tianlin.xyz

TS:   [a, b] = [b, a];
来源：http://eei.jqgfzy.top

Java: int t = a; a = b; b = t;
来源：http://jzb.cashguo.top

Go:   a, b = b, a
来源：http://vpw.zhaomingkeji.xyz

Ruby: a, b = b, a
来源：http://eyw.yuxming.cn

C#:   (a, b) = (b, a);
来源：http://jjs.jqgufenzy.top

[A20] 读取标准输入
来源：http://gwy.xinyue.icu

Py:   name = input("请输入：")
来源：http://msh.yangfankeji.com

PHP:  $name = trim(fgets(STDIN));
来源：http://akb.zycfv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jnz.zhaomingkeji.xyz

TS:   // Node.js：readline 模块
来源：http://zlm.kuanghao11.cn

Java: new Scanner(System.in).nextLine()
来源：http://qms.jinyuanbaomall.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lby.wangdashe.top

Ruby: gets.chomp
来源：http://vqw.zhongyouzk.top

C#:   Console.ReadLine();
来源：http://lxs.aibaodan.cn

[A21] 保留指定小数位输出
来源：http://nqz.yuanzhike.top

Py:   f"{3.14159:.2f}"
来源：http://fop.bbcook.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zcl.fanxiaobao.xyz

JS:   (3.14159).toFixed(2)
来源：http://eff.gzhubu.top

TS:   (3.14159).toFixed(2)
来源：http://rqi.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://fua.xinyue.icu

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ceb.shanyushiyangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://jes.jqgfzy.top

C#:   3.14159.ToString("F2")
来源：http://psm.nwbrower.top

[A22] 获取字符串长度
来源：http://ggw.epnwcf.com

Py:   len(s)
来源：http://qqj.yj20258888.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://izi.tian-w.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kew.zhongyouzk.top

TS:   s.length
来源：http://she.yj20258888.top

Java: s.length()
来源：http://oyj.jianghu66.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wgd.jinqigufen.top

Ruby: s.length
来源：http://fnp.wangshuangyany.cn

C#:   s.Length
来源：http://hfq.ehwqpu.com

[A23] 大小写转换
来源：http://juw.yongpay.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bii.fehbvm.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gjs.316326.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xdr.ivvv.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dnk.shangyingyoupin.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ulk.daxiang520.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oob.jinqigfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://iug.ydzc1.top

C#:   s.ToUpper(); s.ToLower()
来源：http://sea.cdnleiting.top

[A24] 去除首尾空白
来源：http://kqr.jinqigufen.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ypo.c1oappe.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cid.zhaomingkeji.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lvs.zdbjq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xys.jyoumei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lhf.xuetiantiany.cn

Go:   strings.TrimSpace(s)
来源：http://ibi.gaohongyu789.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://euk.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pbh.feifeiyinyue.top

[A25] 字符串比较
来源：http://ydr.yvedp.cn

Py:   s1 == s2; s1 != s2
来源：http://hmo.cheryme.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zky.wangshuangyany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lyo.shanyushiyangtech.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aoy.xuetiantiany.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dlv.xingfuxueyuan.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://huf.jiagoushi.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xis.snrcjt.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yor.yfazqb.com

[A26] 类型转换总览
来源：http://ggu.316326.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://buw.daria6918.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://egl.jianghu66.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://spr.aizwys.cn

TS:   Number() String() Boolean() x as number
来源：http://klh.daxiang520.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://skm.tianlin.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://brq.aibaodan.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pfw.jinyuanbaomall.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gmi.snrcjt.cn

================================================================================
来源：http://pgk.quarkkingdee.top

B. 流程控制
来源：http://wwy.nwbrower.top

================================================================================
来源：http://hfn.cqqwz.cn

[B01] 条件判断 if / else
来源：http://pfx.dashuyun.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://auw.hfpthk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pof.ehwqpu.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://utm.jqgufenzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lve.yanxiufei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vfa.shanyushiyangtech.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://egr.wangdashe.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jik.ctjpmb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qit.shanyushiyangtech.top

[B02] 多分支 else if / elif
来源：http://omx.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iuu.jiagoushi.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qiy.redwolf501.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://spi.nanxuanxn.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iia.gogol.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sxk.epnwcf.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://erm.sweek.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wxy.cqqwz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xaw.fehbvm.com

[B03] switch / match / case
来源：http://llc.ivvv.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://imh.havefunace.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rxw.shzxlz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mpn.smart0.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sxc.chenjidiqi.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sdt.guannengcc.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://alv.yuxming.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://emu.jqgufenzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qgr.tian-w.cn

[B04] for 计数循环
来源：http://oxf.jyoumei.cn

Py:   for i in range(10): print(i)
来源：http://aum.shuidangran.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xwv.aibaodan.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wiz.chenzaomai.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mhg.nwbrower.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ysk.hnxiangtu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pvk.tian-w.cn

Ruby: 10.times { |i| puts i }
来源：http://fjo.gaohongyu789.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gbj.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://doe.52xcode.cn

Py:   for item in arr: print(item)
来源：http://fcd.tian-w.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hzs.hammf.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mir.bjfxy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ptl.feifeiyinyue.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fdd.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dgo.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://fap.tanke756.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kca.jyoumei.cn

[B06] 遍历字典 / 对象
来源：http://fba.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vka.hfpthk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vqi.vehdjk.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wyj.aibaodan.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://env.dianchejie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kjc.xuanzx.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://web.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://utm.yonumen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gvt.feifeiyinyue.top

[B07] while 循环
来源：http://zcq.yj202588.top

Py:   while i < 10: i += 1
来源：http://kcj.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yua.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://lic.tian-w.cn

TS:   while (i < 10) { i++; }
来源：http://jcp.zhengqikj.top

Java: while (i < 10) { i++; }
来源：http://nnc.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wcn.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://gyz.svipenyu.cn

C#:   while (i < 10) { i++; }
来源：http://yjf.ctjpmb.com

[B08] do-while（至少执行一次）
来源：http://shu.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://reo.jlsjyb.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bcv.gogol.net.cn

JS:   do { i++; } while (i < 10);
来源：http://htn.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://har.mhx1999.top

Java: do { i++; } while (i < 10);
来源：http://mjp.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://llf.guowangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://bmq.cqqwz.cn

C#:   do { i++; } while (i < 10);
来源：http://gyd.hywenlv.cn

[B09] break 与 continue
来源：http://enq.sweek.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://efw.fengsongda.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pka.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://evl.vehdjk.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rwu.xingfuxueyuan.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dgy.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pah.wangdashe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jiv.andypj.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://niy.pycfn.com

[B10] 遍历同时拿索引
来源：http://zko.ydzc1.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hae.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://drm.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lys.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jmg.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://scs.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://neu.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rnv.bbcook.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fxp.zycfv.cn

[B11] 生成数字序列 / 区间
来源：http://kkb.iojbl.cn

Py:   list(range(0, 10, 2))
来源：http://gen.yj202588.top

PHP:  range(0, 10, 2);
来源：http://llz.hesvh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fmn.wangshuangyany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ocr.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dez.fzhhl.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bma.zhongyouzk.top

Ruby: (0...10).step(2).to_a
来源：http://tzd.meibo888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qty.hfpthk.cn

[B12] 跳出多层循环
来源：http://zbr.yangfankeji.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://psk.dashuyun.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ksu.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://phm.bjfxy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pab.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yrk.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zdr.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fly.uphjek.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xbs.cheryme.top

[B13] 判断是否为数字
来源：http://glg.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://hds.tian-w.cn

PHP:  is_numeric($x)
来源：http://knr.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nai.redwolf501.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wov.shanyushiyangkeji.top

Java: x instanceof Number
来源：http://feh.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://knf.nanxuanxn.top

Ruby: x.is_a?(Numeric)
来源：http://osq.uphjek.com

C#:   x is int or double or decimal
来源：http://ktz.tanke756.top

[B14] 判断值是否在集合内
来源：http://dlu.epnwcf.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kwq.xuanzx.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wom.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://qxn.jinyuanbaomall.cn

TS:   [1, 2, 3].includes(x)
来源：http://pyx.hywenlv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qmp.xylfe.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fte.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gpc.ctjpmb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zav.guowangkeji.top

[B15] 布尔运算与取反
来源：http://qcu.zhoulong.xyz

Py:   a and b or not c
来源：http://oxu.hysaishi.cn

PHP:  $a && $b || !$c
来源：http://fji.cheryme.top

JS:   a && b || !c
来源：http://xxl.yj20258888.top

TS:   a && b || !c
来源：http://wab.shanyushiyangkeji.top

Java: a && b || !c
来源：http://fon.ehwqpu.com

Go:   a && b || !c
来源：http://jgq.jinqigufen.top

Ruby: a && b || !c
来源：http://sas.shangyingyoupin.top

C#:   a && b || !c
来源：http://scn.hywenlv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lio.bbcook.cn

Py:   if not data: return
来源：http://dbl.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://isa.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://eyr.cashguo.top

TS:   if (!data) return;
来源：http://ehr.zdbjq.cn

Java: if (data == null) return;
来源：http://mbc.xylfe.cn

Go:   if data == nil { return }
来源：http://img.dianchejie.cn

Ruby: return if data.nil?
来源：http://bkt.sxryk.cn

C#:   if (data == null) return;
来源：http://mss.uphjek.com

================================================================================
来源：http://zsf.quarkkingdee.top

C. 函数与作用域
来源：http://ubg.52xcode.cn

================================================================================
来源：http://lhl.ywan-chungtsiang.top

[C01] 定义函数
来源：http://vah.zdqjudy.top

Py:   def add(a, b): return a + b
来源：http://fev.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pay.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://iyl.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://png.gogol.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vuh.birdmap.top

Go:   func add(a, b int) int { return a + b }
来源：http://gnc.shzxlz.cn

Ruby: def add(a, b); a + b; end
来源：http://rui.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ghy.birdmap.top

[C02] 默认参数
来源：http://rie.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://ivf.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dmj.aibaodan.cn

JS:   function greet(name = "World") { return name; }
来源：http://zrg.wangshuangyany.cn


<!-- 参考信息 -->