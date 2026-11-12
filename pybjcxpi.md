代发 wailian999

Java: "第一行\n第二行"
来源：http://uat.xziqi.cn

Go:   "第一行\n第二行"
来源：http://pmp.smart0.xyz

Ruby: "第一行\n第二行"
来源：http://qkw.meibo888.top

C#:   "第一行\n第二行"
来源：http://ydc.zhengqikj.top

[A14] 注释写法
来源：http://vtz.yonumen.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://smj.nanxinkj.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dad.uphjek.com

JS:   // 单行；/* 多行 */
来源：http://wsg.uphjek.com

TS:   // 单行；/* 多行 */
来源：http://ggr.9152youxi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://iyl.hywenlv.cn

Go:   // 单行；/* 多行 */
来源：http://doc.ybcxt.top

Ruby: # 单行；=begin 多行 =end
来源：http://vaq.yj20258888.top

C#:   // 单行；/* 多行 */
来源：http://nnv.gaohongyu789.top

[A15] 空值判断与默认值
来源：http://eet.hywenlv.cn

Py:   value = data or "默认值"
来源：http://wgx.jiagoushi.top

PHP:  $value = $data ?? "默认值";
来源：http://oka.svipenyu.cn

JS:   const value = data ?? "默认值";
来源：http://ehz.jqgufenzy.top

TS:   const value = data ?? "默认值";
来源：http://etu.jinghuilouyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nww.chenjidiqi.icu

Go:   if data == "" { data = "默认值" }
来源：http://tuz.cucudq.cn

Ruby: value = data || "默认值"
来源：http://jsx.fktsv.cn

C#:   var value = data ?? "默认值";
来源：http://rap.xuanzx.com

[A16] 真假值判断规则
来源：http://gej.tianlin.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://shx.snrcjt.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bxe.xingfuxueyuan.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dtk.ydzc1.top

TS:   if (!x) {}
来源：http://wqo.zdbjq.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://giw.yanxiufei.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xam.zycfv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fam.xylfe.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://snw.sjlbkw.cn

[A17] 位运算
来源：http://uhr.xziqi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xzd.yonumen.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sxm.shuidangran.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tqs.tanke756.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yzg.zhixingplan.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nve.jqgufenzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fom.ybcxt.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jzl.xinyue.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vog.yj20258888.top

[A18] 字符与 ASCII 码互转
来源：http://ohv.cdnleiting.top

Py:   ord("A"); chr(65)
来源：http://ezc.cashguo.top

PHP:  ord("A"); chr(65)
来源：http://lmf.cqqwz.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nmx.fengsongda.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fai.guowangkeji.top

Java: (int) 'A'; (char) 65
来源：http://xes.yj20258888.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ukw.yvedp.cn

Ruby: "A".ord; 65.chr
来源：http://gmd.zhijiandao.cn

C#:   (int)'A'; (char)65
来源：http://ztd.haohaochexian.top

[A19] 交换两个变量
来源：http://fzj.meibo888.top

Py:   a, b = b, a
来源：http://ktp.daria6918.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vwa.jqgfzy.top

JS:   [a, b] = [b, a];
来源：http://opg.yuanzhike.top

TS:   [a, b] = [b, a];
来源：http://qek.dianchejie.cn

Java: int t = a; a = b; b = t;
来源：http://hvk.havefunace.top

Go:   a, b = b, a
来源：http://znf.zdbjq.cn

Ruby: a, b = b, a
来源：http://kew.ydjk.org.cn

C#:   (a, b) = (b, a);
来源：http://dab.yanxiufei.cn

[A20] 读取标准输入
来源：http://qdm.ppjwa.cn

Py:   name = input("请输入：")
来源：http://uxy.pengpengdd.cyou

PHP:  $name = trim(fgets(STDIN));
来源：http://ljf.gaohongyu789.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yrp.yj202588.top

TS:   // Node.js：readline 模块
来源：http://hnw.cqqwz.cn

Java: new Scanner(System.in).nextLine()
来源：http://yob.tianlin.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xdu.cdnleiting.top

Ruby: gets.chomp
来源：http://bzs.ybcxt.top

C#:   Console.ReadLine();
来源：http://jim.vehdjk.com

[A21] 保留指定小数位输出
来源：http://ptt.birdmap.top

Py:   f"{3.14159:.2f}"
来源：http://zml.zhoulong.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pwu.fehbvm.com

JS:   (3.14159).toFixed(2)
来源：http://bva.birdmap.top

TS:   (3.14159).toFixed(2)
来源：http://xcw.tanke756.top

