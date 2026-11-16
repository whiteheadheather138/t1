代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://awz.xuetiantiany.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sjm.daria6918.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://chd.sufxvd.cn

[A09] 绝对值与最大最小值
来源：http://uxe.zhongyouzk.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jpx.fanxiaobao.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yva.yanxiufei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wbl.cdnleiting.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lrw.ydzc1.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://amn.cucudq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://efc.fktsv.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blx.wangshuangyany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qci.yonumen.top

[A10] 生成随机数
来源：http://qjm.uphjek.com

Py:   import random; random.randint(1, 100)
来源：http://sib.quarkkingdee.top

PHP:  random_int(1, 100);
来源：http://jsm.wangdashe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yoa.wangdashe.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hme.cucudq.cn

Java: new Random().nextInt(100) + 1
来源：http://gfu.xziqi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://flo.ivvv.top

Ruby: rand(1..100)
来源：http://kga.hysaishi.cn

C#:   new Random().Next(1, 101)
来源：http://afe.yj20258888.top

[A11] 条件表达式（三元）
来源：http://put.gotoacloud.top

Py:   "yes" if x > 0 else "no"
来源：http://hzm.sxryk.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mnl.hfpthk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://oho.yongpay.top

TS:   x > 0 ? "yes" : "no"
来源：http://tpk.yj20258888.top

Java: x > 0 ? "yes" : "no"
来源：http://joq.cheryme.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jzd.chenjidiqi.icu

Ruby: x > 0 ? "yes" : "no"
来源：http://wax.yuanzhike.top

C#:   x > 0 ? "yes" : "no"
来源：http://vwz.hesvh.cn

[A12] 字符串插值 / 格式化
来源：http://gqa.hammf.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xmw.yanxiufei.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dei.yueranfly.top

JS:   `Hello, ${name}!`
来源：http://prx.xylfe.cn

TS:   `Hello, ${name}!`
来源：http://xps.vehdjk.com

Java: "Hello, %s!".formatted(name)
来源：http://nqp.shanyushiyangtech.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sgk.zhongyouzk.top

Ruby: "Hello, #{name}!"
来源：http://wun.kuanghao11.cn

C#:   $"Hello, {name}!"
来源：http://iag.shanyushiyangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://xeo.chenlongwang.top

Py:   "第一行\n第二行"
来源：http://vqr.zdbjq.cn

PHP:  "第一行\n第二行"
来源：http://asf.sufxvd.cn

JS:   "第一行\n第二行"
来源：http://chm.quarkkingdee.top

TS:   "第一行\n第二行"
来源：http://ovc.hesvh.cn

Java: "第一行\n第二行"
来源：http://hud.yvedp.cn

Go:   "第一行\n第二行"
来源：http://uau.jinqigufen.top

Ruby: "第一行\n第二行"
来源：http://god.havefunace.top

C#:   "第一行\n第二行"
来源：http://wjk.quarkkingdee.top

[A14] 注释写法
来源：http://lee.ehwqpu.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://vwb.andypj.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://zif.cheryme.top

JS:   // 单行；/* 多行 */
来源：http://siy.fzhhl.top

TS:   // 单行；/* 多行 */
来源：http://dwi.gaohongyu789.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cpl.gogol.net.cn

Go:   // 单行；/* 多行 */
来源：http://dcm.yj20258.top

Ruby: # 单行；=begin 多行 =end
来源：http://uim.vqdsnc.cn

C#:   // 单行；/* 多行 */
来源：http://dmv.xziqi.cn

[A15] 空值判断与默认值
来源：http://oys.shanyushiyangtech.top

Py:   value = data or "默认值"
来源：http://dbo.chenjidiqi.icu

PHP:  $value = $data ?? "默认值";
来源：http://cbi.xinyue.icu

JS:   const value = data ?? "默认值";
来源：http://qev.xziqi.cn

TS:   const value = data ?? "默认值";
来源：http://fuv.daria6918.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://irr.c1oappe.top

Go:   if data == "" { data = "默认值" }
来源：http://xlz.gzhubu.top

Ruby: value = data || "默认值"
来源：http://upi.hnxiangtu.top

C#:   var value = data ?? "默认值";
来源：http://iav.zhiwuduotai.top

[A16] 真假值判断规则
来源：http://dzg.cashguo.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rcn.yueranfly.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://krx.gogol.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://afi.shanyushiyangkeji.top

TS:   if (!x) {}
来源：http://mgv.smart0.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ryz.gaohongyu789.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://izq.gaohongyu789.top

Ruby: unless x            # nil 与 false 为假
来源：http://qck.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bfp.ivvv.top

[A17] 位运算
来源：http://awo.cashguo.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ayj.andypj.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ycl.nanxuanxn.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jwc.yj20258888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hel.cucudq.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rje.sxryk.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rrh.guowangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vpw.yonumen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kwr.hcnkem.com

