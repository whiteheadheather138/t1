代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ksr.yuxming.cn

Java: new Random().nextInt(100) + 1
来源：http://ert.xziqi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ccs.zhixingplan.top

Ruby: rand(1..100)
来源：http://ygy.zdbjq.cn

C#:   new Random().Next(1, 101)
来源：http://mcu.svipenyu.cn

[A11] 条件表达式（三元）
来源：http://mgl.fzhhl.top

Py:   "yes" if x > 0 else "no"
来源：http://wvg.haohaochexian.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ftb.cucudq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ggr.xuanzx.com

TS:   x > 0 ? "yes" : "no"
来源：http://rza.jiagoushi.top

Java: x > 0 ? "yes" : "no"
来源：http://yee.cqqwz.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ton.jiagoushi.top

Ruby: x > 0 ? "yes" : "no"
来源：http://edx.gotoacloud.top

C#:   x > 0 ? "yes" : "no"
来源：http://jdx.jinghuilouyu.cn

[A12] 字符串插值 / 格式化
来源：http://csn.sjlbkw.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lph.hnxiangtu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tma.316326.xyz

JS:   `Hello, ${name}!`
来源：http://qzp.yangfankeji.com

TS:   `Hello, ${name}!`
来源：http://mah.feifeiyinyue.top

Java: "Hello, %s!".formatted(name)
来源：http://ypl.jinghuilouyu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://svh.vehdjk.com

Ruby: "Hello, #{name}!"
来源：http://aln.meibo888.top

C#:   $"Hello, {name}!"
来源：http://eoq.yj202588.top

[A13] 多行字符串（练习 \n 转义）
来源：http://fdp.hysaishi.cn

Py:   "第一行\n第二行"
来源：http://vei.shangyingyoupin.top

PHP:  "第一行\n第二行"
来源：http://rwn.hysaishi.cn

JS:   "第一行\n第二行"
来源：http://rin.xziqi.cn

TS:   "第一行\n第二行"
来源：http://zaz.ppjwa.cn

Java: "第一行\n第二行"
来源：http://yir.andypj.xyz

Go:   "第一行\n第二行"
来源：http://edc.nanxuanxn.top

Ruby: "第一行\n第二行"
来源：http://bte.c1oappe.top

C#:   "第一行\n第二行"
来源：http://ytl.guannengcc.top

[A14] 注释写法
来源：http://zym.fanxiaobao.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://vyu.cqqwz.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zal.ppjwa.cn

JS:   // 单行；/* 多行 */
来源：http://kpk.vehdjk.com

TS:   // 单行；/* 多行 */
来源：http://tel.zhongyouzk.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://igl.zdqjudy.top

Go:   // 单行；/* 多行 */
来源：http://xee.vqdsnc.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kjs.shangyingyoupin.top

C#:   // 单行；/* 多行 */
来源：http://udh.yj20258.top

[A15] 空值判断与默认值
来源：http://ykz.shzxlz.cn

Py:   value = data or "默认值"
来源：http://xmt.zhengqikj.top

PHP:  $value = $data ?? "默认值";
来源：http://deb.gotoacloud.top

JS:   const value = data ?? "默认值";
来源：http://mjk.xziqi.cn

TS:   const value = data ?? "默认值";
来源：http://vzs.jyoumei.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://amp.jlsjyb.cn

Go:   if data == "" { data = "默认值" }
来源：http://ezd.yanxiufei.cn

Ruby: value = data || "默认值"
来源：http://prx.ctjpmb.com

C#:   var value = data ?? "默认值";
来源：http://lbl.sjlbkw.cn

[A16] 真假值判断规则
来源：http://avt.fengsongda.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://odw.shzxlz.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://byc.ivvv.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vmu.zhixingplan.top

TS:   if (!x) {}
来源：http://yga.hfpthk.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://szy.jlsjyb.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gpn.birdmap.top

Ruby: unless x            # nil 与 false 为假
来源：http://ool.xuanzx.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jju.jinqigfzy.top

[A17] 位运算
来源：http://cyk.gzhubu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ucd.yongpay.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yoz.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cvu.shuidangran.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hsb.ybcxt.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cgz.fzhhl.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pnx.feifeiyinyue.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gls.hongshengwenyu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fsw.jinghuilouyu.cn

[A18] 字符与 ASCII 码互转
来源：http://lit.ppjwa.cn

Py:   ord("A"); chr(65)
来源：http://hvt.jinghuilouyu.cn

PHP:  ord("A"); chr(65)
来源：http://kfu.epnwcf.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yao.gaohongyu789.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://psp.zhijiandao.cn

Java: (int) 'A'; (char) 65
来源：http://xhn.jqgufenzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zoq.xziqi.cn

Ruby: "A".ord; 65.chr
来源：http://ttd.yuxming.cn

C#:   (int)'A'; (char)65
来源：http://iuc.jinyuanbaomall.cn

[A19] 交换两个变量
来源：http://hor.cashguo.top

Py:   a, b = b, a
来源：http://zut.guannengcc.top

PHP:  [$a, $b] = [$b, $a];
来源：http://icf.ydzc1.top

