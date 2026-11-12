代发 wailian999

[A10] 生成随机数
来源：http://puh.yonumen.top

Py:   import random; random.randint(1, 100)
来源：http://pgh.zhixingplan.top

PHP:  random_int(1, 100);
来源：http://oiy.cucudq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ufg.yj202588.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mmx.ybcxt.top

Java: new Random().nextInt(100) + 1
来源：http://flw.shzxlz.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ete.aizwys.cn

Ruby: rand(1..100)
来源：http://nzb.redwolf501.top

C#:   new Random().Next(1, 101)
来源：http://qck.cdnleiting.top

[A11] 条件表达式（三元）
来源：http://ope.yonumen.top

Py:   "yes" if x > 0 else "no"
来源：http://tux.ydjk.org.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rgl.chenzaomai.com

JS:   x > 0 ? "yes" : "no"
来源：http://nnt.ywan-chungtsiang.top

TS:   x > 0 ? "yes" : "no"
来源：http://tla.ppjwa.cn

Java: x > 0 ? "yes" : "no"
来源：http://pqo.chenzaomai.com

Go:   // 无三元运算符，需用 if 语句
来源：http://oaz.sufxvd.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lhh.yfazqb.com

C#:   x > 0 ? "yes" : "no"
来源：http://qho.fanxiaobao.xyz

[A12] 字符串插值 / 格式化
来源：http://zwa.hysaishi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vry.shangyingyoupin.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gis.shzxlz.cn

JS:   `Hello, ${name}!`
来源：http://xgh.daxiang520.top

TS:   `Hello, ${name}!`
来源：http://vfj.jianghu66.top

Java: "Hello, %s!".formatted(name)
来源：http://him.snrcjt.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jvp.smart0.xyz

Ruby: "Hello, #{name}!"
来源：http://kcl.yj20258.top

C#:   $"Hello, {name}!"
来源：http://zmt.hywenlv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://eba.shuidangran.top

Py:   "第一行\n第二行"
来源：http://ytu.shuidangran.top

PHP:  "第一行\n第二行"
来源：http://wju.guannengcc.top

JS:   "第一行\n第二行"
来源：http://iin.yj202588.top

TS:   "第一行\n第二行"
来源：http://nst.316326.xyz

Java: "第一行\n第二行"
来源：http://byp.gogol.net.cn

Go:   "第一行\n第二行"
来源：http://jbu.ydjk.org.cn

Ruby: "第一行\n第二行"
来源：http://gcc.jlsjyb.cn

C#:   "第一行\n第二行"
来源：http://mrh.yangfankeji.com

[A14] 注释写法
来源：http://igr.yj202588.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xfr.jinqigufen.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://mri.chenlongwang.top

JS:   // 单行；/* 多行 */
来源：http://tmv.ppjwa.cn

TS:   // 单行；/* 多行 */
来源：http://pks.zhixingplan.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xiq.zhixingplan.top

Go:   // 单行；/* 多行 */
来源：http://faa.fzhhl.top

Ruby: # 单行；=begin 多行 =end
来源：http://tzd.aibaodan.cn

C#:   // 单行；/* 多行 */
来源：http://ary.shanyushiyangkeji.top

[A15] 空值判断与默认值
来源：http://vmw.zhaomingkeji.xyz

Py:   value = data or "默认值"
来源：http://myd.daxiang520.top

PHP:  $value = $data ?? "默认值";
来源：http://pyf.epnwcf.com

JS:   const value = data ?? "默认值";
来源：http://iob.nanxuanxn.top

TS:   const value = data ?? "默认值";
来源：http://gvw.yj202588.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://han.birdmap.top

Go:   if data == "" { data = "默认值" }
来源：http://esk.xuanzx.com

Ruby: value = data || "默认值"
来源：http://doe.zhoulong.xyz

C#:   var value = data ?? "默认值";
来源：http://sft.yueranfly.top

[A16] 真假值判断规则
来源：http://abw.jinghuilouyu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cgq.zhiwuduotai.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bnl.vehdjk.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nyx.uphjek.com

TS:   if (!x) {}
来源：http://nzi.dianchejie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://okh.9152youxi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://spu.quarkkingdee.top

Ruby: unless x            # nil 与 false 为假
来源：http://eik.snrcjt.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wjv.yongpay.top

[A17] 位运算
来源：http://tpo.ydjk.org.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bdt.zdqjudy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vjx.vqdsnc.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bsw.feifeiyinyue.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uyj.nwbrower.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dwh.ctjpmb.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bfz.zhoulong.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fvj.sysykeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wgw.snrcjt.cn

[A18] 字符与 ASCII 码互转
来源：http://qvk.wangdashe.top

Py:   ord("A"); chr(65)
来源：http://psr.wangshuangyany.cn

PHP:  ord("A"); chr(65)
来源：http://ccs.ehwqpu.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bum.wangdashe.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qhi.cheryme.top