[A18] 字符与 ASCII 码互转
来源：http://nco.yanxiufei.cn

Py:   ord("A"); chr(65)
来源：http://hfn.cheryme.top

PHP:  ord("A"); chr(65)
来源：http://nph.jinqigfzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://srp.jinqigufen.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lhl.tianlin.xyz

Java: (int) 'A'; (char) 65
来源：http://ktp.zhiwuduotai.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wcj.tanke756.top

Ruby: "A".ord; 65.chr
来源：http://kgn.tarul.cn

C#:   (int)'A'; (char)65
来源：http://ont.guowangkeji.top

[A19] 交换两个变量
来源：http://xtz.jqgufenzy.top

Py:   a, b = b, a
来源：http://fhv.zhongyouzk.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ktf.pycfn.com

JS:   [a, b] = [b, a];
来源：http://kto.yangfankeji.com

TS:   [a, b] = [b, a];
来源：http://dgl.jinyuanbaomall.cn

Java: int t = a; a = b; b = t;
来源：http://blu.jqgufenzy.top

Go:   a, b = b, a
来源：http://flx.hcnkem.com

Ruby: a, b = b, a
来源：http://ceb.gotoacloud.top

C#:   (a, b) = (b, a);
来源：http://rad.yanxiufei.cn

[A20] 读取标准输入
来源：http://oej.gaohongyu789.top

Py:   name = input("请输入：")
来源：http://vfx.sjlbkw.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zia.mhx1999.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eac.yongpay.top

TS:   // Node.js：readline 模块
来源：http://jwh.tian-w.cn

Java: new Scanner(System.in).nextLine()
来源：http://bkj.zhongyouzk.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://oml.gogol.net.cn

Ruby: gets.chomp
来源：http://brb.zycfv.cn

C#:   Console.ReadLine();
来源：http://nvb.tarul.cn

[A21] 保留指定小数位输出
来源：http://koo.hammf.cn

Py:   f"{3.14159:.2f}"
来源：http://zsm.wangshuangyany.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cof.hfpthk.cn

JS:   (3.14159).toFixed(2)
来源：http://xab.pycfn.com

TS:   (3.14159).toFixed(2)
来源：http://muq.nanxinkj.top

Java: String.format("%.2f", 3.14159)
来源：http://zcd.fanxiaobao.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ttn.svipenyu.cn

Ruby: format("%.2f", 3.14159)
来源：http://rty.snrcjt.cn

C#:   3.14159.ToString("F2")
来源：http://xxo.bbcook.cn

[A22] 获取字符串长度
来源：http://gaa.daria6918.cn

Py:   len(s)
来源：http://jrj.tianlin.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ltq.52xcode.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eaz.nanxinkj.top

TS:   s.length
来源：http://chu.ehwqpu.com

Java: s.length()
来源：http://qrd.jianghu66.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hej.xinyue.icu

Ruby: s.length
来源：http://txy.ppjwa.cn

C#:   s.Length
来源：http://ugb.fanxiaobao.xyz

[A23] 大小写转换
来源：http://cio.c1oappe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wcp.ydjk.org.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zyp.xuetiantiany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wzk.guannengcc.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://aad.dashuyun.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qzm.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zdw.hysaishi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lpo.mhx1999.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lnm.zycfv.cn

[A24] 去除首尾空白
来源：http://zyt.fengsongda.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tod.svipenyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nct.hnqzz.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oiz.fengsongda.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jgv.chenlongwang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lzs.hcnkem.com

Go:   strings.TrimSpace(s)
来源：http://bpj.nwbrower.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mtv.zhixingplan.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dkk.yanxiufei.cn

[A25] 字符串比较
来源：http://zxs.tian-w.cn

Py:   s1 == s2; s1 != s2
来源：http://upw.mhx1999.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fdq.jinqigfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tsv.fengsongda.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://roo.meibo888.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eam.c1oappe.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tzc.fzhhl.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bgy.gzhubu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ady.vehdjk.com

[A26] 类型转换总览
来源：http://xfs.yangfankeji.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sev.cashguo.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wjw.ydzc1.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nbr.pengpengdd.cyou

TS:   Number() String() Boolean() x as number
来源：http://ybg.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vlc.hnqzz.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fzn.hnqzz.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kup.epnwcf.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wad.tianlin.xyz

================================================================================
来源：http://ken.sweek.top

B. 流程控制
来源：http://dbm.guowangkeji.top

================================================================================
来源：http://gjp.vehdjk.com

[B01] 条件判断 if / else
来源：http://ixq.wangdashe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zof.wangdashe.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wbf.yfazqb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eaa.vehdjk.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rkn.vehdjk.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://oxj.tanke756.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://abu.zhiwuduotai.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jfv.feifeiyinyue.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pde.yuanzhike.top

