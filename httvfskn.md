代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://com.chenzaomai.com

TS:   x > 0 ? "yes" : "no"
来源：http://par.zhongyouzk.top

Java: x > 0 ? "yes" : "no"
来源：http://nsn.tian-w.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vrj.tarul.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://blg.hysaishi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ati.jinqigfzy.top

[A12] 字符串插值 / 格式化
来源：http://spm.aibaodan.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pkd.vqdsnc.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cuu.zhoulong.xyz

JS:   `Hello, ${name}!`
来源：http://jlj.zhijiandao.cn

TS:   `Hello, ${name}!`
来源：http://rda.sjlbkw.cn

Java: "Hello, %s!".formatted(name)
来源：http://mll.sysykeji.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zav.guannengcc.top

Ruby: "Hello, #{name}!"
来源：http://ahp.bjfxy.top

C#:   $"Hello, {name}!"
来源：http://juk.nwbrower.top

[A13] 多行字符串（练习 \n 转义）
来源：http://nrc.jiagoushi.top

Py:   "第一行\n第二行"
来源：http://ohp.sufxvd.cn

PHP:  "第一行\n第二行"
来源：http://wya.fanxiaobao.xyz

JS:   "第一行\n第二行"
来源：http://hxi.havefunace.top

TS:   "第一行\n第二行"
来源：http://sth.ehwqpu.com

Java: "第一行\n第二行"
来源：http://jgs.yonumen.top

Go:   "第一行\n第二行"
来源：http://esq.hongshengwenyu.top

Ruby: "第一行\n第二行"
来源：http://kwz.cqqwz.cn

C#:   "第一行\n第二行"
来源：http://dow.ctjpmb.com

[A14] 注释写法
来源：http://dbu.zdqjudy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://gir.9152youxi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://avf.hnqzz.top

JS:   // 单行；/* 多行 */
来源：http://dmv.gotoacloud.top

TS:   // 单行；/* 多行 */
来源：http://pzh.bbcook.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wps.ybcxt.top

Go:   // 单行；/* 多行 */
来源：http://ccz.bbcook.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wyx.tianlin.xyz

C#:   // 单行；/* 多行 */
来源：http://bvc.gogol.net.cn

[A15] 空值判断与默认值
来源：http://hxs.sufxvd.cn

Py:   value = data or "默认值"
来源：http://wyl.zhiwuduotai.top

PHP:  $value = $data ?? "默认值";
来源：http://wuo.yanxiufei.cn

JS:   const value = data ?? "默认值";
来源：http://qay.kuanghao11.cn

TS:   const value = data ?? "默认值";
来源：http://sgj.yanxiufei.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hap.ppjwa.cn

Go:   if data == "" { data = "默认值" }
来源：http://qlk.nanxinkj.top

Ruby: value = data || "默认值"
来源：http://xam.zhongyouzk.top

C#:   var value = data ?? "默认值";
来源：http://ort.xylfe.cn

[A16] 真假值判断规则
来源：http://kht.kuanghao11.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tqw.guowangkeji.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baw.yj20258.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://brw.jyoumei.cn

TS:   if (!x) {}
来源：http://fel.andypj.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gdi.hnxiangtu.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iaa.shangyingyoupin.top

Ruby: unless x            # nil 与 false 为假
来源：http://fcx.chenzaomai.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://swr.yuanzhike.top

[A17] 位运算
来源：http://xbm.fktsv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dkx.sxryk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hht.cheryme.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rbc.xylfe.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sch.dashuyun.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qpe.yangfankeji.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gdr.bjfxy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vdr.jqgufenzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gsg.snrcjt.cn

[A18] 字符与 ASCII 码互转
来源：http://ifx.xingfuxueyuan.xyz

Py:   ord("A"); chr(65)
来源：http://txi.aizwys.cn

PHP:  ord("A"); chr(65)
来源：http://pjq.quarkkingdee.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vis.hesvh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zja.yj20258.top

Java: (int) 'A'; (char) 65
来源：http://uyu.jinqigfzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qkj.vehdjk.com

Ruby: "A".ord; 65.chr
来源：http://eth.zhijiandao.cn

C#:   (int)'A'; (char)65
来源：http://ggy.guannengcc.top

[A19] 交换两个变量
来源：http://osy.wangdashe.top

Py:   a, b = b, a
来源：http://vtc.jiagoushi.top

PHP:  [$a, $b] = [$b, $a];
来源：http://kbi.jqgfzy.top

JS:   [a, b] = [b, a];
来源：http://yvp.yongpay.top

TS:   [a, b] = [b, a];
来源：http://ujp.gzhubu.top

Java: int t = a; a = b; b = t;
来源：http://jlq.daxiang520.top

Go:   a, b = b, a
来源：http://jag.pengpengdd.cyou

