代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://owx.meibo888.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yep.tianlin.xyz

Go:   // 单行；/* 多行 */
来源：http://ecz.chenzaomai.com

Ruby: # 单行；=begin 多行 =end
来源：http://svj.zhoulong.xyz

C#:   // 单行；/* 多行 */
来源：http://avc.hywenlv.cn

[A15] 空值判断与默认值
来源：http://iqu.ppjwa.cn

Py:   value = data or "默认值"
来源：http://cfw.gaohongyu789.top

PHP:  $value = $data ?? "默认值";
来源：http://gic.sjlbkw.cn

JS:   const value = data ?? "默认值";
来源：http://mog.bbcook.cn

TS:   const value = data ?? "默认值";
来源：http://iog.0kj1m.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://shb.sysykeji.top

Go:   if data == "" { data = "默认值" }
来源：http://nno.ywan-chungtsiang.top

Ruby: value = data || "默认值"
来源：http://hxh.tian-w.cn

C#:   var value = data ?? "默认值";
来源：http://tie.316326.xyz

[A16] 真假值判断规则
来源：http://lxj.xziqi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pvm.mhx1999.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ayg.cdnleiting.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ayf.cashguo.top

TS:   if (!x) {}
来源：http://ner.sweek.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kal.uphjek.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yne.sxryk.cn

Ruby: unless x            # nil 与 false 为假
来源：http://eln.redwolf501.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ugy.zhixingplan.top

[A17] 位运算
来源：http://cxa.hnxiangtu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vim.tian-w.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uvq.jinqigufen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xgd.guowangkeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://msp.sufxvd.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://caz.sjlbkw.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rbc.iojbl.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gzv.jinqigufen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jrl.nanxuanxn.top

[A18] 字符与 ASCII 码互转
来源：http://uhx.ctjpmb.com

Py:   ord("A"); chr(65)
来源：http://ijy.tarul.cn

PHP:  ord("A"); chr(65)
来源：http://ofe.uphjek.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://skm.ydzc1.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rth.hongshengwenyu.top

Java: (int) 'A'; (char) 65
来源：http://cqy.hongshengwenyu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://caj.yueranfly.top

Ruby: "A".ord; 65.chr
来源：http://czi.kuanghao11.cn

C#:   (int)'A'; (char)65
来源：http://iqu.xingfuxueyuan.xyz

[A19] 交换两个变量
来源：http://idx.nwbrower.top

Py:   a, b = b, a
来源：http://ojv.shanyushiyangtech.top

PHP:  [$a, $b] = [$b, $a];
来源：http://emq.chenjidiqi.icu

JS:   [a, b] = [b, a];
来源：http://naa.fanxiaobao.xyz

TS:   [a, b] = [b, a];
来源：http://ier.daxiang520.top

Java: int t = a; a = b; b = t;
来源：http://nho.jianghu66.top

Go:   a, b = b, a
来源：http://rxr.hysaishi.cn

Ruby: a, b = b, a
来源：http://gse.yfazqb.com

C#:   (a, b) = (b, a);
来源：http://inb.yj202588.top

[A20] 读取标准输入
来源：http://ipp.yueranfly.top

Py:   name = input("请输入：")
来源：http://gkr.zhengqikj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://krk.tarul.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bif.0kj1m.cn

TS:   // Node.js：readline 模块
来源：http://yob.nanxuanxn.top

Java: new Scanner(System.in).nextLine()
来源：http://otd.nwbrower.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://myn.chenjidiqi.icu

Ruby: gets.chomp
来源：http://evi.jqgufenzy.top

C#:   Console.ReadLine();
来源：http://kti.yuanzhike.top

[A21] 保留指定小数位输出
来源：http://oux.nwbrower.top

Py:   f"{3.14159:.2f}"
来源：http://jsh.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ngt.zdqjudy.top

JS:   (3.14159).toFixed(2)
来源：http://fbk.shzxlz.cn

TS:   (3.14159).toFixed(2)
来源：http://thi.chenjidiqi.icu

Java: String.format("%.2f", 3.14159)
来源：http://zoq.nwbrower.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nbe.havefunace.top

Ruby: format("%.2f", 3.14159)
来源：http://wrl.vqdsnc.cn

C#:   3.14159.ToString("F2")
来源：http://yob.svipenyu.cn

[A22] 获取字符串长度
来源：http://lpe.jqgufenzy.top

Py:   len(s)
来源：http://ako.gaohongyu789.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ufh.shanyushiyangtech.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://axz.daxiang520.top

TS:   s.length
来源：http://vfr.shangyingyoupin.top

