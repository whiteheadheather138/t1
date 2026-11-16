代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tap.tian-w.cn

Ruby: "Hello, #{name}!"
来源：http://vnf.snrcjt.cn

C#:   $"Hello, {name}!"
来源：http://ewk.jqgfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://pbb.kuanghao11.cn

Py:   "第一行\n第二行"
来源：http://vbw.xuanzx.com

PHP:  "第一行\n第二行"
来源：http://ukv.hywenlv.cn

JS:   "第一行\n第二行"
来源：http://feq.cdnleiting.top

TS:   "第一行\n第二行"
来源：http://ipo.fanxiaobao.xyz

Java: "第一行\n第二行"
来源：http://lfx.ybcxt.top

Go:   "第一行\n第二行"
来源：http://fba.zhijiandao.cn

Ruby: "第一行\n第二行"
来源：http://ora.yj20258.top

C#:   "第一行\n第二行"
来源：http://mpv.smart0.xyz

[A14] 注释写法
来源：http://zvb.snrcjt.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pzv.hnxiangtu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://kec.cucudq.cn

JS:   // 单行；/* 多行 */
来源：http://fcf.uphjek.com

TS:   // 单行；/* 多行 */
来源：http://cux.fzhhl.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://emy.smart0.xyz

Go:   // 单行；/* 多行 */
来源：http://nhs.hammf.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pfh.shzxlz.cn

C#:   // 单行；/* 多行 */
来源：http://ijz.jqgfzy.top

[A15] 空值判断与默认值
来源：http://orr.jinghuilouyu.cn

Py:   value = data or "默认值"
来源：http://xvg.zhongyouzk.top

PHP:  $value = $data ?? "默认值";
来源：http://vob.yuanzhike.top

JS:   const value = data ?? "默认值";
来源：http://ywu.jianghu66.top

TS:   const value = data ?? "默认值";
来源：http://rox.fzhhl.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jmz.guannengcc.top

Go:   if data == "" { data = "默认值" }
来源：http://ymk.ivvv.top

Ruby: value = data || "默认值"
来源：http://nvk.hnxiangtu.top

C#:   var value = data ?? "默认值";
来源：http://mkt.quarkkingdee.top

[A16] 真假值判断规则
来源：http://yzj.fehbvm.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sqm.shuidangran.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qwl.nanxinkj.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://svs.pengpengdd.cyou

TS:   if (!x) {}
来源：http://ayy.gzhubu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ajw.nwbrower.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://udt.zdqjudy.top

Ruby: unless x            # nil 与 false 为假
来源：http://coi.snrcjt.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yzm.cheryme.top

[A17] 位运算
来源：http://bya.shanyushiyangkeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://myo.gogol.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rmp.hnxiangtu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ceb.bjfxy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://eey.haohaochexian.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lai.fengsongda.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ymp.daxiang520.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://udc.sysykeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ntm.mhx1999.top

[A18] 字符与 ASCII 码互转
来源：http://xmk.ctjpmb.com

Py:   ord("A"); chr(65)
来源：http://qcy.hesvh.cn

PHP:  ord("A"); chr(65)
来源：http://zxn.zhixingplan.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sbl.yj202588.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kmq.haohaochexian.top

Java: (int) 'A'; (char) 65
来源：http://szn.hongshengwenyu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pga.ydzc1.top

Ruby: "A".ord; 65.chr
来源：http://qqc.sufxvd.cn

C#:   (int)'A'; (char)65
来源：http://ztn.zhongyouzk.top

[A19] 交换两个变量
来源：http://glo.vqdsnc.cn

Py:   a, b = b, a
来源：http://ivj.zhaomingkeji.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://nzv.meibo888.top

JS:   [a, b] = [b, a];
来源：http://qrd.smart0.xyz

TS:   [a, b] = [b, a];
来源：http://okx.sweek.top

Java: int t = a; a = b; b = t;
来源：http://vis.jinyuanbaomall.cn

Go:   a, b = b, a
来源：http://tus.shuidangran.top

Ruby: a, b = b, a
来源：http://mab.snrcjt.cn

C#:   (a, b) = (b, a);
来源：http://ess.xuetiantiany.cn

[A20] 读取标准输入
来源：http://dca.pycfn.com

Py:   name = input("请输入：")
来源：http://eya.quarkkingdee.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vcb.yfazqb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yfo.cheryme.top

TS:   // Node.js：readline 模块
来源：http://uvh.yj20258888.top

Java: new Scanner(System.in).nextLine()
来源：http://kxe.ydjk.org.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hdt.ivvv.top

Ruby: gets.chomp
来源：http://rsw.gzhubu.top

C#:   Console.ReadLine();
来源：http://lmb.hnxiangtu.top

[A21] 保留指定小数位输出
来源：http://wha.chenzaomai.com

Py:   f"{3.14159:.2f}"
来源：http://hku.zhixingplan.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cah.xingfuxueyuan.xyz

