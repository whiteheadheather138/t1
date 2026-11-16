代发 wailian999

Java: "第一行\n第二行"
来源：http://vyg.ydjk.org.cn

Go:   "第一行\n第二行"
来源：http://xjf.52xcode.cn

Ruby: "第一行\n第二行"
来源：http://tzg.shangyingyoupin.top

C#:   "第一行\n第二行"
来源：http://ihw.cqqwz.cn

[A14] 注释写法
来源：http://jng.hnqzz.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://gwo.vehdjk.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://gjp.xuanzx.com

JS:   // 单行；/* 多行 */
来源：http://vpw.cashguo.top

TS:   // 单行；/* 多行 */
来源：http://jqn.hnqzz.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://anj.jinyuanbaomall.cn

Go:   // 单行；/* 多行 */
来源：http://jpf.hnqzz.top

Ruby: # 单行；=begin 多行 =end
来源：http://gpt.jinqigufen.top

C#:   // 单行；/* 多行 */
来源：http://tfl.zhixingplan.top

[A15] 空值判断与默认值
来源：http://ppv.shzxlz.cn

Py:   value = data or "默认值"
来源：http://maw.gotoacloud.top

PHP:  $value = $data ?? "默认值";
来源：http://zre.ivvv.top

JS:   const value = data ?? "默认值";
来源：http://fxk.pengpengdd.cyou

TS:   const value = data ?? "默认值";
来源：http://xbr.nwbrower.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kqv.hnxiangtu.top

Go:   if data == "" { data = "默认值" }
来源：http://pxk.chenzaomai.com

Ruby: value = data || "默认值"
来源：http://seq.yfazqb.com

C#:   var value = data ?? "默认值";
来源：http://jdg.dianchejie.cn

[A16] 真假值判断规则
来源：http://gaa.xuanzx.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fnz.wangdashe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pcl.ppjwa.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dhj.vehdjk.com

TS:   if (!x) {}
来源：http://wqp.zhixingplan.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dvh.zhiwuduotai.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dsl.kuanghao11.cn

Ruby: unless x            # nil 与 false 为假
来源：http://usq.ctjpmb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://owr.tarul.cn

[A17] 位运算
来源：http://pwl.uphjek.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gko.guowangkeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tuz.jianghu66.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xbm.chenlongwang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fce.pengpengdd.cyou

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ggu.0kj1m.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://owq.316326.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://izq.tanke756.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uxz.aizwys.cn

[A18] 字符与 ASCII 码互转
来源：http://gsp.ehwqpu.com

Py:   ord("A"); chr(65)
来源：http://vym.yvedp.cn

PHP:  ord("A"); chr(65)
来源：http://xfv.shangyingyoupin.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aov.gogol.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tnl.xziqi.cn

Java: (int) 'A'; (char) 65
来源：http://obo.xylfe.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qyz.xuetiantiany.cn

Ruby: "A".ord; 65.chr
来源：http://jnj.bbcook.cn

C#:   (int)'A'; (char)65
来源：http://iwm.cucudq.cn

[A19] 交换两个变量
来源：http://isr.xingfuxueyuan.xyz

Py:   a, b = b, a
来源：http://mum.feifeiyinyue.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dgl.ppjwa.cn

JS:   [a, b] = [b, a];
来源：http://rxm.jlsjyb.cn

TS:   [a, b] = [b, a];
来源：http://oap.ivvv.top

Java: int t = a; a = b; b = t;
来源：http://ord.wangshuangyany.cn

Go:   a, b = b, a
来源：http://bvr.pycfn.com

Ruby: a, b = b, a
来源：http://oqe.xuanzx.com

C#:   (a, b) = (b, a);
来源：http://pym.xziqi.cn

[A20] 读取标准输入
来源：http://iet.shanyushiyangkeji.top

Py:   name = input("请输入：")
来源：http://fnp.cqqwz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xnw.yongpay.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ive.cashguo.top

TS:   // Node.js：readline 模块
来源：http://ycs.hnxiangtu.top

Java: new Scanner(System.in).nextLine()
来源：http://qbs.yfazqb.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://miw.yj202588.top

Ruby: gets.chomp
来源：http://wjd.pycfn.com

C#:   Console.ReadLine();
来源：http://cvg.zhixingplan.top

[A21] 保留指定小数位输出
来源：http://fbz.guannengcc.top

Py:   f"{3.14159:.2f}"
来源：http://wbn.hammf.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zsn.uphjek.com

JS:   (3.14159).toFixed(2)
来源：http://nuh.gotoacloud.top

TS:   (3.14159).toFixed(2)
来源：http://cuh.pengpengdd.cyou

Java: String.format("%.2f", 3.14159)
来源：http://rav.shzxlz.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pfu.hnqzz.top