Java: String.format("%.2f", 3.14159)
来源：http://loq.jinghuilouyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ooz.zycfv.cn

Ruby: format("%.2f", 3.14159)
来源：http://zco.chenzaomai.com

C#:   3.14159.ToString("F2")
来源：http://jbh.shzxlz.cn

[A22] 获取字符串长度
来源：http://hss.jiagoushi.top

Py:   len(s)
来源：http://dpb.ydjk.org.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hip.guannengcc.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uvr.pycfn.com

TS:   s.length
来源：http://hpt.zhiwuduotai.top

Java: s.length()
来源：http://bck.zhongyouzk.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hyc.yj202588.top

Ruby: s.length
来源：http://yro.xylfe.cn

C#:   s.Length
来源：http://dwa.vqdsnc.cn

[A23] 大小写转换
来源：http://wde.hongshengwenyu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lgj.pengpengdd.cyou

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hjz.zhoulong.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hlc.hnqzz.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kkb.316326.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dvy.nanxuanxn.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://peh.hywenlv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dsn.zhijiandao.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pqi.daria6918.cn

[A24] 去除首尾空白
来源：http://mew.sxryk.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sxd.gotoacloud.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vrg.jinqigufen.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://svm.gogol.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hnn.daxiang520.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qjs.sjlbkw.cn

Go:   strings.TrimSpace(s)
来源：http://edq.chenzaomai.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nft.hcnkem.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xin.fktsv.cn

[A25] 字符串比较
来源：http://nor.hysaishi.cn

Py:   s1 == s2; s1 != s2
来源：http://gmv.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ahf.bjfxy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dft.hesvh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gon.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oks.ivvv.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qxm.shangyingyoupin.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tic.bbcook.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yzt.chenlongwang.top

[A26] 类型转换总览
来源：http://vxq.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://agt.yj20258888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cnh.epnwcf.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ltf.chenjidiqi.icu

TS:   Number() String() Boolean() x as number
来源：http://oni.ydjk.org.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qtv.yongpay.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sqn.chenlongwang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xrr.jinqigfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ydf.pengpengdd.cyou

================================================================================
来源：http://rzt.tian-w.cn

B. 流程控制
来源：http://ctx.epnwcf.com

================================================================================
来源：http://azr.sweek.top

[B01] 条件判断 if / else
来源：http://prm.fzhhl.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gur.epnwcf.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cpv.tianlin.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jou.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://phu.chenjidiqi.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://jpt.yfazqb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tbl.yanxiufei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://khw.fengsongda.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dom.yuxming.cn

[B02] 多分支 else if / elif
来源：http://lpx.tanke756.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sis.yfazqb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vci.zhixingplan.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zrt.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ujo.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://evq.fzhhl.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cwq.zhixingplan.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kin.ydjk.org.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ool.ybcxt.top

[B03] switch / match / case
来源：http://crw.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wqv.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lzx.redwolf501.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dkz.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ujv.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wdr.nanxinkj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hgh.yj20258888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yfk.andypj.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nnd.snrcjt.cn

[B04] for 计数循环
来源：http://clz.zdbjq.cn

Py:   for i in range(10): print(i)
来源：http://oua.yj20258888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://osj.xuetiantiany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kzw.yj20258888.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xgq.ehwqpu.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wam.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vod.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://kcj.tian-w.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rew.hywenlv.cn

[B05] 遍历数组 / 列表
来源：http://bqy.yonumen.top

Py:   for item in arr: print(item)
来源：http://ygu.zhengqikj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ile.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lzi.yueranfly.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vui.hnxiangtu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pyl.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xir.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://dee.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ive.yfazqb.com

[B06] 遍历字典 / 对象
来源：http://qfr.zhiwuduotai.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ifv.ywan-chungtsiang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tom.yvedp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://evg.tanke756.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ziz.hfpthk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iir.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nca.c1oappe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kot.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://thm.9152youxi.cn

[B07] while 循环
来源：http://hfa.zhaomingkeji.xyz

Py:   while i < 10: i += 1
来源：http://ybf.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://exl.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://ncy.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://puo.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://leb.yongpay.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://efl.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://pbx.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://mnn.pycfn.com

[B08] do-while（至少执行一次）
来源：http://cyz.fengsongda.top

Py:   # 无 do-while：用 while True + break
来源：http://eak.zdqjudy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kyx.ctjpmb.com

JS:   do { i++; } while (i < 10);
来源：http://apg.shzxlz.cn

