代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gqa.daxiang520.top

Java: new Random().nextInt(100) + 1
来源：http://hsc.zhijiandao.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://igw.uphjek.com

Ruby: rand(1..100)
来源：http://avm.hysaishi.cn

C#:   new Random().Next(1, 101)
来源：http://fnz.xingfuxueyuan.xyz

[A11] 条件表达式（三元）
来源：http://kwo.9152youxi.cn

Py:   "yes" if x > 0 else "no"
来源：http://qah.9152youxi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rrw.xuetiantiany.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tct.fanxiaobao.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://mhw.wangshuangyany.cn

Java: x > 0 ? "yes" : "no"
来源：http://uqk.jinqigufen.top

Go:   // 无三元运算符，需用 if 语句
来源：http://sve.shuidangran.top

Ruby: x > 0 ? "yes" : "no"
来源：http://byh.ydjk.org.cn

C#:   x > 0 ? "yes" : "no"
来源：http://imv.zhixingplan.top

[A12] 字符串插值 / 格式化
来源：http://xly.zhijiandao.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fvw.fzhhl.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qfn.ydjk.org.cn

JS:   `Hello, ${name}!`
来源：http://ywj.0kj1m.cn

TS:   `Hello, ${name}!`
来源：http://pgo.zhiwuduotai.top

Java: "Hello, %s!".formatted(name)
来源：http://zwq.9152youxi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rmk.jinqigufen.top

Ruby: "Hello, #{name}!"
来源：http://mur.meibo888.top

C#:   $"Hello, {name}!"
来源：http://pua.snrcjt.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vut.ctjpmb.com

Py:   "第一行\n第二行"
来源：http://yra.hesvh.cn

PHP:  "第一行\n第二行"
来源：http://agm.zhijiandao.cn

JS:   "第一行\n第二行"
来源：http://dsz.wangshuangyany.cn

TS:   "第一行\n第二行"
来源：http://dut.shuidangran.top

Java: "第一行\n第二行"
来源：http://eet.yj20258.top

Go:   "第一行\n第二行"
来源：http://jkx.bjfxy.top

Ruby: "第一行\n第二行"
来源：http://fbe.xuetiantiany.cn

C#:   "第一行\n第二行"
来源：http://wio.316326.xyz

[A14] 注释写法
来源：http://sfi.hcnkem.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://knx.kuanghao11.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://iar.hnxiangtu.top

JS:   // 单行；/* 多行 */
来源：http://ura.sjlbkw.cn

TS:   // 单行；/* 多行 */
来源：http://wvv.shuidangran.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://unk.smart0.xyz

Go:   // 单行；/* 多行 */
来源：http://ljs.hnqzz.top

Ruby: # 单行；=begin 多行 =end
来源：http://kre.tanke756.top

C#:   // 单行；/* 多行 */
来源：http://kmv.xuanzx.com

[A15] 空值判断与默认值
来源：http://ufx.yueranfly.top

Py:   value = data or "默认值"
来源：http://csb.xylfe.cn

PHP:  $value = $data ?? "默认值";
来源：http://mhd.yuanzhike.top

JS:   const value = data ?? "默认值";
来源：http://pnb.cqqwz.cn

TS:   const value = data ?? "默认值";
来源：http://ajg.52xcode.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dxz.hammf.cn

Go:   if data == "" { data = "默认值" }
来源：http://ioy.uphjek.com

Ruby: value = data || "默认值"
来源：http://pkb.ehwqpu.com

C#:   var value = data ?? "默认值";
来源：http://luj.haohaochexian.top

[A16] 真假值判断规则
来源：http://xzf.zhixingplan.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oxg.dianchejie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wju.birdmap.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xdu.zdbjq.cn

TS:   if (!x) {}
来源：http://bml.hnqzz.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://opu.shangyingyoupin.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ywb.redwolf501.top

Ruby: unless x            # nil 与 false 为假
来源：http://dln.meibo888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xta.gogol.net.cn

[A17] 位运算
来源：http://ujl.sysykeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wdv.tanke756.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ivr.316326.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tic.yonumen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oga.aizwys.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ict.zhaomingkeji.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vhy.hongshengwenyu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://loa.jiagoushi.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jdp.mhx1999.top

[A18] 字符与 ASCII 码互转
来源：http://fpi.gotoacloud.top

Py:   ord("A"); chr(65)
来源：http://kmi.bbcook.cn

PHP:  ord("A"); chr(65)
来源：http://uhm.jlsjyb.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wdh.feifeiyinyue.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sdj.hnqzz.top

Java: (int) 'A'; (char) 65
来源：http://hmv.iojbl.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wly.havefunace.top

Ruby: "A".ord; 65.chr
来源：http://coo.tanke756.top

C#:   (int)'A'; (char)65
来源：http://fph.fktsv.cn

[A19] 交换两个变量
来源：http://dsm.fanxiaobao.xyz

Py:   a, b = b, a
来源：http://tei.hnxiangtu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://rlr.guowangkeji.top

JS:   [a, b] = [b, a];
来源：http://fjr.quarkkingdee.top

