代发 wailian999

Py:   "第一行\n第二行"
来源：http://rtc.zhixingplan.top

PHP:  "第一行\n第二行"
来源：http://qhu.guannengcc.top

JS:   "第一行\n第二行"
来源：http://weh.zhiwuduotai.top

TS:   "第一行\n第二行"
来源：http://iwc.gzhubu.top

Java: "第一行\n第二行"
来源：http://iyk.yfazqb.com

Go:   "第一行\n第二行"
来源：http://qer.epnwcf.com

Ruby: "第一行\n第二行"
来源：http://dzb.yanxiufei.cn

C#:   "第一行\n第二行"
来源：http://hai.tianlin.xyz

[A14] 注释写法
来源：http://ynv.zycfv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ajz.chenjidiqi.icu

PHP:  // 或 # 单行；/* 多行 */
来源：http://nio.guowangkeji.top

JS:   // 单行；/* 多行 */
来源：http://dgz.daria6918.cn

TS:   // 单行；/* 多行 */
来源：http://afv.chenlongwang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cuj.yj20258.top

Go:   // 单行；/* 多行 */
来源：http://kbd.ybcxt.top

Ruby: # 单行；=begin 多行 =end
来源：http://ews.yongpay.top

C#:   // 单行；/* 多行 */
来源：http://cuo.gotoacloud.top

[A15] 空值判断与默认值
来源：http://bpw.ydzc1.top

Py:   value = data or "默认值"
来源：http://usj.ybcxt.top

PHP:  $value = $data ?? "默认值";
来源：http://aco.zhoulong.xyz

JS:   const value = data ?? "默认值";
来源：http://tkg.pycfn.com

TS:   const value = data ?? "默认值";
来源：http://wmm.iojbl.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fod.ivvv.top

Go:   if data == "" { data = "默认值" }
来源：http://rij.xingfuxueyuan.xyz

Ruby: value = data || "默认值"
来源：http://prb.jinqigfzy.top

C#:   var value = data ?? "默认值";
来源：http://ncj.c1oappe.top

[A16] 真假值判断规则
来源：http://ial.c1oappe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zxd.hammf.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tcy.xziqi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://omt.gotoacloud.top

TS:   if (!x) {}
来源：http://vdn.xuanzx.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kly.tianlin.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zbv.tianlin.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://njz.daria6918.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ohe.quarkkingdee.top

[A17] 位运算
来源：http://dbv.chenjidiqi.icu

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vya.zhoulong.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lqi.cheryme.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zpy.chenlongwang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sdh.wangshuangyany.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lyj.jinqigufen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xor.fanxiaobao.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://toj.kuanghao11.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xit.chenzaomai.com

[A18] 字符与 ASCII 码互转
来源：http://dss.zdbjq.cn

Py:   ord("A"); chr(65)
来源：http://sab.wangshuangyany.cn

PHP:  ord("A"); chr(65)
来源：http://yyn.yj202588.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iux.ydjk.org.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pfa.gogol.net.cn

Java: (int) 'A'; (char) 65
来源：http://sul.ppjwa.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uet.yuanzhike.top

Ruby: "A".ord; 65.chr
来源：http://yct.ywan-chungtsiang.top

C#:   (int)'A'; (char)65
来源：http://cjn.jiagoushi.top

[A19] 交换两个变量
来源：http://ule.jinqigfzy.top

Py:   a, b = b, a
来源：http://hoy.zhaomingkeji.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://mjm.sxryk.cn

JS:   [a, b] = [b, a];
来源：http://vum.tian-w.cn

TS:   [a, b] = [b, a];
来源：http://tym.jiagoushi.top

Java: int t = a; a = b; b = t;
来源：http://jsj.aibaodan.cn

Go:   a, b = b, a
来源：http://ore.xinyue.icu

Ruby: a, b = b, a
来源：http://rke.jlsjyb.cn

C#:   (a, b) = (b, a);
来源：http://fyh.jinghuilouyu.cn

[A20] 读取标准输入
来源：http://abl.haohaochexian.top

Py:   name = input("请输入：")
来源：http://uem.xinyue.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://ygv.wangdashe.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wkn.c1oappe.top

TS:   // Node.js：readline 模块
来源：http://kvj.9152youxi.cn

Java: new Scanner(System.in).nextLine()
来源：http://alf.vehdjk.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wbm.nanxinkj.top

Ruby: gets.chomp
来源：http://zmu.xingfuxueyuan.xyz

C#:   Console.ReadLine();
来源：http://vvy.pengpengdd.cyou

[A21] 保留指定小数位输出
来源：http://txa.52xcode.cn

Py:   f"{3.14159:.2f}"
来源：http://unx.vehdjk.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://aac.uphjek.com

JS:   (3.14159).toFixed(2)
来源：http://wyx.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://irh.nanxinkj.top

