代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://hpi.sweek.top

[A11] 条件表达式（三元）
来源：http://bdz.wangdashe.top

Py:   "yes" if x > 0 else "no"
来源：http://cwp.guannengcc.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://rec.hongshengwenyu.top

JS:   x > 0 ? "yes" : "no"
来源：http://ubk.xuanzx.com

TS:   x > 0 ? "yes" : "no"
来源：http://gim.jinghuilouyu.cn

Java: x > 0 ? "yes" : "no"
来源：http://rkd.0kj1m.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://imh.kuanghao11.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mdg.cdnleiting.top

C#:   x > 0 ? "yes" : "no"
来源：http://qji.ctjpmb.com

[A12] 字符串插值 / 格式化
来源：http://sgf.sweek.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://knp.bjfxy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pdw.yongpay.top

JS:   `Hello, ${name}!`
来源：http://hbc.yonumen.top

TS:   `Hello, ${name}!`
来源：http://fju.uphjek.com

Java: "Hello, %s!".formatted(name)
来源：http://lqt.snrcjt.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tvg.cheryme.top

Ruby: "Hello, #{name}!"
来源：http://iej.vqdsnc.cn

C#:   $"Hello, {name}!"
来源：http://osa.redwolf501.top

[A13] 多行字符串（练习 \n 转义）
来源：http://cie.jianghu66.top

Py:   "第一行\n第二行"
来源：http://eqe.zhijiandao.cn

PHP:  "第一行\n第二行"
来源：http://mge.ctjpmb.com

JS:   "第一行\n第二行"
来源：http://tab.fzhhl.top

TS:   "第一行\n第二行"
来源：http://amh.yanxiufei.cn

Java: "第一行\n第二行"
来源：http://eyf.sjlbkw.cn

Go:   "第一行\n第二行"
来源：http://iuh.gogol.net.cn

Ruby: "第一行\n第二行"
来源：http://plb.yvedp.cn

C#:   "第一行\n第二行"
来源：http://wiz.nwbrower.top

[A14] 注释写法
来源：http://nfl.smart0.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://vsu.andypj.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://zjc.cqqwz.cn

JS:   // 单行；/* 多行 */
来源：http://rvy.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://ffn.tianlin.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jbp.wangdashe.top

Go:   // 单行；/* 多行 */
来源：http://tta.0kj1m.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zlb.jqgfzy.top

C#:   // 单行；/* 多行 */
来源：http://cek.shangyingyoupin.top

[A15] 空值判断与默认值
来源：http://lto.jiagoushi.top

Py:   value = data or "默认值"
来源：http://lol.jinqigfzy.top

PHP:  $value = $data ?? "默认值";
来源：http://tly.yj20258888.top

JS:   const value = data ?? "默认值";
来源：http://syi.fanxiaobao.xyz

TS:   const value = data ?? "默认值";
来源：http://rma.nanxuanxn.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gye.aizwys.cn

Go:   if data == "" { data = "默认值" }
来源：http://uxc.hywenlv.cn

Ruby: value = data || "默认值"
来源：http://fbi.hcnkem.com

C#:   var value = data ?? "默认值";
来源：http://qae.gaohongyu789.top

[A16] 真假值判断规则
来源：http://vnv.yj20258.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pbz.yvedp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lkx.cashguo.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zps.jlsjyb.cn

TS:   if (!x) {}
来源：http://fie.svipenyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ixs.tian-w.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uhh.jyoumei.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kja.bjfxy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://trx.zhoulong.xyz

[A17] 位运算
来源：http://zsz.andypj.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hbp.bjfxy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://osu.yongpay.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vwm.yfazqb.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xlf.hywenlv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xtb.sweek.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://eqt.hongshengwenyu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lvl.fktsv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rgp.feifeiyinyue.top

[A18] 字符与 ASCII 码互转
来源：http://hka.tarul.cn

Py:   ord("A"); chr(65)
来源：http://tel.zhoulong.xyz

PHP:  ord("A"); chr(65)
来源：http://jiz.yangfankeji.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sku.jqgufenzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pzo.jinqigufen.top

Java: (int) 'A'; (char) 65
来源：http://enn.zhengqikj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://los.sxryk.cn

Ruby: "A".ord; 65.chr
来源：http://osh.hywenlv.cn

C#:   (int)'A'; (char)65
来源：http://ziy.aizwys.cn

[A19] 交换两个变量
来源：http://yma.zhengqikj.top

Py:   a, b = b, a
来源：http://qvr.jqgufenzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://oya.ydzc1.top

JS:   [a, b] = [b, a];
来源：http://ivu.gzhubu.top

TS:   [a, b] = [b, a];
来源：http://hed.316326.xyz

Java: int t = a; a = b; b = t;
来源：http://ynn.ivvv.top

Go:   a, b = b, a
来源：http://ujc.cqqwz.cn

