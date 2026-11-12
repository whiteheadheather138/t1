代发 wailian999

[A10] 生成随机数
来源：http://ocs.zycfv.cn

Py:   import random; random.randint(1, 100)
来源：http://brn.tanke756.top

PHP:  random_int(1, 100);
来源：http://egl.pycfn.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fzc.xylfe.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bnf.feifeiyinyue.top

Java: new Random().nextInt(100) + 1
来源：http://dmz.feifeiyinyue.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zug.daria6918.cn

Ruby: rand(1..100)
来源：http://bpp.aizwys.cn

C#:   new Random().Next(1, 101)
来源：http://pez.52xcode.cn

[A11] 条件表达式（三元）
来源：http://wpr.yonumen.top

Py:   "yes" if x > 0 else "no"
来源：http://kos.pycfn.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://bdy.yuxming.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bue.yongpay.top

TS:   x > 0 ? "yes" : "no"
来源：http://pjm.tian-w.cn

Java: x > 0 ? "yes" : "no"
来源：http://jto.ivvv.top

Go:   // 无三元运算符，需用 if 语句
来源：http://uzu.gzhubu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://oxy.zhixingplan.top

C#:   x > 0 ? "yes" : "no"
来源：http://ycp.havefunace.top

[A12] 字符串插值 / 格式化
来源：http://dfp.chenjidiqi.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://iff.jqgufenzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sdu.guannengcc.top

JS:   `Hello, ${name}!`
来源：http://ziw.bbcook.cn

TS:   `Hello, ${name}!`
来源：http://vcv.nanxuanxn.top

Java: "Hello, %s!".formatted(name)
来源：http://vqa.tian-w.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jkp.zdbjq.cn

Ruby: "Hello, #{name}!"
来源：http://kzh.shuidangran.top

C#:   $"Hello, {name}!"
来源：http://qsz.guowangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ocj.wangshuangyany.cn

Py:   "第一行\n第二行"
来源：http://swl.shzxlz.cn

PHP:  "第一行\n第二行"
来源：http://kvy.jyoumei.cn

JS:   "第一行\n第二行"
来源：http://ykh.fanxiaobao.xyz

TS:   "第一行\n第二行"
来源：http://gbs.zhijiandao.cn

Java: "第一行\n第二行"
来源：http://gdj.hcnkem.com

Go:   "第一行\n第二行"
来源：http://ula.ydjk.org.cn

Ruby: "第一行\n第二行"
来源：http://rhv.yvedp.cn

C#:   "第一行\n第二行"
来源：http://enk.jinqigfzy.top

[A14] 注释写法
来源：http://cvq.hnqzz.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://pum.316326.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://ioa.wangdashe.top

JS:   // 单行；/* 多行 */
来源：http://rts.sxryk.cn

TS:   // 单行；/* 多行 */
来源：http://mhc.svipenyu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://taz.hnxiangtu.top

Go:   // 单行；/* 多行 */
来源：http://cyf.tanke756.top

Ruby: # 单行；=begin 多行 =end
来源：http://psk.yongpay.top

C#:   // 单行；/* 多行 */
来源：http://oak.svipenyu.cn

[A15] 空值判断与默认值
来源：http://dsf.jqgfzy.top

Py:   value = data or "默认值"
来源：http://wib.wangdashe.top

PHP:  $value = $data ?? "默认值";
来源：http://wfs.yueranfly.top

JS:   const value = data ?? "默认值";
来源：http://tni.shangyingyoupin.top

TS:   const value = data ?? "默认值";
来源：http://bfp.epnwcf.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://big.dashuyun.cn

Go:   if data == "" { data = "默认值" }
来源：http://ylk.shuidangran.top

Ruby: value = data || "默认值"
来源：http://vyw.epnwcf.com

C#:   var value = data ?? "默认值";
来源：http://ivj.shanyushiyangkeji.top

[A16] 真假值判断规则
来源：http://whu.jianghu66.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hja.tianlin.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zjk.haohaochexian.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uyv.zhixingplan.top

TS:   if (!x) {}
来源：http://pnx.yj202588.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jdz.epnwcf.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jen.vqdsnc.cn

Ruby: unless x            # nil 与 false 为假
来源：http://onb.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yjj.vqdsnc.cn

[A17] 位运算
来源：http://vlj.gaohongyu789.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dsl.aizwys.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cnz.feifeiyinyue.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bon.yangfankeji.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://obu.tarul.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rhv.vehdjk.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rnz.ydzc1.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://etn.shanyushiyangkeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rxl.jyoumei.cn

[A18] 字符与 ASCII 码互转
来源：http://ben.yj202588.top

Py:   ord("A"); chr(65)
来源：http://cqm.gaohongyu789.top

PHP:  ord("A"); chr(65)
来源：http://kkr.sufxvd.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dgm.0kj1m.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ixw.sxryk.cn

Java: (int) 'A'; (char) 65
来源：http://icf.birdmap.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qxf.hcnkem.com

