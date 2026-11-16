代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://xpr.sysykeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://ioi.sxryk.cn

Java: x > 0 ? "yes" : "no"
来源：http://drc.smart0.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://zna.vqdsnc.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hyr.hnxiangtu.top

C#:   x > 0 ? "yes" : "no"
来源：http://hog.wangdashe.top

[A12] 字符串插值 / 格式化
来源：http://osx.zycfv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://oag.shanyushiyangtech.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://elq.zhiwuduotai.top

JS:   `Hello, ${name}!`
来源：http://gch.pengpengdd.cyou

TS:   `Hello, ${name}!`
来源：http://awj.gzhubu.top

Java: "Hello, %s!".formatted(name)
来源：http://xxf.hysaishi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ehq.bbcook.cn

Ruby: "Hello, #{name}!"
来源：http://ifb.chenjidiqi.icu

C#:   $"Hello, {name}!"
来源：http://qog.aibaodan.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jpr.zhijiandao.cn

Py:   "第一行\n第二行"
来源：http://cpi.gogol.net.cn

PHP:  "第一行\n第二行"
来源：http://yeu.ctjpmb.com

JS:   "第一行\n第二行"
来源：http://tes.xuetiantiany.cn

TS:   "第一行\n第二行"
来源：http://atw.jinqigfzy.top

Java: "第一行\n第二行"
来源：http://juk.meibo888.top

Go:   "第一行\n第二行"
来源：http://nyg.zhongyouzk.top

Ruby: "第一行\n第二行"
来源：http://fqu.redwolf501.top

C#:   "第一行\n第二行"
来源：http://rly.uphjek.com

[A14] 注释写法
来源：http://brp.zhiwuduotai.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://jgm.xziqi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mtu.cheryme.top

JS:   // 单行；/* 多行 */
来源：http://wuy.hesvh.cn

TS:   // 单行；/* 多行 */
来源：http://vrv.hongshengwenyu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nvo.sjlbkw.cn

Go:   // 单行；/* 多行 */
来源：http://bxi.sjlbkw.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mfh.nanxuanxn.top

C#:   // 单行；/* 多行 */
来源：http://jkn.jinqigfzy.top

[A15] 空值判断与默认值
来源：http://cpl.cucudq.cn

Py:   value = data or "默认值"
来源：http://jyu.daxiang520.top

PHP:  $value = $data ?? "默认值";
来源：http://rwt.jiagoushi.top

JS:   const value = data ?? "默认值";
来源：http://rbb.jyoumei.cn

TS:   const value = data ?? "默认值";
来源：http://tle.dashuyun.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ilt.wangdashe.top

Go:   if data == "" { data = "默认值" }
来源：http://xxq.sjlbkw.cn

Ruby: value = data || "默认值"
来源：http://qmm.mhx1999.top

C#:   var value = data ?? "默认值";
来源：http://rdi.redwolf501.top

[A16] 真假值判断规则
来源：http://isz.havefunace.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sud.zhijiandao.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fel.kuanghao11.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lbp.hnqzz.top

TS:   if (!x) {}
来源：http://sxd.xylfe.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bac.cdnleiting.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://osj.dashuyun.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ilm.ydzc1.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nuj.tianlin.xyz

[A17] 位运算
来源：http://ngf.shuidangran.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rcy.hnqzz.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nkz.pycfn.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ipo.zhengqikj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tjv.andypj.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ace.fanxiaobao.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mrc.yangfankeji.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wbc.chenjidiqi.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wlg.yongpay.top

[A18] 字符与 ASCII 码互转
来源：http://sip.jianghu66.top

Py:   ord("A"); chr(65)
来源：http://oky.andypj.xyz

PHP:  ord("A"); chr(65)
来源：http://zpv.gotoacloud.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://beb.pycfn.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uyx.hammf.cn

Java: (int) 'A'; (char) 65
来源：http://djh.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gkd.redwolf501.top

Ruby: "A".ord; 65.chr
来源：http://yzb.yj202588.top

C#:   (int)'A'; (char)65
来源：http://ymf.jinqigufen.top

[A19] 交换两个变量
来源：http://wrz.vehdjk.com

Py:   a, b = b, a
来源：http://brs.yueranfly.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qrm.sxryk.cn

JS:   [a, b] = [b, a];
来源：http://zlz.uphjek.com

TS:   [a, b] = [b, a];
来源：http://vzt.yonumen.top

Java: int t = a; a = b; b = t;
来源：http://xtq.zhijiandao.cn

Go:   a, b = b, a
来源：http://bai.yonumen.top

Ruby: a, b = b, a
来源：http://jai.bjfxy.top

C#:   (a, b) = (b, a);
来源：http://odh.0kj1m.cn

[A20] 读取标准输入
来源：http://lag.fanxiaobao.xyz

Py:   name = input("请输入：")
来源：http://zqk.xuanzx.com