Ruby: a, b = b, a
来源：http://fej.9152youxi.cn

C#:   (a, b) = (b, a);
来源：http://rjb.meibo888.top

[A20] 读取标准输入
来源：http://exm.nanxuanxn.top

Py:   name = input("请输入：")
来源：http://ras.fzhhl.top

PHP:  $name = trim(fgets(STDIN));
来源：http://tzh.guowangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vwv.yangfankeji.com

TS:   // Node.js：readline 模块
来源：http://lqr.xuetiantiany.cn

Java: new Scanner(System.in).nextLine()
来源：http://bma.yonumen.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://upw.wangdashe.top

Ruby: gets.chomp
来源：http://spu.zhoulong.xyz

C#:   Console.ReadLine();
来源：http://fwm.jianghu66.top

[A21] 保留指定小数位输出
来源：http://zdy.redwolf501.top

Py:   f"{3.14159:.2f}"
来源：http://uyv.cucudq.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wbe.jinqigufen.top

JS:   (3.14159).toFixed(2)
来源：http://xwd.cdnleiting.top

TS:   (3.14159).toFixed(2)
来源：http://vtb.sysykeji.top

Java: String.format("%.2f", 3.14159)
来源：http://msk.fengsongda.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://utk.hnxiangtu.top

Ruby: format("%.2f", 3.14159)
来源：http://pax.yangfankeji.com

C#:   3.14159.ToString("F2")
来源：http://vdy.bjfxy.top

[A22] 获取字符串长度
来源：http://hva.sysykeji.top

Py:   len(s)
来源：http://gxm.zhongyouzk.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ktf.zycfv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ryr.jinqigufen.top

TS:   s.length
来源：http://kig.svipenyu.cn

Java: s.length()
来源：http://vsq.jinyuanbaomall.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wfh.yvedp.cn

Ruby: s.length
来源：http://fdv.haohaochexian.top

C#:   s.Length
来源：http://iie.meibo888.top

[A23] 大小写转换
来源：http://alm.tianlin.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://xqs.cheryme.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://abp.smart0.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wbo.jinqigufen.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vlz.yongpay.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pet.redwolf501.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dce.tarul.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zft.ppjwa.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nzx.haohaochexian.top

[A24] 去除首尾空白
来源：http://kkx.gaohongyu789.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jai.cucudq.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://atd.daria6918.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wfi.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ivu.zhijiandao.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://unz.hcnkem.com

Go:   strings.TrimSpace(s)
来源：http://hja.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fvj.sufxvd.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tpl.svipenyu.cn

[A25] 字符串比较
来源：http://hdp.shzxlz.cn

Py:   s1 == s2; s1 != s2
来源：http://gwf.redwolf501.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dqn.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nbq.jinyuanbaomall.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ibt.hywenlv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://phj.daxiang520.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ich.yueranfly.top

Ruby: s1 == s2; s1 <=> s2
来源：http://smh.fengsongda.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://amp.hnqzz.top

[A26] 类型转换总览
来源：http://plj.hesvh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zvk.zdbjq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hji.bjfxy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://joq.shangyingyoupin.top

TS:   Number() String() Boolean() x as number
来源：http://ttq.cqqwz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://usq.pengpengdd.cyou

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://trg.yongpay.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qln.guowangkeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zad.hywenlv.cn

================================================================================
来源：http://gnh.yuanzhike.top

B. 流程控制
来源：http://iaa.yj202588.top

================================================================================
来源：http://fcq.guannengcc.top

[B01] 条件判断 if / else
来源：http://qcg.fzhhl.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xmo.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cic.jqgufenzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rwt.hnxiangtu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hdk.yangfankeji.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://pgg.9152youxi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bla.tanke756.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ghi.jinyuanbaomall.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vsc.aibaodan.cn

[B02] 多分支 else if / elif
来源：http://xuh.ybcxt.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bcz.pycfn.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eau.dashuyun.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hex.zhengqikj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nzw.ivvv.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rdd.snrcjt.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tme.ywan-chungtsiang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kyu.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yrj.hcnkem.com

[B03] switch / match / case
来源：http://bsj.sysykeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yom.sjlbkw.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fya.jlsjyb.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vpd.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://icr.zhoulong.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qay.sufxvd.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zzi.yangfankeji.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gpt.guowangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qnp.cheryme.top

[B04] for 计数循环
来源：http://mtw.hysaishi.cn

Py:   for i in range(10): print(i)
来源：http://ack.jlsjyb.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yoc.andypj.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eev.hesvh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jxa.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://huc.chenzaomai.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vjc.uphjek.com

Ruby: 10.times { |i| puts i }
来源：http://qni.sufxvd.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wxc.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://alu.gotoacloud.top

Py:   for item in arr: print(item)
来源：http://sin.jinqigufen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jlv.sysykeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://onx.xinyue.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://ktd.yonumen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uym.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ehx.gotoacloud.top

