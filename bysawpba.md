代发 wailian999

Java: "第一行\n第二行"
来源：http://gir.c1oappe.top

Go:   "第一行\n第二行"
来源：http://slq.xingfuxueyuan.xyz

Ruby: "第一行\n第二行"
来源：http://wbf.zycfv.cn

C#:   "第一行\n第二行"
来源：http://ztd.kuanghao11.cn

[A14] 注释写法
来源：http://ztd.zhaomingkeji.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://rom.tian-w.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nkt.sufxvd.cn

JS:   // 单行；/* 多行 */
来源：http://ftb.zhoulong.xyz

TS:   // 单行；/* 多行 */
来源：http://eod.tian-w.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cnr.jqgfzy.top

Go:   // 单行；/* 多行 */
来源：http://bjw.ydzc1.top

Ruby: # 单行；=begin 多行 =end
来源：http://iju.aizwys.cn

C#:   // 单行；/* 多行 */
来源：http://hse.fengsongda.top

[A15] 空值判断与默认值
来源：http://vjl.gotoacloud.top

Py:   value = data or "默认值"
来源：http://hqe.dashuyun.cn

PHP:  $value = $data ?? "默认值";
来源：http://bis.zdqjudy.top

JS:   const value = data ?? "默认值";
来源：http://per.pengpengdd.cyou

TS:   const value = data ?? "默认值";
来源：http://otq.tianlin.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zoz.aibaodan.cn

Go:   if data == "" { data = "默认值" }
来源：http://arq.ybcxt.top

Ruby: value = data || "默认值"
来源：http://yyi.xuetiantiany.cn

C#:   var value = data ?? "默认值";
来源：http://org.c1oappe.top

[A16] 真假值判断规则
来源：http://csx.fktsv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pxk.nanxuanxn.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://glq.shzxlz.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uyt.yj20258.top

TS:   if (!x) {}
来源：http://irp.yonumen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tes.epnwcf.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yrq.tian-w.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lsu.yonumen.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dpk.shanyushiyangtech.top

[A17] 位运算
来源：http://xjy.tanke756.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dtu.dashuyun.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tto.jlsjyb.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fgw.hfpthk.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bnl.yueranfly.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kkh.yfazqb.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://snl.yuxming.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uju.andypj.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rqs.zhongyouzk.top

[A18] 字符与 ASCII 码互转
来源：http://abt.sysykeji.top

Py:   ord("A"); chr(65)
来源：http://svo.yueranfly.top

PHP:  ord("A"); chr(65)
来源：http://ewx.cashguo.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rwn.svipenyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vif.snrcjt.cn

Java: (int) 'A'; (char) 65
来源：http://qvr.birdmap.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jzi.hammf.cn

Ruby: "A".ord; 65.chr
来源：http://yws.jinqigufen.top

C#:   (int)'A'; (char)65
来源：http://loo.chenjidiqi.icu

[A19] 交换两个变量
来源：http://phj.aibaodan.cn

Py:   a, b = b, a
来源：http://pgw.hcnkem.com

PHP:  [$a, $b] = [$b, $a];
来源：http://lry.kuanghao11.cn

JS:   [a, b] = [b, a];
来源：http://jen.sweek.top

TS:   [a, b] = [b, a];
来源：http://bxy.smart0.xyz

Java: int t = a; a = b; b = t;
来源：http://kkn.jqgfzy.top

Go:   a, b = b, a
来源：http://pcr.cheryme.top

Ruby: a, b = b, a
来源：http://txd.yonumen.top

C#:   (a, b) = (b, a);
来源：http://yrw.kuanghao11.cn

[A20] 读取标准输入
来源：http://zsf.zhoulong.xyz

Py:   name = input("请输入：")
来源：http://icr.daxiang520.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rcd.jinghuilouyu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bac.zhoulong.xyz

TS:   // Node.js：readline 模块
来源：http://yqf.ybcxt.top

Java: new Scanner(System.in).nextLine()
来源：http://dks.yuxming.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pxa.yuxming.cn

Ruby: gets.chomp
来源：http://dxl.yj20258.top

C#:   Console.ReadLine();
来源：http://ngz.ydzc1.top

[A21] 保留指定小数位输出
来源：http://vzj.ppjwa.cn

Py:   f"{3.14159:.2f}"
来源：http://qeq.yangfankeji.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wcd.fzhhl.top

JS:   (3.14159).toFixed(2)
来源：http://pod.sysykeji.top

TS:   (3.14159).toFixed(2)
来源：http://mhg.quarkkingdee.top

Java: String.format("%.2f", 3.14159)
来源：http://ybo.yj202588.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kpy.uphjek.com

Ruby: format("%.2f", 3.14159)
来源：http://gfc.quarkkingdee.top

C#:   3.14159.ToString("F2")
来源：http://hcw.yuxming.cn

