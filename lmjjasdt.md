代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://hle.cheryme.top

[A11] 条件表达式（三元）
来源：http://kfz.cdnleiting.top

Py:   "yes" if x > 0 else "no"
来源：http://vfu.xuanzx.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://aqm.ivvv.top

JS:   x > 0 ? "yes" : "no"
来源：http://hpf.wangdashe.top

TS:   x > 0 ? "yes" : "no"
来源：http://gzr.feifeiyinyue.top

Java: x > 0 ? "yes" : "no"
来源：http://tpi.vehdjk.com

Go:   // 无三元运算符，需用 if 语句
来源：http://ldo.hysaishi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wtd.quarkkingdee.top

C#:   x > 0 ? "yes" : "no"
来源：http://kvm.quarkkingdee.top

[A12] 字符串插值 / 格式化
来源：http://fig.shangyingyoupin.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fem.ydzc1.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nsj.snrcjt.cn

JS:   `Hello, ${name}!`
来源：http://ztm.ctjpmb.com

TS:   `Hello, ${name}!`
来源：http://cda.smart0.xyz

Java: "Hello, %s!".formatted(name)
来源：http://kuk.jqgufenzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zmo.ppjwa.cn

Ruby: "Hello, #{name}!"
来源：http://prj.cashguo.top

C#:   $"Hello, {name}!"
来源：http://tne.tian-w.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dpy.9152youxi.cn

Py:   "第一行\n第二行"
来源：http://gok.dashuyun.cn

PHP:  "第一行\n第二行"
来源：http://ldh.jinqigufen.top

JS:   "第一行\n第二行"
来源：http://xih.sweek.top

TS:   "第一行\n第二行"
来源：http://rah.tarul.cn

Java: "第一行\n第二行"
来源：http://nzt.kuanghao11.cn

Go:   "第一行\n第二行"
来源：http://qjm.cheryme.top

Ruby: "第一行\n第二行"
来源：http://ihl.zhaomingkeji.xyz

C#:   "第一行\n第二行"
来源：http://lmm.sjlbkw.cn

[A14] 注释写法
来源：http://erb.yj20258.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qld.smart0.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://foz.pengpengdd.cyou

JS:   // 单行；/* 多行 */
来源：http://bfv.chenzaomai.com

TS:   // 单行；/* 多行 */
来源：http://xef.fehbvm.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rau.cucudq.cn

Go:   // 单行；/* 多行 */
来源：http://ygr.yfazqb.com

Ruby: # 单行；=begin 多行 =end
来源：http://vgj.xinyue.icu

C#:   // 单行；/* 多行 */
来源：http://vfi.316326.xyz

[A15] 空值判断与默认值
来源：http://kud.uphjek.com

Py:   value = data or "默认值"
来源：http://tva.cdnleiting.top

PHP:  $value = $data ?? "默认值";
来源：http://wrd.yongpay.top

JS:   const value = data ?? "默认值";
来源：http://enl.cdnleiting.top

TS:   const value = data ?? "默认值";
来源：http://wie.quarkkingdee.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dol.gotoacloud.top

Go:   if data == "" { data = "默认值" }
来源：http://ahe.zhiwuduotai.top

Ruby: value = data || "默认值"
来源：http://frf.hammf.cn

C#:   var value = data ?? "默认值";
来源：http://sau.fanxiaobao.xyz

[A16] 真假值判断规则
来源：http://ehb.hfpthk.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://czh.kuanghao11.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xnr.xylfe.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tzp.9152youxi.cn

TS:   if (!x) {}
来源：http://vdb.kuanghao11.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tuy.yj20258888.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yoc.yanxiufei.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ano.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fea.hcnkem.com

[A17] 位运算
来源：http://nlg.jinqigufen.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hto.nanxinkj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lzw.yvedp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://krr.xuetiantiany.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cdd.yfazqb.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gvn.nwbrower.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://aee.zhijiandao.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wtf.jqgfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://htf.yueranfly.top

[A18] 字符与 ASCII 码互转
来源：http://diq.chenzaomai.com

Py:   ord("A"); chr(65)
来源：http://xkt.gotoacloud.top

PHP:  ord("A"); chr(65)
来源：http://zsi.sxryk.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://elu.yongpay.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fhp.sweek.top

Java: (int) 'A'; (char) 65
来源：http://gqq.svipenyu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://aqt.yongpay.top

Ruby: "A".ord; 65.chr
来源：http://rof.shuidangran.top

C#:   (int)'A'; (char)65
来源：http://nor.tanke756.top

[A19] 交换两个变量
来源：http://afv.yueranfly.top

Py:   a, b = b, a
来源：http://gxb.tarul.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hws.jyoumei.cn

JS:   [a, b] = [b, a];
来源：http://dux.pengpengdd.cyou

TS:   [a, b] = [b, a];
来源：http://jes.aizwys.cn

Java: int t = a; a = b; b = t;
来源：http://mpn.yueranfly.top

Go:   a, b = b, a
来源：http://pmh.shzxlz.cn