Ruby: arr.each { |item| puts item }
来源：http://cln.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vtf.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://knb.yuanzhike.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lwn.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ncn.shuidangran.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wcp.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xhq.xinyue.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dmb.jyoumei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eya.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://auq.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://opl.meibo888.top

[B07] while 循环
来源：http://ade.chenzaomai.com

Py:   while i < 10: i += 1
来源：http://dqr.shuidangran.top

PHP:  while ($i < 10) { $i++; }
来源：http://aoy.ybcxt.top

JS:   while (i < 10) { i++; }
来源：http://gox.wangshuangyany.cn

TS:   while (i < 10) { i++; }
来源：http://rub.zdqjudy.top

Java: while (i < 10) { i++; }
来源：http://yly.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dlf.svipenyu.cn

Ruby: while i < 10; i += 1; end
来源：http://dgj.hammf.cn

C#:   while (i < 10) { i++; }
来源：http://avb.xylfe.cn

[B08] do-while（至少执行一次）
来源：http://wem.yj20258888.top

Py:   # 无 do-while：用 while True + break
来源：http://eeu.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zdx.redwolf501.top

JS:   do { i++; } while (i < 10);
来源：http://nqx.yongpay.top

TS:   do { i++; } while (i < 10);
来源：http://mxq.zycfv.cn

Java: do { i++; } while (i < 10);
来源：http://ees.hcnkem.com

Go:   for { i++; if i >= 10 { break } }
来源：http://suf.svipenyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uun.sysykeji.top

C#:   do { i++; } while (i < 10);
来源：http://vem.mhx1999.top

[B09] break 与 continue
来源：http://gqa.nanxuanxn.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kvf.dianchejie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kds.sweek.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fjl.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://for.hesvh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jaz.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jhc.uphjek.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hzz.iojbl.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gme.xuanzx.com

[B10] 遍历同时拿索引
来源：http://qqo.kuanghao11.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vmv.feifeiyinyue.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xht.hnxiangtu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jga.hongshengwenyu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kdn.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bbv.dianchejie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tpy.ywan-chungtsiang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cdv.xinyue.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yvc.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://mrd.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://ten.vqdsnc.cn

PHP:  range(0, 10, 2);
来源：http://ray.hesvh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zun.hfpthk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pxm.jinqigfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://krh.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dxu.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://mly.jinghuilouyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wnh.hammf.cn

[B12] 跳出多层循环
来源：http://mut.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://pce.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://pri.yueranfly.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vxq.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dgc.sweek.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mko.svipenyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jks.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hik.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aio.zhaomingkeji.xyz

[B13] 判断是否为数字
来源：http://qui.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://tok.dianchejie.cn

PHP:  is_numeric($x)
来源：http://zwr.fktsv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rck.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jzk.316326.xyz

Java: x instanceof Number
来源：http://jkn.jqgfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uei.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://tkk.gotoacloud.top

C#:   x is int or double or decimal
来源：http://dyv.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://pcf.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fmg.jinyuanbaomall.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://azt.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://nqq.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://hkv.zhijiandao.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fkz.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ubp.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://ktm.fanxiaobao.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mfs.yj20258888.top

[B15] 布尔运算与取反
来源：http://amn.shanyushiyangkeji.top

Py:   a and b or not c
来源：http://fuu.yj202588.top

PHP:  $a && $b || !$c
来源：http://xdk.xuanzx.com

JS:   a && b || !c
来源：http://eda.jlsjyb.cn

TS:   a && b || !c
来源：http://thg.ppjwa.cn

Java: a && b || !c
来源：http://wxj.shuidangran.top

Go:   a && b || !c
来源：http://ekz.birdmap.top

Ruby: a && b || !c
来源：http://frd.vqdsnc.cn

C#:   a && b || !c
来源：http://yha.jyoumei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zgg.xylfe.cn

Py:   if not data: return
来源：http://pkm.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://dwb.shangyingyoupin.top

JS:   if (!data) return;
来源：http://tyo.pycfn.com

TS:   if (!data) return;
来源：http://paw.hnqzz.top

Java: if (data == null) return;
来源：http://sgf.zdqjudy.top

Go:   if data == nil { return }
来源：http://oat.0kj1m.cn

Ruby: return if data.nil?
来源：http://kwf.gotoacloud.top

C#:   if (data == null) return;
来源：http://uzq.daria6918.cn

================================================================================
来源：http://vrl.cashguo.top

C. 函数与作用域
来源：http://hgj.shanyushiyangkeji.top

================================================================================
来源：http://lpg.fanxiaobao.xyz

[C01] 定义函数
来源：http://myc.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://vin.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nzw.hesvh.cn

JS:   function add(a, b) { return a + b; }
来源：http://yhn.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hlu.zhijiandao.cn


<!-- 参考信息 -->