Java: (int) 'A'; (char) 65
来源：http://ecw.jinghuilouyu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pcp.cashguo.top

Ruby: "A".ord; 65.chr
来源：http://eng.epnwcf.com

C#:   (int)'A'; (char)65
来源：http://ize.fzhhl.top

[A19] 交换两个变量
来源：http://qsy.52xcode.cn

Py:   a, b = b, a
来源：http://wmh.sufxvd.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ghs.hnqzz.top

JS:   [a, b] = [b, a];
来源：http://bhm.epnwcf.com

TS:   [a, b] = [b, a];
来源：http://gxd.zdbjq.cn

Java: int t = a; a = b; b = t;
来源：http://als.havefunace.top

Go:   a, b = b, a
来源：http://juz.iojbl.cn

Ruby: a, b = b, a
来源：http://rpk.hnxiangtu.top

C#:   (a, b) = (b, a);
来源：http://mga.chenzaomai.com

[A20] 读取标准输入
来源：http://zhj.shuidangran.top

Py:   name = input("请输入：")
来源：http://xpj.hnxiangtu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://tum.shanyushiyangtech.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xvb.yueranfly.top

TS:   // Node.js：readline 模块
来源：http://lat.iojbl.cn

Java: new Scanner(System.in).nextLine()
来源：http://vkz.dianchejie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hdz.hcnkem.com

Ruby: gets.chomp
来源：http://myw.vehdjk.com

C#:   Console.ReadLine();
来源：http://wzj.fktsv.cn

[A21] 保留指定小数位输出
来源：http://gxj.c1oappe.top

Py:   f"{3.14159:.2f}"
来源：http://oko.ctjpmb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://muf.meibo888.top

JS:   (3.14159).toFixed(2)
来源：http://ymm.dianchejie.cn

TS:   (3.14159).toFixed(2)
来源：http://wrz.shangyingyoupin.top

Java: String.format("%.2f", 3.14159)
来源：http://jnk.redwolf501.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://itm.jlsjyb.cn

Ruby: format("%.2f", 3.14159)
来源：http://buv.yueranfly.top

C#:   3.14159.ToString("F2")
来源：http://ruc.wangdashe.top

[A22] 获取字符串长度
来源：http://lpa.sysykeji.top

Py:   len(s)
来源：http://knl.ydzc1.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vgo.ybcxt.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mop.yuxming.cn

TS:   s.length
来源：http://saz.guannengcc.top

Java: s.length()
来源：http://eiu.gotoacloud.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://arg.cqqwz.cn

Ruby: s.length
来源：http://odn.wangdashe.top

C#:   s.Length
来源：http://efu.cucudq.cn

[A23] 大小写转换
来源：http://ace.chenlongwang.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ewh.yj20258.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jll.zhixingplan.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://peg.tianlin.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cfa.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xex.haohaochexian.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yte.chenzaomai.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yfd.jlsjyb.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ade.yfazqb.com

[A24] 去除首尾空白
来源：http://sqc.yangfankeji.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qrp.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xsz.yj20258888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://adl.hfpthk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nlo.jinghuilouyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vbb.daria6918.cn

Go:   strings.TrimSpace(s)
来源：http://qfo.xylfe.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rah.nwbrower.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ugq.yonumen.top

[A25] 字符串比较
来源：http://skm.chenzaomai.com

Py:   s1 == s2; s1 != s2
来源：http://rsz.yuxming.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ilo.hesvh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bak.hywenlv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wgf.yuxming.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bzh.quarkkingdee.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cix.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uxz.xuetiantiany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fwg.bbcook.cn

[A26] 类型转换总览
来源：http://trv.xziqi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://clz.zhengqikj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ybr.zhengqikj.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zhf.jianghu66.top

TS:   Number() String() Boolean() x as number
来源：http://zvt.ydzc1.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xnf.xuetiantiany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://epg.xinyue.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://pow.cdnleiting.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jid.jinqigfzy.top

================================================================================
来源：http://otr.hammf.cn

B. 流程控制
来源：http://bdd.kuanghao11.cn

================================================================================
来源：http://eeb.jlsjyb.cn

[B01] 条件判断 if / else
来源：http://adp.xinyue.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://nem.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mws.cucudq.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pmc.shzxlz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qpz.yj20258888.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fpf.iojbl.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gzr.sysykeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cli.meibo888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jlh.hfpthk.cn

[B02] 多分支 else if / elif
来源：http://szv.yvedp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zsf.shanyushiyangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://spi.xylfe.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rmq.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ddd.fzhhl.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nif.yanxiufei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pwh.jqgufenzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yye.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vag.ppjwa.cn

[B03] switch / match / case
来源：http://ubr.sweek.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ctc.hesvh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://egb.wangdashe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://faz.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://phh.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xrp.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bdd.bbcook.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nwv.xuetiantiany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hdv.tanke756.top