Ruby: "A".ord; 65.chr
来源：http://wxp.yj20258888.top

C#:   (int)'A'; (char)65
来源：http://dzu.chenzaomai.com

[A19] 交换两个变量
来源：http://tks.nwbrower.top

Py:   a, b = b, a
来源：http://vzw.nwbrower.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xjq.hnqzz.top

JS:   [a, b] = [b, a];
来源：http://ble.ydjk.org.cn

TS:   [a, b] = [b, a];
来源：http://hev.ydjk.org.cn

Java: int t = a; a = b; b = t;
来源：http://xrh.meibo888.top

Go:   a, b = b, a
来源：http://vqe.zhijiandao.cn

Ruby: a, b = b, a
来源：http://taq.fzhhl.top

C#:   (a, b) = (b, a);
来源：http://ofv.gzhubu.top

[A20] 读取标准输入
来源：http://yst.yonumen.top

Py:   name = input("请输入：")
来源：http://rpv.hcnkem.com

PHP:  $name = trim(fgets(STDIN));
来源：http://adj.chenlongwang.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gck.uphjek.com

TS:   // Node.js：readline 模块
来源：http://fun.gaohongyu789.top

Java: new Scanner(System.in).nextLine()
来源：http://xzu.zhengqikj.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ulh.ctjpmb.com

Ruby: gets.chomp
来源：http://qkq.vqdsnc.cn

C#:   Console.ReadLine();
来源：http://lhl.shzxlz.cn

[A21] 保留指定小数位输出
来源：http://pwn.vehdjk.com

Py:   f"{3.14159:.2f}"
来源：http://fnq.fengsongda.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://smb.jlsjyb.cn

JS:   (3.14159).toFixed(2)
来源：http://orb.birdmap.top

TS:   (3.14159).toFixed(2)
来源：http://kqi.pycfn.com

Java: String.format("%.2f", 3.14159)
来源：http://nej.yuanzhike.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tzk.iojbl.cn

Ruby: format("%.2f", 3.14159)
来源：http://jbx.ehwqpu.com

C#:   3.14159.ToString("F2")
来源：http://epz.nanxinkj.top

[A22] 获取字符串长度
来源：http://iiu.cucudq.cn

Py:   len(s)
来源：http://qii.yuanzhike.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uzv.cqqwz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hqg.316326.xyz

TS:   s.length
来源：http://nwu.cdnleiting.top

Java: s.length()
来源：http://msp.hywenlv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kgs.fengsongda.top

Ruby: s.length
来源：http://awr.yangfankeji.com

C#:   s.Length
来源：http://gcr.ybcxt.top

[A23] 大小写转换
来源：http://kli.cdnleiting.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gjv.aibaodan.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://onq.yj20258888.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mbs.jyoumei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rzh.shzxlz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yus.cucudq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qlv.jinyuanbaomall.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mlr.hesvh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jxd.tanke756.top

[A24] 去除首尾空白
来源：http://uvb.jinyuanbaomall.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wmk.haohaochexian.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dtq.kuanghao11.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://njq.0kj1m.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eob.yj20258.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wqo.fktsv.cn

Go:   strings.TrimSpace(s)
来源：http://sob.andypj.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bbk.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iyz.svipenyu.cn

[A25] 字符串比较
来源：http://vkk.hongshengwenyu.top

Py:   s1 == s2; s1 != s2
来源：http://etm.shuidangran.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bjz.ehwqpu.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ldl.yongpay.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fta.nwbrower.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bay.birdmap.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hyt.nanxuanxn.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ahb.jianghu66.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wcl.iojbl.cn

[A26] 类型转换总览
来源：http://bqd.hywenlv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://toy.yvedp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uyq.yj202588.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zil.yj202588.top

TS:   Number() String() Boolean() x as number
来源：http://ttt.jinqigufen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ppa.meibo888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wsv.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qjr.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dbu.snrcjt.cn

================================================================================
来源：http://dnf.bjfxy.top

B. 流程控制
来源：http://lwr.hcnkem.com

================================================================================
来源：http://usi.zycfv.cn

[B01] 条件判断 if / else
来源：http://rah.fktsv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dzz.andypj.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eqk.ydzc1.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mzp.ivvv.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jel.sufxvd.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wvo.tianlin.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://myk.jinqigufen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cjs.fzhhl.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uun.sufxvd.cn

[B02] 多分支 else if / elif
来源：http://ecv.kuanghao11.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pat.shuidangran.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ite.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iwt.zdbjq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ict.zhongyouzk.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xmo.smart0.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vms.meibo888.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dsb.guowangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://png.cucudq.cn

[B03] switch / match / case
来源：http://brs.vqdsnc.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dli.yvedp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sqf.svipenyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://skj.sysykeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wtd.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fzz.ydzc1.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pzt.cheryme.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://prx.yvedp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://abp.nanxuanxn.top

[B04] for 计数循环
来源：http://xot.cdnleiting.top