JS:   (3.14159).toFixed(2)
来源：http://jkg.cdnleiting.top

TS:   (3.14159).toFixed(2)
来源：http://jcy.xziqi.cn

Java: String.format("%.2f", 3.14159)
来源：http://lcd.316326.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qca.nanxuanxn.top

Ruby: format("%.2f", 3.14159)
来源：http://off.hnxiangtu.top

C#:   3.14159.ToString("F2")
来源：http://urg.chenlongwang.top

[A22] 获取字符串长度
来源：http://rbk.yanxiufei.cn

Py:   len(s)
来源：http://cwi.bjfxy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fgw.sysykeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://thb.gogol.net.cn

TS:   s.length
来源：http://zin.ywan-chungtsiang.top

Java: s.length()
来源：http://aqv.xingfuxueyuan.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cji.9152youxi.cn

Ruby: s.length
来源：http://sbn.nwbrower.top

C#:   s.Length
来源：http://xmb.cucudq.cn

[A23] 大小写转换
来源：http://shm.jiagoushi.top

Py:   s.upper(); s.lower(); s.title()
来源：http://rqc.sysykeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://woa.tanke756.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zdi.fengsongda.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kxa.nwbrower.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xbx.ydzc1.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qis.316326.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bzc.yuanzhike.top

C#:   s.ToUpper(); s.ToLower()
来源：http://cdt.jianghu66.top

[A24] 去除首尾空白
来源：http://qkh.tanke756.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mli.hammf.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ldg.smart0.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mdh.hammf.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dqz.zhoulong.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ltm.shangyingyoupin.top

Go:   strings.TrimSpace(s)
来源：http://sbi.smart0.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://suv.sjlbkw.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iyp.hongshengwenyu.top

[A25] 字符串比较
来源：http://wic.xingfuxueyuan.xyz

Py:   s1 == s2; s1 != s2
来源：http://zsd.bjfxy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dua.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://egk.chenjidiqi.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pdo.gotoacloud.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ioo.vehdjk.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bhb.meibo888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://uza.zhijiandao.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jip.chenlongwang.top

[A26] 类型转换总览
来源：http://cve.daria6918.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oaj.feifeiyinyue.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://afk.ybcxt.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mra.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://ohh.xuetiantiany.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://six.gotoacloud.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://csk.fengsongda.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://lif.snrcjt.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gwa.316326.xyz

================================================================================
来源：http://fqb.zhoulong.xyz

B. 流程控制
来源：http://deq.fengsongda.top

================================================================================
来源：http://gfg.xinyue.icu

[B01] 条件判断 if / else
来源：http://dqf.jinghuilouyu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://eoi.cheryme.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bhd.zdbjq.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ehc.xuetiantiany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hqk.gaohongyu789.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qwd.zhaomingkeji.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://axy.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yxb.xuetiantiany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pju.52xcode.cn

[B02] 多分支 else if / elif
来源：http://xhq.ehwqpu.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ptw.jianghu66.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yjm.jinqigfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://izx.9152youxi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qzp.ydjk.org.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://msa.yvedp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qnk.xinyue.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xyt.ctjpmb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mti.cqqwz.cn

[B03] switch / match / case
来源：http://vxe.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://frc.fktsv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hme.yongpay.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nra.jiagoushi.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nat.hesvh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://efx.xylfe.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wak.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://okq.feifeiyinyue.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zwa.jinqigufen.top

[B04] for 计数循环
来源：http://jby.316326.xyz

Py:   for i in range(10): print(i)
来源：http://otw.jiagoushi.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xlz.smart0.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hff.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ijl.mhx1999.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aze.sufxvd.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pqe.tian-w.cn

Ruby: 10.times { |i| puts i }
来源：http://ies.ybcxt.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ano.gaohongyu789.top

[B05] 遍历数组 / 列表
来源：http://twy.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://hqg.cqqwz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gwh.shuidangran.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hgn.fengsongda.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ayf.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bdn.jinqigfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lka.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://kef.yangfankeji.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jxx.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://hrn.jinqigfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hvd.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xxl.mhx1999.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rsz.zhaomingkeji.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pmw.jqgufenzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fyk.cashguo.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://boo.wangshuangyany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://boj.birdmap.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bqs.wangshuangyany.cn

[B07] while 循环
来源：http://dtb.xinyue.icu

Py:   while i < 10: i += 1
来源：http://qqw.sxryk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eoo.ctjpmb.com

JS:   while (i < 10) { i++; }
来源：http://hqx.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://twq.nanxinkj.top

Java: while (i < 10) { i++; }
来源：http://upy.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ytj.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://epz.fzhhl.top

C#:   while (i < 10) { i++; }
来源：http://ito.yuxming.cn

[B08] do-while（至少执行一次）
来源：http://cdj.pengpengdd.cyou

