代发 wailian999

[A10] 生成随机数
来源：http://zwh.yanxiufei.cn

Py:   import random; random.randint(1, 100)
来源：http://kbc.yj202588.top

PHP:  random_int(1, 100);
来源：http://ovd.fanxiaobao.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kez.ywan-chungtsiang.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://grj.daria6918.cn

Java: new Random().nextInt(100) + 1
来源：http://ezx.fengsongda.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dep.chenzaomai.com

Ruby: rand(1..100)
来源：http://qjj.316326.xyz

C#:   new Random().Next(1, 101)
来源：http://teg.yuxming.cn

[A11] 条件表达式（三元）
来源：http://eob.chenjidiqi.icu

Py:   "yes" if x > 0 else "no"
来源：http://xub.sweek.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://dfv.svipenyu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cpe.ppjwa.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pqc.ctjpmb.com

Java: x > 0 ? "yes" : "no"
来源：http://dpg.yj202588.top

Go:   // 无三元运算符，需用 if 语句
来源：http://vrg.jqgfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://wpl.gzhubu.top

C#:   x > 0 ? "yes" : "no"
来源：http://rwj.jinqigufen.top

[A12] 字符串插值 / 格式化
来源：http://tjj.snrcjt.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qcl.ydzc1.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wrb.hongshengwenyu.top

JS:   `Hello, ${name}!`
来源：http://dmj.ivvv.top

TS:   `Hello, ${name}!`
来源：http://cfi.zhiwuduotai.top

Java: "Hello, %s!".formatted(name)
来源：http://nag.meibo888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://alm.tarul.cn

Ruby: "Hello, #{name}!"
来源：http://dnw.tanke756.top

C#:   $"Hello, {name}!"
来源：http://ras.gotoacloud.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dvn.xziqi.cn

Py:   "第一行\n第二行"
来源：http://wsh.cqqwz.cn

PHP:  "第一行\n第二行"
来源：http://wle.zhaomingkeji.xyz

JS:   "第一行\n第二行"
来源：http://uqi.sjlbkw.cn

TS:   "第一行\n第二行"
来源：http://swn.gogol.net.cn

Java: "第一行\n第二行"
来源：http://xdm.ydjk.org.cn

Go:   "第一行\n第二行"
来源：http://tfs.guannengcc.top

Ruby: "第一行\n第二行"
来源：http://jjk.zdbjq.cn

C#:   "第一行\n第二行"
来源：http://gjg.quarkkingdee.top

[A14] 注释写法
来源：http://zmt.shanyushiyangtech.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qot.dashuyun.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hng.52xcode.cn

JS:   // 单行；/* 多行 */
来源：http://pse.yongpay.top

TS:   // 单行；/* 多行 */
来源：http://oui.jyoumei.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pke.hcnkem.com

Go:   // 单行；/* 多行 */
来源：http://vjg.hysaishi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mqk.ywan-chungtsiang.top

C#:   // 单行；/* 多行 */
来源：http://ccd.zdbjq.cn

[A15] 空值判断与默认值
来源：http://pry.ppjwa.cn

Py:   value = data or "默认值"
来源：http://gss.gzhubu.top

PHP:  $value = $data ?? "默认值";
来源：http://nxi.fanxiaobao.xyz

JS:   const value = data ?? "默认值";
来源：http://wuw.jinqigfzy.top

TS:   const value = data ?? "默认值";
来源：http://nxn.fengsongda.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fet.xuetiantiany.cn

Go:   if data == "" { data = "默认值" }
来源：http://vff.smart0.xyz

Ruby: value = data || "默认值"
来源：http://jue.sjlbkw.cn

C#:   var value = data ?? "默认值";
来源：http://bmf.bjfxy.top

[A16] 真假值判断规则
来源：http://qty.yvedp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://puo.yuanzhike.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zvk.gogol.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xfp.nanxinkj.top

TS:   if (!x) {}
来源：http://ler.sjlbkw.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uyi.cqqwz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tbx.tanke756.top

Ruby: unless x            # nil 与 false 为假
来源：http://pvv.snrcjt.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hkm.316326.xyz

[A17] 位运算
来源：http://tob.jqgufenzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lsu.zycfv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bnn.ivvv.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xwh.wangshuangyany.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bjj.sjlbkw.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nuu.bbcook.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nbz.hnxiangtu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bzo.gaohongyu789.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hbt.yuanzhike.top

[A18] 字符与 ASCII 码互转
来源：http://kcw.xuetiantiany.cn

Py:   ord("A"); chr(65)
来源：http://xus.shangyingyoupin.top

PHP:  ord("A"); chr(65)
来源：http://jso.yonumen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tsg.fktsv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kpg.cashguo.top

Java: (int) 'A'; (char) 65
来源：http://hwq.fzhhl.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sbp.xingfuxueyuan.xyz

Ruby: "A".ord; 65.chr
来源：http://eyh.dianchejie.cn

C#:   (int)'A'; (char)65
来源：http://ztn.zycfv.cn

