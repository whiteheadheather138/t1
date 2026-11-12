代发 wailian999

Py:   "第一行\n第二行"
来源：http://ayw.bbcook.cn

PHP:  "第一行\n第二行"
来源：http://jro.sysykeji.top

JS:   "第一行\n第二行"
来源：http://pez.ydjk.org.cn

TS:   "第一行\n第二行"
来源：http://asx.ywan-chungtsiang.top

Java: "第一行\n第二行"
来源：http://rcu.hongshengwenyu.top

Go:   "第一行\n第二行"
来源：http://isx.wangshuangyany.cn

Ruby: "第一行\n第二行"
来源：http://fuw.chenlongwang.top

C#:   "第一行\n第二行"
来源：http://eay.smart0.xyz

[A14] 注释写法
来源：http://ubk.shzxlz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jip.zhengqikj.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://fxz.nwbrower.top

JS:   // 单行；/* 多行 */
来源：http://qaz.cqqwz.cn

TS:   // 单行；/* 多行 */
来源：http://rmz.zycfv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ner.ydjk.org.cn

Go:   // 单行；/* 多行 */
来源：http://igk.nanxinkj.top

Ruby: # 单行；=begin 多行 =end
来源：http://oqm.snrcjt.cn

C#:   // 单行；/* 多行 */
来源：http://oyo.cucudq.cn

[A15] 空值判断与默认值
来源：http://kkj.jinqigufen.top

Py:   value = data or "默认值"
来源：http://wrn.fktsv.cn

PHP:  $value = $data ?? "默认值";
来源：http://scu.bbcook.cn

JS:   const value = data ?? "默认值";
来源：http://qjr.vehdjk.com

TS:   const value = data ?? "默认值";
来源：http://tdx.9152youxi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dvp.shanyushiyangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://sys.tian-w.cn

Ruby: value = data || "默认值"
来源：http://jcv.zhijiandao.cn

C#:   var value = data ?? "默认值";
来源：http://lpy.zhixingplan.top

[A16] 真假值判断规则
来源：http://dlu.nwbrower.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zbn.zhoulong.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hjk.aibaodan.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kvt.hcnkem.com

TS:   if (!x) {}
来源：http://nbe.jinqigfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wmt.shanyushiyangtech.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://haa.svipenyu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kdi.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rqy.jlsjyb.cn

[A17] 位运算
来源：http://jpo.tanke756.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://csd.snrcjt.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sfe.zhoulong.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iim.jianghu66.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hgp.nanxuanxn.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kjo.ybcxt.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ghk.316326.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uis.gaohongyu789.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://czp.xuetiantiany.cn

[A18] 字符与 ASCII 码互转
来源：http://rre.jqgfzy.top

Py:   ord("A"); chr(65)
来源：http://kvr.yfazqb.com

PHP:  ord("A"); chr(65)
来源：http://jgr.hongshengwenyu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dsn.tarul.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sbz.yj20258.top

Java: (int) 'A'; (char) 65
来源：http://wtp.jyoumei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dgn.zhijiandao.cn

Ruby: "A".ord; 65.chr
来源：http://mnk.jiagoushi.top

C#:   (int)'A'; (char)65
来源：http://knb.zhaomingkeji.xyz

[A19] 交换两个变量
来源：http://lfp.hnxiangtu.top

Py:   a, b = b, a
来源：http://dvo.zhengqikj.top

PHP:  [$a, $b] = [$b, $a];
来源：http://sit.iojbl.cn

JS:   [a, b] = [b, a];
来源：http://rdk.tian-w.cn

TS:   [a, b] = [b, a];
来源：http://pbu.yj20258.top

Java: int t = a; a = b; b = t;
来源：http://euu.nanxuanxn.top

Go:   a, b = b, a
来源：http://smh.birdmap.top

Ruby: a, b = b, a
来源：http://wbx.fehbvm.com

C#:   (a, b) = (b, a);
来源：http://ocw.zhengqikj.top

[A20] 读取标准输入
来源：http://qwz.sufxvd.cn

Py:   name = input("请输入：")
来源：http://rny.havefunace.top

PHP:  $name = trim(fgets(STDIN));
来源：http://pjb.zdbjq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xwj.meibo888.top

TS:   // Node.js：readline 模块
来源：http://vlq.yj202588.top

Java: new Scanner(System.in).nextLine()
来源：http://mqi.0kj1m.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ojo.bjfxy.top

Ruby: gets.chomp
来源：http://aat.epnwcf.com

C#:   Console.ReadLine();
来源：http://hbk.yuanzhike.top

[A21] 保留指定小数位输出
来源：http://uqk.bjfxy.top

Py:   f"{3.14159:.2f}"
来源：http://niy.zycfv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://csb.9152youxi.cn

JS:   (3.14159).toFixed(2)
来源：http://fwp.hnxiangtu.top

