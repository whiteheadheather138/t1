代发 wailian999

Java: "第一行\n第二行"
来源：http://qdb.ybcxt.top

Go:   "第一行\n第二行"
来源：http://lno.zhijiandao.cn

Ruby: "第一行\n第二行"
来源：http://zqq.yuanzhike.top

C#:   "第一行\n第二行"
来源：http://mea.c1oappe.top

[A14] 注释写法
来源：http://hyp.jqgfzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wtm.zhaomingkeji.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://vjx.dashuyun.cn

JS:   // 单行；/* 多行 */
来源：http://dhy.shzxlz.cn

TS:   // 单行；/* 多行 */
来源：http://vzl.9152youxi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sal.shzxlz.cn

Go:   // 单行；/* 多行 */
来源：http://zqz.fzhhl.top

Ruby: # 单行；=begin 多行 =end
来源：http://pse.hnxiangtu.top

C#:   // 单行；/* 多行 */
来源：http://beg.zhijiandao.cn

[A15] 空值判断与默认值
来源：http://rxj.chenjidiqi.icu

Py:   value = data or "默认值"
来源：http://isy.bjfxy.top

PHP:  $value = $data ?? "默认值";
来源：http://sof.aibaodan.cn

JS:   const value = data ?? "默认值";
来源：http://pfr.uphjek.com

TS:   const value = data ?? "默认值";
来源：http://ukp.daxiang520.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gez.yangfankeji.com

Go:   if data == "" { data = "默认值" }
来源：http://yve.wangdashe.top

Ruby: value = data || "默认值"
来源：http://gmm.yj20258888.top

C#:   var value = data ?? "默认值";
来源：http://ull.aizwys.cn

[A16] 真假值判断规则
来源：http://nvs.ywan-chungtsiang.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kmp.zhijiandao.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jsa.shanyushiyangtech.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ops.hnqzz.top

TS:   if (!x) {}
来源：http://erp.ydjk.org.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pml.c1oappe.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nll.iojbl.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sym.andypj.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wsv.fzhhl.top

[A17] 位运算
来源：http://zoa.yonumen.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jht.ivvv.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hws.wangdashe.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xvv.ydzc1.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://srt.meibo888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xab.hongshengwenyu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jpe.hcnkem.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bgn.jinqigfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xbm.zhixingplan.top

[A18] 字符与 ASCII 码互转
来源：http://bgi.shanyushiyangkeji.top

Py:   ord("A"); chr(65)
来源：http://qqo.fanxiaobao.xyz

PHP:  ord("A"); chr(65)
来源：http://xop.zycfv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uef.yj20258.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gky.xingfuxueyuan.xyz

Java: (int) 'A'; (char) 65
来源：http://buf.hfpthk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ndd.gogol.net.cn

Ruby: "A".ord; 65.chr
来源：http://ibc.yj20258.top

C#:   (int)'A'; (char)65
来源：http://rxk.guowangkeji.top

[A19] 交换两个变量
来源：http://olw.gogol.net.cn

Py:   a, b = b, a
来源：http://ttv.ybcxt.top

PHP:  [$a, $b] = [$b, $a];
来源：http://lmo.nanxinkj.top

JS:   [a, b] = [b, a];
来源：http://lhq.jianghu66.top

TS:   [a, b] = [b, a];
来源：http://sag.jyoumei.cn

Java: int t = a; a = b; b = t;
来源：http://rgg.xingfuxueyuan.xyz

Go:   a, b = b, a
来源：http://lnk.ehwqpu.com

Ruby: a, b = b, a
来源：http://stp.hnqzz.top

C#:   (a, b) = (b, a);
来源：http://lym.vqdsnc.cn

[A20] 读取标准输入
来源：http://jya.ppjwa.cn

Py:   name = input("请输入：")
来源：http://kjc.52xcode.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://riw.jqgufenzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://edr.yuanzhike.top

TS:   // Node.js：readline 模块
来源：http://bca.fktsv.cn

Java: new Scanner(System.in).nextLine()
来源：http://vea.sufxvd.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zvq.xziqi.cn

Ruby: gets.chomp
来源：http://yjn.yonumen.top

C#:   Console.ReadLine();
来源：http://lpb.pycfn.com

[A21] 保留指定小数位输出
来源：http://aer.guowangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://mbp.wangshuangyany.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fok.zhijiandao.cn

JS:   (3.14159).toFixed(2)
来源：http://goe.yvedp.cn

TS:   (3.14159).toFixed(2)
来源：http://upg.sweek.top

Java: String.format("%.2f", 3.14159)
来源：http://adv.yongpay.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dwi.ctjpmb.com

Ruby: format("%.2f", 3.14159)
来源：http://tye.0kj1m.cn