[B02] 多分支 else if / elif
来源：http://crj.jyoumei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rtz.nanxuanxn.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://alh.yj20258.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jww.zhoulong.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://shi.52xcode.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kva.yongpay.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xub.aibaodan.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zsi.jinghuilouyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ygi.pycfn.com

[B03] switch / match / case
来源：http://uwr.nanxinkj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rma.yongpay.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uqc.jiagoushi.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jpn.c1oappe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wzz.iojbl.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rrd.ybcxt.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vdw.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cvl.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nhv.jinqigfzy.top

[B04] for 计数循环
来源：http://jwh.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://pth.feifeiyinyue.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hxf.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lon.wangdashe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qeo.ydzc1.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pzp.feifeiyinyue.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://snx.cashguo.top

Ruby: 10.times { |i| puts i }
来源：http://teb.ehwqpu.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pcn.xylfe.cn

[B05] 遍历数组 / 列表
来源：http://yvk.xziqi.cn

Py:   for item in arr: print(item)
来源：http://vbn.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://knz.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vhj.ivvv.top

TS:   for (const item of arr) { console.log(item); }
来源：http://euf.snrcjt.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vdw.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ryk.vqdsnc.cn

Ruby: arr.each { |item| puts item }
来源：http://psn.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ipp.jlsjyb.cn

[B06] 遍历字典 / 对象
来源：http://gfk.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gwt.zdqjudy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://toi.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dbd.guannengcc.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://czh.mhx1999.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tsx.yj202588.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ttt.hywenlv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hzj.havefunace.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fdp.yonumen.top

[B07] while 循环
来源：http://ckw.9152youxi.cn

Py:   while i < 10: i += 1
来源：http://vkj.sweek.top

PHP:  while ($i < 10) { $i++; }
来源：http://ehw.jyoumei.cn

JS:   while (i < 10) { i++; }
来源：http://ffh.chenjidiqi.icu

TS:   while (i < 10) { i++; }
来源：http://ahj.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://qjb.daxiang520.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dml.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://njo.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://qud.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://atl.fehbvm.com

Py:   # 无 do-while：用 while True + break
来源：http://szp.gotoacloud.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kne.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://kka.c1oappe.top

TS:   do { i++; } while (i < 10);
来源：http://usg.hcnkem.com

Java: do { i++; } while (i < 10);
来源：http://pbx.zycfv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sjc.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://miz.yuanzhike.top

C#:   do { i++; } while (i < 10);
来源：http://acl.fzhhl.top

[B09] break 与 continue
来源：http://zrf.zhixingplan.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cnn.yuanzhike.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://czf.iojbl.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://shk.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://owq.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gcw.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://myq.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://swm.snrcjt.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lyh.ppjwa.cn

[B10] 遍历同时拿索引
来源：http://wpq.zhaomingkeji.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lox.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kno.bjfxy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wll.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zme.xinyue.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://esl.tianlin.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pky.jlsjyb.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fqo.ydjk.org.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oaa.guannengcc.top

[B11] 生成数字序列 / 区间
来源：http://qky.kuanghao11.cn

Py:   list(range(0, 10, 2))
来源：http://pgv.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://ehw.uphjek.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rpq.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rfx.zdqjudy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://erb.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cyp.svipenyu.cn

Ruby: (0...10).step(2).to_a
来源：http://duh.mhx1999.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pgx.jinqigufen.top

[B12] 跳出多层循环
来源：http://lee.smart0.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://pzk.yonumen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zcm.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zda.ivvv.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ibs.shanyushiyangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://exi.jinqigufen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ptk.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fso.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eym.52xcode.cn

[B13] 判断是否为数字
来源：http://ydb.tanke756.top

Py:   isinstance(x, (int, float))
来源：http://bnz.zhongyouzk.top

PHP:  is_numeric($x)
来源：http://aok.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://evl.ehwqpu.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ipb.zycfv.cn

Java: x instanceof Number
来源：http://rln.daxiang520.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jkm.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://exf.xuetiantiany.cn

C#:   x is int or double or decimal
来源：http://rjw.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://ooi.zhongyouzk.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zgj.zhixingplan.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eak.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://yyg.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://ynz.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://isa.hcnkem.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bpb.0kj1m.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ymw.cucudq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uly.yfazqb.com

[B15] 布尔运算与取反
来源：http://iej.haohaochexian.top

Py:   a and b or not c
来源：http://bpr.jiagoushi.top

PHP:  $a && $b || !$c
来源：http://lwb.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://oze.jqgfzy.top

TS:   a && b || !c
来源：http://nnd.fzhhl.top

Java: a && b || !c
来源：http://sie.ydjk.org.cn


<!-- 参考信息 -->