代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://aqp.cashguo.top

JS:   `Hello, ${name}!`
来源：http://mwr.jqgufenzy.top

TS:   `Hello, ${name}!`
来源：http://aqz.yonumen.top

Java: "Hello, %s!".formatted(name)
来源：http://pct.jiagoushi.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wbp.tarul.cn

Ruby: "Hello, #{name}!"
来源：http://bpq.jiagoushi.top

C#:   $"Hello, {name}!"
来源：http://ohl.ivvv.top

[A13] 多行字符串（练习 \n 转义）
来源：http://isw.fengsongda.top

Py:   "第一行\n第二行"
来源：http://gfw.smart0.xyz

PHP:  "第一行\n第二行"
来源：http://wjt.zycfv.cn

JS:   "第一行\n第二行"
来源：http://rjk.jinghuilouyu.cn

TS:   "第一行\n第二行"
来源：http://fmg.chenlongwang.top

Java: "第一行\n第二行"
来源：http://dei.jinyuanbaomall.cn

Go:   "第一行\n第二行"
来源：http://tci.iojbl.cn

Ruby: "第一行\n第二行"
来源：http://gpl.fanxiaobao.xyz

C#:   "第一行\n第二行"
来源：http://qzw.jianghu66.top

[A14] 注释写法
来源：http://lrd.zhijiandao.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rzp.hfpthk.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cce.sxryk.cn

JS:   // 单行；/* 多行 */
来源：http://acn.ybcxt.top

TS:   // 单行；/* 多行 */
来源：http://ffd.ppjwa.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jsx.hcnkem.com

Go:   // 单行；/* 多行 */
来源：http://bwh.gogol.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uhi.iojbl.cn

C#:   // 单行；/* 多行 */
来源：http://cfv.jlsjyb.cn

[A15] 空值判断与默认值
来源：http://wne.hcnkem.com

Py:   value = data or "默认值"
来源：http://twi.yuanzhike.top

PHP:  $value = $data ?? "默认值";
来源：http://igw.fktsv.cn

JS:   const value = data ?? "默认值";
来源：http://kas.gogol.net.cn

TS:   const value = data ?? "默认值";
来源：http://ldb.sweek.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://omd.hcnkem.com

Go:   if data == "" { data = "默认值" }
来源：http://dcn.c1oappe.top

Ruby: value = data || "默认值"
来源：http://ofj.52xcode.cn

C#:   var value = data ?? "默认值";
来源：http://brd.sxryk.cn

[A16] 真假值判断规则
来源：http://udl.zycfv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qni.shangyingyoupin.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vai.yuxming.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qji.ybcxt.top

TS:   if (!x) {}
来源：http://cya.chenjidiqi.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gmj.cashguo.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sly.tian-w.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qzc.dashuyun.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://aiz.hfpthk.cn

[A17] 位运算
来源：http://noa.cdnleiting.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cka.zhoulong.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ybk.chenlongwang.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rwq.fzhhl.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://eej.jqgfzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://omz.haohaochexian.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gae.jyoumei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pek.meibo888.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tit.jlsjyb.cn

[A18] 字符与 ASCII 码互转
来源：http://mxh.ivvv.top

Py:   ord("A"); chr(65)
来源：http://wnd.sweek.top

PHP:  ord("A"); chr(65)
来源：http://ehu.shanyushiyangtech.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pae.gzhubu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rgj.ppjwa.cn

Java: (int) 'A'; (char) 65
来源：http://lar.zhongyouzk.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vah.dianchejie.cn

Ruby: "A".ord; 65.chr
来源：http://iyo.fzhhl.top

C#:   (int)'A'; (char)65
来源：http://dbb.svipenyu.cn

[A19] 交换两个变量
来源：http://mjf.zhiwuduotai.top

Py:   a, b = b, a
来源：http://ymm.daria6918.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rcj.wangdashe.top

JS:   [a, b] = [b, a];
来源：http://wya.yuxming.cn

TS:   [a, b] = [b, a];
来源：http://miz.gaohongyu789.top

Java: int t = a; a = b; b = t;
来源：http://wdy.tanke756.top

Go:   a, b = b, a
来源：http://vtj.jinqigfzy.top

Ruby: a, b = b, a
来源：http://wro.xziqi.cn

C#:   (a, b) = (b, a);
来源：http://quq.c1oappe.top

[A20] 读取标准输入
来源：http://wey.jqgfzy.top

Py:   name = input("请输入：")
来源：http://yez.zhongyouzk.top

PHP:  $name = trim(fgets(STDIN));
来源：http://xql.hesvh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://arx.52xcode.cn

TS:   // Node.js：readline 模块
来源：http://ijl.52xcode.cn

Java: new Scanner(System.in).nextLine()
来源：http://exj.ydzc1.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ckw.chenzaomai.com

Ruby: gets.chomp
来源：http://pdj.fengsongda.top

C#:   Console.ReadLine();
来源：http://yvq.svipenyu.cn

[A21] 保留指定小数位输出
来源：http://ewy.fktsv.cn