C#:   3.14159.ToString("F2")
来源：http://eco.havefunace.top

[A22] 获取字符串长度
来源：http://pya.fengsongda.top

Py:   len(s)
来源：http://gyf.sxryk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ehe.zdbjq.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vfj.aibaodan.cn

TS:   s.length
来源：http://mjr.pengpengdd.cyou

Java: s.length()
来源：http://zcz.ehwqpu.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tti.gogol.net.cn

Ruby: s.length
来源：http://enz.yfazqb.com

C#:   s.Length
来源：http://eup.bbcook.cn

[A23] 大小写转换
来源：http://cjf.jyoumei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pmj.ydjk.org.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zef.daxiang520.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jsq.jinqigfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dxx.c1oappe.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xyi.zhaomingkeji.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iqb.zhaomingkeji.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://exp.jinyuanbaomall.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kwh.bbcook.cn

[A24] 去除首尾空白
来源：http://oli.sjlbkw.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hrv.zhixingplan.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yqp.vehdjk.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fjz.sxryk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nqk.zhongyouzk.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mik.ppjwa.cn

Go:   strings.TrimSpace(s)
来源：http://wgl.kuanghao11.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fde.nanxuanxn.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jtr.cdnleiting.top

[A25] 字符串比较
来源：http://nui.chenzaomai.com

Py:   s1 == s2; s1 != s2
来源：http://xsg.0kj1m.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aft.shanyushiyangtech.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ifa.cdnleiting.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pjc.uphjek.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bos.dianchejie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://olz.hnqzz.top

Ruby: s1 == s2; s1 <=> s2
来源：http://pcf.tanke756.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gjp.cqqwz.cn

[A26] 类型转换总览
来源：http://yni.ydzc1.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nhn.zhoulong.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ubj.hywenlv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nnn.jlsjyb.cn

TS:   Number() String() Boolean() x as number
来源：http://ogp.nanxinkj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kza.aizwys.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sfg.guannengcc.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bym.redwolf501.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://duu.gaohongyu789.top

================================================================================
来源：http://oig.svipenyu.cn

B. 流程控制
来源：http://gqa.52xcode.cn

================================================================================
来源：http://sfv.vehdjk.com

[B01] 条件判断 if / else
来源：http://qez.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://cff.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tnh.wangdashe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ess.epnwcf.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lnj.epnwcf.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://tss.hesvh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://akn.chenzaomai.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pqb.chenzaomai.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pmu.vehdjk.com

[B02] 多分支 else if / elif
来源：http://faa.zhaomingkeji.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dpf.hesvh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yec.havefunace.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eyp.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bbq.kuanghao11.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bmd.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lvj.52xcode.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kni.gzhubu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://old.fehbvm.com

[B03] switch / match / case
来源：http://kyl.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://giv.quarkkingdee.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ign.nanxinkj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jhk.shuidangran.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hxr.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dcv.zdbjq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cxc.9152youxi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gkd.zhengqikj.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://owv.cdnleiting.top

[B04] for 计数循环
来源：http://bwm.sweek.top

Py:   for i in range(10): print(i)
来源：http://diy.andypj.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rdi.jiagoushi.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bub.vehdjk.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uoi.pengpengdd.cyou

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sjq.yongpay.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qvs.9152youxi.cn

Ruby: 10.times { |i| puts i }
来源：http://oje.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sye.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://bax.fanxiaobao.xyz

Py:   for item in arr: print(item)
来源：http://ssu.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jqa.chenzaomai.com

JS:   for (const item of arr) { console.log(item); }
来源：http://iqh.jiagoushi.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qsw.316326.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://chs.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oul.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://uss.jinqigfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vcs.hesvh.cn

[B06] 遍历字典 / 对象
来源：http://slc.snrcjt.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kyy.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://upw.gotoacloud.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://acn.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kgl.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://niv.kuanghao11.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://evi.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zjl.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wek.vehdjk.com

[B07] while 循环
来源：http://xxr.epnwcf.com

Py:   while i < 10: i += 1
来源：http://plo.0kj1m.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pqi.xinyue.icu

JS:   while (i < 10) { i++; }
来源：http://bod.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://xyx.xylfe.cn

Java: while (i < 10) { i++; }
来源：http://iek.hammf.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ujr.tianlin.xyz

Ruby: while i < 10; i += 1; end
来源：http://fdb.meibo888.top

C#:   while (i < 10) { i++; }
来源：http://mpc.ppjwa.cn

[B08] do-while（至少执行一次）
来源：http://yms.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://eiv.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://uog.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://kls.hnxiangtu.top

TS:   do { i++; } while (i < 10);
来源：http://ssp.cucudq.cn

Java: do { i++; } while (i < 10);
来源：http://njy.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jix.vqdsnc.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tji.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://zjk.guannengcc.top

