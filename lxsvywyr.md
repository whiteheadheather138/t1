代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ifd.dashuyun.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cch.chenjidiqi.icu

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tzf.shuidangran.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hyq.ywan-chungtsiang.top

[A10] 生成随机数
来源：http://mbz.xinyue.icu

Py:   import random; random.randint(1, 100)
来源：http://ixs.shanyushiyangtech.top

PHP:  random_int(1, 100);
来源：http://rfb.aizwys.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ivu.cqqwz.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ipx.hammf.cn

Java: new Random().nextInt(100) + 1
来源：http://mzb.gaohongyu789.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jpw.kuanghao11.cn

Ruby: rand(1..100)
来源：http://ekk.gzhubu.top

C#:   new Random().Next(1, 101)
来源：http://tfm.cucudq.cn

[A11] 条件表达式（三元）
来源：http://lgx.bbcook.cn

Py:   "yes" if x > 0 else "no"
来源：http://zis.vqdsnc.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xue.birdmap.top

JS:   x > 0 ? "yes" : "no"
来源：http://hqt.chenzaomai.com

TS:   x > 0 ? "yes" : "no"
来源：http://drr.dashuyun.cn

Java: x > 0 ? "yes" : "no"
来源：http://yas.xziqi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://blx.316326.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://rxn.guowangkeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://tqo.snrcjt.cn

[A12] 字符串插值 / 格式化
来源：http://vmm.yj20258.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wwd.316326.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zar.fehbvm.com

JS:   `Hello, ${name}!`
来源：http://irk.jinyuanbaomall.cn

TS:   `Hello, ${name}!`
来源：http://ngb.jinyuanbaomall.cn

Java: "Hello, %s!".formatted(name)
来源：http://phc.fanxiaobao.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wls.iojbl.cn

Ruby: "Hello, #{name}!"
来源：http://mqt.52xcode.cn

C#:   $"Hello, {name}!"
来源：http://wsi.zdqjudy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lsc.jinyuanbaomall.cn

Py:   "第一行\n第二行"
来源：http://fja.yvedp.cn

PHP:  "第一行\n第二行"
来源：http://wwy.jinqigufen.top

JS:   "第一行\n第二行"
来源：http://xlb.hfpthk.cn

TS:   "第一行\n第二行"
来源：http://pwr.ydzc1.top

Java: "第一行\n第二行"
来源：http://erj.zhaomingkeji.xyz

Go:   "第一行\n第二行"
来源：http://jkt.shuidangran.top

Ruby: "第一行\n第二行"
来源：http://qjl.haohaochexian.top

C#:   "第一行\n第二行"
来源：http://end.cheryme.top

[A14] 注释写法
来源：http://tyw.aibaodan.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://exx.hongshengwenyu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ifx.shuidangran.top

JS:   // 单行；/* 多行 */
来源：http://rwq.andypj.xyz

TS:   // 单行；/* 多行 */
来源：http://xhs.epnwcf.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lja.aizwys.cn

Go:   // 单行；/* 多行 */
来源：http://qha.52xcode.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zyo.jianghu66.top

C#:   // 单行；/* 多行 */
来源：http://wsn.yangfankeji.com

[A15] 空值判断与默认值
来源：http://oxd.yvedp.cn

Py:   value = data or "默认值"
来源：http://wbo.mhx1999.top

PHP:  $value = $data ?? "默认值";
来源：http://aer.yfazqb.com

JS:   const value = data ?? "默认值";
来源：http://hkh.hnqzz.top

TS:   const value = data ?? "默认值";
来源：http://amp.shanyushiyangkeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rim.iojbl.cn

Go:   if data == "" { data = "默认值" }
来源：http://cka.pycfn.com

Ruby: value = data || "默认值"
来源：http://njl.smart0.xyz

C#:   var value = data ?? "默认值";
来源：http://kou.daxiang520.top

[A16] 真假值判断规则
来源：http://kwi.zhongyouzk.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rkk.uphjek.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vld.0kj1m.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://spt.hywenlv.cn

TS:   if (!x) {}
来源：http://oby.jiagoushi.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://arg.xingfuxueyuan.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wco.zhoulong.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://ghm.yj202588.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://svs.316326.xyz

[A17] 位运算
来源：http://omm.svipenyu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zvo.yfazqb.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://klo.pycfn.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gae.mhx1999.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://elz.jyoumei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ede.52xcode.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rgp.yongpay.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sqs.redwolf501.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nzq.zycfv.cn

[A18] 字符与 ASCII 码互转
来源：http://fve.vehdjk.com

Py:   ord("A"); chr(65)
来源：http://dwh.sufxvd.cn

PHP:  ord("A"); chr(65)
来源：http://pvu.chenlongwang.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kqd.zdqjudy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bos.cdnleiting.top

Java: (int) 'A'; (char) 65
来源：http://tmi.daria6918.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hjw.ydjk.org.cn

Ruby: "A".ord; 65.chr
来源：http://axu.daxiang520.top

