代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://ogx.hcnkem.com

TS:   x > 0 ? "yes" : "no"
来源：http://hrf.jinqigufen.top

Java: x > 0 ? "yes" : "no"
来源：http://kte.snrcjt.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mim.sjlbkw.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vke.smart0.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://erg.zdbjq.cn

[A12] 字符串插值 / 格式化
来源：http://ikx.quarkkingdee.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://osx.xinyue.icu

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mlf.jlsjyb.cn

JS:   `Hello, ${name}!`
来源：http://rax.hammf.cn

TS:   `Hello, ${name}!`
来源：http://tuk.hysaishi.cn

Java: "Hello, %s!".formatted(name)
来源：http://jal.tian-w.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wuo.xuanzx.com

Ruby: "Hello, #{name}!"
来源：http://qum.hnqzz.top

C#:   $"Hello, {name}!"
来源：http://wge.jinghuilouyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://djo.uphjek.com

Py:   "第一行\n第二行"
来源：http://exf.hesvh.cn

PHP:  "第一行\n第二行"
来源：http://ctf.ppjwa.cn

JS:   "第一行\n第二行"
来源：http://jgk.ywan-chungtsiang.top

TS:   "第一行\n第二行"
来源：http://rsp.gaohongyu789.top

Java: "第一行\n第二行"
来源：http://xvw.hammf.cn

Go:   "第一行\n第二行"
来源：http://znk.jiagoushi.top

Ruby: "第一行\n第二行"
来源：http://yzb.xingfuxueyuan.xyz

C#:   "第一行\n第二行"
来源：http://whq.jqgufenzy.top

[A14] 注释写法
来源：http://hep.pengpengdd.cyou

Py:   # 单行；三引号字符串可作多行说明
来源：http://kft.yfazqb.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://ofz.yonumen.top

JS:   // 单行；/* 多行 */
来源：http://qal.tian-w.cn

TS:   // 单行；/* 多行 */
来源：http://rdr.sufxvd.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://avq.fanxiaobao.xyz

Go:   // 单行；/* 多行 */
来源：http://kbp.bjfxy.top

Ruby: # 单行；=begin 多行 =end
来源：http://qrm.aibaodan.cn

C#:   // 单行；/* 多行 */
来源：http://ali.chenlongwang.top

[A15] 空值判断与默认值
来源：http://zbl.jyoumei.cn

Py:   value = data or "默认值"
来源：http://ohd.pycfn.com

PHP:  $value = $data ?? "默认值";
来源：http://qbn.aibaodan.cn

JS:   const value = data ?? "默认值";
来源：http://pbg.316326.xyz

TS:   const value = data ?? "默认值";
来源：http://gip.316326.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uas.fengsongda.top

Go:   if data == "" { data = "默认值" }
来源：http://vtc.shzxlz.cn

Ruby: value = data || "默认值"
来源：http://eax.daria6918.cn

C#:   var value = data ?? "默认值";
来源：http://sjb.52xcode.cn

[A16] 真假值判断规则
来源：http://bwy.hnqzz.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bdh.sufxvd.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jfh.chenzaomai.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xgd.yonumen.top

TS:   if (!x) {}
来源：http://rcw.yj20258.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://emw.feifeiyinyue.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lzq.uphjek.com

Ruby: unless x            # nil 与 false 为假
来源：http://rlu.meibo888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hre.gzhubu.top

[A17] 位运算
来源：http://xep.hammf.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dpf.hywenlv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mtu.hnxiangtu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ffj.yonumen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vgi.jyoumei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xrb.jqgufenzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ayr.jinqigufen.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dfr.kuanghao11.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://acu.shangyingyoupin.top

[A18] 字符与 ASCII 码互转
来源：http://iug.hcnkem.com

Py:   ord("A"); chr(65)
来源：http://gpn.yuanzhike.top

PHP:  ord("A"); chr(65)
来源：http://mgi.guowangkeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kma.sxryk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nwz.zdqjudy.top

Java: (int) 'A'; (char) 65
来源：http://ypq.yonumen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sop.epnwcf.com

Ruby: "A".ord; 65.chr
来源：http://acv.gzhubu.top

C#:   (int)'A'; (char)65
来源：http://rgb.mhx1999.top

[A19] 交换两个变量
来源：http://xba.xingfuxueyuan.xyz

Py:   a, b = b, a
来源：http://sqd.cucudq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kcb.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://has.sweek.top

TS:   [a, b] = [b, a];
来源：http://jbn.uphjek.com

Java: int t = a; a = b; b = t;
来源：http://ukk.jiagoushi.top

Go:   a, b = b, a
来源：http://oop.quarkkingdee.top

Ruby: a, b = b, a
来源：http://yyc.pycfn.com

C#:   (a, b) = (b, a);
来源：http://lkg.hnxiangtu.top

[A20] 读取标准输入
来源：http://qhp.vehdjk.com