[A19] 交换两个变量
来源：http://wfu.ivvv.top

Py:   a, b = b, a
来源：http://pwv.zhijiandao.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ogt.yuxming.cn

JS:   [a, b] = [b, a];
来源：http://gbq.xingfuxueyuan.xyz

TS:   [a, b] = [b, a];
来源：http://qgd.jqgfzy.top

Java: int t = a; a = b; b = t;
来源：http://uwf.316326.xyz

Go:   a, b = b, a
来源：http://vwy.gotoacloud.top

Ruby: a, b = b, a
来源：http://wcd.9152youxi.cn

C#:   (a, b) = (b, a);
来源：http://xyy.kuanghao11.cn

[A20] 读取标准输入
来源：http://dfu.daria6918.cn

Py:   name = input("请输入：")
来源：http://jfu.jiagoushi.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bzs.hnqzz.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vrc.bjfxy.top

TS:   // Node.js：readline 模块
来源：http://pfb.kuanghao11.cn

Java: new Scanner(System.in).nextLine()
来源：http://ebi.zhiwuduotai.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zbk.zhijiandao.cn

Ruby: gets.chomp
来源：http://epg.shanyushiyangtech.top

C#:   Console.ReadLine();
来源：http://zrl.xuanzx.com

[A21] 保留指定小数位输出
来源：http://rdi.guowangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://eeq.fanxiaobao.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zya.xziqi.cn

JS:   (3.14159).toFixed(2)
来源：http://wjw.gzhubu.top

TS:   (3.14159).toFixed(2)
来源：http://tkj.iojbl.cn

Java: String.format("%.2f", 3.14159)
来源：http://psf.zhongyouzk.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dly.cheryme.top

Ruby: format("%.2f", 3.14159)
来源：http://oaw.zhixingplan.top

C#:   3.14159.ToString("F2")
来源：http://ikp.guowangkeji.top

[A22] 获取字符串长度
来源：http://ria.ehwqpu.com

Py:   len(s)
来源：http://fnt.wangshuangyany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kxy.jqgfzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eyc.hesvh.cn

TS:   s.length
来源：http://uja.jqgufenzy.top

Java: s.length()
来源：http://irz.pycfn.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xec.yj202588.top

Ruby: s.length
来源：http://eom.cashguo.top

C#:   s.Length
来源：http://fro.zhongyouzk.top

[A23] 大小写转换
来源：http://dpe.jiagoushi.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xau.kuanghao11.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rxv.jqgfzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fmz.ywan-chungtsiang.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rbv.52xcode.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hhr.snrcjt.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ngl.zhongyouzk.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://syj.jinqigufen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://weg.fengsongda.top

[A24] 去除首尾空白
来源：http://mhc.uphjek.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hor.jinqigfzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vjp.havefunace.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hkr.dashuyun.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hve.yongpay.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ilv.sweek.top

Go:   strings.TrimSpace(s)
来源：http://xpm.yuxming.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rwu.fanxiaobao.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tbf.uphjek.com

[A25] 字符串比较
来源：http://xnv.zdqjudy.top

Py:   s1 == s2; s1 != s2
来源：http://zms.c1oappe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qwe.xuanzx.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mnb.ppjwa.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eji.yuxming.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jza.fktsv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wiu.kuanghao11.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pcy.gotoacloud.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iak.yonumen.top

[A26] 类型转换总览
来源：http://epn.ydjk.org.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://psx.c1oappe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://edd.fehbvm.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ioj.cdnleiting.top

TS:   Number() String() Boolean() x as number
来源：http://xeb.cucudq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bre.fktsv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xft.cdnleiting.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://szr.hywenlv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://irv.cqqwz.cn

================================================================================
来源：http://ttk.zhoulong.xyz

B. 流程控制
来源：http://hhn.fanxiaobao.xyz

================================================================================
来源：http://zoe.xinyue.icu

[B01] 条件判断 if / else
来源：http://aqa.bjfxy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fhq.cheryme.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://njd.fengsongda.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qum.yuanzhike.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kkj.52xcode.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gsy.zhixingplan.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dge.hnxiangtu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qhs.shanyushiyangtech.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://udl.xuanzx.com

[B02] 多分支 else if / elif
来源：http://cyx.nanxinkj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xsl.jqgufenzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ecp.zhongyouzk.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://slj.zycfv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mbr.cucudq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zaa.ybcxt.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bat.yuanzhike.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rjg.sysykeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ivt.cucudq.cn

[B03] switch / match / case
来源：http://ptg.yvedp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wti.sysykeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lbe.cheryme.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mjz.tarul.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yic.hammf.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tee.yj20258888.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gfw.epnwcf.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ewl.shzxlz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pbs.ehwqpu.com

[B04] for 计数循环
来源：http://sev.yuxming.cn

Py:   for i in range(10): print(i)
来源：http://iti.mhx1999.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qie.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://laa.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ovw.ctjpmb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zue.fktsv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jto.aizwys.cn

Ruby: 10.times { |i| puts i }
来源：http://joh.nanxinkj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ist.ivvv.top