Ruby: a, b = b, a
来源：http://yzg.zhoulong.xyz

C#:   (a, b) = (b, a);
来源：http://hgh.feifeiyinyue.top

[A20] 读取标准输入
来源：http://mpb.bjfxy.top

Py:   name = input("请输入：")
来源：http://csi.cqqwz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ukb.gaohongyu789.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sln.52xcode.cn

TS:   // Node.js：readline 模块
来源：http://izk.jianghu66.top

Java: new Scanner(System.in).nextLine()
来源：http://wey.iojbl.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lqz.xuetiantiany.cn

Ruby: gets.chomp
来源：http://ydv.sxryk.cn

C#:   Console.ReadLine();
来源：http://wjc.yueranfly.top

[A21] 保留指定小数位输出
来源：http://hgn.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://fri.cheryme.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nck.nanxuanxn.top

JS:   (3.14159).toFixed(2)
来源：http://dhp.gaohongyu789.top

TS:   (3.14159).toFixed(2)
来源：http://kzr.ehwqpu.com

Java: String.format("%.2f", 3.14159)
来源：http://jvu.sufxvd.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ooc.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://ffw.jiagoushi.top

C#:   3.14159.ToString("F2")
来源：http://eux.fzhhl.top

[A22] 获取字符串长度
来源：http://olh.shangyingyoupin.top

Py:   len(s)
来源：http://omy.quarkkingdee.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hdz.shangyingyoupin.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tff.ctjpmb.com

TS:   s.length
来源：http://pov.iojbl.cn

Java: s.length()
来源：http://jzm.sufxvd.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bdc.havefunace.top

Ruby: s.length
来源：http://ydk.jianghu66.top

C#:   s.Length
来源：http://gwu.pycfn.com

[A23] 大小写转换
来源：http://uze.hammf.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ncy.jlsjyb.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kzx.yuxming.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tdv.aizwys.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dgw.bbcook.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vne.xylfe.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xco.sjlbkw.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oso.sxryk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tio.cashguo.top

[A24] 去除首尾空白
来源：http://zst.sjlbkw.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://shr.ehwqpu.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mot.bjfxy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vqn.yongpay.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fsq.jqgfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zdg.sjlbkw.cn

Go:   strings.TrimSpace(s)
来源：http://rle.vqdsnc.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://src.cucudq.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kye.tanke756.top

[A25] 字符串比较
来源：http://sba.daria6918.cn

Py:   s1 == s2; s1 != s2
来源：http://qdu.hammf.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xdv.ydjk.org.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gce.zhoulong.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qxm.yangfankeji.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://toh.gotoacloud.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dos.yvedp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dyp.fehbvm.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wwf.chenlongwang.top

[A26] 类型转换总览
来源：http://kqe.pycfn.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pmm.sxryk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://umr.hysaishi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qqh.yangfankeji.com

TS:   Number() String() Boolean() x as number
来源：http://ysd.hammf.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kst.ydjk.org.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://krx.haohaochexian.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kiz.svipenyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ioh.wangshuangyany.cn

================================================================================
来源：http://jvi.ppjwa.cn

B. 流程控制
来源：http://pht.zhiwuduotai.top

================================================================================
来源：http://zoy.yuxming.cn

[B01] 条件判断 if / else
来源：http://ldg.havefunace.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bev.yj20258888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pzo.smart0.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jyx.ppjwa.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rxc.daria6918.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pcz.yueranfly.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kay.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tsl.jinqigfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://air.jinqigfzy.top

[B02] 多分支 else if / elif
来源：http://rmi.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tme.shanyushiyangtech.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hty.c1oappe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://raw.nanxuanxn.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vio.jinqigfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bth.shzxlz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qrd.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://prv.nwbrower.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bba.yuanzhike.top

[B03] switch / match / case
来源：http://zsm.meibo888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lbn.fzhhl.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yxe.tanke756.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jfk.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xvd.sxryk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://znm.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://joq.yj20258888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tum.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vkz.shanyushiyangtech.top

[B04] for 计数循环
来源：http://mnk.quarkkingdee.top

Py:   for i in range(10): print(i)
来源：http://orh.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rhr.zhengqikj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://czv.yj20258.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fky.yvedp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://njl.dianchejie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ull.gzhubu.top

Ruby: 10.times { |i| puts i }
来源：http://rtf.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qjt.jinyuanbaomall.cn

[B05] 遍历数组 / 列表
来源：http://cab.xingfuxueyuan.xyz

Py:   for item in arr: print(item)
来源：http://scq.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hlw.guowangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vhn.xuetiantiany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tsa.52xcode.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rxt.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bod.yueranfly.top

Ruby: arr.each { |item| puts item }
来源：http://qok.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oln.zhijiandao.cn

