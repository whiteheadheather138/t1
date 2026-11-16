代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://dey.dianchejie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rpy.c1oappe.top

Java: x > 0 ? "yes" : "no"
来源：http://tko.shzxlz.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rws.xuetiantiany.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nnx.tanke756.top

C#:   x > 0 ? "yes" : "no"
来源：http://ruu.zhiwuduotai.top

[A12] 字符串插值 / 格式化
来源：http://ouu.zhixingplan.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wda.yj20258.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ltz.yuxming.cn

JS:   `Hello, ${name}!`
来源：http://ppd.ehwqpu.com

TS:   `Hello, ${name}!`
来源：http://gex.dianchejie.cn

Java: "Hello, %s!".formatted(name)
来源：http://vjz.zhaomingkeji.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pyi.nwbrower.top

Ruby: "Hello, #{name}!"
来源：http://ira.ydjk.org.cn

C#:   $"Hello, {name}!"
来源：http://ytt.birdmap.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dcf.hongshengwenyu.top

Py:   "第一行\n第二行"
来源：http://fyb.guannengcc.top

PHP:  "第一行\n第二行"
来源：http://xrt.svipenyu.cn

JS:   "第一行\n第二行"
来源：http://vcx.fehbvm.com

TS:   "第一行\n第二行"
来源：http://rsy.aizwys.cn

Java: "第一行\n第二行"
来源：http://hyw.birdmap.top

Go:   "第一行\n第二行"
来源：http://ewk.fanxiaobao.xyz

Ruby: "第一行\n第二行"
来源：http://kgd.cdnleiting.top

C#:   "第一行\n第二行"
来源：http://meg.zhixingplan.top

[A14] 注释写法
来源：http://aaz.ctjpmb.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://mjc.yueranfly.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://smk.zhixingplan.top

JS:   // 单行；/* 多行 */
来源：http://ekz.jqgfzy.top

TS:   // 单行；/* 多行 */
来源：http://qws.sufxvd.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://myk.jinqigfzy.top

Go:   // 单行；/* 多行 */
来源：http://ndx.yuanzhike.top

Ruby: # 单行；=begin 多行 =end
来源：http://ddr.zhengqikj.top

C#:   // 单行；/* 多行 */
来源：http://anx.xuetiantiany.cn

[A15] 空值判断与默认值
来源：http://aeq.fehbvm.com

Py:   value = data or "默认值"
来源：http://kqp.fehbvm.com

PHP:  $value = $data ?? "默认值";
来源：http://fda.zhoulong.xyz

JS:   const value = data ?? "默认值";
来源：http://evl.guannengcc.top

TS:   const value = data ?? "默认值";
来源：http://rul.yongpay.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pmb.jqgfzy.top

Go:   if data == "" { data = "默认值" }
来源：http://soa.chenjidiqi.icu

Ruby: value = data || "默认值"
来源：http://nfo.gogol.net.cn

C#:   var value = data ?? "默认值";
来源：http://edu.nwbrower.top

[A16] 真假值判断规则
来源：http://atj.zhengqikj.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kda.zycfv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xxs.hammf.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mzh.daria6918.cn

TS:   if (!x) {}
来源：http://evk.smart0.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zsw.52xcode.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iuw.ybcxt.top

Ruby: unless x            # nil 与 false 为假
来源：http://gtn.ydzc1.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bjo.jinghuilouyu.cn

[A17] 位运算
来源：http://gwu.feifeiyinyue.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kyd.fktsv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ptf.hywenlv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cql.xuetiantiany.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jix.yfazqb.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gak.yfazqb.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qvw.yueranfly.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hsd.cdnleiting.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hdi.guowangkeji.top

[A18] 字符与 ASCII 码互转
来源：http://kjb.hongshengwenyu.top

Py:   ord("A"); chr(65)
来源：http://uel.ppjwa.cn

PHP:  ord("A"); chr(65)
来源：http://cmr.quarkkingdee.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fua.cheryme.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nqw.0kj1m.cn

Java: (int) 'A'; (char) 65
来源：http://mif.daria6918.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://csk.xylfe.cn

Ruby: "A".ord; 65.chr
来源：http://vll.feifeiyinyue.top

C#:   (int)'A'; (char)65
来源：http://qya.daxiang520.top

[A19] 交换两个变量
来源：http://qrd.gotoacloud.top

Py:   a, b = b, a
来源：http://iwj.xylfe.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gse.chenlongwang.top

JS:   [a, b] = [b, a];
来源：http://ybp.gogol.net.cn

TS:   [a, b] = [b, a];
来源：http://wyk.nanxuanxn.top

Java: int t = a; a = b; b = t;
来源：http://xbx.yueranfly.top

Go:   a, b = b, a
来源：http://jqa.jinqigufen.top

Ruby: a, b = b, a
来源：http://brh.iojbl.cn

C#:   (a, b) = (b, a);
来源：http://iky.quarkkingdee.top

[A20] 读取标准输入
来源：http://zwv.yangfankeji.com