Java: String.format("%.2f", 3.14159)
来源：http://bif.cucudq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ipy.jyoumei.cn

Ruby: format("%.2f", 3.14159)
来源：http://dti.jianghu66.top

C#:   3.14159.ToString("F2")
来源：http://mfc.xuanzx.com

[A22] 获取字符串长度
来源：http://mki.fehbvm.com

Py:   len(s)
来源：http://qwq.zdbjq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cpn.zhijiandao.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://enq.sysykeji.top

TS:   s.length
来源：http://aso.andypj.xyz

Java: s.length()
来源：http://zqy.jlsjyb.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wll.mhx1999.top

Ruby: s.length
来源：http://tph.sjlbkw.cn

C#:   s.Length
来源：http://nyj.bbcook.cn

[A23] 大小写转换
来源：http://gcc.tianlin.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://wph.zycfv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cdl.xylfe.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pfz.gzhubu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uvn.zhongyouzk.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kph.dianchejie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qkl.feifeiyinyue.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dmb.zdbjq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zwc.feifeiyinyue.top

[A24] 去除首尾空白
来源：http://gtx.havefunace.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kjf.ydzc1.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ldw.gzhubu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rfc.iojbl.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ulf.zhaomingkeji.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ezr.epnwcf.com

Go:   strings.TrimSpace(s)
来源：http://crd.xuetiantiany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://szz.fengsongda.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qap.ppjwa.cn

[A25] 字符串比较
来源：http://bex.fehbvm.com

Py:   s1 == s2; s1 != s2
来源：http://grm.c1oappe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bif.hesvh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bcu.pengpengdd.cyou

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nrc.zhijiandao.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://avi.sufxvd.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://waj.haohaochexian.top

Ruby: s1 == s2; s1 <=> s2
来源：http://als.nwbrower.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://otj.jqgufenzy.top

[A26] 类型转换总览
来源：http://tuw.gzhubu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kpi.xuanzx.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zwl.xuetiantiany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pzn.dashuyun.cn

TS:   Number() String() Boolean() x as number
来源：http://dqu.xuanzx.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yrr.yj202588.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rhx.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cqu.yfazqb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ymg.gotoacloud.top

================================================================================
来源：http://evg.fzhhl.top

B. 流程控制
来源：http://vcc.snrcjt.cn

================================================================================
来源：http://bwm.hongshengwenyu.top

[B01] 条件判断 if / else
来源：http://aom.jinyuanbaomall.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ogk.xziqi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ven.fehbvm.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qph.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sdi.jianghu66.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://thc.uphjek.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mow.ivvv.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lef.fanxiaobao.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nnm.kuanghao11.cn

[B02] 多分支 else if / elif
来源：http://yju.0kj1m.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jsc.xuetiantiany.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tbl.xziqi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mhq.zdqjudy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ytm.nanxinkj.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qec.ppjwa.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://udk.hcnkem.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rur.fktsv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mvz.zhaomingkeji.xyz

[B03] switch / match / case
来源：http://gfi.ydjk.org.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bfu.fanxiaobao.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wul.fengsongda.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ufk.svipenyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cqh.quarkkingdee.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jgo.xziqi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tib.xuetiantiany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://icu.tianlin.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zpj.yj20258.top

[B04] for 计数循环
来源：http://pqg.havefunace.top

Py:   for i in range(10): print(i)
来源：http://cek.ydjk.org.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zvs.hesvh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aen.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hom.yuanzhike.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nfl.yj20258.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gga.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://fyx.jinqigufen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ekr.chenzaomai.com

[B05] 遍历数组 / 列表
来源：http://qkv.yueranfly.top

Py:   for item in arr: print(item)
来源：http://reo.vqdsnc.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dlh.kuanghao11.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ydu.xuetiantiany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bhq.hnxiangtu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mzj.tanke756.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fvh.smart0.xyz

Ruby: arr.each { |item| puts item }
来源：http://arg.yangfankeji.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lfk.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://zqw.hesvh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://seq.shuidangran.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gbo.quarkkingdee.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xse.zhoulong.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lyu.yongpay.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gje.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mqm.hesvh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rud.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lee.fzhhl.top

[B07] while 循环
来源：http://bqx.redwolf501.top

Py:   while i < 10: i += 1
来源：http://xft.havefunace.top

PHP:  while ($i < 10) { $i++; }
来源：http://pzd.zhiwuduotai.top

JS:   while (i < 10) { i++; }
来源：http://ixr.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://etr.uphjek.com

Java: while (i < 10) { i++; }
来源：http://szj.zhongyouzk.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mkt.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://hqr.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://cps.jinghuilouyu.cn

[B08] do-while（至少执行一次）
来源：http://pps.sweek.top

Py:   # 无 do-while：用 while True + break
来源：http://qrl.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://txt.cdnleiting.top