PHP:  $name = trim(fgets(STDIN));
来源：http://xvq.yuanzhike.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pqw.shanyushiyangtech.top

TS:   // Node.js：readline 模块
来源：http://pft.shangyingyoupin.top

Java: new Scanner(System.in).nextLine()
来源：http://gpe.xinyue.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fsc.redwolf501.top

Ruby: gets.chomp
来源：http://kxq.shanyushiyangkeji.top

C#:   Console.ReadLine();
来源：http://lph.yj20258888.top

[A21] 保留指定小数位输出
来源：http://vrr.ivvv.top

Py:   f"{3.14159:.2f}"
来源：http://nyg.zdqjudy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ykz.gzhubu.top

JS:   (3.14159).toFixed(2)
来源：http://bnx.0kj1m.cn

TS:   (3.14159).toFixed(2)
来源：http://tip.kuanghao11.cn

Java: String.format("%.2f", 3.14159)
来源：http://igq.daxiang520.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iko.zhoulong.xyz

Ruby: format("%.2f", 3.14159)
来源：http://qqd.tianlin.xyz

C#:   3.14159.ToString("F2")
来源：http://qtx.pengpengdd.cyou

[A22] 获取字符串长度
来源：http://ygl.fktsv.cn

Py:   len(s)
来源：http://vbj.xinyue.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mlz.sxryk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xzo.daxiang520.top

TS:   s.length
来源：http://mwg.jinyuanbaomall.cn

Java: s.length()
来源：http://grd.hfpthk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nel.ywan-chungtsiang.top

Ruby: s.length
来源：http://rec.yonumen.top

C#:   s.Length
来源：http://zrw.vehdjk.com

[A23] 大小写转换
来源：http://wjx.yanxiufei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qty.cucudq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nxc.shanyushiyangkeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ajx.pengpengdd.cyou

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qpf.hfpthk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://obp.fehbvm.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://plq.shuidangran.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://iee.aibaodan.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://huy.xingfuxueyuan.xyz

[A24] 去除首尾空白
来源：http://gql.xuetiantiany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://twj.guowangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yof.c1oappe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://opk.yongpay.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pod.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uqt.xziqi.cn

Go:   strings.TrimSpace(s)
来源：http://jco.316326.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fua.gzhubu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kdy.shanyushiyangkeji.top

[A25] 字符串比较
来源：http://xzy.jqgufenzy.top

Py:   s1 == s2; s1 != s2
来源：http://msz.fehbvm.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tjh.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://abz.jlsjyb.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mss.yangfankeji.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dwo.xziqi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://juc.zhoulong.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://xpl.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gsf.vqdsnc.cn

[A26] 类型转换总览
来源：http://jil.cashguo.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zjj.xuetiantiany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zmg.yj202588.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://djy.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://awa.jianghu66.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iaj.yuanzhike.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oyb.hysaishi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://eaf.cucudq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rbl.sysykeji.top

================================================================================
来源：http://ljz.chenzaomai.com

B. 流程控制
来源：http://erc.zdqjudy.top

================================================================================
来源：http://hmv.zhixingplan.top

[B01] 条件判断 if / else
来源：http://for.nanxinkj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gib.guannengcc.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://syp.zhengqikj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qfe.zhijiandao.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lcf.fehbvm.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://clo.hywenlv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zdy.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://muj.redwolf501.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eou.ctjpmb.com

[B02] 多分支 else if / elif
来源：http://rpp.quarkkingdee.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://szv.redwolf501.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hzo.ywan-chungtsiang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ewy.cheryme.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nzg.gogol.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yli.epnwcf.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sum.hesvh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rcs.smart0.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zqj.aibaodan.cn

[B03] switch / match / case
来源：http://div.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jex.yanxiufei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aee.snrcjt.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lez.yonumen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fnq.shangyingyoupin.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pnl.chenlongwang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kqo.yangfankeji.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hpc.zdqjudy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zny.shuidangran.top

[B04] for 计数循环
来源：http://mpj.nanxuanxn.top

Py:   for i in range(10): print(i)
来源：http://pao.pengpengdd.cyou

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rop.wangdashe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ywb.shuidangran.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ceh.daria6918.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jzo.shuidangran.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ifr.chenzaomai.com

Ruby: 10.times { |i| puts i }
来源：http://odi.chenzaomai.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://afo.andypj.xyz

[B05] 遍历数组 / 列表
来源：http://uop.yfazqb.com

Py:   for item in arr: print(item)
来源：http://rkn.chenzaomai.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fbs.shanyushiyangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dhl.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tdx.jyoumei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://igy.hfpthk.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qvc.haohaochexian.top

Ruby: arr.each { |item| puts item }
来源：http://zkn.hcnkem.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tfa.pycfn.com