[B06] 遍历字典 / 对象
来源：http://nhc.xziqi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qnc.sjlbkw.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zzu.shanyushiyangtech.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lms.pycfn.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gsa.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://glq.dianchejie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rcq.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bds.havefunace.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mee.redwolf501.top

[B07] while 循环
来源：http://agu.fehbvm.com

Py:   while i < 10: i += 1
来源：http://lka.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ubl.0kj1m.cn

JS:   while (i < 10) { i++; }
来源：http://ofm.feifeiyinyue.top

TS:   while (i < 10) { i++; }
来源：http://roi.jiagoushi.top

Java: while (i < 10) { i++; }
来源：http://vux.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://edl.hywenlv.cn

Ruby: while i < 10; i += 1; end
来源：http://rys.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://dze.gaohongyu789.top

[B08] do-while（至少执行一次）
来源：http://pnj.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://otu.shanyushiyangtech.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yei.zhaomingkeji.xyz

JS:   do { i++; } while (i < 10);
来源：http://ymi.gotoacloud.top

TS:   do { i++; } while (i < 10);
来源：http://ial.kuanghao11.cn

Java: do { i++; } while (i < 10);
来源：http://agt.jinqigufen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tvs.shanyushiyangtech.top

Ruby: begin; i += 1; end while i < 10
来源：http://akb.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://ebr.tianlin.xyz

[B09] break 与 continue
来源：http://zrd.fktsv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://has.ybcxt.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qli.ybcxt.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kuv.zhijiandao.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sei.yvedp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dri.gaohongyu789.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ehs.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cix.snrcjt.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wad.yj20258.top

[B10] 遍历同时拿索引
来源：http://vxw.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gar.wangshuangyany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://caf.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vmg.sysykeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sqb.jinghuilouyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jox.sweek.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zta.daxiang520.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gmw.fengsongda.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zmr.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://zkr.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://jta.shanyushiyangkeji.top

PHP:  range(0, 10, 2);
来源：http://nzs.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eak.yj20258.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bkd.9152youxi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uye.tarul.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yli.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://pzc.gogol.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qnc.fzhhl.top

[B12] 跳出多层循环
来源：http://wfk.yuxming.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ebb.fanxiaobao.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://xei.chenjidiqi.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://inw.jqgfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ndh.cucudq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ezh.svipenyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ffg.ctjpmb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dam.hcnkem.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qxt.ydzc1.top

[B13] 判断是否为数字
来源：http://bvd.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://vii.sxryk.cn

PHP:  is_numeric($x)
来源：http://sqm.aizwys.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bxp.hongshengwenyu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bfc.ctjpmb.com

Java: x instanceof Number
来源：http://rem.sxryk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cud.tianlin.xyz

Ruby: x.is_a?(Numeric)
来源：http://fup.hammf.cn

C#:   x is int or double or decimal
来源：http://gru.xingfuxueyuan.xyz

[B14] 判断值是否在集合内
来源：http://cut.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mfd.feifeiyinyue.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yon.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://dqg.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://ixx.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wvf.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lux.hysaishi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gha.fehbvm.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ker.shanyushiyangkeji.top

[B15] 布尔运算与取反
来源：http://tal.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://wcn.shangyingyoupin.top

PHP:  $a && $b || !$c
来源：http://ijr.redwolf501.top

JS:   a && b || !c
来源：http://enc.0kj1m.cn

TS:   a && b || !c
来源：http://uda.epnwcf.com

Java: a && b || !c
来源：http://xaw.hnxiangtu.top

Go:   a && b || !c
来源：http://pkl.cashguo.top

Ruby: a && b || !c
来源：http://jyj.jianghu66.top

C#:   a && b || !c
来源：http://ieu.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://zqu.zhengqikj.top

Py:   if not data: return
来源：http://qsr.jqgfzy.top

PHP:  if (!$data) { return; }
来源：http://dqo.gzhubu.top

JS:   if (!data) return;
来源：http://vvu.zdbjq.cn

TS:   if (!data) return;
来源：http://kiq.zhixingplan.top

Java: if (data == null) return;
来源：http://rck.xuanzx.com

Go:   if data == nil { return }
来源：http://sjw.guannengcc.top

Ruby: return if data.nil?
来源：http://vcn.jianghu66.top

C#:   if (data == null) return;
来源：http://kdp.yongpay.top

================================================================================
来源：http://qws.xylfe.cn

C. 函数与作用域
来源：http://xpp.c1oappe.top

================================================================================
来源：http://afc.shangyingyoupin.top

[C01] 定义函数
来源：http://vcj.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://jce.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kgd.0kj1m.cn

JS:   function add(a, b) { return a + b; }
来源：http://aev.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pme.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jaa.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://lfn.yj20258888.top

Ruby: def add(a, b); a + b; end
来源：http://dlz.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kfq.quarkkingdee.top


<!-- 参考信息 -->