Py:   # 无 do-while：用 while True + break
来源：http://wmy.sufxvd.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mqh.c1oappe.top

JS:   do { i++; } while (i < 10);
来源：http://gnt.yuanzhike.top

TS:   do { i++; } while (i < 10);
来源：http://qnf.sweek.top

Java: do { i++; } while (i < 10);
来源：http://zlc.zhengqikj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pua.yj202588.top

Ruby: begin; i += 1; end while i < 10
来源：http://tvz.tian-w.cn

C#:   do { i++; } while (i < 10);
来源：http://oon.ydjk.org.cn

[B09] break 与 continue
来源：http://nkn.dianchejie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tgi.ppjwa.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fou.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ljx.chenzaomai.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hto.meibo888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iiw.pycfn.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kvx.xinyue.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pae.shzxlz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mmn.quarkkingdee.top

[B10] 遍历同时拿索引
来源：http://eij.fktsv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zss.xuanzx.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://txq.jqgufenzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nzc.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ahh.zdqjudy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ghc.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ggp.fehbvm.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eyg.pengpengdd.cyou

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://myn.gotoacloud.top

[B11] 生成数字序列 / 区间
来源：http://ros.tanke756.top

Py:   list(range(0, 10, 2))
来源：http://hck.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://wys.ydzc1.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fpv.jqgufenzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mwk.tian-w.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xoj.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cya.cqqwz.cn

Ruby: (0...10).step(2).to_a
来源：http://rof.aizwys.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iai.daria6918.cn

[B12] 跳出多层循环
来源：http://icc.ivvv.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mfy.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lqv.dashuyun.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xvq.xingfuxueyuan.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ofr.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://owj.mhx1999.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://skp.yonumen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gvo.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vfs.bjfxy.top

[B13] 判断是否为数字
来源：http://aae.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://qbz.meibo888.top

PHP:  is_numeric($x)
来源：http://azm.shanyushiyangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qaa.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jbw.shuidangran.top

Java: x instanceof Number
来源：http://zha.meibo888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lsk.tian-w.cn

Ruby: x.is_a?(Numeric)
来源：http://jhn.aibaodan.cn

C#:   x is int or double or decimal
来源：http://mwq.wangdashe.top

[B14] 判断值是否在集合内
来源：http://civ.hammf.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vsm.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gim.jinqigufen.top

JS:   [1, 2, 3].includes(x)
来源：http://ttg.vehdjk.com

TS:   [1, 2, 3].includes(x)
来源：http://osi.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://byh.iojbl.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kum.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://khx.shanyushiyangtech.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fdj.jqgufenzy.top

[B15] 布尔运算与取反
来源：http://ilj.aizwys.cn

Py:   a and b or not c
来源：http://jpo.hcnkem.com

PHP:  $a && $b || !$c
来源：http://yms.hfpthk.cn

JS:   a && b || !c
来源：http://lrg.hesvh.cn

TS:   a && b || !c
来源：http://gvt.shanyushiyangtech.top

Java: a && b || !c
来源：http://wwu.sjlbkw.cn

Go:   a && b || !c
来源：http://kmn.ywan-chungtsiang.top

Ruby: a && b || !c
来源：http://jyz.ehwqpu.com

C#:   a && b || !c
来源：http://ofx.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://ncw.yanxiufei.cn

Py:   if not data: return
来源：http://wyo.vehdjk.com

PHP:  if (!$data) { return; }
来源：http://xpp.zdqjudy.top

JS:   if (!data) return;
来源：http://jyg.guannengcc.top

TS:   if (!data) return;
来源：http://nfh.yj20258.top

Java: if (data == null) return;
来源：http://bxv.xuanzx.com

Go:   if data == nil { return }
来源：http://nwp.nanxinkj.top

Ruby: return if data.nil?
来源：http://bmt.cucudq.cn

C#:   if (data == null) return;
来源：http://txg.shanyushiyangkeji.top

================================================================================
来源：http://ndb.svipenyu.cn

C. 函数与作用域
来源：http://vxw.yangfankeji.com

================================================================================
来源：http://jsw.kuanghao11.cn

[C01] 定义函数
来源：http://prc.hysaishi.cn

Py:   def add(a, b): return a + b
来源：http://wqz.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yar.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://ncw.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://psl.meibo888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kdv.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://qxg.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://mxw.daxiang520.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eig.nanxinkj.top

[C02] 默认参数
来源：http://bck.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://xhf.bjfxy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dvb.yfazqb.com

JS:   function greet(name = "World") { return name; }
来源：http://guo.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lci.jlsjyb.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ufl.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lqv.snrcjt.cn

Ruby: def greet(name = "World") = name
来源：http://kxf.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://boi.guannengcc.top

[C03] 可变参数
来源：http://ulq.zhengqikj.top

Py:   def total(*args): return sum(args)
来源：http://zha.jinghuilouyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wvg.52xcode.cn


<!-- 参考信息 -->