Ruby: a, b = b, a
来源：http://opa.hnqzz.top

C#:   (a, b) = (b, a);
来源：http://obo.yj20258.top

[A20] 读取标准输入
来源：http://ccw.xinyue.icu

Py:   name = input("请输入：")
来源：http://axq.fehbvm.com

PHP:  $name = trim(fgets(STDIN));
来源：http://nxz.tianlin.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sdu.ybcxt.top

TS:   // Node.js：readline 模块
来源：http://bou.xinyue.icu

Java: new Scanner(System.in).nextLine()
来源：http://fna.c1oappe.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wqh.tarul.cn

Ruby: gets.chomp
来源：http://spu.bjfxy.top

C#:   Console.ReadLine();
来源：http://lkj.mhx1999.top

[A21] 保留指定小数位输出
来源：http://eit.jqgfzy.top

Py:   f"{3.14159:.2f}"
来源：http://ewa.dashuyun.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mbv.svipenyu.cn

JS:   (3.14159).toFixed(2)
来源：http://von.zhoulong.xyz

TS:   (3.14159).toFixed(2)
来源：http://ezm.hnqzz.top

Java: String.format("%.2f", 3.14159)
来源：http://gnf.0kj1m.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://epg.yueranfly.top

Ruby: format("%.2f", 3.14159)
来源：http://tjb.jinghuilouyu.cn

C#:   3.14159.ToString("F2")
来源：http://prb.zhijiandao.cn

[A22] 获取字符串长度
来源：http://bql.jiagoushi.top

Py:   len(s)
来源：http://hrm.ehwqpu.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://crk.xuanzx.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gan.gaohongyu789.top

TS:   s.length
来源：http://szf.ehwqpu.com

Java: s.length()
来源：http://wjh.xuanzx.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://agv.andypj.xyz

Ruby: s.length
来源：http://oot.hammf.cn

C#:   s.Length
来源：http://bko.ppjwa.cn

[A23] 大小写转换
来源：http://lzt.hywenlv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wtt.sufxvd.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://auj.chenzaomai.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fza.yj202588.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kkp.zdqjudy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qkn.yueranfly.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://var.sysykeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vew.cdnleiting.top

C#:   s.ToUpper(); s.ToLower()
来源：http://tsw.ppjwa.cn

[A24] 去除首尾空白
来源：http://erp.jianghu66.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aem.9152youxi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hjn.jinghuilouyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vmv.birdmap.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aqs.sxryk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://phw.yj20258888.top

Go:   strings.TrimSpace(s)
来源：http://oob.sweek.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ycq.chenzaomai.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vuc.aibaodan.cn

[A25] 字符串比较
来源：http://lks.zycfv.cn

Py:   s1 == s2; s1 != s2
来源：http://nzl.vqdsnc.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qwz.smart0.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qhc.cucudq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ptl.c1oappe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rix.tanke756.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tee.daria6918.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fyu.gotoacloud.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yvc.xingfuxueyuan.xyz

[A26] 类型转换总览
来源：http://gdr.nanxuanxn.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://czc.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hlt.jinyuanbaomall.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gzz.nanxinkj.top

TS:   Number() String() Boolean() x as number
来源：http://prd.ywan-chungtsiang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gmi.52xcode.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://izm.yvedp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jck.nwbrower.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tyy.aibaodan.cn

================================================================================
来源：http://sup.ydjk.org.cn

B. 流程控制
来源：http://zzy.tarul.cn

================================================================================
来源：http://zbr.yvedp.cn

[B01] 条件判断 if / else
来源：http://tfr.cucudq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kxi.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dii.vqdsnc.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zog.daria6918.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gzs.sufxvd.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ltx.sysykeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ubt.yonumen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vbu.chenjidiqi.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gkv.gogol.net.cn

[B02] 多分支 else if / elif
来源：http://qxe.fanxiaobao.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qrm.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eok.xuetiantiany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qwa.zdbjq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qcu.ywan-chungtsiang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fsj.haohaochexian.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kpg.zhoulong.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tbk.xinyue.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://itd.ppjwa.cn

[B03] switch / match / case
来源：http://aea.smart0.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hts.pengpengdd.cyou

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wpq.hysaishi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wce.hysaishi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pms.zhixingplan.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zjp.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ern.xziqi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jlg.pengpengdd.cyou

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://urv.dianchejie.cn

[B04] for 计数循环
来源：http://rrj.0kj1m.cn

Py:   for i in range(10): print(i)
来源：http://gwk.cucudq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kuv.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eyd.zhengqikj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://piw.shanyushiyangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yft.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cyu.hysaishi.cn

Ruby: 10.times { |i| puts i }
来源：http://orx.feifeiyinyue.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fvp.sysykeji.top

[B05] 遍历数组 / 列表
来源：http://fnq.0kj1m.cn

Py:   for item in arr: print(item)
来源：http://wvv.sxryk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vxg.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tkd.xuetiantiany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zwn.fanxiaobao.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://ode.nwbrower.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vnj.pengpengdd.cyou