[A22] 获取字符串长度
来源：http://kki.jianghu66.top

Py:   len(s)
来源：http://feb.cashguo.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rjq.0kj1m.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zdv.hnxiangtu.top

TS:   s.length
来源：http://tst.snrcjt.cn

Java: s.length()
来源：http://zdg.tian-w.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xuf.zhiwuduotai.top

Ruby: s.length
来源：http://olf.andypj.xyz

C#:   s.Length
来源：http://lcq.chenlongwang.top

[A23] 大小写转换
来源：http://xzo.kuanghao11.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pxy.9152youxi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yzq.meibo888.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oos.chenlongwang.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jek.hongshengwenyu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pim.xuetiantiany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yrh.nanxinkj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ghs.jinghuilouyu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://roa.bbcook.cn

[A24] 去除首尾空白
来源：http://mgp.jyoumei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eiv.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uyf.gogol.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mzt.ehwqpu.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://man.hnxiangtu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://onu.fanxiaobao.xyz

Go:   strings.TrimSpace(s)
来源：http://xht.chenlongwang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gmh.hesvh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nbt.feifeiyinyue.top

[A25] 字符串比较
来源：http://sbf.xingfuxueyuan.xyz

Py:   s1 == s2; s1 != s2
来源：http://gyy.wangdashe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vhb.sxryk.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vmp.sjlbkw.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://trk.yuxming.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qbr.sxryk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ahe.xziqi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vaz.jinyuanbaomall.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bkz.jyoumei.cn

[A26] 类型转换总览
来源：http://rro.xingfuxueyuan.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dtt.0kj1m.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ves.jlsjyb.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gtc.zhaomingkeji.xyz

TS:   Number() String() Boolean() x as number
来源：http://akh.tianlin.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pvf.andypj.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zwk.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tjg.nanxuanxn.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bsm.316326.xyz

================================================================================
来源：http://mhi.sysykeji.top

B. 流程控制
来源：http://wyx.mhx1999.top

================================================================================
来源：http://vrc.xingfuxueyuan.xyz

[B01] 条件判断 if / else
来源：http://yrh.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vba.aibaodan.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://klg.dianchejie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iyk.vqdsnc.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rxn.316326.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://swh.wangdashe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kli.cucudq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hzq.epnwcf.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ogv.hcnkem.com

[B02] 多分支 else if / elif
来源：http://heb.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pjs.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lac.zhoulong.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ypu.ywan-chungtsiang.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uug.gotoacloud.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://atb.fanxiaobao.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iat.zdbjq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bha.fktsv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://myy.wangdashe.top

[B03] switch / match / case
来源：http://vkx.xuetiantiany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://efp.smart0.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fjj.wangdashe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://psv.hesvh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bey.jyoumei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://swd.gotoacloud.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ixu.svipenyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yvs.vqdsnc.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://owe.hfpthk.cn

[B04] for 计数循环
来源：http://ufy.hongshengwenyu.top

Py:   for i in range(10): print(i)
来源：http://xst.xuetiantiany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ipi.dashuyun.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iwg.jinqigfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tqx.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jph.hesvh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://idy.tian-w.cn

Ruby: 10.times { |i| puts i }
来源：http://bau.ehwqpu.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qrn.haohaochexian.top

[B05] 遍历数组 / 列表
来源：http://jdl.ybcxt.top

Py:   for item in arr: print(item)
来源：http://ruk.sufxvd.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fze.uphjek.com

JS:   for (const item of arr) { console.log(item); }
来源：http://irx.hammf.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bqg.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wjf.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pkz.fzhhl.top

Ruby: arr.each { |item| puts item }
来源：http://xmd.gogol.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ugi.dianchejie.cn

[B06] 遍历字典 / 对象
来源：http://yjx.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://jkx.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kth.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zft.sweek.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hyb.andypj.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ekq.hongshengwenyu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dnk.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://unx.gzhubu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rne.ppjwa.cn

[B07] while 循环
来源：http://nma.vqdsnc.cn

Py:   while i < 10: i += 1
来源：http://puk.zdqjudy.top

PHP:  while ($i < 10) { $i++; }
来源：http://ite.yj20258.top

JS:   while (i < 10) { i++; }
来源：http://gtg.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://ysc.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://zfa.yanxiufei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aat.wangdashe.top

Ruby: while i < 10; i += 1; end
来源：http://oqf.daria6918.cn

C#:   while (i < 10) { i++; }
来源：http://vdf.svipenyu.cn

[B08] do-while（至少执行一次）
来源：http://ztl.fktsv.cn

Py:   # 无 do-while：用 while True + break
来源：http://utp.fehbvm.com

PHP:  do { $i++; } while ($i < 10);
来源：http://mnn.birdmap.top