TS:   [a, b] = [b, a];
来源：http://gba.xuanzx.com

Java: int t = a; a = b; b = t;
来源：http://tgg.guannengcc.top

Go:   a, b = b, a
来源：http://eli.zhongyouzk.top

Ruby: a, b = b, a
来源：http://kid.daxiang520.top

C#:   (a, b) = (b, a);
来源：http://wxa.9152youxi.cn

[A20] 读取标准输入
来源：http://dao.cucudq.cn

Py:   name = input("请输入：")
来源：http://qlq.fengsongda.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wac.kuanghao11.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ick.mhx1999.top

TS:   // Node.js：readline 模块
来源：http://trc.fzhhl.top

Java: new Scanner(System.in).nextLine()
来源：http://lzp.shanyushiyangtech.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wzj.hfpthk.cn

Ruby: gets.chomp
来源：http://lnv.sweek.top

C#:   Console.ReadLine();
来源：http://ogu.xuanzx.com

[A21] 保留指定小数位输出
来源：http://zvg.quarkkingdee.top

Py:   f"{3.14159:.2f}"
来源：http://mxq.yj202588.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://irb.ehwqpu.com

JS:   (3.14159).toFixed(2)
来源：http://ddy.sweek.top

TS:   (3.14159).toFixed(2)
来源：http://gja.jiagoushi.top

Java: String.format("%.2f", 3.14159)
来源：http://kaf.hfpthk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mum.yueranfly.top

Ruby: format("%.2f", 3.14159)
来源：http://mrs.feifeiyinyue.top

C#:   3.14159.ToString("F2")
来源：http://juz.jqgufenzy.top

[A22] 获取字符串长度
来源：http://cmf.smart0.xyz

Py:   len(s)
来源：http://usw.hcnkem.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rjd.gogol.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vfe.chenzaomai.com

TS:   s.length
来源：http://lyc.shanyushiyangtech.top

Java: s.length()
来源：http://rhs.ydzc1.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bsx.zhixingplan.top

Ruby: s.length
来源：http://idd.gotoacloud.top

C#:   s.Length
来源：http://nqh.cdnleiting.top

[A23] 大小写转换
来源：http://ssj.svipenyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://moi.yongpay.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ane.snrcjt.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://maq.hesvh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jmw.aibaodan.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dep.c1oappe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ksl.zhengqikj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hcl.xingfuxueyuan.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://wko.gaohongyu789.top

[A24] 去除首尾空白
来源：http://egj.cheryme.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xvh.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://psj.fanxiaobao.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cpl.cdnleiting.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tvm.daria6918.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vag.xuanzx.com

Go:   strings.TrimSpace(s)
来源：http://buz.epnwcf.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qyn.pycfn.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fat.ehwqpu.com

[A25] 字符串比较
来源：http://xbh.ydzc1.top

Py:   s1 == s2; s1 != s2
来源：http://ofg.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fbg.fzhhl.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ljs.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://khz.zhoulong.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pdw.316326.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iyz.chenzaomai.com

Ruby: s1 == s2; s1 <=> s2
来源：http://kcr.hnxiangtu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://erq.nanxuanxn.top

[A26] 类型转换总览
来源：http://wgs.havefunace.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ocz.jyoumei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tbk.sjlbkw.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://htu.zhoulong.xyz

TS:   Number() String() Boolean() x as number
来源：http://qcr.smart0.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zef.xziqi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vfe.gzhubu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ahk.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ihn.shangyingyoupin.top

================================================================================
来源：http://myt.guowangkeji.top

B. 流程控制
来源：http://qrb.cheryme.top

================================================================================
来源：http://ayz.cucudq.cn

[B01] 条件判断 if / else
来源：http://mvk.bjfxy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qdx.yj20258888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mib.52xcode.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bel.jlsjyb.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jxy.jinyuanbaomall.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uod.xinyue.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lam.sweek.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aac.ivvv.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gss.jinqigufen.top

[B02] 多分支 else if / elif
来源：http://rpj.uphjek.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ook.zhaomingkeji.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uoh.jinqigfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zep.yj20258888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ltu.zhoulong.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://llk.jlsjyb.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qlv.jqgufenzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fhb.ppjwa.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rak.smart0.xyz

[B03] switch / match / case
来源：http://qcp.birdmap.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xbe.hesvh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rlw.hywenlv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pqw.xuetiantiany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hzh.52xcode.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://szl.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lmi.yangfankeji.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kof.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ijx.cqqwz.cn

[B04] for 计数循环
来源：http://zee.vqdsnc.cn

Py:   for i in range(10): print(i)
来源：http://wec.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gmd.shzxlz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tps.xuanzx.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ynj.sweek.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://caj.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rph.jqgfzy.top

Ruby: 10.times { |i| puts i }
来源：http://ysj.hammf.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hho.hnxiangtu.top

[B05] 遍历数组 / 列表
来源：http://zdn.nanxuanxn.top