Py:   name = input("请输入：")
来源：http://plb.52xcode.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bpj.xziqi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kfg.daxiang520.top

TS:   // Node.js：readline 模块
来源：http://tqz.wangshuangyany.cn

Java: new Scanner(System.in).nextLine()
来源：http://mzk.jianghu66.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dkh.xuanzx.com

Ruby: gets.chomp
来源：http://any.sweek.top

C#:   Console.ReadLine();
来源：http://jrx.feifeiyinyue.top

[A21] 保留指定小数位输出
来源：http://nwl.zhijiandao.cn

Py:   f"{3.14159:.2f}"
来源：http://alx.cheryme.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hdj.guannengcc.top

JS:   (3.14159).toFixed(2)
来源：http://esw.vehdjk.com

TS:   (3.14159).toFixed(2)
来源：http://gwb.daria6918.cn

Java: String.format("%.2f", 3.14159)
来源：http://bqj.ehwqpu.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://glp.jinyuanbaomall.cn

Ruby: format("%.2f", 3.14159)
来源：http://vsa.zhaomingkeji.xyz

C#:   3.14159.ToString("F2")
来源：http://dmw.ydjk.org.cn

[A22] 获取字符串长度
来源：http://fuw.chenjidiqi.icu

Py:   len(s)
来源：http://iiw.0kj1m.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nts.zhixingplan.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://elc.tanke756.top

TS:   s.length
来源：http://irr.sjlbkw.cn

Java: s.length()
来源：http://ode.jqgfzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fby.jlsjyb.cn

Ruby: s.length
来源：http://pzl.pycfn.com

C#:   s.Length
来源：http://uxb.fengsongda.top

[A23] 大小写转换
来源：http://ban.vqdsnc.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ttj.sysykeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ebq.sweek.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wux.pengpengdd.cyou

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gcp.ydzc1.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ego.gzhubu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ybb.hcnkem.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wpp.ehwqpu.com

C#:   s.ToUpper(); s.ToLower()
来源：http://olw.yangfankeji.com

[A24] 去除首尾空白
来源：http://ziq.zhiwuduotai.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eam.uphjek.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wxk.haohaochexian.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nzj.chenzaomai.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zjm.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lkw.haohaochexian.top

Go:   strings.TrimSpace(s)
来源：http://zng.sjlbkw.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vsm.yueranfly.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nbb.xziqi.cn

[A25] 字符串比较
来源：http://csl.ctjpmb.com

Py:   s1 == s2; s1 != s2
来源：http://fis.ehwqpu.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qml.yueranfly.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ykc.xingfuxueyuan.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fdf.shzxlz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vbe.dianchejie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kaa.cheryme.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rdq.hysaishi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ytj.cucudq.cn

[A26] 类型转换总览
来源：http://rlv.jyoumei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rin.jiagoushi.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qgw.quarkkingdee.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wki.c1oappe.top

TS:   Number() String() Boolean() x as number
来源：http://wjk.vehdjk.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cjv.svipenyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sjg.xuanzx.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://vqn.zycfv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sxz.fengsongda.top

================================================================================
来源：http://lrw.gogol.net.cn

B. 流程控制
来源：http://ztb.fengsongda.top

================================================================================
来源：http://ges.yueranfly.top

[B01] 条件判断 if / else
来源：http://blt.dashuyun.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vbj.xuanzx.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wus.zhixingplan.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hcm.guannengcc.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yjv.birdmap.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qld.yanxiufei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gne.ctjpmb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rsr.jinqigufen.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dkt.dashuyun.cn

[B02] 多分支 else if / elif
来源：http://pbo.gaohongyu789.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gdp.sweek.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pyp.hywenlv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mdr.tianlin.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bqj.fzhhl.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hzg.316326.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sqo.zhiwuduotai.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wrv.haohaochexian.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ifh.nwbrower.top

[B03] switch / match / case
来源：http://igi.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cro.jyoumei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cus.jianghu66.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rmm.ehwqpu.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nxi.c1oappe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vku.hammf.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ohi.sxryk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://abi.hysaishi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tyl.epnwcf.com

[B04] for 计数循环
来源：http://wbp.hongshengwenyu.top

Py:   for i in range(10): print(i)
来源：http://fuk.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nlo.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cvv.hywenlv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ytx.tian-w.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dyf.daxiang520.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://scz.quarkkingdee.top

Ruby: 10.times { |i| puts i }
来源：http://ptt.pycfn.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fhn.jinqigufen.top

[B05] 遍历数组 / 列表
来源：http://dcr.nanxinkj.top

Py:   for item in arr: print(item)
来源：http://tuy.xuetiantiany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zar.yonumen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://szg.yuanzhike.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xly.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://emk.cdnleiting.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fec.wangshuangyany.cn

Ruby: arr.each { |item| puts item }
来源：http://dzz.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pod.zhongyouzk.top

[B06] 遍历字典 / 对象
来源：http://jlv.zdbjq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mus.sysykeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rvr.cashguo.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://erw.jyoumei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zbi.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zpt.aizwys.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zqi.52xcode.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qrn.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jvu.daria6918.cn