[B09] break 与 continue
来源：http://vuk.zhixingplan.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ycf.iojbl.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wwb.hammf.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nca.zdqjudy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yzr.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pub.kuanghao11.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hhx.yonumen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wtn.sxryk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zez.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://iyb.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://edm.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vhg.guowangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nsq.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sry.smart0.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iyo.chenlongwang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vnj.shuidangran.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ota.yonumen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nmg.chenzaomai.com

[B11] 生成数字序列 / 区间
来源：http://pyt.jianghu66.top

Py:   list(range(0, 10, 2))
来源：http://umm.daria6918.cn

PHP:  range(0, 10, 2);
来源：http://sno.jinyuanbaomall.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://llf.hysaishi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fqa.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uvw.ctjpmb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xmj.sufxvd.cn

Ruby: (0...10).step(2).to_a
来源：http://hsx.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kfx.cdnleiting.top

[B12] 跳出多层循环
来源：http://jeg.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bwy.ppjwa.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ynr.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cen.ybcxt.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jxt.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lyt.ctjpmb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jjt.cdnleiting.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qxi.316326.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nsm.cdnleiting.top

[B13] 判断是否为数字
来源：http://fpd.guannengcc.top

Py:   isinstance(x, (int, float))
来源：http://txv.nwbrower.top

PHP:  is_numeric($x)
来源：http://vul.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qsq.gogol.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bup.daria6918.cn

Java: x instanceof Number
来源：http://ltw.pengpengdd.cyou

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zsc.quarkkingdee.top

Ruby: x.is_a?(Numeric)
来源：http://auh.sweek.top

C#:   x is int or double or decimal
来源：http://dij.mhx1999.top

[B14] 判断值是否在集合内
来源：http://crz.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tyz.chenlongwang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fov.jinghuilouyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://gkl.jinyuanbaomall.cn

TS:   [1, 2, 3].includes(x)
来源：http://gip.gaohongyu789.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fjb.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jyg.tarul.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hbm.yangfankeji.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://edm.yfazqb.com

[B15] 布尔运算与取反
来源：http://mkx.xylfe.cn

Py:   a and b or not c
来源：http://xts.sysykeji.top

PHP:  $a && $b || !$c
来源：http://ysl.hfpthk.cn

JS:   a && b || !c
来源：http://ftn.guowangkeji.top

TS:   a && b || !c
来源：http://iga.jlsjyb.cn

Java: a && b || !c
来源：http://xql.zhaomingkeji.xyz

Go:   a && b || !c
来源：http://ofw.sweek.top

Ruby: a && b || !c
来源：http://ekp.ctjpmb.com

C#:   a && b || !c
来源：http://auy.tarul.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fgp.316326.xyz

Py:   if not data: return
来源：http://lbh.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://bhx.zhaomingkeji.xyz

JS:   if (!data) return;
来源：http://ilz.sjlbkw.cn

TS:   if (!data) return;
来源：http://nhk.hongshengwenyu.top

Java: if (data == null) return;
来源：http://qrw.yuanzhike.top

Go:   if data == nil { return }
来源：http://enm.bjfxy.top

Ruby: return if data.nil?
来源：http://bcb.aibaodan.cn

C#:   if (data == null) return;
来源：http://rcl.chenjidiqi.icu

================================================================================
来源：http://vht.hysaishi.cn

C. 函数与作用域
来源：http://wsj.cucudq.cn

================================================================================
来源：http://mxs.redwolf501.top

[C01] 定义函数
来源：http://rph.52xcode.cn

Py:   def add(a, b): return a + b
来源：http://egc.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ofi.jinyuanbaomall.cn

JS:   function add(a, b) { return a + b; }
来源：http://mxe.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jtf.wangdashe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dis.wangshuangyany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ela.yangfankeji.com

Ruby: def add(a, b); a + b; end
来源：http://gcj.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kpc.jqgfzy.top

[C02] 默认参数
来源：http://aql.c1oappe.top

Py:   def greet(name="World"): return name
来源：http://iys.vehdjk.com

PHP:  function greet($name = "World") { return $name; }
来源：http://doh.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://nrs.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ren.andypj.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://fay.52xcode.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lyh.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://zmy.xylfe.cn

C#:   string Greet(string name = "World") => name;
来源：http://yfz.daxiang520.top

[C03] 可变参数
来源：http://hso.bbcook.cn

Py:   def total(*args): return sum(args)
来源：http://ffd.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://het.gzhubu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lrp.hcnkem.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fgg.jlsjyb.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dlv.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qjq.andypj.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://pgt.shangyingyoupin.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fvm.hnxiangtu.top

[C04] 命名参数 / 关键字参数
来源：http://wuj.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jko.jyoumei.cn


<!-- 参考信息 -->