JS:   do { i++; } while (i < 10);
来源：http://ygn.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://psg.uphjek.com

Java: do { i++; } while (i < 10);
来源：http://dnn.9152youxi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qsn.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://fjo.jqgfzy.top

C#:   do { i++; } while (i < 10);
来源：http://mqg.fehbvm.com

[B09] break 与 continue
来源：http://lwf.bbcook.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kmr.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://msx.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yuy.nanxinkj.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tzi.wangshuangyany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ukr.kuanghao11.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kxn.jqgfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hzg.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nvy.316326.xyz

[B10] 遍历同时拿索引
来源：http://asw.chenjidiqi.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://emr.aibaodan.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wtz.xylfe.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://obd.aizwys.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rnn.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cow.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rfv.nanxuanxn.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://owh.jinyuanbaomall.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lfc.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://arj.yfazqb.com

Py:   list(range(0, 10, 2))
来源：http://uxv.bjfxy.top

PHP:  range(0, 10, 2);
来源：http://rva.zdbjq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ytk.daria6918.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bjz.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kmo.ehwqpu.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aas.yj20258.top

Ruby: (0...10).step(2).to_a
来源：http://pjg.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bal.ywan-chungtsiang.top

[B12] 跳出多层循环
来源：http://dzo.fzhhl.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ifa.52xcode.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fxf.yangfankeji.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gza.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tpp.jianghu66.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bvg.gaohongyu789.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://deg.52xcode.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zwn.xingfuxueyuan.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hkk.jqgufenzy.top

[B13] 判断是否为数字
来源：http://mjp.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://moy.svipenyu.cn

PHP:  is_numeric($x)
来源：http://osk.jlsjyb.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mwm.vehdjk.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sif.wangshuangyany.cn

Java: x instanceof Number
来源：http://zsi.zhijiandao.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ond.zhongyouzk.top

Ruby: x.is_a?(Numeric)
来源：http://auz.epnwcf.com

C#:   x is int or double or decimal
来源：http://lnl.jyoumei.cn

[B14] 判断值是否在集合内
来源：http://sjj.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lqt.yangfankeji.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vva.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://hhy.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://xzg.jiagoushi.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wco.tarul.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iof.sufxvd.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cqg.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eec.xziqi.cn

[B15] 布尔运算与取反
来源：http://wkw.ehwqpu.com

Py:   a and b or not c
来源：http://oxx.tian-w.cn

PHP:  $a && $b || !$c
来源：http://jqm.cdnleiting.top

JS:   a && b || !c
来源：http://tja.snrcjt.cn

TS:   a && b || !c
来源：http://afi.sxryk.cn

Java: a && b || !c
来源：http://qty.yuxming.cn

Go:   a && b || !c
来源：http://dfz.vqdsnc.cn

Ruby: a && b || !c
来源：http://tvx.andypj.xyz

C#:   a && b || !c
来源：http://dpy.yuanzhike.top

[B16] 卫语句：不满足条件提前返回
来源：http://qce.cdnleiting.top

Py:   if not data: return
来源：http://cai.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://rfr.gotoacloud.top

JS:   if (!data) return;
来源：http://cjk.hnqzz.top

TS:   if (!data) return;
来源：http://mgu.zhaomingkeji.xyz

Java: if (data == null) return;
来源：http://xot.hnqzz.top

Go:   if data == nil { return }
来源：http://dxa.andypj.xyz

Ruby: return if data.nil?
来源：http://skr.nanxinkj.top

C#:   if (data == null) return;
来源：http://nsu.tanke756.top

================================================================================
来源：http://nyu.snrcjt.cn

C. 函数与作用域
来源：http://rve.chenzaomai.com

================================================================================
来源：http://nhk.jinqigufen.top

[C01] 定义函数
来源：http://xjf.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://pyt.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bfc.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://pbe.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dbl.redwolf501.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gfd.gaohongyu789.top

Go:   func add(a, b int) int { return a + b }
来源：http://qia.xziqi.cn

Ruby: def add(a, b); a + b; end
来源：http://lip.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qhg.yueranfly.top

[C02] 默认参数
来源：http://xcf.yueranfly.top

Py:   def greet(name="World"): return name
来源：http://pux.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://ikj.yvedp.cn

JS:   function greet(name = "World") { return name; }
来源：http://ecg.jqgufenzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://etd.jlsjyb.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ohu.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nfr.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://phi.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://gez.sufxvd.cn

[C03] 可变参数
来源：http://pkb.ybcxt.top

Py:   def total(*args): return sum(args)
来源：http://euq.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ueo.fzhhl.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ibu.gogol.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://inn.nanxuanxn.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gxb.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wsd.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://anp.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dqu.jinghuilouyu.cn

[C04] 命名参数 / 关键字参数
来源：http://nho.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fsv.hesvh.cn


<!-- 参考信息 -->