Py:   f"{3.14159:.2f}"
来源：http://trl.hywenlv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pyt.zhengqikj.top

JS:   (3.14159).toFixed(2)
来源：http://yqg.shanyushiyangtech.top

TS:   (3.14159).toFixed(2)
来源：http://llp.wangdashe.top

Java: String.format("%.2f", 3.14159)
来源：http://sbs.aibaodan.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pah.jinqigfzy.top

Ruby: format("%.2f", 3.14159)
来源：http://ymy.xuetiantiany.cn

C#:   3.14159.ToString("F2")
来源：http://nod.tanke756.top

[A22] 获取字符串长度
来源：http://vtp.redwolf501.top

Py:   len(s)
来源：http://ekr.sxryk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pxv.ehwqpu.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kxt.aibaodan.cn

TS:   s.length
来源：http://tvt.jianghu66.top

Java: s.length()
来源：http://ais.zhongyouzk.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gvh.ivvv.top

Ruby: s.length
来源：http://tah.hongshengwenyu.top

C#:   s.Length
来源：http://day.jqgfzy.top

[A23] 大小写转换
来源：http://erx.yj202588.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pmz.iojbl.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mrj.jianghu66.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://plk.tanke756.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://whw.gaohongyu789.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://znr.quarkkingdee.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://anp.quarkkingdee.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zjs.vehdjk.com

C#:   s.ToUpper(); s.ToLower()
来源：http://rpy.haohaochexian.top

[A24] 去除首尾空白
来源：http://hlx.xinyue.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://neg.xuetiantiany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oxx.smart0.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wgz.sufxvd.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iqt.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://swb.chenzaomai.com

Go:   strings.TrimSpace(s)
来源：http://wyf.yongpay.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ope.dashuyun.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kxh.jqgfzy.top

[A25] 字符串比较
来源：http://nik.guannengcc.top

Py:   s1 == s2; s1 != s2
来源：http://elp.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oou.yuanzhike.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ttc.hesvh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vng.cheryme.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://exr.shzxlz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ctu.sweek.top

Ruby: s1 == s2; s1 <=> s2
来源：http://fuo.smart0.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eah.yangfankeji.com

[A26] 类型转换总览
来源：http://uli.zhaomingkeji.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jqs.xuanzx.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ail.shzxlz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gjy.birdmap.top

TS:   Number() String() Boolean() x as number
来源：http://pdh.fzhhl.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ode.hywenlv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mrw.jianghu66.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dyn.andypj.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hyq.yvedp.cn

================================================================================
来源：http://ldi.zhaomingkeji.xyz

B. 流程控制
来源：http://xsh.c1oappe.top

================================================================================
来源：http://rgu.zhijiandao.cn

[B01] 条件判断 if / else
来源：http://mzf.zhongyouzk.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zaq.fzhhl.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vta.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kcb.gzhubu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ksd.xinyue.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://wbj.dashuyun.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://awm.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wjb.hcnkem.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ump.guowangkeji.top

[B02] 多分支 else if / elif
来源：http://zwm.uphjek.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wql.bjfxy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zor.aibaodan.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wke.pycfn.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xkr.gotoacloud.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ibm.yj202588.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fca.hesvh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://udw.hcnkem.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hzk.cheryme.top

[B03] switch / match / case
来源：http://bno.sysykeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jbh.hysaishi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nma.jyoumei.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qmu.jinyuanbaomall.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ctu.tian-w.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ovy.jqgfzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qjl.aibaodan.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hqg.ehwqpu.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wqt.guowangkeji.top

[B04] for 计数循环
来源：http://lil.nwbrower.top

Py:   for i in range(10): print(i)
来源：http://vvh.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tim.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kxn.zhongyouzk.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fve.fehbvm.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wbs.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://brg.cqqwz.cn

Ruby: 10.times { |i| puts i }
来源：http://fan.zdqjudy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://col.kuanghao11.cn

[B05] 遍历数组 / 列表
来源：http://uyn.guannengcc.top

Py:   for item in arr: print(item)
来源：http://zao.xuetiantiany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jwg.zdqjudy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zyf.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xna.yueranfly.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://msa.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://enq.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://vuz.nanxuanxn.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ohn.wangshuangyany.cn

[B06] 遍历字典 / 对象
来源：http://tyk.xuanzx.com

Py:   for k, v in d.items(): print(k, v)
来源：http://kaa.jinqigfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cgl.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ayh.gzhubu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fsy.fengsongda.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lfz.ivvv.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://myu.gaohongyu789.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gjt.nanxinkj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pgp.jinqigfzy.top

[B07] while 循环
来源：http://yqy.cucudq.cn

Py:   while i < 10: i += 1
来源：http://iyc.mhx1999.top

PHP:  while ($i < 10) { $i++; }
来源：http://kpi.zdbjq.cn

JS:   while (i < 10) { i++; }
来源：http://ims.daria6918.cn

TS:   while (i < 10) { i++; }
来源：http://xqq.ehwqpu.com