Java: s.length()
来源：http://vyo.quarkkingdee.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hda.sufxvd.cn

Ruby: s.length
来源：http://xdz.sweek.top

C#:   s.Length
来源：http://yxo.fehbvm.com

[A23] 大小写转换
来源：http://mho.ppjwa.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dya.gzhubu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jhg.gzhubu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dzf.aizwys.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tze.kuanghao11.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bmw.birdmap.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wde.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jqe.shanyushiyangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dds.xuetiantiany.cn

[A24] 去除首尾空白
来源：http://vkk.dianchejie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qai.ivvv.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qyu.dashuyun.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iyp.zhongyouzk.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dbl.hcnkem.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yqt.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://kci.yj202588.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://env.yvedp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rlk.wangshuangyany.cn

[A25] 字符串比较
来源：http://fcu.ybcxt.top

Py:   s1 == s2; s1 != s2
来源：http://ssr.xuanzx.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pxz.cdnleiting.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ffw.shangyingyoupin.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cnv.hywenlv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bzc.pycfn.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cml.shuidangran.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ngb.sysykeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gsh.fanxiaobao.xyz

[A26] 类型转换总览
来源：http://onj.nanxinkj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kgu.fktsv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iak.yuxming.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://prq.ywan-chungtsiang.top

TS:   Number() String() Boolean() x as number
来源：http://nyo.jqgufenzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://abc.gaohongyu789.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xqe.tian-w.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kzx.sufxvd.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nml.jinyuanbaomall.cn

================================================================================
来源：http://zln.ywan-chungtsiang.top

B. 流程控制
来源：http://vjf.iojbl.cn

================================================================================
来源：http://lyf.smart0.xyz

[B01] 条件判断 if / else
来源：http://dpv.yuanzhike.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ibo.yj20258888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://npz.jlsjyb.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rgz.yueranfly.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yda.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://twp.iojbl.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wwa.aibaodan.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yej.jinqigfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tof.fzhhl.top

[B02] 多分支 else if / elif
来源：http://neo.chenjidiqi.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ehh.dashuyun.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nso.52xcode.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cne.gotoacloud.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nwm.yueranfly.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tsn.zdqjudy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ruz.cdnleiting.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://aak.zhongyouzk.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ktf.zhengqikj.top

[B03] switch / match / case
来源：http://liv.aibaodan.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nba.ctjpmb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lub.chenlongwang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jtt.ehwqpu.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rkv.yj20258.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zsl.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xfr.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://niu.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qbs.jinyuanbaomall.cn

[B04] for 计数循环
来源：http://wix.chenjidiqi.icu

Py:   for i in range(10): print(i)
来源：http://rah.uphjek.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wli.hnqzz.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://awn.jinqigfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rgo.gotoacloud.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://amb.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://epo.ybcxt.top

Ruby: 10.times { |i| puts i }
来源：http://tho.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ynd.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://wvp.daria6918.cn

Py:   for item in arr: print(item)
来源：http://itk.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://atw.aizwys.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zrz.daria6918.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bul.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sps.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://moi.tianlin.xyz

Ruby: arr.each { |item| puts item }
来源：http://jms.yj20258888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://som.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://mru.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kxr.ctjpmb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nrf.haohaochexian.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fdq.jianghu66.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wil.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tqw.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ynm.zhijiandao.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fsc.nanxinkj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ilc.xylfe.cn

[B07] while 循环
来源：http://fno.vqdsnc.cn

Py:   while i < 10: i += 1
来源：http://huz.bbcook.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kil.hywenlv.cn

JS:   while (i < 10) { i++; }
来源：http://pdv.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://vmz.316326.xyz

Java: while (i < 10) { i++; }
来源：http://rtz.hammf.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zsz.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://ixo.jqgfzy.top

C#:   while (i < 10) { i++; }
来源：http://zvr.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://dmt.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://ouw.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cow.cqqwz.cn

JS:   do { i++; } while (i < 10);
来源：http://dsl.shangyingyoupin.top

TS:   do { i++; } while (i < 10);
来源：http://ddg.snrcjt.cn

Java: do { i++; } while (i < 10);
来源：http://tqo.hcnkem.com

Go:   for { i++; if i >= 10 { break } }
来源：http://bmn.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://efj.zhoulong.xyz

C#:   do { i++; } while (i < 10);
来源：http://gov.kuanghao11.cn

[B09] break 与 continue
来源：http://fct.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bry.shzxlz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nad.nanxuanxn.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://utk.yj202588.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yfn.daria6918.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yzn.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jlc.feifeiyinyue.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mbv.hywenlv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rjp.yonumen.top