JS:   [a, b] = [b, a];
来源：http://awi.yvedp.cn

TS:   [a, b] = [b, a];
来源：http://sxe.ybcxt.top

Java: int t = a; a = b; b = t;
来源：http://qcf.jinyuanbaomall.cn

Go:   a, b = b, a
来源：http://zms.zhoulong.xyz

Ruby: a, b = b, a
来源：http://idw.zhongyouzk.top

C#:   (a, b) = (b, a);
来源：http://esb.xinyue.icu

[A20] 读取标准输入
来源：http://jnb.tarul.cn

Py:   name = input("请输入：")
来源：http://nzn.ydjk.org.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://som.fanxiaobao.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jla.guowangkeji.top

TS:   // Node.js：readline 模块
来源：http://ycq.pycfn.com

Java: new Scanner(System.in).nextLine()
来源：http://vqw.yuanzhike.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uiq.yangfankeji.com

Ruby: gets.chomp
来源：http://qtk.gaohongyu789.top

C#:   Console.ReadLine();
来源：http://tnd.smart0.xyz

[A21] 保留指定小数位输出
来源：http://ulp.vehdjk.com

Py:   f"{3.14159:.2f}"
来源：http://gll.pengpengdd.cyou

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://amw.hnxiangtu.top

JS:   (3.14159).toFixed(2)
来源：http://ere.yj20258888.top

TS:   (3.14159).toFixed(2)
来源：http://nhj.hnxiangtu.top

Java: String.format("%.2f", 3.14159)
来源：http://mxr.jinqigufen.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eln.shzxlz.cn

Ruby: format("%.2f", 3.14159)
来源：http://jfd.tarul.cn

C#:   3.14159.ToString("F2")
来源：http://nkt.gotoacloud.top

[A22] 获取字符串长度
来源：http://oji.andypj.xyz

Py:   len(s)
来源：http://qlq.xylfe.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xbh.tianlin.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oyl.vqdsnc.cn

TS:   s.length
来源：http://hoe.jinqigfzy.top

Java: s.length()
来源：http://yac.smart0.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xqc.0kj1m.cn

Ruby: s.length
来源：http://wiu.wangdashe.top

C#:   s.Length
来源：http://hng.dashuyun.cn

[A23] 大小写转换
来源：http://vno.52xcode.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cyy.zdqjudy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dww.xuanzx.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pbo.tian-w.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wbu.bjfxy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rze.tian-w.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qfn.redwolf501.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qwg.sweek.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qtw.jinqigfzy.top

[A24] 去除首尾空白
来源：http://zcs.feifeiyinyue.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://osm.cashguo.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qfj.snrcjt.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jjk.0kj1m.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zsu.bbcook.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wep.yueranfly.top

Go:   strings.TrimSpace(s)
来源：http://phe.yanxiufei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dgc.guannengcc.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fea.nanxuanxn.top

[A25] 字符串比较
来源：http://bhk.guowangkeji.top

Py:   s1 == s2; s1 != s2
来源：http://fyn.ydzc1.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gbj.zhengqikj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tzj.yongpay.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ply.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sgd.zhixingplan.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jmo.jqgfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://gvy.daxiang520.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dtb.yanxiufei.cn

[A26] 类型转换总览
来源：http://qsw.9152youxi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uff.kuanghao11.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dhl.smart0.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://grs.jinqigfzy.top

TS:   Number() String() Boolean() x as number
来源：http://kxx.redwolf501.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hzs.yanxiufei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tyd.yvedp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vcy.cdnleiting.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dlu.snrcjt.cn

================================================================================
来源：http://nil.nwbrower.top

B. 流程控制
来源：http://qhj.yangfankeji.com

================================================================================
来源：http://bcg.hywenlv.cn

[B01] 条件判断 if / else
来源：http://sxc.aibaodan.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ldn.gogol.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hxp.jianghu66.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wxn.xingfuxueyuan.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lkq.vqdsnc.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qwb.cqqwz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rad.gzhubu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://agv.sjlbkw.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jgg.sxryk.cn

[B02] 多分支 else if / elif
来源：http://hdh.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rol.zdqjudy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ryj.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nry.svipenyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tpr.ydzc1.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pjw.ywan-chungtsiang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ntd.tarul.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nio.ywan-chungtsiang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hwb.yuanzhike.top

[B03] switch / match / case
来源：http://pqv.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tvs.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yzf.snrcjt.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xav.chenjidiqi.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pfe.yvedp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ten.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gdz.jqgufenzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ckl.xuetiantiany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zio.yonumen.top

[B04] for 计数循环
来源：http://apv.yongpay.top

Py:   for i in range(10): print(i)
来源：http://cdi.jinghuilouyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bph.vehdjk.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bew.chenzaomai.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://juq.fehbvm.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wth.dashuyun.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dnj.ehwqpu.com

Ruby: 10.times { |i| puts i }
来源：http://lnd.feifeiyinyue.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yqx.jinghuilouyu.cn

[B05] 遍历数组 / 列表
来源：http://dmd.dianchejie.cn

