代发 wailian999

Py:   "第一行\n第二行"
来源：http://aus.xuanzx.com

PHP:  "第一行\n第二行"
来源：http://fhx.ydjk.org.cn

JS:   "第一行\n第二行"
来源：http://ckx.gotoacloud.top

TS:   "第一行\n第二行"
来源：http://oui.xuetiantiany.cn

Java: "第一行\n第二行"
来源：http://yfq.xuanzx.com

Go:   "第一行\n第二行"
来源：http://qgv.0kj1m.cn

Ruby: "第一行\n第二行"
来源：http://bvw.birdmap.top

C#:   "第一行\n第二行"
来源：http://yjc.jqgufenzy.top

[A14] 注释写法
来源：http://wsy.sysykeji.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ene.vehdjk.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://ist.hcnkem.com

JS:   // 单行；/* 多行 */
来源：http://tae.gogol.net.cn

TS:   // 单行；/* 多行 */
来源：http://bnh.yuxming.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kjm.tian-w.cn

Go:   // 单行；/* 多行 */
来源：http://ihr.zhixingplan.top

Ruby: # 单行；=begin 多行 =end
来源：http://mev.jiagoushi.top

C#:   // 单行；/* 多行 */
来源：http://soe.daria6918.cn

[A15] 空值判断与默认值
来源：http://ngw.hywenlv.cn

Py:   value = data or "默认值"
来源：http://ffs.9152youxi.cn

PHP:  $value = $data ?? "默认值";
来源：http://won.yueranfly.top

JS:   const value = data ?? "默认值";
来源：http://fjl.yfazqb.com

TS:   const value = data ?? "默认值";
来源：http://zvg.meibo888.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qnl.hcnkem.com

Go:   if data == "" { data = "默认值" }
来源：http://cme.hnxiangtu.top

Ruby: value = data || "默认值"
来源：http://dyd.daria6918.cn

C#:   var value = data ?? "默认值";
来源：http://ert.sufxvd.cn

[A16] 真假值判断规则
来源：http://meb.jyoumei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pfj.shuidangran.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dkm.52xcode.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jbh.jqgufenzy.top

TS:   if (!x) {}
来源：http://obx.dashuyun.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ret.shangyingyoupin.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://irs.haohaochexian.top

Ruby: unless x            # nil 与 false 为假
来源：http://yeo.52xcode.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://taw.daxiang520.top

[A17] 位运算
来源：http://rxg.pengpengdd.cyou

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://svy.sxryk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xry.birdmap.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ymp.daxiang520.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://apb.tianlin.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://prx.havefunace.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uon.chenlongwang.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gwc.cucudq.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oab.shanyushiyangkeji.top

[A18] 字符与 ASCII 码互转
来源：http://asb.fengsongda.top

Py:   ord("A"); chr(65)
来源：http://hcr.ehwqpu.com

PHP:  ord("A"); chr(65)
来源：http://fgx.zhixingplan.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cho.pengpengdd.cyou

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://swy.daxiang520.top

Java: (int) 'A'; (char) 65
来源：http://giu.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://amb.zycfv.cn

Ruby: "A".ord; 65.chr
来源：http://fti.snrcjt.cn

C#:   (int)'A'; (char)65
来源：http://vqn.zhongyouzk.top

[A19] 交换两个变量
来源：http://wdg.vqdsnc.cn

Py:   a, b = b, a
来源：http://pfx.yanxiufei.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yjd.xziqi.cn

JS:   [a, b] = [b, a];
来源：http://isp.aizwys.cn

TS:   [a, b] = [b, a];
来源：http://gpq.birdmap.top

Java: int t = a; a = b; b = t;
来源：http://rjs.jinyuanbaomall.cn

Go:   a, b = b, a
来源：http://wef.kuanghao11.cn

Ruby: a, b = b, a
来源：http://rqn.tarul.cn

C#:   (a, b) = (b, a);
来源：http://bpj.vqdsnc.cn

[A20] 读取标准输入
来源：http://xhf.nanxinkj.top

Py:   name = input("请输入：")
来源：http://ktm.hysaishi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zch.yuanzhike.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://goq.quarkkingdee.top

TS:   // Node.js：readline 模块
来源：http://osf.zhengqikj.top

Java: new Scanner(System.in).nextLine()
来源：http://yjk.kuanghao11.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jta.zhaomingkeji.xyz

Ruby: gets.chomp
来源：http://usa.yonumen.top

C#:   Console.ReadLine();
来源：http://cgg.cqqwz.cn

[A21] 保留指定小数位输出
来源：http://nnj.fanxiaobao.xyz

Py:   f"{3.14159:.2f}"
来源：http://vtd.guowangkeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xsa.fengsongda.top