C#:   (int)'A'; (char)65
来源：http://tfs.yuanzhike.top

[A19] 交换两个变量
来源：http://goo.jinqigufen.top

Py:   a, b = b, a
来源：http://djn.zycfv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dkx.zhixingplan.top

JS:   [a, b] = [b, a];
来源：http://xfp.shuidangran.top

TS:   [a, b] = [b, a];
来源：http://srp.fanxiaobao.xyz

Java: int t = a; a = b; b = t;
来源：http://wcy.shzxlz.cn

Go:   a, b = b, a
来源：http://nla.guannengcc.top

Ruby: a, b = b, a
来源：http://sly.feifeiyinyue.top

C#:   (a, b) = (b, a);
来源：http://hlr.bbcook.cn

[A20] 读取标准输入
来源：http://aoq.yj202588.top

Py:   name = input("请输入：")
来源：http://vaw.yfazqb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://ntp.ppjwa.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rgj.sysykeji.top

TS:   // Node.js：readline 模块
来源：http://fih.xziqi.cn

Java: new Scanner(System.in).nextLine()
来源：http://lsh.zhijiandao.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qbe.cqqwz.cn

Ruby: gets.chomp
来源：http://ima.hnxiangtu.top

C#:   Console.ReadLine();
来源：http://lvd.hnqzz.top

[A21] 保留指定小数位输出
来源：http://vaa.316326.xyz

Py:   f"{3.14159:.2f}"
来源：http://lmk.52xcode.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vgg.hnqzz.top

JS:   (3.14159).toFixed(2)
来源：http://wnf.shuidangran.top

TS:   (3.14159).toFixed(2)
来源：http://gsc.c1oappe.top

Java: String.format("%.2f", 3.14159)
来源：http://gih.fzhhl.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ybc.yj202588.top

Ruby: format("%.2f", 3.14159)
来源：http://tvd.yj20258.top

C#:   3.14159.ToString("F2")
来源：http://xpx.havefunace.top

[A22] 获取字符串长度
来源：http://ord.jyoumei.cn

Py:   len(s)
来源：http://fui.bbcook.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ycv.yonumen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hjc.hywenlv.cn

TS:   s.length
来源：http://biu.xylfe.cn

Java: s.length()
来源：http://eza.yonumen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://syn.meibo888.top

Ruby: s.length
来源：http://inx.wangdashe.top

C#:   s.Length
来源：http://hii.cheryme.top

[A23] 大小写转换
来源：http://gnm.yangfankeji.com

Py:   s.upper(); s.lower(); s.title()
来源：http://pdd.zhongyouzk.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gec.guowangkeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xul.tian-w.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://psg.52xcode.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gwu.dashuyun.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://izd.sufxvd.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hig.birdmap.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lhj.zycfv.cn

[A24] 去除首尾空白
来源：http://tgj.kuanghao11.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xaz.9152youxi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iru.chenjidiqi.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ahv.ydzc1.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kst.jiagoushi.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://adj.guannengcc.top

Go:   strings.TrimSpace(s)
来源：http://svn.zdbjq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xlh.guannengcc.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ijq.sysykeji.top

[A25] 字符串比较
来源：http://cyj.xinyue.icu

Py:   s1 == s2; s1 != s2
来源：http://jbr.bjfxy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mqs.hfpthk.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hax.nwbrower.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://emq.zhixingplan.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://idz.yuanzhike.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gix.yangfankeji.com

Ruby: s1 == s2; s1 <=> s2
来源：http://xtn.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lne.cashguo.top

[A26] 类型转换总览
来源：http://pvp.zdbjq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iae.tian-w.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dfu.smart0.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ecg.zycfv.cn

TS:   Number() String() Boolean() x as number
来源：http://uzk.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xky.hongshengwenyu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hil.hongshengwenyu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kop.xziqi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wzi.cheryme.top

================================================================================
来源：http://pqu.smart0.xyz

B. 流程控制
来源：http://wpi.dashuyun.cn

================================================================================
来源：http://xxy.meibo888.top

[B01] 条件判断 if / else
来源：http://fdf.ydjk.org.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cdt.yanxiufei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ndi.wangshuangyany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vhw.jianghu66.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ogz.wangshuangyany.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sun.sxryk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://npq.ehwqpu.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oby.gotoacloud.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sbh.sjlbkw.cn

[B02] 多分支 else if / elif
来源：http://vvv.tarul.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rxw.nanxuanxn.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oxr.yj20258.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mmm.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kvj.haohaochexian.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kql.cucudq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jal.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bln.yanxiufei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kii.haohaochexian.top

[B03] switch / match / case
来源：http://mjt.hammf.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yxw.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nrm.yuanzhike.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hox.zdbjq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rmb.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fcn.tian-w.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gzv.fzhhl.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ckp.ctjpmb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dxm.guowangkeji.top

[B04] for 计数循环
来源：http://ddm.yuxming.cn