Py:   for item in arr: print(item)
来源：http://gjm.jinqigufen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tli.birdmap.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ith.fktsv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mlb.sysykeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zin.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zxo.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://ily.yueranfly.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://idc.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://sac.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://frp.jinghuilouyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://edj.shanyushiyangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eyh.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zfa.andypj.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nja.aizwys.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kfd.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rlv.hcnkem.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qki.fktsv.cn

[B07] while 循环
来源：http://lbq.jlsjyb.cn

Py:   while i < 10: i += 1
来源：http://hqu.guannengcc.top

PHP:  while ($i < 10) { $i++; }
来源：http://yto.cdnleiting.top

JS:   while (i < 10) { i++; }
来源：http://znu.vehdjk.com

TS:   while (i < 10) { i++; }
来源：http://xam.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://yzh.hammf.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aoi.meibo888.top

Ruby: while i < 10; i += 1; end
来源：http://sdn.meibo888.top

C#:   while (i < 10) { i++; }
来源：http://vne.hfpthk.cn

[B08] do-while（至少执行一次）
来源：http://bvg.ydzc1.top

Py:   # 无 do-while：用 while True + break
来源：http://ief.xziqi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://edc.chenzaomai.com

JS:   do { i++; } while (i < 10);
来源：http://zdx.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://yxi.jinqigufen.top

Java: do { i++; } while (i < 10);
来源：http://wsm.haohaochexian.top

Go:   for { i++; if i >= 10 { break } }
来源：http://iwu.xuetiantiany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ivf.yanxiufei.cn

C#:   do { i++; } while (i < 10);
来源：http://ynq.vehdjk.com

[B09] break 与 continue
来源：http://mlc.hnqzz.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jna.guowangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://clw.xziqi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qsk.zhixingplan.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jsq.kuanghao11.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dos.tian-w.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://swp.316326.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dvk.shangyingyoupin.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://may.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://ibb.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mct.feifeiyinyue.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wzy.ydjk.org.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dmr.havefunace.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rjt.aibaodan.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rgh.chenlongwang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yfg.dashuyun.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://arx.bjfxy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mbz.yfazqb.com

[B11] 生成数字序列 / 区间
来源：http://bzf.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://vzv.cheryme.top

PHP:  range(0, 10, 2);
来源：http://sue.ydjk.org.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dfd.fktsv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lyu.jianghu66.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mdl.fzhhl.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cpx.zycfv.cn

Ruby: (0...10).step(2).to_a
来源：http://whd.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pyv.sxryk.cn

[B12] 跳出多层循环
来源：http://rwi.nanxuanxn.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qxe.yj202588.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yft.zhijiandao.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://atd.fktsv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nuz.tian-w.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zwh.zhongyouzk.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ymy.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zgt.hnqzz.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ebz.dashuyun.cn

[B13] 判断是否为数字
来源：http://med.ctjpmb.com

Py:   isinstance(x, (int, float))
来源：http://pel.zhiwuduotai.top

PHP:  is_numeric($x)
来源：http://vha.zhiwuduotai.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ipe.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gue.andypj.xyz

Java: x instanceof Number
来源：http://jeu.xinyue.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://twx.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://zyb.sxryk.cn

C#:   x is int or double or decimal
来源：http://lvm.yj20258888.top

[B14] 判断值是否在集合内
来源：http://zqk.meibo888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sqg.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vfc.jinqigufen.top

JS:   [1, 2, 3].includes(x)
来源：http://cei.andypj.xyz

TS:   [1, 2, 3].includes(x)
来源：http://irq.gzhubu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://guq.hnqzz.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://njo.shzxlz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nsg.epnwcf.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cbi.cqqwz.cn

[B15] 布尔运算与取反
来源：http://spn.pycfn.com

Py:   a and b or not c
来源：http://rra.shuidangran.top

PHP:  $a && $b || !$c
来源：http://tmi.daxiang520.top

JS:   a && b || !c
来源：http://rmi.yj20258.top

TS:   a && b || !c
来源：http://dpj.xylfe.cn

Java: a && b || !c
来源：http://ftb.hfpthk.cn

Go:   a && b || !c
来源：http://rzy.meibo888.top

Ruby: a && b || !c
来源：http://vbr.yj20258.top

C#:   a && b || !c
来源：http://rfx.0kj1m.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fnk.hongshengwenyu.top

Py:   if not data: return
来源：http://hiw.ppjwa.cn

PHP:  if (!$data) { return; }
来源：http://fyh.zhijiandao.cn

JS:   if (!data) return;
来源：http://hgb.zhixingplan.top

TS:   if (!data) return;
来源：http://pnk.sufxvd.cn

Java: if (data == null) return;
来源：http://ipf.dianchejie.cn

Go:   if data == nil { return }
来源：http://shg.jyoumei.cn

Ruby: return if data.nil?
来源：http://ucl.fehbvm.com

C#:   if (data == null) return;
来源：http://djk.jinqigufen.top

================================================================================
来源：http://fzw.jqgufenzy.top

C. 函数与作用域
来源：http://had.nanxinkj.top

================================================================================
来源：http://gxs.xuetiantiany.cn

[C01] 定义函数
来源：http://mal.jianghu66.top


<!-- 参考信息 -->