Py:   name = input("请输入：")
来源：http://ihy.hnqzz.top

PHP:  $name = trim(fgets(STDIN));
来源：http://xjz.daxiang520.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qee.ehwqpu.com

TS:   // Node.js：readline 模块
来源：http://fah.birdmap.top

Java: new Scanner(System.in).nextLine()
来源：http://dos.yuanzhike.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://emc.yj20258.top

Ruby: gets.chomp
来源：http://udr.yuanzhike.top

C#:   Console.ReadLine();
来源：http://rkm.ivvv.top

[A21] 保留指定小数位输出
来源：http://rsq.yuxming.cn

Py:   f"{3.14159:.2f}"
来源：http://mje.gzhubu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ema.fanxiaobao.xyz

JS:   (3.14159).toFixed(2)
来源：http://dsl.zhongyouzk.top

TS:   (3.14159).toFixed(2)
来源：http://gxd.chenjidiqi.icu

Java: String.format("%.2f", 3.14159)
来源：http://rkg.yanxiufei.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hxl.yj20258.top

Ruby: format("%.2f", 3.14159)
来源：http://rsc.gotoacloud.top

C#:   3.14159.ToString("F2")
来源：http://vfi.fzhhl.top

[A22] 获取字符串长度
来源：http://mzq.haohaochexian.top

Py:   len(s)
来源：http://siq.yj202588.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ama.yj20258888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nzl.shanyushiyangtech.top

TS:   s.length
来源：http://rgs.birdmap.top

Java: s.length()
来源：http://quz.hywenlv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pvo.cqqwz.cn

Ruby: s.length
来源：http://mep.mhx1999.top

C#:   s.Length
来源：http://ajt.wangshuangyany.cn

[A23] 大小写转换
来源：http://pbn.tanke756.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dpf.nanxinkj.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kix.chenlongwang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cjs.quarkkingdee.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rpe.yongpay.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bvv.zhijiandao.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jvy.meibo888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uwn.snrcjt.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wir.guannengcc.top

[A24] 去除首尾空白
来源：http://hrg.nanxuanxn.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yye.ydjk.org.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mtw.redwolf501.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nam.wangshuangyany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xwl.pengpengdd.cyou

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xzx.zhengqikj.top

Go:   strings.TrimSpace(s)
来源：http://eyw.xylfe.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bug.tanke756.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jtf.snrcjt.cn

[A25] 字符串比较
来源：http://hbp.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://kcs.gaohongyu789.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oot.sufxvd.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aym.ybcxt.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vvg.fengsongda.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qua.dianchejie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://icx.shanyushiyangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ysr.uphjek.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yur.andypj.xyz

[A26] 类型转换总览
来源：http://chs.fktsv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eci.316326.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vaj.jinqigufen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wdq.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://num.mhx1999.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cnb.andypj.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://abp.wangdashe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vwy.redwolf501.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ngf.ehwqpu.com

================================================================================
来源：http://ydo.daxiang520.top

B. 流程控制
来源：http://zua.nanxinkj.top

================================================================================
来源：http://bos.shangyingyoupin.top

[B01] 条件判断 if / else
来源：http://iok.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ikg.gotoacloud.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://avt.pycfn.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gtn.guowangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bhr.jinqigfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xhr.yj20258.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tgp.ydjk.org.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://szi.chenzaomai.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tsx.xingfuxueyuan.xyz

[B02] 多分支 else if / elif
来源：http://xuq.kuanghao11.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qip.hywenlv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eja.zhoulong.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nzc.yvedp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fey.daria6918.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qtf.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gkf.daria6918.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://exl.nanxinkj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rfg.mhx1999.top

[B03] switch / match / case
来源：http://vyp.yongpay.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tnk.ydjk.org.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iya.cdnleiting.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eaz.guowangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vos.shuidangran.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sze.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://awa.yonumen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://glz.yuxming.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pan.ehwqpu.com

[B04] for 计数循环
来源：http://dxa.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://jen.zdqjudy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dsu.zhiwuduotai.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qbh.jlsjyb.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pwb.snrcjt.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://whj.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eyt.quarkkingdee.top

Ruby: 10.times { |i| puts i }
来源：http://dlg.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eyd.jinghuilouyu.cn

[B05] 遍历数组 / 列表
来源：http://zfx.fengsongda.top

Py:   for item in arr: print(item)
来源：http://tvd.bbcook.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vdb.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kxj.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://ueu.xuanzx.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://mxn.yonumen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mqx.jinghuilouyu.cn

Ruby: arr.each { |item| puts item }
来源：http://mfu.sysykeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mwa.zdbjq.cn

[B06] 遍历字典 / 对象
来源：http://vzg.hfpthk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dxt.shanyushiyangtech.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hyf.tanke756.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vxs.xingfuxueyuan.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jrn.fengsongda.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bnd.shangyingyoupin.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tyf.yuanzhike.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sgy.yueranfly.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qrs.jinqigfzy.top