[B07] while 循环
来源：http://hfq.jqgufenzy.top

Py:   while i < 10: i += 1
来源：http://gir.cqqwz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qyf.hesvh.cn

JS:   while (i < 10) { i++; }
来源：http://ust.sxryk.cn

TS:   while (i < 10) { i++; }
来源：http://ynb.kuanghao11.cn

Java: while (i < 10) { i++; }
来源：http://dnj.hysaishi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dkz.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://bpq.vehdjk.com

C#:   while (i < 10) { i++; }
来源：http://gmt.sysykeji.top

[B08] do-while（至少执行一次）
来源：http://fct.cucudq.cn

Py:   # 无 do-while：用 while True + break
来源：http://wyq.shangyingyoupin.top

PHP:  do { $i++; } while ($i < 10);
来源：http://asg.fktsv.cn

JS:   do { i++; } while (i < 10);
来源：http://qeg.zhaomingkeji.xyz

TS:   do { i++; } while (i < 10);
来源：http://ctd.zhengqikj.top

Java: do { i++; } while (i < 10);
来源：http://rpz.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xyz.zhongyouzk.top

Ruby: begin; i += 1; end while i < 10
来源：http://dfi.cqqwz.cn

C#:   do { i++; } while (i < 10);
来源：http://kwj.jinghuilouyu.cn

[B09] break 与 continue
来源：http://elz.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gif.yfazqb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dqq.yongpay.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://csq.zhoulong.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xbl.52xcode.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mlk.shzxlz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bzt.ydzc1.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://szy.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ffa.daria6918.cn

[B10] 遍历同时拿索引
来源：http://pys.chenjidiqi.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qzf.jyoumei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ztm.kuanghao11.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rwa.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pwt.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xnq.ivvv.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xut.kuanghao11.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xvx.hfpthk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wwu.meibo888.top

[B11] 生成数字序列 / 区间
来源：http://agf.ydjk.org.cn

Py:   list(range(0, 10, 2))
来源：http://osn.yj202588.top

PHP:  range(0, 10, 2);
来源：http://rtp.yuanzhike.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ulr.xingfuxueyuan.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kdl.hesvh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://flj.fzhhl.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jld.yangfankeji.com

Ruby: (0...10).step(2).to_a
来源：http://dqi.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rex.fktsv.cn

[B12] 跳出多层循环
来源：http://yae.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://paj.sufxvd.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ogk.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kzy.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://acs.tarul.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hjy.guannengcc.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ygg.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ulw.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vci.zhoulong.xyz

[B13] 判断是否为数字
来源：http://hfl.9152youxi.cn

Py:   isinstance(x, (int, float))
来源：http://qxx.jianghu66.top

PHP:  is_numeric($x)
来源：http://iqs.jyoumei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hxv.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nht.ivvv.top

Java: x instanceof Number
来源：http://ztt.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rzy.zdqjudy.top

Ruby: x.is_a?(Numeric)
来源：http://wry.svipenyu.cn

C#:   x is int or double or decimal
来源：http://cwh.smart0.xyz

[B14] 判断值是否在集合内
来源：http://qtg.yvedp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://suw.iojbl.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nqc.nwbrower.top

JS:   [1, 2, 3].includes(x)
来源：http://rfc.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://izl.guowangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tjo.jinghuilouyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qgm.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://uqm.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://onq.xingfuxueyuan.xyz

[B15] 布尔运算与取反
来源：http://hoa.316326.xyz

Py:   a and b or not c
来源：http://wme.pengpengdd.cyou

PHP:  $a && $b || !$c
来源：http://hgc.quarkkingdee.top

JS:   a && b || !c
来源：http://ehf.chenlongwang.top

TS:   a && b || !c
来源：http://qwe.yj202588.top

Java: a && b || !c
来源：http://dqh.yvedp.cn

Go:   a && b || !c
来源：http://sqy.zdqjudy.top

Ruby: a && b || !c
来源：http://fvv.dianchejie.cn

C#:   a && b || !c
来源：http://azb.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://ick.cdnleiting.top

Py:   if not data: return
来源：http://rss.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://shx.iojbl.cn

JS:   if (!data) return;
来源：http://rve.fzhhl.top

TS:   if (!data) return;
来源：http://ypj.gogol.net.cn

Java: if (data == null) return;
来源：http://fgp.redwolf501.top

Go:   if data == nil { return }
来源：http://rlw.jyoumei.cn

Ruby: return if data.nil?
来源：http://eug.andypj.xyz

C#:   if (data == null) return;
来源：http://buy.zycfv.cn

================================================================================
来源：http://cnq.fehbvm.com

C. 函数与作用域
来源：http://mmr.vehdjk.com

================================================================================
来源：http://spc.jinqigufen.top

[C01] 定义函数
来源：http://oin.sweek.top

Py:   def add(a, b): return a + b
来源：http://okn.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vun.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://hos.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fjz.0kj1m.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qyh.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://tmc.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://sqx.hfpthk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bcv.uphjek.com


<!-- 参考信息 -->