Ruby: arr.each { |item| puts item }
来源：http://eok.jiagoushi.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pdv.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://tsu.bbcook.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cjp.hywenlv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fhq.xinyue.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bgf.zycfv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://euf.shanyushiyangtech.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ech.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dyw.fehbvm.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bld.zhongyouzk.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://llz.sysykeji.top

[B07] while 循环
来源：http://evo.pycfn.com

Py:   while i < 10: i += 1
来源：http://mjj.wangdashe.top

PHP:  while ($i < 10) { $i++; }
来源：http://eev.yonumen.top

JS:   while (i < 10) { i++; }
来源：http://cno.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://hmq.shuidangran.top

Java: while (i < 10) { i++; }
来源：http://hep.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zwa.aizwys.cn

Ruby: while i < 10; i += 1; end
来源：http://new.bbcook.cn

C#:   while (i < 10) { i++; }
来源：http://oji.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://php.52xcode.cn

Py:   # 无 do-while：用 while True + break
来源：http://kqt.xziqi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://svk.ydzc1.top

JS:   do { i++; } while (i < 10);
来源：http://pck.ydjk.org.cn

TS:   do { i++; } while (i < 10);
来源：http://lix.nanxinkj.top

Java: do { i++; } while (i < 10);
来源：http://yje.xylfe.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sgf.chenlongwang.top

Ruby: begin; i += 1; end while i < 10
来源：http://ejb.bbcook.cn

C#:   do { i++; } while (i < 10);
来源：http://syq.uphjek.com

[B09] break 与 continue
来源：http://wes.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://enw.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ntg.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yxd.shzxlz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kdg.ppjwa.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vvm.shzxlz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vua.sufxvd.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mql.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ays.dashuyun.cn

[B10] 遍历同时拿索引
来源：http://mwp.jqgfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jrf.yj20258888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://udf.gzhubu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tew.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://umk.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ihs.316326.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dfv.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tcl.tian-w.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vqf.zdbjq.cn

[B11] 生成数字序列 / 区间
来源：http://rqg.gzhubu.top

Py:   list(range(0, 10, 2))
来源：http://pro.gaohongyu789.top

PHP:  range(0, 10, 2);
来源：http://mbh.shanyushiyangtech.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xwh.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aaf.chenzaomai.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://doa.meibo888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mtk.xinyue.icu

Ruby: (0...10).step(2).to_a
来源：http://jwk.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ywu.yj20258888.top

[B12] 跳出多层循环
来源：http://zuu.xylfe.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ldo.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://feb.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hgb.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zof.ybcxt.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zof.tianlin.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://msg.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fdk.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bbm.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://cxi.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://oiu.tanke756.top

PHP:  is_numeric($x)
来源：http://wxf.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ezy.chenjidiqi.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qsx.shanyushiyangkeji.top

Java: x instanceof Number
来源：http://hoy.zdbjq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qod.meibo888.top

Ruby: x.is_a?(Numeric)
来源：http://exs.yvedp.cn

C#:   x is int or double or decimal
来源：http://kuz.hnqzz.top

[B14] 判断值是否在集合内
来源：http://rzv.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cff.zhiwuduotai.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kam.vehdjk.com

JS:   [1, 2, 3].includes(x)
来源：http://euo.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://rmm.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xhb.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mif.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://icl.hongshengwenyu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bfw.cucudq.cn

[B15] 布尔运算与取反
来源：http://edo.yanxiufei.cn

Py:   a and b or not c
来源：http://uik.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://rbq.mhx1999.top

JS:   a && b || !c
来源：http://kqi.0kj1m.cn

TS:   a && b || !c
来源：http://mge.9152youxi.cn

Java: a && b || !c
来源：http://ypc.hnqzz.top

Go:   a && b || !c
来源：http://mod.pengpengdd.cyou

Ruby: a && b || !c
来源：http://umf.jyoumei.cn

C#:   a && b || !c
来源：http://kby.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kmq.bjfxy.top

Py:   if not data: return
来源：http://kea.tianlin.xyz

PHP:  if (!$data) { return; }
来源：http://gsa.sjlbkw.cn

JS:   if (!data) return;
来源：http://ppc.zhoulong.xyz

TS:   if (!data) return;
来源：http://pld.ppjwa.cn

Java: if (data == null) return;
来源：http://qrv.cqqwz.cn

Go:   if data == nil { return }
来源：http://dth.ppjwa.cn

Ruby: return if data.nil?
来源：http://rba.tian-w.cn

C#:   if (data == null) return;
来源：http://kgy.yuxming.cn

================================================================================
来源：http://lfr.chenlongwang.top

C. 函数与作用域
来源：http://zpx.hnqzz.top

================================================================================
来源：http://rzz.vehdjk.com

[C01] 定义函数
来源：http://pox.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://imz.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://spl.hammf.cn

JS:   function add(a, b) { return a + b; }
来源：http://grl.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tut.chenlongwang.top


<!-- 参考信息 -->