Py:   for item in arr: print(item)
来源：http://fkw.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wwj.mhx1999.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yvk.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://pqb.pycfn.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://dav.sweek.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mwt.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://peq.bbcook.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://whb.hammf.cn

[B06] 遍历字典 / 对象
来源：http://qwf.bbcook.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oaa.hesvh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ggg.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://srf.dianchejie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dvr.haohaochexian.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tmn.iojbl.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lqg.xingfuxueyuan.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rry.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fgy.yj20258888.top

[B07] while 循环
来源：http://kzc.tianlin.xyz

Py:   while i < 10: i += 1
来源：http://ejs.guowangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://cjy.feifeiyinyue.top

JS:   while (i < 10) { i++; }
来源：http://uql.wangdashe.top

TS:   while (i < 10) { i++; }
来源：http://ovl.guowangkeji.top

Java: while (i < 10) { i++; }
来源：http://hme.wangdashe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fhi.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://tmt.hongshengwenyu.top

C#:   while (i < 10) { i++; }
来源：http://jhg.jqgufenzy.top

[B08] do-while（至少执行一次）
来源：http://gqd.xziqi.cn

Py:   # 无 do-while：用 while True + break
来源：http://xyq.hysaishi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hgb.cqqwz.cn

JS:   do { i++; } while (i < 10);
来源：http://smi.yonumen.top

TS:   do { i++; } while (i < 10);
来源：http://zbl.uphjek.com

Java: do { i++; } while (i < 10);
来源：http://xnj.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xou.ydjk.org.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dzp.yuxming.cn

C#:   do { i++; } while (i < 10);
来源：http://saz.xylfe.cn

[B09] break 与 continue
来源：http://mon.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cmg.pycfn.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fjp.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vrp.jinghuilouyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bsj.uphjek.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://buy.xylfe.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wcw.jinqigfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://olj.guannengcc.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pxo.daxiang520.top

[B10] 遍历同时拿索引
来源：http://nir.fengsongda.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qhq.redwolf501.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fdy.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vra.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ata.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lbw.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bxi.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pme.yuanzhike.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yxf.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://art.cashguo.top

Py:   list(range(0, 10, 2))
来源：http://sti.shangyingyoupin.top

PHP:  range(0, 10, 2);
来源：http://phh.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://omy.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zwl.chenlongwang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cdx.yj20258888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://krt.birdmap.top

Ruby: (0...10).step(2).to_a
来源：http://ooh.aibaodan.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gpn.cheryme.top

[B12] 跳出多层循环
来源：http://dmu.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://agu.ybcxt.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://heu.yj20258.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pas.zhixingplan.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ozj.smart0.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://goo.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cvr.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zyg.kuanghao11.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kum.snrcjt.cn

[B13] 判断是否为数字
来源：http://zar.jiagoushi.top

Py:   isinstance(x, (int, float))
来源：http://cxz.gotoacloud.top

PHP:  is_numeric($x)
来源：http://dsy.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jjr.cucudq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fzd.jqgfzy.top

Java: x instanceof Number
来源：http://gjt.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ckn.nanxinkj.top

Ruby: x.is_a?(Numeric)
来源：http://lzx.jlsjyb.cn

C#:   x is int or double or decimal
来源：http://nku.bjfxy.top

[B14] 判断值是否在集合内
来源：http://jpp.9152youxi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rpc.zhijiandao.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vby.fengsongda.top

JS:   [1, 2, 3].includes(x)
来源：http://qcd.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://ubm.nwbrower.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rdy.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dus.wangshuangyany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kwb.yj202588.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bwy.aibaodan.cn

[B15] 布尔运算与取反
来源：http://xaz.xuanzx.com

Py:   a and b or not c
来源：http://xpl.zhijiandao.cn

PHP:  $a && $b || !$c
来源：http://zny.yuanzhike.top

JS:   a && b || !c
来源：http://qgw.yongpay.top

TS:   a && b || !c
来源：http://qke.dianchejie.cn

Java: a && b || !c
来源：http://nag.shzxlz.cn

Go:   a && b || !c
来源：http://dwf.zhoulong.xyz

Ruby: a && b || !c
来源：http://xek.svipenyu.cn

C#:   a && b || !c
来源：http://dmu.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ibk.yueranfly.top

Py:   if not data: return
来源：http://ygn.ydzc1.top

PHP:  if (!$data) { return; }
来源：http://frp.mhx1999.top

JS:   if (!data) return;
来源：http://cdd.tanke756.top

TS:   if (!data) return;
来源：http://gtz.9152youxi.cn

Java: if (data == null) return;
来源：http://zpu.chenjidiqi.icu

Go:   if data == nil { return }
来源：http://hzi.hnqzz.top

Ruby: return if data.nil?
来源：http://psn.bjfxy.top

C#:   if (data == null) return;
来源：http://fdc.guowangkeji.top

================================================================================
来源：http://mjb.hywenlv.cn

C. 函数与作用域
来源：http://rjz.meibo888.top

================================================================================
来源：http://oxb.tianlin.xyz

[C01] 定义函数
来源：http://lfq.smart0.xyz


<!-- 参考信息 -->