[B05] 遍历数组 / 列表
来源：http://gtn.chenjidiqi.icu

Py:   for item in arr: print(item)
来源：http://xht.daria6918.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fsc.ybcxt.top

JS:   for (const item of arr) { console.log(item); }
来源：http://num.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ziy.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://wpk.svipenyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pmw.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://pdj.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xfb.aizwys.cn

[B06] 遍历字典 / 对象
来源：http://zra.zhoulong.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://jkw.nanxuanxn.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gfs.gaohongyu789.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kcg.cashguo.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jmm.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ibn.dianchejie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xts.jinqigfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qki.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zoq.ydjk.org.cn

[B07] while 循环
来源：http://ywi.jinqigufen.top

Py:   while i < 10: i += 1
来源：http://nuk.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mik.shzxlz.cn

JS:   while (i < 10) { i++; }
来源：http://wpz.hongshengwenyu.top

TS:   while (i < 10) { i++; }
来源：http://xoj.yfazqb.com

Java: while (i < 10) { i++; }
来源：http://plm.ydjk.org.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kvz.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://aqk.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://kjk.jinghuilouyu.cn

[B08] do-while（至少执行一次）
来源：http://ifx.aizwys.cn

Py:   # 无 do-while：用 while True + break
来源：http://fbv.tanke756.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ccz.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://voe.hywenlv.cn

TS:   do { i++; } while (i < 10);
来源：http://cyd.ehwqpu.com

Java: do { i++; } while (i < 10);
来源：http://zpz.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hkd.snrcjt.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xhf.xuetiantiany.cn

C#:   do { i++; } while (i < 10);
来源：http://vpj.hywenlv.cn

[B09] break 与 continue
来源：http://kuz.daria6918.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tom.jinqigufen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qzn.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dbn.zdqjudy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vom.hesvh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uko.hysaishi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://llk.vehdjk.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ixz.chenzaomai.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ngc.gotoacloud.top

[B10] 遍历同时拿索引
来源：http://cgf.uphjek.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zsi.sjlbkw.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://myn.jqgufenzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zsv.hfpthk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hyb.wangdashe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ssy.sysykeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oiv.guowangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kum.gaohongyu789.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blw.meibo888.top

[B11] 生成数字序列 / 区间
来源：http://bah.guannengcc.top

Py:   list(range(0, 10, 2))
来源：http://kgb.yuanzhike.top

PHP:  range(0, 10, 2);
来源：http://duy.bjfxy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lnh.hammf.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gcb.feifeiyinyue.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ldf.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rqs.zhongyouzk.top

Ruby: (0...10).step(2).to_a
来源：http://oev.yvedp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qkr.epnwcf.com

[B12] 跳出多层循环
来源：http://lky.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kbm.0kj1m.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qrl.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sqh.yonumen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oyu.fengsongda.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://trf.hnqzz.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kjf.zhaomingkeji.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qok.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hpl.smart0.xyz

[B13] 判断是否为数字
来源：http://hwv.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://cxy.vehdjk.com

PHP:  is_numeric($x)
来源：http://vyk.kuanghao11.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aik.zhoulong.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aku.meibo888.top

Java: x instanceof Number
来源：http://wwg.redwolf501.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kcr.cqqwz.cn

Ruby: x.is_a?(Numeric)
来源：http://whq.chenlongwang.top

C#:   x is int or double or decimal
来源：http://wzz.chenjidiqi.icu

[B14] 判断值是否在集合内
来源：http://ssu.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ful.vqdsnc.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://izr.tianlin.xyz

JS:   [1, 2, 3].includes(x)
来源：http://ypq.zhongyouzk.top

TS:   [1, 2, 3].includes(x)
来源：http://yfk.andypj.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://wbc.gotoacloud.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bfp.svipenyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mos.chenlongwang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://biy.yj202588.top

[B15] 布尔运算与取反
来源：http://gzq.wangshuangyany.cn

Py:   a and b or not c
来源：http://rgp.hammf.cn

PHP:  $a && $b || !$c
来源：http://zef.cashguo.top

JS:   a && b || !c
来源：http://mcp.c1oappe.top

TS:   a && b || !c
来源：http://xlb.xziqi.cn

Java: a && b || !c
来源：http://kjt.nanxinkj.top

Go:   a && b || !c
来源：http://okj.andypj.xyz

Ruby: a && b || !c
来源：http://jbz.smart0.xyz

C#:   a && b || !c
来源：http://zgc.shanyushiyangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://xae.wangshuangyany.cn

Py:   if not data: return
来源：http://ldp.yvedp.cn

PHP:  if (!$data) { return; }
来源：http://ixj.kuanghao11.cn

JS:   if (!data) return;
来源：http://ppv.nwbrower.top

TS:   if (!data) return;
来源：http://kwp.jinghuilouyu.cn

Java: if (data == null) return;
来源：http://dvy.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://wzx.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://kfd.birdmap.top

C#:   if (data == null) return;
来源：http://abx.shzxlz.cn


<!-- 参考信息 -->