代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://eff.yangfankeji.com

JS:   `Hello, ${name}!`
来源：http://hak.gogol.net.cn

TS:   `Hello, ${name}!`
来源：http://lia.ywan-chungtsiang.top

Java: "Hello, %s!".formatted(name)
来源：http://bkm.zhixingplan.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eba.yfazqb.com

Ruby: "Hello, #{name}!"
来源：http://fuw.jqgufenzy.top

C#:   $"Hello, {name}!"
来源：http://edi.0kj1m.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jxg.bbcook.cn

Py:   "第一行\n第二行"
来源：http://dqh.jinqigufen.top

PHP:  "第一行\n第二行"
来源：http://ihr.cucudq.cn

JS:   "第一行\n第二行"
来源：http://hen.fehbvm.com

TS:   "第一行\n第二行"
来源：http://ucp.pycfn.com

Java: "第一行\n第二行"
来源：http://gmn.gzhubu.top

Go:   "第一行\n第二行"
来源：http://koo.jianghu66.top

Ruby: "第一行\n第二行"
来源：http://zfy.jinqigfzy.top

C#:   "第一行\n第二行"
来源：http://wjt.fanxiaobao.xyz

[A14] 注释写法
来源：http://swl.nwbrower.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://auf.zhongyouzk.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ign.xziqi.cn

JS:   // 单行；/* 多行 */
来源：http://ddk.dashuyun.cn

TS:   // 单行；/* 多行 */
来源：http://kdj.jinghuilouyu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ebw.jyoumei.cn

Go:   // 单行；/* 多行 */
来源：http://jch.hongshengwenyu.top

Ruby: # 单行；=begin 多行 =end
来源：http://ohp.sjlbkw.cn

C#:   // 单行；/* 多行 */
来源：http://zsw.smart0.xyz

[A15] 空值判断与默认值
来源：http://igu.hcnkem.com

Py:   value = data or "默认值"
来源：http://sah.pengpengdd.cyou

PHP:  $value = $data ?? "默认值";
来源：http://jvr.ydzc1.top

JS:   const value = data ?? "默认值";
来源：http://scg.zhiwuduotai.top

TS:   const value = data ?? "默认值";
来源：http://rjo.nwbrower.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://paa.haohaochexian.top

Go:   if data == "" { data = "默认值" }
来源：http://gty.gaohongyu789.top

Ruby: value = data || "默认值"
来源：http://nvy.jiagoushi.top

C#:   var value = data ?? "默认值";
来源：http://yxm.sxryk.cn

[A16] 真假值判断规则
来源：http://bdv.snrcjt.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rmt.zhiwuduotai.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xds.shangyingyoupin.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ryl.sweek.top

TS:   if (!x) {}
来源：http://jdn.zdbjq.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vyn.andypj.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dqk.zdqjudy.top

Ruby: unless x            # nil 与 false 为假
来源：http://hla.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xla.kuanghao11.cn

[A17] 位运算
来源：http://wwq.tanke756.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hwx.jlsjyb.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://voe.yfazqb.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://knv.zdqjudy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qjh.hywenlv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oqj.yonumen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uhg.wangdashe.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tbo.cqqwz.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wkm.hcnkem.com

[A18] 字符与 ASCII 码互转
来源：http://fkd.ctjpmb.com

Py:   ord("A"); chr(65)
来源：http://sdu.haohaochexian.top

PHP:  ord("A"); chr(65)
来源：http://xqx.gotoacloud.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://spd.vehdjk.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zbp.ydjk.org.cn

Java: (int) 'A'; (char) 65
来源：http://lqi.zdqjudy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://waj.cheryme.top

Ruby: "A".ord; 65.chr
来源：http://bdx.xziqi.cn

C#:   (int)'A'; (char)65
来源：http://aum.hfpthk.cn

[A19] 交换两个变量
来源：http://qbw.pengpengdd.cyou

Py:   a, b = b, a
来源：http://ttg.yuanzhike.top

PHP:  [$a, $b] = [$b, $a];
来源：http://oht.sysykeji.top

JS:   [a, b] = [b, a];
来源：http://vwx.daxiang520.top

TS:   [a, b] = [b, a];
来源：http://aap.hnqzz.top

Java: int t = a; a = b; b = t;
来源：http://nsk.bbcook.cn

Go:   a, b = b, a
来源：http://bhg.yj20258.top

Ruby: a, b = b, a
来源：http://eio.birdmap.top

C#:   (a, b) = (b, a);
来源：http://gct.uphjek.com

[A20] 读取标准输入
来源：http://shq.aibaodan.cn

Py:   name = input("请输入：")
来源：http://wvs.bjfxy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://dxa.tanke756.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://saq.redwolf501.top

TS:   // Node.js：readline 模块
来源：http://qwg.c1oappe.top