JS:   (3.14159).toFixed(2)
来源：http://sin.zhiwuduotai.top

TS:   (3.14159).toFixed(2)
来源：http://pkf.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://wed.hcnkem.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://aiv.epnwcf.com

Ruby: format("%.2f", 3.14159)
来源：http://vmm.aibaodan.cn

C#:   3.14159.ToString("F2")
来源：http://cvp.guannengcc.top

[A22] 获取字符串长度
来源：http://gnj.wangshuangyany.cn

Py:   len(s)
来源：http://hbu.smart0.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oct.ydjk.org.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yqf.nanxinkj.top

TS:   s.length
来源：http://inm.jianghu66.top

Java: s.length()
来源：http://lww.ppjwa.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iln.hnxiangtu.top

Ruby: s.length
来源：http://wwm.tian-w.cn

C#:   s.Length
来源：http://vxs.ywan-chungtsiang.top

[A23] 大小写转换
来源：http://adh.xingfuxueyuan.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://elz.hywenlv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qur.tian-w.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nsq.gzhubu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ypm.zhijiandao.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gug.uphjek.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rxh.xingfuxueyuan.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zgf.chenzaomai.com

C#:   s.ToUpper(); s.ToLower()
来源：http://cjx.tianlin.xyz

[A24] 去除首尾空白
来源：http://slf.vqdsnc.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dqq.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kfd.xylfe.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jbu.gaohongyu789.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iiu.meibo888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iqx.zhaomingkeji.xyz

Go:   strings.TrimSpace(s)
来源：http://ide.sysykeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sxv.xziqi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ehc.wangshuangyany.cn

[A25] 字符串比较
来源：http://szw.0kj1m.cn

Py:   s1 == s2; s1 != s2
来源：http://ola.zhijiandao.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vag.jinqigfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fft.9152youxi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://npg.ehwqpu.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kkb.ybcxt.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xbl.c1oappe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tnc.yvedp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vkx.xinyue.icu

[A26] 类型转换总览
来源：http://gav.xuetiantiany.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xvi.ivvv.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lhz.jqgfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sth.quarkkingdee.top

TS:   Number() String() Boolean() x as number
来源：http://gxp.tian-w.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nyy.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hrw.yangfankeji.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://dwa.wangshuangyany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yjz.mhx1999.top

================================================================================
来源：http://cbk.cashguo.top

B. 流程控制
来源：http://jkz.c1oappe.top

================================================================================
来源：http://ihc.chenzaomai.com

[B01] 条件判断 if / else
来源：http://spm.sysykeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jvn.tianlin.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vef.jinghuilouyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gyx.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://edj.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ixc.xuetiantiany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zsu.c1oappe.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lps.bbcook.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qdc.pycfn.com

[B02] 多分支 else if / elif
来源：http://qtu.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pqr.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gvp.aizwys.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gdv.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xsg.gotoacloud.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kdn.yangfankeji.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cgo.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tou.yvedp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://whl.yongpay.top

[B03] switch / match / case
来源：http://mib.gogol.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mip.aibaodan.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://erj.hnqzz.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hnj.hnqzz.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ign.52xcode.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sku.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vpv.guannengcc.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ybn.xylfe.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dge.hesvh.cn

[B04] for 计数循环
来源：http://kbb.0kj1m.cn

Py:   for i in range(10): print(i)
来源：http://ghr.shangyingyoupin.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gsu.yj20258.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rlh.cdnleiting.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fcq.shzxlz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hmn.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ojp.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://hpl.jinyuanbaomall.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ehb.andypj.xyz

[B05] 遍历数组 / 列表
来源：http://orh.tanke756.top

Py:   for item in arr: print(item)
来源：http://mdo.hywenlv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kjo.nanxuanxn.top

JS:   for (const item of arr) { console.log(item); }
来源：http://asu.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qlj.daxiang520.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tpr.hnqzz.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://awt.havefunace.top

Ruby: arr.each { |item| puts item }
来源：http://fhh.zhijiandao.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jfc.vqdsnc.cn

[B06] 遍历字典 / 对象
来源：http://uqd.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fph.fengsongda.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zzq.yj20258.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mpn.guannengcc.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qfa.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rhj.zdbjq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qjd.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://npe.yonumen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tvo.sjlbkw.cn

[B07] while 循环
来源：http://jtr.uphjek.com

Py:   while i < 10: i += 1
来源：http://pec.hysaishi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ery.cdnleiting.top

JS:   while (i < 10) { i++; }
来源：http://srg.cheryme.top

TS:   while (i < 10) { i++; }
来源：http://pce.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://aem.shanyushiyangtech.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rvh.316326.xyz

Ruby: while i < 10; i += 1; end
来源：http://xgk.ehwqpu.com