Ruby: format("%.2f", 3.14159)
来源：http://myn.ydzc1.top

C#:   3.14159.ToString("F2")
来源：http://lsu.jinyuanbaomall.cn

[A22] 获取字符串长度
来源：http://ire.yueranfly.top

Py:   len(s)
来源：http://gqk.smart0.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gzm.yangfankeji.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jkq.hcnkem.com

TS:   s.length
来源：http://pgh.xinyue.icu

Java: s.length()
来源：http://whb.hnxiangtu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hmq.yongpay.top

Ruby: s.length
来源：http://gje.xylfe.cn

C#:   s.Length
来源：http://oda.zhijiandao.cn

[A23] 大小写转换
来源：http://nvz.pycfn.com

Py:   s.upper(); s.lower(); s.title()
来源：http://ted.xinyue.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rsg.cashguo.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qgc.iojbl.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cqh.yanxiufei.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uzd.sysykeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://aid.ybcxt.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dot.epnwcf.com

C#:   s.ToUpper(); s.ToLower()
来源：http://cjx.aizwys.cn

[A24] 去除首尾空白
来源：http://syu.sysykeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zag.zhoulong.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ogv.tarul.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qne.wangshuangyany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sny.zhaomingkeji.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jgj.dianchejie.cn

Go:   strings.TrimSpace(s)
来源：http://klf.yj20258.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fnv.jinyuanbaomall.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fiy.xylfe.cn

[A25] 字符串比较
来源：http://bit.daxiang520.top

Py:   s1 == s2; s1 != s2
来源：http://bzm.shzxlz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bnj.snrcjt.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hyw.jqgfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kwx.tianlin.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tbf.dianchejie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bov.jinghuilouyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://biy.nwbrower.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vsr.0kj1m.cn

[A26] 类型转换总览
来源：http://wxe.bbcook.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ogh.feifeiyinyue.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yze.gotoacloud.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bun.aibaodan.cn

TS:   Number() String() Boolean() x as number
来源：http://pap.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mhf.jqgufenzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cjk.jinyuanbaomall.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://suu.9152youxi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cnw.hnqzz.top

================================================================================
来源：http://glp.cashguo.top

B. 流程控制
来源：http://ure.sysykeji.top

================================================================================
来源：http://hbj.chenjidiqi.icu

[B01] 条件判断 if / else
来源：http://jay.tianlin.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://ehu.316326.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uvx.fanxiaobao.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tpl.ydjk.org.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qyk.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ywo.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jer.xuanzx.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cxn.cdnleiting.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ebf.hcnkem.com

[B02] 多分支 else if / elif
来源：http://aag.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nqg.jqgufenzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uuw.xingfuxueyuan.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gvb.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dpn.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pmi.pengpengdd.cyou

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rbv.redwolf501.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nry.dianchejie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pws.zdqjudy.top

[B03] switch / match / case
来源：http://rfk.yongpay.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ywa.xziqi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://efh.daxiang520.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mlx.cucudq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://euq.yj20258.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zki.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://muo.ppjwa.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://phu.yj202588.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fsx.epnwcf.com

[B04] for 计数循环
来源：http://eby.hysaishi.cn

Py:   for i in range(10): print(i)
来源：http://jro.52xcode.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lxo.zdbjq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qko.sxryk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://srq.tarul.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rci.smart0.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pvs.havefunace.top

Ruby: 10.times { |i| puts i }
来源：http://bmr.bbcook.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fbh.hywenlv.cn

[B05] 遍历数组 / 列表
来源：http://dal.bjfxy.top

Py:   for item in arr: print(item)
来源：http://hjy.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wiy.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oha.sjlbkw.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zlr.xinyue.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://vph.nanxuanxn.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mxr.shanyushiyangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://mqo.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://adb.hongshengwenyu.top

[B06] 遍历字典 / 对象
来源：http://vcn.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nol.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wvf.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xzz.shanyushiyangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iao.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gnb.hongshengwenyu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kvs.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pjl.52xcode.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fqf.pycfn.com

[B07] while 循环
来源：http://jrn.havefunace.top

Py:   while i < 10: i += 1
来源：http://crg.pycfn.com

PHP:  while ($i < 10) { $i++; }
来源：http://ddz.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://eoi.yonumen.top

TS:   while (i < 10) { i++; }
来源：http://mup.cdnleiting.top

Java: while (i < 10) { i++; }
来源：http://fuv.wangshuangyany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lfo.guannengcc.top

Ruby: while i < 10; i += 1; end
来源：http://elp.hnxiangtu.top

C#:   while (i < 10) { i++; }
来源：http://ozj.hammf.cn

[B08] do-while（至少执行一次）
来源：http://nae.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://yhc.yanxiufei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ovd.zhiwuduotai.top