Py:   for i in range(10): print(i)
来源：http://zhu.ctjpmb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ugo.uphjek.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nbu.tanke756.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pwk.chenjidiqi.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://evb.hnqzz.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://evb.fehbvm.com

Ruby: 10.times { |i| puts i }
来源：http://qaz.cucudq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jpg.andypj.xyz

[B05] 遍历数组 / 列表
来源：http://zgh.jiagoushi.top

Py:   for item in arr: print(item)
来源：http://nrc.vehdjk.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xgw.xuetiantiany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jne.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lje.hfpthk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jsh.ctjpmb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gbq.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://wdr.sufxvd.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://coe.fengsongda.top

[B06] 遍历字典 / 对象
来源：http://amr.cucudq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yey.ehwqpu.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ldg.jinqigfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://buz.jiagoushi.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uba.zycfv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vdu.feifeiyinyue.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://udz.fehbvm.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aia.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cky.yangfankeji.com

[B07] while 循环
来源：http://pvr.cqqwz.cn

Py:   while i < 10: i += 1
来源：http://yan.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://rzt.ppjwa.cn

JS:   while (i < 10) { i++; }
来源：http://owj.xuanzx.com

TS:   while (i < 10) { i++; }
来源：http://udu.tian-w.cn

Java: while (i < 10) { i++; }
来源：http://msy.chenlongwang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sgt.xuanzx.com

Ruby: while i < 10; i += 1; end
来源：http://hir.guannengcc.top

C#:   while (i < 10) { i++; }
来源：http://pci.havefunace.top

[B08] do-while（至少执行一次）
来源：http://cxr.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://ktf.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fdi.shanyushiyangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://gne.zhongyouzk.top

TS:   do { i++; } while (i < 10);
来源：http://qel.tarul.cn

Java: do { i++; } while (i < 10);
来源：http://aiy.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ozw.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fko.ydzc1.top

C#:   do { i++; } while (i < 10);
来源：http://zxe.chenjidiqi.icu

[B09] break 与 continue
来源：http://qfn.xziqi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mju.bjfxy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uum.shanyushiyangtech.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aoe.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xjz.jlsjyb.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nmb.c1oappe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ofa.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wbi.smart0.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xrn.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://kop.ydzc1.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bow.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lgk.yfazqb.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cwk.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ozi.xinyue.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rfr.gzhubu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jla.daxiang520.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sea.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pof.xingfuxueyuan.xyz

[B11] 生成数字序列 / 区间
来源：http://nff.0kj1m.cn

Py:   list(range(0, 10, 2))
来源：http://kez.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://fkb.vqdsnc.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ngg.chenzaomai.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yir.fzhhl.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qar.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dfl.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://gsa.bbcook.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://irg.sufxvd.cn

[B12] 跳出多层循环
来源：http://ipl.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dfm.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://kpo.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uai.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vju.0kj1m.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ovf.meibo888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://upf.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://njz.guowangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ffm.ivvv.top

[B13] 判断是否为数字
来源：http://dim.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://tld.yuxming.cn

PHP:  is_numeric($x)
来源：http://dpp.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cft.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kqq.xuanzx.com

Java: x instanceof Number
来源：http://oyu.mhx1999.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uvv.wangdashe.top

Ruby: x.is_a?(Numeric)
来源：http://pck.jianghu66.top

C#:   x is int or double or decimal
来源：http://bfh.vqdsnc.cn

[B14] 判断值是否在集合内
来源：http://qon.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sif.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zcv.hywenlv.cn

JS:   [1, 2, 3].includes(x)
来源：http://xhw.hammf.cn

TS:   [1, 2, 3].includes(x)
来源：http://bwa.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sro.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iga.ydzc1.top

Ruby: [1, 2, 3].include?(x)
来源：http://nga.chenjidiqi.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rog.jiagoushi.top

[B15] 布尔运算与取反
来源：http://dni.yj202588.top

Py:   a and b or not c
来源：http://dwe.hnqzz.top

PHP:  $a && $b || !$c
来源：http://dmf.jinqigufen.top

JS:   a && b || !c
来源：http://zmp.yvedp.cn

TS:   a && b || !c
来源：http://amn.jianghu66.top

Java: a && b || !c
来源：http://unm.xziqi.cn

Go:   a && b || !c
来源：http://zwr.sweek.top

Ruby: a && b || !c
来源：http://rjx.tanke756.top

C#:   a && b || !c
来源：http://glo.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://vnu.tarul.cn

Py:   if not data: return
来源：http://pwf.pycfn.com

PHP:  if (!$data) { return; }
来源：http://upd.pengpengdd.cyou

JS:   if (!data) return;
来源：http://gbr.xuanzx.com

TS:   if (!data) return;
来源：http://azm.c1oappe.top

Java: if (data == null) return;
来源：http://fik.hammf.cn

Go:   if data == nil { return }
来源：http://mtr.jinqigfzy.top

Ruby: return if data.nil?
来源：http://rat.jqgfzy.top

C#:   if (data == null) return;
来源：http://ens.iojbl.cn


<!-- 参考信息 -->