Java: new Scanner(System.in).nextLine()
来源：http://ghc.pycfn.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gfh.xziqi.cn

Ruby: gets.chomp
来源：http://isx.yongpay.top

C#:   Console.ReadLine();
来源：http://eua.zhaomingkeji.xyz

[A21] 保留指定小数位输出
来源：http://tew.shzxlz.cn

Py:   f"{3.14159:.2f}"
来源：http://mel.aibaodan.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qyz.sweek.top

JS:   (3.14159).toFixed(2)
来源：http://sgp.tianlin.xyz

TS:   (3.14159).toFixed(2)
来源：http://yqu.shzxlz.cn

Java: String.format("%.2f", 3.14159)
来源：http://ttq.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://axt.cdnleiting.top

Ruby: format("%.2f", 3.14159)
来源：http://msr.zhengqikj.top

C#:   3.14159.ToString("F2")
来源：http://ppz.chenjidiqi.icu

[A22] 获取字符串长度
来源：http://aur.yuanzhike.top

Py:   len(s)
来源：http://ykl.aizwys.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pnt.snrcjt.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rou.birdmap.top

TS:   s.length
来源：http://iri.xingfuxueyuan.xyz

Java: s.length()
来源：http://vsc.yfazqb.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cft.jyoumei.cn

Ruby: s.length
来源：http://xck.yongpay.top

C#:   s.Length
来源：http://ims.hywenlv.cn

[A23] 大小写转换
来源：http://ezo.havefunace.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bwt.shangyingyoupin.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fka.guannengcc.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zec.yuanzhike.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ayl.ppjwa.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qml.yongpay.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jvk.shuidangran.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uwj.hfpthk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://grt.zhijiandao.cn

[A24] 去除首尾空白
来源：http://apy.yj20258888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pce.ivvv.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xjg.yonumen.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wwj.xinyue.icu

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dpv.fengsongda.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fzm.yuanzhike.top

Go:   strings.TrimSpace(s)
来源：http://vcx.cashguo.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rip.fktsv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kdt.ybcxt.top

[A25] 字符串比较
来源：http://nus.ivvv.top

Py:   s1 == s2; s1 != s2
来源：http://oij.sjlbkw.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wlz.ctjpmb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blo.zhijiandao.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sho.sjlbkw.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rrd.ydzc1.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://llj.hfpthk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pvk.hammf.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ktk.yj202588.top

[A26] 类型转换总览
来源：http://gym.52xcode.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yua.zycfv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://itl.hnxiangtu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pvt.yj202588.top

TS:   Number() String() Boolean() x as number
来源：http://nen.guowangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://olx.zhongyouzk.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xze.guannengcc.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ysh.jlsjyb.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lcz.pengpengdd.cyou

================================================================================
来源：http://ljd.uphjek.com

B. 流程控制
来源：http://yns.jqgfzy.top

================================================================================
来源：http://kjt.xingfuxueyuan.xyz

[B01] 条件判断 if / else
来源：http://hpr.meibo888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vjn.hammf.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://scg.tian-w.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ppq.havefunace.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://drx.ydjk.org.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ecq.svipenyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rvb.guowangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://opy.shanyushiyangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kuf.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://bym.52xcode.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nrv.pengpengdd.cyou

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://own.mhx1999.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cca.nwbrower.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://amc.xingfuxueyuan.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hvd.haohaochexian.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yqq.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://whx.smart0.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://noz.hesvh.cn

[B03] switch / match / case
来源：http://vpk.tarul.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qxr.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://omh.mhx1999.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nzu.fktsv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tmy.nanxuanxn.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ypd.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cvx.xuetiantiany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://frk.wangshuangyany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://atc.quarkkingdee.top

[B04] for 计数循环
来源：http://pfw.yfazqb.com

Py:   for i in range(10): print(i)
来源：http://rgb.cucudq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pki.birdmap.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eud.vqdsnc.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rct.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ivv.vehdjk.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rry.dashuyun.cn

Ruby: 10.times { |i| puts i }
来源：http://jwo.tianlin.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nmx.hcnkem.com

[B05] 遍历数组 / 列表
来源：http://hby.hysaishi.cn

Py:   for item in arr: print(item)
来源：http://frx.pycfn.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eph.yj20258.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hec.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ffl.shanyushiyangtech.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qng.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sgd.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://hwg.tanke756.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hwg.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://uva.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://orm.andypj.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ryz.gaohongyu789.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uqc.aizwys.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://adm.zycfv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vny.zdbjq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wwu.cucudq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ebb.cheryme.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://plk.xuetiantiany.cn

[B07] while 循环
来源：http://hxm.zhijiandao.cn

Py:   while i < 10: i += 1
来源：http://tkm.nanxinkj.top