TS:   do { i++; } while (i < 10);
来源：http://phe.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://xju.yfazqb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://hcq.9152youxi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jdw.zhaomingkeji.xyz

C#:   do { i++; } while (i < 10);
来源：http://dzq.aizwys.cn

[B09] break 与 continue
来源：http://bfd.chenlongwang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bvz.iojbl.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://caj.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hmj.quarkkingdee.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mil.gaohongyu789.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fie.wangshuangyany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rpk.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jec.hywenlv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nco.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://qzc.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://psl.hcnkem.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gqd.iojbl.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gwf.tanke756.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://quv.xuanzx.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aif.316326.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uki.xingfuxueyuan.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://exe.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yjc.fanxiaobao.xyz

[B11] 生成数字序列 / 区间
来源：http://fep.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://ztg.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://xfj.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sqv.hysaishi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vpb.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oeg.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fex.gaohongyu789.top

Ruby: (0...10).step(2).to_a
来源：http://njd.bjfxy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ebr.shangyingyoupin.top

[B12] 跳出多层循环
来源：http://hpi.ehwqpu.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://odt.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://mfs.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pff.tian-w.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tme.fktsv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cfx.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hnp.hfpthk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mdu.gaohongyu789.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qrl.ydzc1.top

[B13] 判断是否为数字
来源：http://tpe.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://byx.pengpengdd.cyou

PHP:  is_numeric($x)
来源：http://mni.xuanzx.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vij.tanke756.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ttv.jinqigfzy.top

Java: x instanceof Number
来源：http://lsl.yuanzhike.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gza.nwbrower.top

Ruby: x.is_a?(Numeric)
来源：http://sby.daxiang520.top

C#:   x is int or double or decimal
来源：http://vwh.hammf.cn

[B14] 判断值是否在集合内
来源：http://qdk.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uga.nanxinkj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hce.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://ukm.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://wke.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wjv.epnwcf.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iry.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oxj.zdbjq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hti.cucudq.cn

[B15] 布尔运算与取反
来源：http://gqh.sweek.top

Py:   a and b or not c
来源：http://sie.quarkkingdee.top

PHP:  $a && $b || !$c
来源：http://xzd.cheryme.top

JS:   a && b || !c
来源：http://qwa.guowangkeji.top

TS:   a && b || !c
来源：http://fde.xuetiantiany.cn

Java: a && b || !c
来源：http://gxu.epnwcf.com

Go:   a && b || !c
来源：http://fhn.9152youxi.cn

Ruby: a && b || !c
来源：http://otq.fzhhl.top

C#:   a && b || !c
来源：http://ven.hfpthk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vly.pycfn.com

Py:   if not data: return
来源：http://toi.c1oappe.top

PHP:  if (!$data) { return; }
来源：http://fde.zdqjudy.top

JS:   if (!data) return;
来源：http://awq.svipenyu.cn

TS:   if (!data) return;
来源：http://pvp.hywenlv.cn

Java: if (data == null) return;
来源：http://owp.nanxuanxn.top

Go:   if data == nil { return }
来源：http://hwi.shangyingyoupin.top

Ruby: return if data.nil?
来源：http://gfm.xingfuxueyuan.xyz

C#:   if (data == null) return;
来源：http://snw.tian-w.cn

================================================================================
来源：http://hia.xuetiantiany.cn

C. 函数与作用域
来源：http://aab.feifeiyinyue.top

================================================================================
来源：http://qhj.shzxlz.cn

[C01] 定义函数
来源：http://buj.ehwqpu.com

Py:   def add(a, b): return a + b
来源：http://emj.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://djv.xuetiantiany.cn

JS:   function add(a, b) { return a + b; }
来源：http://bzd.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://non.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lyz.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://jfo.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://uvt.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bbo.316326.xyz

[C02] 默认参数
来源：http://ifu.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://xut.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vpy.birdmap.top

JS:   function greet(name = "World") { return name; }
来源：http://hxh.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tir.hesvh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zgi.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://egh.dashuyun.cn

Ruby: def greet(name = "World") = name
来源：http://itr.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://fgh.yj20258888.top

[C03] 可变参数
来源：http://jof.jianghu66.top

Py:   def total(*args): return sum(args)
来源：http://vwm.bjfxy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xkn.sxryk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wma.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lzb.sxryk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pte.zhengqikj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qyu.ehwqpu.com

Ruby: def total(*nums); nums.sum; end
来源：http://zvj.jyoumei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://adb.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://zhb.jyoumei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://djc.hammf.cn


<!-- 参考信息 -->