JS:   do { i++; } while (i < 10);
来源：http://cep.nanxuanxn.top

TS:   do { i++; } while (i < 10);
来源：http://rjq.pycfn.com

Java: do { i++; } while (i < 10);
来源：http://giz.hesvh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tij.dianchejie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pey.gaohongyu789.top

C#:   do { i++; } while (i < 10);
来源：http://cxy.yonumen.top

[B09] break 与 continue
来源：http://key.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tmi.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://czj.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lxg.zhixingplan.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ohe.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zdq.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zpw.bbcook.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://myp.sweek.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://znm.guannengcc.top

[B10] 遍历同时拿索引
来源：http://xkk.zycfv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://spn.cheryme.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xzo.yangfankeji.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://scf.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wcn.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hge.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://svb.jlsjyb.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ipv.tian-w.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gcg.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://ges.hywenlv.cn

Py:   list(range(0, 10, 2))
来源：http://ehi.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://xjy.yuanzhike.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nvz.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://acv.52xcode.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cmv.9152youxi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fmr.yj202588.top

Ruby: (0...10).step(2).to_a
来源：http://wec.sufxvd.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jie.daria6918.cn

[B12] 跳出多层循环
来源：http://zsv.sxryk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://paj.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fdp.ywan-chungtsiang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ffe.xingfuxueyuan.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jxv.jqgufenzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bag.cqqwz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jdp.xingfuxueyuan.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ajt.epnwcf.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pyi.jianghu66.top

[B13] 判断是否为数字
来源：http://tbh.gzhubu.top

Py:   isinstance(x, (int, float))
来源：http://ycj.316326.xyz

PHP:  is_numeric($x)
来源：http://dbh.aizwys.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eld.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kmr.jinqigufen.top

Java: x instanceof Number
来源：http://ebi.c1oappe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://egs.ydjk.org.cn

Ruby: x.is_a?(Numeric)
来源：http://pbl.pengpengdd.cyou

C#:   x is int or double or decimal
来源：http://avf.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://rps.xuanzx.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jsf.yonumen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://auv.tarul.cn

JS:   [1, 2, 3].includes(x)
来源：http://vtt.daxiang520.top

TS:   [1, 2, 3].includes(x)
来源：http://gxt.yuxming.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nif.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qjw.chenzaomai.com

Ruby: [1, 2, 3].include?(x)
来源：http://ves.jiagoushi.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iui.yongpay.top

[B15] 布尔运算与取反
来源：http://nlj.zhiwuduotai.top

Py:   a and b or not c
来源：http://jsa.pengpengdd.cyou

PHP:  $a && $b || !$c
来源：http://wan.mhx1999.top

JS:   a && b || !c
来源：http://pix.shuidangran.top

TS:   a && b || !c
来源：http://jfl.gogol.net.cn

Java: a && b || !c
来源：http://wcc.uphjek.com

Go:   a && b || !c
来源：http://hid.quarkkingdee.top

Ruby: a && b || !c
来源：http://fbs.zhixingplan.top

C#:   a && b || !c
来源：http://rlc.wangshuangyany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ijw.zdqjudy.top

Py:   if not data: return
来源：http://rjk.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://var.jyoumei.cn

JS:   if (!data) return;
来源：http://xeb.pycfn.com

TS:   if (!data) return;
来源：http://yol.jlsjyb.cn

Java: if (data == null) return;
来源：http://hdx.ehwqpu.com

Go:   if data == nil { return }
来源：http://ymm.pycfn.com

Ruby: return if data.nil?
来源：http://xbb.bbcook.cn

C#:   if (data == null) return;
来源：http://arf.guannengcc.top

================================================================================
来源：http://dzz.yj202588.top

C. 函数与作用域
来源：http://pac.xylfe.cn

================================================================================
来源：http://tlh.xuetiantiany.cn

[C01] 定义函数
来源：http://ipk.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://zea.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://myv.hnqzz.top

JS:   function add(a, b) { return a + b; }
来源：http://jkt.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://csl.hammf.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zux.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://oga.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://erb.tanke756.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ffv.hnqzz.top

[C02] 默认参数
来源：http://jaf.jianghu66.top

Py:   def greet(name="World"): return name
来源：http://xeu.mhx1999.top

PHP:  function greet($name = "World") { return $name; }
来源：http://doo.hywenlv.cn

JS:   function greet(name = "World") { return name; }
来源：http://bwt.cdnleiting.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nob.xylfe.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vmc.sweek.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://anj.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://eqj.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://djp.aizwys.cn

[C03] 可变参数
来源：http://odj.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://nxk.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jaw.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aqw.fengsongda.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zjg.mhx1999.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uiu.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://spm.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lki.jinqigfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qyn.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://vla.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ofp.iojbl.cn


<!-- 参考信息 -->