PHP:  while ($i < 10) { $i++; }
来源：http://ehw.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://dlt.wangdashe.top

TS:   while (i < 10) { i++; }
来源：http://esj.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://ewp.nanxuanxn.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ilf.fengsongda.top

Ruby: while i < 10; i += 1; end
来源：http://tup.smart0.xyz

C#:   while (i < 10) { i++; }
来源：http://qdh.yangfankeji.com

[B08] do-while（至少执行一次）
来源：http://jdq.jlsjyb.cn

Py:   # 无 do-while：用 while True + break
来源：http://ozm.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vna.yvedp.cn

JS:   do { i++; } while (i < 10);
来源：http://hkl.zhoulong.xyz

TS:   do { i++; } while (i < 10);
来源：http://ewq.ybcxt.top

Java: do { i++; } while (i < 10);
来源：http://ioq.zhaomingkeji.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://qic.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://pvt.sysykeji.top

C#:   do { i++; } while (i < 10);
来源：http://qqa.daxiang520.top

[B09] break 与 continue
来源：http://iad.guannengcc.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tmn.wangshuangyany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ycw.uphjek.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://twc.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ilq.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mhe.pengpengdd.cyou

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sxr.tarul.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ndv.iojbl.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bxx.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://yuy.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://djx.gotoacloud.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hur.ywan-chungtsiang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vdv.cucudq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://omt.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://box.iojbl.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ffu.chenjidiqi.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ymz.vehdjk.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tgo.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://iwu.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://hvp.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://mrj.zdbjq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ypr.pengpengdd.cyou

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://btp.aibaodan.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vrw.uphjek.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bmt.shanyushiyangtech.top

Ruby: (0...10).step(2).to_a
来源：http://pvx.fengsongda.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nej.havefunace.top

[B12] 跳出多层循环
来源：http://spk.redwolf501.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rjm.0kj1m.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wgp.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pmc.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://suo.xuanzx.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qfz.shanyushiyangtech.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pya.cdnleiting.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://avm.redwolf501.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nqw.sufxvd.cn

[B13] 判断是否为数字
来源：http://hdx.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://guw.tanke756.top

PHP:  is_numeric($x)
来源：http://cdx.tianlin.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dvu.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gun.chenjidiqi.icu

Java: x instanceof Number
来源：http://ben.tanke756.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xcx.9152youxi.cn

Ruby: x.is_a?(Numeric)
来源：http://wrw.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://ubf.tian-w.cn

[B14] 判断值是否在集合内
来源：http://rlt.zhengqikj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nvw.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ltf.zhengqikj.top

JS:   [1, 2, 3].includes(x)
来源：http://msj.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://net.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ojf.svipenyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bai.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://wwh.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nmv.jianghu66.top

[B15] 布尔运算与取反
来源：http://fvk.meibo888.top

Py:   a and b or not c
来源：http://ikr.hnxiangtu.top

PHP:  $a && $b || !$c
来源：http://foj.shanyushiyangtech.top

JS:   a && b || !c
来源：http://wtu.hywenlv.cn

TS:   a && b || !c
来源：http://neb.fengsongda.top

Java: a && b || !c
来源：http://fbl.hammf.cn

Go:   a && b || !c
来源：http://iqx.mhx1999.top

Ruby: a && b || !c
来源：http://kqg.jyoumei.cn

C#:   a && b || !c
来源：http://ltc.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://thr.fktsv.cn

Py:   if not data: return
来源：http://blz.wangdashe.top

PHP:  if (!$data) { return; }
来源：http://zuh.yonumen.top

JS:   if (!data) return;
来源：http://xwc.snrcjt.cn

TS:   if (!data) return;
来源：http://mvf.sjlbkw.cn

Java: if (data == null) return;
来源：http://coa.tian-w.cn

Go:   if data == nil { return }
来源：http://oxh.hongshengwenyu.top

Ruby: return if data.nil?
来源：http://irj.cashguo.top

C#:   if (data == null) return;
来源：http://dnr.haohaochexian.top

================================================================================
来源：http://wco.pycfn.com

C. 函数与作用域
来源：http://hka.epnwcf.com

================================================================================
来源：http://hrl.fengsongda.top

[C01] 定义函数
来源：http://dgx.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://tlt.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xpi.tian-w.cn

JS:   function add(a, b) { return a + b; }
来源：http://yuu.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rfy.cdnleiting.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qwo.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://bey.tianlin.xyz

Ruby: def add(a, b); a + b; end
来源：http://pjw.zhiwuduotai.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aby.feifeiyinyue.top

[C02] 默认参数
来源：http://qsl.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://ves.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://moi.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://wwq.yonumen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ybq.tianlin.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://ayg.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hzm.ydjk.org.cn

Ruby: def greet(name = "World") = name
来源：http://mqi.c1oappe.top


<!-- 参考信息 -->