Py:   for i in range(10): print(i)
来源：http://xjm.chenlongwang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xit.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zpz.tian-w.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mju.yj20258888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lte.hcnkem.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kjq.redwolf501.top

Ruby: 10.times { |i| puts i }
来源：http://ofp.yanxiufei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lat.jinqigufen.top

[B05] 遍历数组 / 列表
来源：http://qif.jinqigufen.top

Py:   for item in arr: print(item)
来源：http://mis.cheryme.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hfd.jqgufenzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tyd.bjfxy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ybb.iojbl.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://psa.cashguo.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lwl.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://wbz.jyoumei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lwt.cheryme.top

[B06] 遍历字典 / 对象
来源：http://qwt.tanke756.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dbq.bjfxy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oqk.xuanzx.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vii.yvedp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ngd.dashuyun.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jea.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hqx.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bxi.kuanghao11.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ocw.hcnkem.com

[B07] while 循环
来源：http://mrb.xinyue.icu

Py:   while i < 10: i += 1
来源：http://qap.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://iop.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://hna.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://zny.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://olm.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zuz.vehdjk.com

Ruby: while i < 10; i += 1; end
来源：http://mzu.chenlongwang.top

C#:   while (i < 10) { i++; }
来源：http://qrq.ctjpmb.com

[B08] do-while（至少执行一次）
来源：http://ftg.ehwqpu.com

Py:   # 无 do-while：用 while True + break
来源：http://qsp.dianchejie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kzg.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://jmy.cdnleiting.top

TS:   do { i++; } while (i < 10);
来源：http://woc.uphjek.com

Java: do { i++; } while (i < 10);
来源：http://hzv.bjfxy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fep.hongshengwenyu.top

Ruby: begin; i += 1; end while i < 10
来源：http://fqd.pengpengdd.cyou

C#:   do { i++; } while (i < 10);
来源：http://nfg.nanxuanxn.top

[B09] break 与 continue
来源：http://bzz.yonumen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zol.hfpthk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vuv.aizwys.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kwv.gotoacloud.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zdz.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jgv.dianchejie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gea.yanxiufei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gzu.0kj1m.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yjt.yj20258888.top

[B10] 遍历同时拿索引
来源：http://wdh.sysykeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sob.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yjr.yangfankeji.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wzm.zhoulong.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gtf.ywan-chungtsiang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yng.cucudq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vem.bjfxy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gam.ctjpmb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nuc.chenjidiqi.icu

[B11] 生成数字序列 / 区间
来源：http://tnf.guannengcc.top

Py:   list(range(0, 10, 2))
来源：http://ukw.cheryme.top

PHP:  range(0, 10, 2);
来源：http://nhh.nanxuanxn.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hvy.feifeiyinyue.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ldv.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mkb.shanyushiyangtech.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qsn.jyoumei.cn

Ruby: (0...10).step(2).to_a
来源：http://xni.chenjidiqi.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gvp.9152youxi.cn

[B12] 跳出多层循环
来源：http://xrm.yueranfly.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://eyu.yuanzhike.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xjc.xuetiantiany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fhk.yj20258888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zmp.wangshuangyany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dqn.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sdy.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://une.kuanghao11.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ujs.sxryk.cn

[B13] 判断是否为数字
来源：http://iih.hesvh.cn

Py:   isinstance(x, (int, float))
来源：http://qin.uphjek.com

PHP:  is_numeric($x)
来源：http://buk.cucudq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://loh.ivvv.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dlc.redwolf501.top

Java: x instanceof Number
来源：http://edv.yuanzhike.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://btz.aizwys.cn

Ruby: x.is_a?(Numeric)
来源：http://qtq.nanxuanxn.top

C#:   x is int or double or decimal
来源：http://aep.snrcjt.cn

[B14] 判断值是否在集合内
来源：http://kmh.jinqigfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bwd.yj202588.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://obs.hysaishi.cn

JS:   [1, 2, 3].includes(x)
来源：http://mki.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://urq.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ncn.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zgu.hfpthk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bqu.hnxiangtu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://drr.birdmap.top

[B15] 布尔运算与取反
来源：http://rpj.xuetiantiany.cn

Py:   a and b or not c
来源：http://akk.zdqjudy.top

PHP:  $a && $b || !$c
来源：http://fpi.shanyushiyangtech.top

JS:   a && b || !c
来源：http://bli.fktsv.cn

TS:   a && b || !c
来源：http://txr.zhiwuduotai.top

Java: a && b || !c
来源：http://euc.bjfxy.top

Go:   a && b || !c
来源：http://qjq.cashguo.top

Ruby: a && b || !c
来源：http://jph.nwbrower.top

C#:   a && b || !c
来源：http://gop.zycfv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zty.gotoacloud.top

Py:   if not data: return
来源：http://tea.ctjpmb.com

PHP:  if (!$data) { return; }
来源：http://adi.pycfn.com

JS:   if (!data) return;
来源：http://izt.zhiwuduotai.top

TS:   if (!data) return;
来源：http://sfk.dianchejie.cn


<!-- 参考信息 -->