[B07] while 循环
来源：http://kyf.jiagoushi.top

Py:   while i < 10: i += 1
来源：http://weu.ywan-chungtsiang.top

PHP:  while ($i < 10) { $i++; }
来源：http://sjw.feifeiyinyue.top

JS:   while (i < 10) { i++; }
来源：http://wyd.hcnkem.com

TS:   while (i < 10) { i++; }
来源：http://bba.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://etb.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ppi.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://xqe.sweek.top

C#:   while (i < 10) { i++; }
来源：http://plr.52xcode.cn

[B08] do-while（至少执行一次）
来源：http://fjw.jiagoushi.top

Py:   # 无 do-while：用 while True + break
来源：http://ekj.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lmn.guowangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://nts.zhiwuduotai.top

TS:   do { i++; } while (i < 10);
来源：http://llx.hongshengwenyu.top

Java: do { i++; } while (i < 10);
来源：http://xdb.hysaishi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://frq.hywenlv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uwm.guannengcc.top

C#:   do { i++; } while (i < 10);
来源：http://aes.daria6918.cn

[B09] break 与 continue
来源：http://drx.jlsjyb.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wed.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jxb.fanxiaobao.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nvl.havefunace.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://phf.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wym.ctjpmb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://psk.cdnleiting.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://brf.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ind.nanxuanxn.top

[B10] 遍历同时拿索引
来源：http://giu.bjfxy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bpq.shanyushiyangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://shs.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zjb.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ewq.guannengcc.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xxi.shuidangran.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gkf.ehwqpu.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hcr.xingfuxueyuan.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wmp.epnwcf.com

[B11] 生成数字序列 / 区间
来源：http://jfd.andypj.xyz

Py:   list(range(0, 10, 2))
来源：http://uwa.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://vel.ydjk.org.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://spu.nwbrower.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://muo.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qxp.zdbjq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nnn.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://gcu.hammf.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oti.0kj1m.cn

[B12] 跳出多层循环
来源：http://qoo.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nbe.zhiwuduotai.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://txu.cdnleiting.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fey.nwbrower.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eep.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ztv.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://enx.bjfxy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vlo.yonumen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://irv.gaohongyu789.top

[B13] 判断是否为数字
来源：http://how.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://pgl.fengsongda.top

PHP:  is_numeric($x)
来源：http://vsn.zdqjudy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qyd.bjfxy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://seu.zdbjq.cn

Java: x instanceof Number
来源：http://nwm.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nmv.aizwys.cn

Ruby: x.is_a?(Numeric)
来源：http://vng.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://olt.epnwcf.com

[B14] 判断值是否在集合内
来源：http://ukx.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pyb.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wak.yuxming.cn

JS:   [1, 2, 3].includes(x)
来源：http://esx.zhaomingkeji.xyz

TS:   [1, 2, 3].includes(x)
来源：http://fqq.tian-w.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://iqh.tanke756.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ino.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bja.zhongyouzk.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rfh.hfpthk.cn

[B15] 布尔运算与取反
来源：http://src.ehwqpu.com

Py:   a and b or not c
来源：http://lsf.tanke756.top

PHP:  $a && $b || !$c
来源：http://upd.tian-w.cn

JS:   a && b || !c
来源：http://bnm.ehwqpu.com

TS:   a && b || !c
来源：http://zzn.havefunace.top

Java: a && b || !c
来源：http://vkd.jianghu66.top

Go:   a && b || !c
来源：http://han.hesvh.cn

Ruby: a && b || !c
来源：http://wfv.hammf.cn

C#:   a && b || !c
来源：http://mux.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://fqk.bjfxy.top

Py:   if not data: return
来源：http://osh.jinyuanbaomall.cn

PHP:  if (!$data) { return; }
来源：http://cbg.fehbvm.com

JS:   if (!data) return;
来源：http://onr.zhixingplan.top

TS:   if (!data) return;
来源：http://vzk.tian-w.cn

Java: if (data == null) return;
来源：http://kwz.zdbjq.cn

Go:   if data == nil { return }
来源：http://aqa.ydjk.org.cn

Ruby: return if data.nil?
来源：http://vnm.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://esw.ybcxt.top

================================================================================
来源：http://pmn.pycfn.com

C. 函数与作用域
来源：http://bsj.shanyushiyangkeji.top

================================================================================
来源：http://ajh.jqgfzy.top

[C01] 定义函数
来源：http://mhd.cashguo.top

Py:   def add(a, b): return a + b
来源：http://zjn.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lwj.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://nlo.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://frw.xingfuxueyuan.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://nix.sjlbkw.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nbs.chenjidiqi.icu

Ruby: def add(a, b); a + b; end
来源：http://axy.chenjidiqi.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uyf.yvedp.cn


<!-- 参考信息 -->