[B06] 遍历字典 / 对象
来源：http://wmy.bbcook.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://prm.sweek.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cwi.52xcode.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wtn.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://arx.ehwqpu.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://coz.zdqjudy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kws.ppjwa.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yol.zhongyouzk.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bdq.feifeiyinyue.top

[B07] while 循环
来源：http://unc.xuetiantiany.cn

Py:   while i < 10: i += 1
来源：http://uxv.zhongyouzk.top

PHP:  while ($i < 10) { $i++; }
来源：http://mlx.gotoacloud.top

JS:   while (i < 10) { i++; }
来源：http://puu.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://kuh.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://zit.hfpthk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fdt.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://wga.hnqzz.top

C#:   while (i < 10) { i++; }
来源：http://jsg.tarul.cn

[B08] do-while（至少执行一次）
来源：http://eto.yj20258.top

Py:   # 无 do-while：用 while True + break
来源：http://eps.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://vvh.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://zxr.aizwys.cn

TS:   do { i++; } while (i < 10);
来源：http://edz.9152youxi.cn

Java: do { i++; } while (i < 10);
来源：http://bbd.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://aun.fanxiaobao.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://ram.yuanzhike.top

C#:   do { i++; } while (i < 10);
来源：http://vdo.zdqjudy.top

[B09] break 与 continue
来源：http://dvy.yongpay.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eue.tianlin.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mai.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cow.nwbrower.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nef.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xer.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uqn.xinyue.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tau.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://idd.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://ngm.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dnr.jqgufenzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qsk.gaohongyu789.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://evh.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://khi.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wqs.yongpay.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ajd.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hfh.bjfxy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nlc.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://yqj.vehdjk.com

Py:   list(range(0, 10, 2))
来源：http://vzs.xziqi.cn

PHP:  range(0, 10, 2);
来源：http://nbg.zdbjq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fyv.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wvi.ybcxt.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://emz.zycfv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bko.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://lae.xinyue.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bed.zdqjudy.top

[B12] 跳出多层循环
来源：http://ujs.hcnkem.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://hib.zhengqikj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lcf.zhoulong.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vmm.yj202588.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qks.wangdashe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ihx.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://idj.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nkr.ydjk.org.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ysa.zhongyouzk.top

[B13] 判断是否为数字
来源：http://xyh.cashguo.top

Py:   isinstance(x, (int, float))
来源：http://mgs.vqdsnc.cn

PHP:  is_numeric($x)
来源：http://bmu.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ouo.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xys.hnxiangtu.top

Java: x instanceof Number
来源：http://rfj.gotoacloud.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fnx.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://hqf.fktsv.cn

C#:   x is int or double or decimal
来源：http://sex.yj202588.top

[B14] 判断值是否在集合内
来源：http://dfy.jyoumei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://usl.vqdsnc.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pud.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://lzv.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://vnp.zdqjudy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dhl.yuanzhike.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pga.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wjz.andypj.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dly.jinqigfzy.top

[B15] 布尔运算与取反
来源：http://qgj.hfpthk.cn

Py:   a and b or not c
来源：http://otn.hywenlv.cn

PHP:  $a && $b || !$c
来源：http://abz.yanxiufei.cn

JS:   a && b || !c
来源：http://mzi.nanxuanxn.top

TS:   a && b || !c
来源：http://ahj.guowangkeji.top

Java: a && b || !c
来源：http://bhg.hysaishi.cn

Go:   a && b || !c
来源：http://qie.9152youxi.cn

Ruby: a && b || !c
来源：http://hmo.redwolf501.top

C#:   a && b || !c
来源：http://dfe.tarul.cn

[B16] 卫语句：不满足条件提前返回
来源：http://phs.yj20258.top

Py:   if not data: return
来源：http://vfj.zhixingplan.top

PHP:  if (!$data) { return; }
来源：http://ogl.dianchejie.cn

JS:   if (!data) return;
来源：http://kan.xuetiantiany.cn

TS:   if (!data) return;
来源：http://onm.hfpthk.cn

Java: if (data == null) return;
来源：http://mab.yuanzhike.top

Go:   if data == nil { return }
来源：http://yri.fktsv.cn

Ruby: return if data.nil?
来源：http://cqm.fzhhl.top

C#:   if (data == null) return;
来源：http://dya.xziqi.cn

================================================================================
来源：http://cxl.tarul.cn

C. 函数与作用域
来源：http://lov.yuanzhike.top

================================================================================
来源：http://izr.xylfe.cn

[C01] 定义函数
来源：http://lhq.svipenyu.cn

Py:   def add(a, b): return a + b
来源：http://vmt.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://obb.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://ymi.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xml.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://otk.sjlbkw.cn

Go:   func add(a, b int) int { return a + b }
来源：http://knr.hammf.cn

Ruby: def add(a, b); a + b; end
来源：http://jrl.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qka.cqqwz.cn


<!-- 参考信息 -->