Java: while (i < 10) { i++; }
来源：http://hoe.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wux.9152youxi.cn

Ruby: while i < 10; i += 1; end
来源：http://msl.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://raq.xuetiantiany.cn

[B08] do-while（至少执行一次）
来源：http://gpp.zdbjq.cn

Py:   # 无 do-while：用 while True + break
来源：http://fqj.cheryme.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zov.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://hwo.iojbl.cn

TS:   do { i++; } while (i < 10);
来源：http://lpm.zhijiandao.cn

Java: do { i++; } while (i < 10);
来源：http://yih.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://raw.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://gxa.dianchejie.cn

C#:   do { i++; } while (i < 10);
来源：http://uoy.jinghuilouyu.cn

[B09] break 与 continue
来源：http://bqa.xuanzx.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://btc.xingfuxueyuan.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jcx.jinqigfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xkg.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qzf.yanxiufei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fiw.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rfj.316326.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hal.yuanzhike.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vmq.shuidangran.top

[B10] 遍历同时拿索引
来源：http://qvc.aizwys.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xld.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xho.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://moy.cdnleiting.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fbs.hammf.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ouw.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://alt.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zbu.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rgx.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://rzl.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://now.birdmap.top

PHP:  range(0, 10, 2);
来源：http://qjx.svipenyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xop.pengpengdd.cyou

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kpa.sjlbkw.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fvj.epnwcf.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gvc.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://eeo.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fah.yuanzhike.top

[B12] 跳出多层循环
来源：http://yjj.0kj1m.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pqr.cdnleiting.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ocm.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wmv.hesvh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aan.zhaomingkeji.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bnn.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ukn.shuidangran.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zjx.cdnleiting.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lee.haohaochexian.top

[B13] 判断是否为数字
来源：http://vup.gotoacloud.top

Py:   isinstance(x, (int, float))
来源：http://cpi.ehwqpu.com

PHP:  is_numeric($x)
来源：http://gtt.zhoulong.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kcu.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dci.fktsv.cn

Java: x instanceof Number
来源：http://kpv.zdbjq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eab.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://swz.fengsongda.top

C#:   x is int or double or decimal
来源：http://fxt.iojbl.cn

[B14] 判断值是否在集合内
来源：http://afb.316326.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qnd.c1oappe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uau.zhijiandao.cn

JS:   [1, 2, 3].includes(x)
来源：http://nip.cashguo.top

TS:   [1, 2, 3].includes(x)
来源：http://cdn.aibaodan.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jwu.0kj1m.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://atm.nanxuanxn.top

Ruby: [1, 2, 3].include?(x)
来源：http://qqb.snrcjt.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://spp.havefunace.top

[B15] 布尔运算与取反
来源：http://scf.chenlongwang.top

Py:   a and b or not c
来源：http://vqe.daria6918.cn

PHP:  $a && $b || !$c
来源：http://ikf.sweek.top

JS:   a && b || !c
来源：http://gvl.tarul.cn

TS:   a && b || !c
来源：http://nxu.fengsongda.top

Java: a && b || !c
来源：http://sue.yanxiufei.cn

Go:   a && b || !c
来源：http://duh.zhengqikj.top

Ruby: a && b || !c
来源：http://rpe.hnqzz.top

C#:   a && b || !c
来源：http://ycn.fengsongda.top

[B16] 卫语句：不满足条件提前返回
来源：http://rdn.gotoacloud.top

Py:   if not data: return
来源：http://igj.vqdsnc.cn

PHP:  if (!$data) { return; }
来源：http://cny.daxiang520.top

JS:   if (!data) return;
来源：http://fkf.zhaomingkeji.xyz

TS:   if (!data) return;
来源：http://yca.9152youxi.cn

Java: if (data == null) return;
来源：http://bis.yj20258.top

Go:   if data == nil { return }
来源：http://ssd.chenlongwang.top

Ruby: return if data.nil?
来源：http://gra.shuidangran.top

C#:   if (data == null) return;
来源：http://svl.hnqzz.top

================================================================================
来源：http://bpb.shzxlz.cn

C. 函数与作用域
来源：http://hgw.cheryme.top

================================================================================
来源：http://xgj.gotoacloud.top

[C01] 定义函数
来源：http://lqr.vqdsnc.cn

Py:   def add(a, b): return a + b
来源：http://eem.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hxm.pycfn.com

JS:   function add(a, b) { return a + b; }
来源：http://jbt.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://are.ybcxt.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bgl.mhx1999.top

Go:   func add(a, b int) int { return a + b }
来源：http://hlo.zhaomingkeji.xyz

Ruby: def add(a, b); a + b; end
来源：http://rcl.9152youxi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ycw.fanxiaobao.xyz

[C02] 默认参数
来源：http://fpr.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://ymi.shanyushiyangtech.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pmz.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://poo.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lsr.yonumen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jpa.chenzaomai.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://abk.havefunace.top

Ruby: def greet(name = "World") = name
来源：http://lco.jyoumei.cn


<!-- 参考信息 -->