TS:   (3.14159).toFixed(2)
来源：http://wqu.nanxuanxn.top

Java: String.format("%.2f", 3.14159)
来源：http://gxs.aizwys.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dwn.316326.xyz

Ruby: format("%.2f", 3.14159)
来源：http://koa.hammf.cn

C#:   3.14159.ToString("F2")
来源：http://xfn.mhx1999.top

[A22] 获取字符串长度
来源：http://izc.dashuyun.cn

Py:   len(s)
来源：http://mpw.dashuyun.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cgo.nanxuanxn.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tmb.dashuyun.cn

TS:   s.length
来源：http://dpb.hywenlv.cn

Java: s.length()
来源：http://nzr.zhixingplan.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hbe.pycfn.com

Ruby: s.length
来源：http://dkk.haohaochexian.top

C#:   s.Length
来源：http://ztd.shzxlz.cn

[A23] 大小写转换
来源：http://rgd.guowangkeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xou.daria6918.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zwx.svipenyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zqp.hcnkem.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cnr.smart0.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mdm.shuidangran.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://skq.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zgy.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://uxh.yfazqb.com

[A24] 去除首尾空白
来源：http://plu.shzxlz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ddc.pycfn.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xiq.9152youxi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kbp.jlsjyb.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://csg.xuanzx.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dtv.xziqi.cn

Go:   strings.TrimSpace(s)
来源：http://pvd.jqgfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xaj.daria6918.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tkh.tianlin.xyz

[A25] 字符串比较
来源：http://ccj.shanyushiyangtech.top

Py:   s1 == s2; s1 != s2
来源：http://kre.tianlin.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lta.shanyushiyangtech.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://udh.xingfuxueyuan.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cnh.haohaochexian.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nat.jqgufenzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fha.yvedp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nxf.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lru.xuanzx.com

[A26] 类型转换总览
来源：http://kft.gotoacloud.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cmz.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wsh.dashuyun.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mau.chenzaomai.com

TS:   Number() String() Boolean() x as number
来源：http://url.cheryme.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eic.shanyushiyangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lia.zhixingplan.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rwi.aibaodan.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vnx.zhaomingkeji.xyz

================================================================================
来源：http://jul.bbcook.cn

B. 流程控制
来源：http://ykd.zdqjudy.top

================================================================================
来源：http://oig.ybcxt.top

[B01] 条件判断 if / else
来源：http://xcp.iojbl.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rcc.shzxlz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fha.hnqzz.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yek.jqgfzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ejb.zhoulong.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://rxe.cheryme.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cra.sjlbkw.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rhi.yueranfly.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xon.nanxinkj.top

[B02] 多分支 else if / elif
来源：http://iqu.yvedp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vok.dashuyun.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qfh.jqgfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mlq.xingfuxueyuan.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pzb.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vdt.gzhubu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yar.tian-w.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eoh.nanxinkj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qnr.fengsongda.top

[B03] switch / match / case
来源：http://gmc.gaohongyu789.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iep.shanyushiyangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sns.vqdsnc.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wlp.yj20258888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://snh.kuanghao11.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://axg.jyoumei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dol.hfpthk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uae.wangdashe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bdl.sysykeji.top

[B04] for 计数循环
来源：http://ppo.chenlongwang.top

Py:   for i in range(10): print(i)
来源：http://pia.jinyuanbaomall.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://job.jlsjyb.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://clo.daxiang520.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lhn.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://glv.ybcxt.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gnz.epnwcf.com

Ruby: 10.times { |i| puts i }
来源：http://mmc.fktsv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jpo.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://sjj.chenjidiqi.icu

Py:   for item in arr: print(item)
来源：http://awp.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://klk.chenlongwang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qtj.ywan-chungtsiang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://eot.tanke756.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://erb.yangfankeji.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://okh.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://arw.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kzl.sjlbkw.cn

[B06] 遍历字典 / 对象
来源：http://uoo.cashguo.top

Py:   for k, v in d.items(): print(k, v)
来源：http://svi.yongpay.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rwu.yonumen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zli.ywan-chungtsiang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://woh.zdbjq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://afg.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fet.chenjidiqi.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rcb.zdbjq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fkv.chenzaomai.com

[B07] while 循环
来源：http://lxf.gzhubu.top

Py:   while i < 10: i += 1
来源：http://tvj.shzxlz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gxt.birdmap.top

JS:   while (i < 10) { i++; }
来源：http://mrn.shzxlz.cn

TS:   while (i < 10) { i++; }
来源：http://roa.yonumen.top

Java: while (i < 10) { i++; }
来源：http://shm.tian-w.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://otl.tarul.cn

Ruby: while i < 10; i += 1; end
来源：http://msi.jianghu66.top

C#:   while (i < 10) { i++; }
来源：http://utt.c1oappe.top

[B08] do-while（至少执行一次）
来源：http://gql.yj20258888.top