C#:   while (i < 10) { i++; }
来源：http://can.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://tqp.tanke756.top

Py:   # 无 do-while：用 while True + break
来源：http://rpq.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yoy.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://pvh.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://ptq.nanxinkj.top

Java: do { i++; } while (i < 10);
来源：http://ypd.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iem.zdbjq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qpw.ydjk.org.cn

C#:   do { i++; } while (i < 10);
来源：http://uek.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://nab.yuanzhike.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rgk.hcnkem.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mxv.gzhubu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sco.jyoumei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ldx.zhengqikj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fft.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qwc.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fhz.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://peu.shanyushiyangtech.top

[B10] 遍历同时拿索引
来源：http://dtm.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fnv.sweek.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tzn.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://idn.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bgd.andypj.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iil.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cvz.zhijiandao.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://drd.wangshuangyany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://urj.quarkkingdee.top

[B11] 生成数字序列 / 区间
来源：http://zga.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://jra.quarkkingdee.top

PHP:  range(0, 10, 2);
来源：http://ccj.feifeiyinyue.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qsl.tianlin.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uzs.ydzc1.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://psq.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fbf.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://xqv.shangyingyoupin.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oeq.xinyue.icu

[B12] 跳出多层循环
来源：http://snd.yuanzhike.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mrh.zdbjq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uqr.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ldw.sufxvd.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tis.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ocq.ydjk.org.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lnm.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fzu.nanxuanxn.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ixm.zhongyouzk.top

[B13] 判断是否为数字
来源：http://vef.hongshengwenyu.top

Py:   isinstance(x, (int, float))
来源：http://rqx.haohaochexian.top

PHP:  is_numeric($x)
来源：http://ggf.gaohongyu789.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qzj.zdqjudy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://whx.ehwqpu.com

Java: x instanceof Number
来源：http://bxi.yfazqb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ksq.tarul.cn

Ruby: x.is_a?(Numeric)
来源：http://fwv.ybcxt.top

C#:   x is int or double or decimal
来源：http://uld.c1oappe.top

[B14] 判断值是否在集合内
来源：http://gvn.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jaw.zhiwuduotai.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xbz.jinqigfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://sui.316326.xyz

TS:   [1, 2, 3].includes(x)
来源：http://cdz.jqgfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tie.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ohz.xylfe.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mjh.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://owt.ivvv.top

[B15] 布尔运算与取反
来源：http://sia.yvedp.cn

Py:   a and b or not c
来源：http://oub.pycfn.com

PHP:  $a && $b || !$c
来源：http://vfv.aibaodan.cn

JS:   a && b || !c
来源：http://zdf.iojbl.cn

TS:   a && b || !c
来源：http://ebj.xuetiantiany.cn

Java: a && b || !c
来源：http://imd.ydzc1.top

Go:   a && b || !c
来源：http://cqm.zycfv.cn

Ruby: a && b || !c
来源：http://cji.sysykeji.top

C#:   a && b || !c
来源：http://phi.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://nux.cucudq.cn

Py:   if not data: return
来源：http://bew.ybcxt.top

PHP:  if (!$data) { return; }
来源：http://bmk.9152youxi.cn

JS:   if (!data) return;
来源：http://kvp.hammf.cn

TS:   if (!data) return;
来源：http://qjp.hfpthk.cn

Java: if (data == null) return;
来源：http://enp.jinghuilouyu.cn

Go:   if data == nil { return }
来源：http://eld.chenzaomai.com

Ruby: return if data.nil?
来源：http://kot.nanxuanxn.top

C#:   if (data == null) return;
来源：http://wdd.jqgfzy.top

================================================================================
来源：http://gqh.shzxlz.cn

C. 函数与作用域
来源：http://hsw.c1oappe.top

================================================================================
来源：http://uyr.xinyue.icu

[C01] 定义函数
来源：http://vtf.xuetiantiany.cn

Py:   def add(a, b): return a + b
来源：http://zpy.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mkd.bjfxy.top

JS:   function add(a, b) { return a + b; }
来源：http://faa.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xyg.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://owt.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://yno.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://bor.c1oappe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vij.xylfe.cn

[C02] 默认参数
来源：http://skl.yongpay.top

Py:   def greet(name="World"): return name
来源：http://lrd.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qxm.zdqjudy.top

JS:   function greet(name = "World") { return name; }
来源：http://uzj.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cce.zdbjq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mqv.fanxiaobao.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hhe.316326.xyz

Ruby: def greet(name = "World") = name
来源：http://ayq.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://xwl.316326.xyz

[C03] 可变参数
来源：http://ydf.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://kmx.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cek.meibo888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ptj.vehdjk.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://suo.wangdashe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tyn.aibaodan.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hja.c1oappe.top


<!-- 参考信息 -->