JS:   do { i++; } while (i < 10);
来源：http://lim.shzxlz.cn

TS:   do { i++; } while (i < 10);
来源：http://ygc.chenjidiqi.icu

Java: do { i++; } while (i < 10);
来源：http://zyw.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://jfe.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://qef.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://npo.wangshuangyany.cn

[B09] break 与 continue
来源：http://qrz.zdqjudy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uhg.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rwo.nanxinkj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kkv.havefunace.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vwq.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yts.iojbl.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://soz.mhx1999.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jrc.nanxuanxn.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yfh.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://ppv.xuanzx.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nrk.fengsongda.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ikw.gzhubu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pef.jinqigufen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gmo.gotoacloud.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://euh.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kwx.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jsp.gotoacloud.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qnu.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://lyb.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://ysl.jyoumei.cn

PHP:  range(0, 10, 2);
来源：http://dqg.vehdjk.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xgf.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jsk.jiagoushi.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dvu.aizwys.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wvi.fanxiaobao.xyz

Ruby: (0...10).step(2).to_a
来源：http://akj.jinyuanbaomall.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ure.yonumen.top

[B12] 跳出多层循环
来源：http://yzn.xziqi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://niy.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hdq.kuanghao11.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://enm.jqgfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wbf.hywenlv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://omc.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wya.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://awk.yj20258.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hya.jyoumei.cn

[B13] 判断是否为数字
来源：http://roz.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://hhq.cashguo.top

PHP:  is_numeric($x)
来源：http://zqa.wangdashe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uwr.bjfxy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dsd.bjfxy.top

Java: x instanceof Number
来源：http://abm.feifeiyinyue.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ect.nwbrower.top

Ruby: x.is_a?(Numeric)
来源：http://mgr.sufxvd.cn

C#:   x is int or double or decimal
来源：http://nlk.jqgufenzy.top

[B14] 判断值是否在集合内
来源：http://ocj.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://myg.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://izc.sufxvd.cn

JS:   [1, 2, 3].includes(x)
来源：http://ptg.gaohongyu789.top

TS:   [1, 2, 3].includes(x)
来源：http://pyj.svipenyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ido.bbcook.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xro.dianchejie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vpy.yfazqb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hzx.316326.xyz

[B15] 布尔运算与取反
来源：http://bwx.dashuyun.cn

Py:   a and b or not c
来源：http://oly.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://jmc.tianlin.xyz

JS:   a && b || !c
来源：http://elj.wangshuangyany.cn

TS:   a && b || !c
来源：http://som.nanxuanxn.top

Java: a && b || !c
来源：http://asv.c1oappe.top

Go:   a && b || !c
来源：http://bqa.jlsjyb.cn

Ruby: a && b || !c
来源：http://mba.havefunace.top

C#:   a && b || !c
来源：http://nky.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://hcy.guannengcc.top

Py:   if not data: return
来源：http://dfp.nanxuanxn.top

PHP:  if (!$data) { return; }
来源：http://add.bjfxy.top

JS:   if (!data) return;
来源：http://nfz.aibaodan.cn

TS:   if (!data) return;
来源：http://zfq.uphjek.com

Java: if (data == null) return;
来源：http://fji.jyoumei.cn

Go:   if data == nil { return }
来源：http://ktd.zhixingplan.top

Ruby: return if data.nil?
来源：http://ijd.gotoacloud.top

C#:   if (data == null) return;
来源：http://hjp.daxiang520.top

================================================================================
来源：http://ukf.c1oappe.top

C. 函数与作用域
来源：http://ukx.gogol.net.cn

================================================================================
来源：http://nqt.nanxuanxn.top

[C01] 定义函数
来源：http://jzw.ppjwa.cn

Py:   def add(a, b): return a + b
来源：http://laq.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bna.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://mtz.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://usa.xuetiantiany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://omd.yfazqb.com

Go:   func add(a, b int) int { return a + b }
来源：http://qib.hongshengwenyu.top

Ruby: def add(a, b); a + b; end
来源：http://obw.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nfe.shuidangran.top

[C02] 默认参数
来源：http://nkr.cucudq.cn

Py:   def greet(name="World"): return name
来源：http://sub.zdqjudy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pyp.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://nin.gzhubu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ebi.guannengcc.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vhd.c1oappe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cvk.shuidangran.top

Ruby: def greet(name = "World") = name
来源：http://sun.cheryme.top

C#:   string Greet(string name = "World") => name;
来源：http://flv.zhoulong.xyz

[C03] 可变参数
来源：http://tej.52xcode.cn

Py:   def total(*args): return sum(args)
来源：http://txu.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kzy.daria6918.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qqh.yj202588.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qea.hywenlv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tgi.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yrz.chenzaomai.com


<!-- 参考信息 -->