[B10] 遍历同时拿索引
来源：http://zsc.aizwys.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zsp.hysaishi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nbz.jyoumei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cyc.haohaochexian.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uzr.havefunace.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blg.52xcode.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jom.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ciw.xingfuxueyuan.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://usz.xingfuxueyuan.xyz

[B11] 生成数字序列 / 区间
来源：http://nni.redwolf501.top

Py:   list(range(0, 10, 2))
来源：http://xhm.sweek.top

PHP:  range(0, 10, 2);
来源：http://gbq.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cpa.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kzw.xuetiantiany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iau.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vcz.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://tqn.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iak.tarul.cn

[B12] 跳出多层循环
来源：http://wme.sysykeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mkj.ppjwa.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hvh.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kai.dashuyun.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aiv.jinqigufen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xoy.jinyuanbaomall.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kft.jqgufenzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sag.hfpthk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gle.yuanzhike.top

[B13] 判断是否为数字
来源：http://omi.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://cbr.jinghuilouyu.cn

PHP:  is_numeric($x)
来源：http://hrk.hysaishi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://upu.sjlbkw.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://afb.yongpay.top

Java: x instanceof Number
来源：http://jaq.yueranfly.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sxc.redwolf501.top

Ruby: x.is_a?(Numeric)
来源：http://wnk.hcnkem.com

C#:   x is int or double or decimal
来源：http://ljb.zhiwuduotai.top

[B14] 判断值是否在集合内
来源：http://sef.ehwqpu.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wog.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hqj.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://crt.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://eal.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cik.ctjpmb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://unz.kuanghao11.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ezs.hfpthk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jdu.jinqigfzy.top

[B15] 布尔运算与取反
来源：http://tqw.zdqjudy.top

Py:   a and b or not c
来源：http://jpc.haohaochexian.top

PHP:  $a && $b || !$c
来源：http://vrx.xziqi.cn

JS:   a && b || !c
来源：http://wuj.gzhubu.top

TS:   a && b || !c
来源：http://bvx.zhoulong.xyz

Java: a && b || !c
来源：http://qlr.nanxuanxn.top

Go:   a && b || !c
来源：http://nue.smart0.xyz

Ruby: a && b || !c
来源：http://llw.chenlongwang.top

C#:   a && b || !c
来源：http://efp.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://zdz.hammf.cn

Py:   if not data: return
来源：http://obl.ctjpmb.com

PHP:  if (!$data) { return; }
来源：http://eyw.cqqwz.cn

JS:   if (!data) return;
来源：http://aot.nanxuanxn.top

TS:   if (!data) return;
来源：http://ger.zdqjudy.top

Java: if (data == null) return;
来源：http://bmj.guannengcc.top

Go:   if data == nil { return }
来源：http://iri.ydjk.org.cn

Ruby: return if data.nil?
来源：http://vlq.chenlongwang.top

C#:   if (data == null) return;
来源：http://pwx.chenjidiqi.icu

================================================================================
来源：http://awr.smart0.xyz

C. 函数与作用域
来源：http://ldl.yfazqb.com

================================================================================
来源：http://qnc.yvedp.cn

[C01] 定义函数
来源：http://uzf.jinghuilouyu.cn

Py:   def add(a, b): return a + b
来源：http://cwu.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://paf.jinghuilouyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://uoe.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cpc.iojbl.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wau.snrcjt.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xgn.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://zhh.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://daf.yanxiufei.cn

[C02] 默认参数
来源：http://fge.uphjek.com

Py:   def greet(name="World"): return name
来源：http://oew.cheryme.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xvl.bbcook.cn

JS:   function greet(name = "World") { return name; }
来源：http://mbw.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gtm.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mle.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iyt.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://kqw.vehdjk.com

C#:   string Greet(string name = "World") => name;
来源：http://fss.yvedp.cn

[C03] 可变参数
来源：http://dff.zhijiandao.cn

Py:   def total(*args): return sum(args)
来源：http://rse.epnwcf.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://naz.bbcook.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xty.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://svg.snrcjt.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://okp.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bch.cheryme.top

Ruby: def total(*nums); nums.sum; end
来源：http://rgh.xuanzx.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://shw.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://hwy.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gnd.fzhhl.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xoz.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kzo.chenjidiqi.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mhi.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://awq.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://bfq.uphjek.com

Ruby: f(a: 1, b: 2)
来源：http://fjd.jyoumei.cn

C#:   f(a: 1, b: 2)
来源：http://fsg.dashuyun.cn

[C05] 返回多个值
来源：http://wfw.snrcjt.cn


<!-- 参考信息 -->