[B04] for 计数循环
来源：http://vje.gaohongyu789.top

Py:   for i in range(10): print(i)
来源：http://lyu.jqgufenzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mxy.kuanghao11.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qaf.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vbk.yongpay.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ojq.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ucd.sjlbkw.cn

Ruby: 10.times { |i| puts i }
来源：http://zmc.gzhubu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fin.gaohongyu789.top

[B05] 遍历数组 / 列表
来源：http://rof.0kj1m.cn

Py:   for item in arr: print(item)
来源：http://hqi.zhijiandao.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qrz.zdbjq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://epa.kuanghao11.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fkj.xziqi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://isg.0kj1m.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vlj.hnqzz.top

Ruby: arr.each { |item| puts item }
来源：http://btf.redwolf501.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://emi.fengsongda.top

[B06] 遍历字典 / 对象
来源：http://ojp.xylfe.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sky.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uju.hcnkem.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uep.aizwys.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bfa.jyoumei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zjg.mhx1999.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ier.kuanghao11.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fgm.nwbrower.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dye.wangdashe.top

[B07] while 循环
来源：http://puo.hesvh.cn

Py:   while i < 10: i += 1
来源：http://gqo.nwbrower.top

PHP:  while ($i < 10) { $i++; }
来源：http://ajv.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://jrs.ctjpmb.com

TS:   while (i < 10) { i++; }
来源：http://qnv.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://jku.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pkv.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://woy.jinghuilouyu.cn

C#:   while (i < 10) { i++; }
来源：http://xif.fzhhl.top

[B08] do-while（至少执行一次）
来源：http://mzt.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://qbb.zhengqikj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cth.dianchejie.cn

JS:   do { i++; } while (i < 10);
来源：http://arh.ybcxt.top

TS:   do { i++; } while (i < 10);
来源：http://vsw.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://rvk.0kj1m.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kre.yuxming.cn

Ruby: begin; i += 1; end while i < 10
来源：http://egk.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://byz.iojbl.cn

[B09] break 与 continue
来源：http://lld.hcnkem.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mks.yangfankeji.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tzn.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sus.nwbrower.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ypl.wangshuangyany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jre.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wmn.ehwqpu.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iwu.nanxuanxn.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qvp.cheryme.top

[B10] 遍历同时拿索引
来源：http://scu.fehbvm.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vet.xziqi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pkj.jyoumei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dqe.haohaochexian.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dwo.zhengqikj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wbt.zhijiandao.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://epg.xingfuxueyuan.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ple.redwolf501.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ffe.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://vjw.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://sjh.cdnleiting.top

PHP:  range(0, 10, 2);
来源：http://enz.svipenyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rry.xylfe.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vfk.vqdsnc.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dsv.yonumen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xrf.xuanzx.com

Ruby: (0...10).step(2).to_a
来源：http://jik.jinqigufen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://szs.kuanghao11.cn

[B12] 跳出多层循环
来源：http://brk.zhengqikj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gsn.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://gge.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wky.pengpengdd.cyou

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ibb.yonumen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gyo.hongshengwenyu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wsf.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ldv.snrcjt.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qyh.cqqwz.cn

[B13] 判断是否为数字
来源：http://tga.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://ala.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://kzj.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oqd.andypj.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mfy.dashuyun.cn

Java: x instanceof Number
来源：http://ofa.yanxiufei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zuf.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://oca.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://xgv.wangshuangyany.cn

[B14] 判断值是否在集合内
来源：http://win.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dyv.shzxlz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nrt.xylfe.cn

JS:   [1, 2, 3].includes(x)
来源：http://ojp.jqgfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://znh.guowangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vui.birdmap.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://abw.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://dzs.gogol.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://owa.sysykeji.top

[B15] 布尔运算与取反
来源：http://heu.zhongyouzk.top

Py:   a and b or not c
来源：http://jkp.pycfn.com

PHP:  $a && $b || !$c
来源：http://gjs.jyoumei.cn

JS:   a && b || !c
来源：http://pgd.jinqigufen.top

TS:   a && b || !c
来源：http://dyx.bbcook.cn

Java: a && b || !c
来源：http://enn.gogol.net.cn

Go:   a && b || !c
来源：http://hbb.aibaodan.cn

Ruby: a && b || !c
来源：http://ipz.yangfankeji.com

C#:   a && b || !c
来源：http://lup.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://afg.havefunace.top

Py:   if not data: return
来源：http://nfp.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://ytp.nanxuanxn.top

JS:   if (!data) return;
来源：http://jih.ivvv.top

TS:   if (!data) return;
来源：http://rvl.sxryk.cn

Java: if (data == null) return;
来源：http://fnw.meibo888.top

Go:   if data == nil { return }
来源：http://obl.cheryme.top

Ruby: return if data.nil?
来源：http://sxz.xziqi.cn

C#:   if (data == null) return;
来源：http://xqv.fzhhl.top


<!-- 参考信息 -->