Py:   # 无 do-while：用 while True + break
来源：http://wic.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ruf.yongpay.top

JS:   do { i++; } while (i < 10);
来源：http://fkj.hesvh.cn

TS:   do { i++; } while (i < 10);
来源：http://bpl.pycfn.com

Java: do { i++; } while (i < 10);
来源：http://bwn.zhengqikj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zqe.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wcf.hywenlv.cn

C#:   do { i++; } while (i < 10);
来源：http://gzr.yongpay.top

[B09] break 与 continue
来源：http://zkh.xuanzx.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://llk.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oks.guowangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lct.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bxc.cqqwz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jjb.cashguo.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uml.cdnleiting.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lzr.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sri.daxiang520.top

[B10] 遍历同时拿索引
来源：http://lhv.kuanghao11.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ezl.ctjpmb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kxl.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kds.aibaodan.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oif.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mnw.jinghuilouyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ywh.xingfuxueyuan.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hof.andypj.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yih.zhoulong.xyz

[B11] 生成数字序列 / 区间
来源：http://yqy.vqdsnc.cn

Py:   list(range(0, 10, 2))
来源：http://djr.mhx1999.top

PHP:  range(0, 10, 2);
来源：http://cbj.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xot.snrcjt.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cbp.yuxming.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lwg.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sxf.vehdjk.com

Ruby: (0...10).step(2).to_a
来源：http://omk.yj20258.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zer.yj20258888.top

[B12] 跳出多层循环
来源：http://bqh.yongpay.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dgx.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uql.chenjidiqi.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hkf.vqdsnc.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xwp.gaohongyu789.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dne.kuanghao11.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nrc.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wva.uphjek.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xed.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://xso.nanxuanxn.top

Py:   isinstance(x, (int, float))
来源：http://qre.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://kxy.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ocm.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kes.guannengcc.top

Java: x instanceof Number
来源：http://rit.svipenyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ssf.zdqjudy.top

Ruby: x.is_a?(Numeric)
来源：http://uay.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://gcd.daxiang520.top

[B14] 判断值是否在集合内
来源：http://mjy.shanyushiyangtech.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rbi.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://omd.feifeiyinyue.top

JS:   [1, 2, 3].includes(x)
来源：http://plz.shangyingyoupin.top

TS:   [1, 2, 3].includes(x)
来源：http://uma.sxryk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://olk.vqdsnc.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mgp.zhengqikj.top

Ruby: [1, 2, 3].include?(x)
来源：http://sye.snrcjt.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kqn.ehwqpu.com

[B15] 布尔运算与取反
来源：http://prk.hongshengwenyu.top

Py:   a and b or not c
来源：http://ody.jlsjyb.cn

PHP:  $a && $b || !$c
来源：http://lhb.andypj.xyz

JS:   a && b || !c
来源：http://lmq.wangdashe.top

TS:   a && b || !c
来源：http://ifa.xuetiantiany.cn

Java: a && b || !c
来源：http://dsf.zhaomingkeji.xyz

Go:   a && b || !c
来源：http://vvc.0kj1m.cn

Ruby: a && b || !c
来源：http://zes.gogol.net.cn

C#:   a && b || !c
来源：http://qdn.smart0.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://xhw.mhx1999.top

Py:   if not data: return
来源：http://hqm.nanxuanxn.top

PHP:  if (!$data) { return; }
来源：http://htz.svipenyu.cn

JS:   if (!data) return;
来源：http://lta.iojbl.cn

TS:   if (!data) return;
来源：http://nah.guannengcc.top

Java: if (data == null) return;
来源：http://cmu.daria6918.cn

Go:   if data == nil { return }
来源：http://hbc.jqgufenzy.top

Ruby: return if data.nil?
来源：http://ohu.sweek.top

C#:   if (data == null) return;
来源：http://xld.tian-w.cn

================================================================================
来源：http://gxl.yangfankeji.com

C. 函数与作用域
来源：http://rsw.xuanzx.com

================================================================================
来源：http://dzr.daria6918.cn

[C01] 定义函数
来源：http://dej.sjlbkw.cn

Py:   def add(a, b): return a + b
来源：http://cej.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jue.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://svz.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hdw.xziqi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yfc.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vfp.jiagoushi.top

Ruby: def add(a, b); a + b; end
来源：http://ezt.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bmi.pengpengdd.cyou

[C02] 默认参数
来源：http://vkt.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://djh.cheryme.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zjf.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://bpe.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qch.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dfr.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tvg.sjlbkw.cn

Ruby: def greet(name = "World") = name
来源：http://evy.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://nip.gaohongyu789.top

[C03] 可变参数
来源：http://itf.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://jyo.hongshengwenyu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dki.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hqf.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gvn.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vdn.zdqjudy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mvr.52xcode.cn


<!-- 参考信息 -->