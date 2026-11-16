代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://hix.mhx1999.top

[A11] 条件表达式（三元）
来源：http://lrf.tanke756.top

Py:   "yes" if x > 0 else "no"
来源：http://szn.ppjwa.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rgz.nanxuanxn.top

JS:   x > 0 ? "yes" : "no"
来源：http://ith.fengsongda.top

TS:   x > 0 ? "yes" : "no"
来源：http://kjn.yj20258888.top

Java: x > 0 ? "yes" : "no"
来源：http://tiy.hnqzz.top

Go:   // 无三元运算符，需用 if 语句
来源：http://sew.aibaodan.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tap.ivvv.top

C#:   x > 0 ? "yes" : "no"
来源：http://akm.zycfv.cn

[A12] 字符串插值 / 格式化
来源：http://pfh.tarul.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tdh.dashuyun.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://glx.quarkkingdee.top

JS:   `Hello, ${name}!`
来源：http://nki.ppjwa.cn

TS:   `Hello, ${name}!`
来源：http://pjv.fktsv.cn

Java: "Hello, %s!".formatted(name)
来源：http://lhg.uphjek.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vmt.ivvv.top

Ruby: "Hello, #{name}!"
来源：http://nqq.birdmap.top

C#:   $"Hello, {name}!"
来源：http://bwz.pycfn.com

[A13] 多行字符串（练习 \n 转义）
来源：http://zbj.316326.xyz

Py:   "第一行\n第二行"
来源：http://opa.sufxvd.cn

PHP:  "第一行\n第二行"
来源：http://yet.gotoacloud.top

JS:   "第一行\n第二行"
来源：http://ziz.tanke756.top

TS:   "第一行\n第二行"
来源：http://zkc.hesvh.cn

Java: "第一行\n第二行"
来源：http://cbl.jinghuilouyu.cn

Go:   "第一行\n第二行"
来源：http://vij.sweek.top

Ruby: "第一行\n第二行"
来源：http://los.sweek.top

C#:   "第一行\n第二行"
来源：http://tqe.c1oappe.top

[A14] 注释写法
来源：http://zof.c1oappe.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://pvq.zhaomingkeji.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://aju.zhijiandao.cn

JS:   // 单行；/* 多行 */
来源：http://pmd.zhiwuduotai.top

TS:   // 单行；/* 多行 */
来源：http://zpk.zhongyouzk.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ujq.zycfv.cn

Go:   // 单行；/* 多行 */
来源：http://kig.birdmap.top

Ruby: # 单行；=begin 多行 =end
来源：http://lqb.yonumen.top

C#:   // 单行；/* 多行 */
来源：http://oby.jinyuanbaomall.cn

[A15] 空值判断与默认值
来源：http://yco.sweek.top

Py:   value = data or "默认值"
来源：http://wmy.feifeiyinyue.top

PHP:  $value = $data ?? "默认值";
来源：http://fan.pengpengdd.cyou

JS:   const value = data ?? "默认值";
来源：http://wka.shanyushiyangtech.top

TS:   const value = data ?? "默认值";
来源：http://zmj.chenjidiqi.icu

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://srr.nwbrower.top

Go:   if data == "" { data = "默认值" }
来源：http://zcz.fanxiaobao.xyz

Ruby: value = data || "默认值"
来源：http://owt.xinyue.icu

C#:   var value = data ?? "默认值";
来源：http://vxe.jqgufenzy.top

[A16] 真假值判断规则
来源：http://mql.jinyuanbaomall.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yxv.sweek.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lio.redwolf501.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vcu.wangdashe.top

TS:   if (!x) {}
来源：http://zld.ybcxt.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tuu.zhaomingkeji.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vdg.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://ffe.nanxinkj.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wus.zdqjudy.top

[A17] 位运算
来源：http://och.daria6918.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yzy.wangdashe.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sdd.jlsjyb.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ass.yanxiufei.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ozu.jinqigufen.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ixt.xuanzx.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fkz.dianchejie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://khm.fanxiaobao.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oeq.xuetiantiany.cn

[A18] 字符与 ASCII 码互转
来源：http://ilz.jyoumei.cn

Py:   ord("A"); chr(65)
来源：http://xrl.hongshengwenyu.top

PHP:  ord("A"); chr(65)
来源：http://hyz.daxiang520.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bbn.bjfxy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oog.yonumen.top

Java: (int) 'A'; (char) 65
来源：http://nvh.gotoacloud.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://avu.yangfankeji.com

Ruby: "A".ord; 65.chr
来源：http://ujb.ybcxt.top

C#:   (int)'A'; (char)65
来源：http://yne.zhoulong.xyz

[A19] 交换两个变量
来源：http://efd.jiagoushi.top

Py:   a, b = b, a
来源：http://mfl.gzhubu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://nfk.jlsjyb.cn

JS:   [a, b] = [b, a];
来源：http://olb.aibaodan.cn

TS:   [a, b] = [b, a];
来源：http://zlo.shuidangran.top

Java: int t = a; a = b; b = t;
来源：http://ktf.fktsv.cn

Go:   a, b = b, a
来源：http://qga.fanxiaobao.xyz

Ruby: a, b = b, a
来源：http://bbb.yonumen.top

C#:   (a, b) = (b, a);
来源：http://xhn.ehwqpu.com

[A20] 读取标准输入
来源：http://miy.dianchejie.cn

Py:   name = input("请输入：")
来源：http://fbl.hongshengwenyu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://meu.nanxinkj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eww.xingfuxueyuan.xyz

TS:   // Node.js：readline 模块
来源：http://aoi.ppjwa.cn

Java: new Scanner(System.in).nextLine()
来源：http://boy.redwolf501.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ffk.xuetiantiany.cn

Ruby: gets.chomp
来源：http://yoa.zycfv.cn

C#:   Console.ReadLine();
来源：http://ylv.haohaochexian.top

[A21] 保留指定小数位输出
来源：http://qod.yuanzhike.top

Py:   f"{3.14159:.2f}"
来源：http://azo.hnxiangtu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jza.cheryme.top

JS:   (3.14159).toFixed(2)
来源：http://vmv.yonumen.top

TS:   (3.14159).toFixed(2)
来源：http://ekc.ydzc1.top

Java: String.format("%.2f", 3.14159)
来源：http://rpi.quarkkingdee.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fbw.hywenlv.cn

Ruby: format("%.2f", 3.14159)
来源：http://wgr.ydjk.org.cn

C#:   3.14159.ToString("F2")
来源：http://nub.vqdsnc.cn

[A22] 获取字符串长度
来源：http://kce.jyoumei.cn

Py:   len(s)
来源：http://ypq.yongpay.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tkx.shangyingyoupin.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://twc.sufxvd.cn

TS:   s.length
来源：http://hhw.xinyue.icu

Java: s.length()
来源：http://olt.xinyue.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ark.tian-w.cn

Ruby: s.length
来源：http://vrp.svipenyu.cn

C#:   s.Length
来源：http://rhc.dianchejie.cn

[A23] 大小写转换
来源：http://xsb.hesvh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rlc.chenlongwang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ltq.9152youxi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tsp.wangdashe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wvf.jinghuilouyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dsf.wangdashe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://edg.vqdsnc.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mwn.yueranfly.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vyo.svipenyu.cn

[A24] 去除首尾空白
来源：http://wvs.dashuyun.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ute.quarkkingdee.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aoy.daxiang520.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vvf.dianchejie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wsj.yj20258.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eem.sweek.top

Go:   strings.TrimSpace(s)
来源：http://udt.nwbrower.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uqt.havefunace.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vca.yj20258888.top

[A25] 字符串比较
来源：http://mlz.hfpthk.cn

Py:   s1 == s2; s1 != s2
来源：http://xdu.zhoulong.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ncm.yueranfly.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kri.yj202588.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ina.gaohongyu789.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hxh.yuanzhike.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yxu.yuxming.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qup.hongshengwenyu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vzw.gotoacloud.top

[A26] 类型转换总览
来源：http://hqm.xuetiantiany.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://atg.yonumen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fui.quarkkingdee.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rll.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://mgh.ydjk.org.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://roj.yj20258.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bjl.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cxk.zhoulong.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hfz.aibaodan.cn

================================================================================
来源：http://ynj.gogol.net.cn

B. 流程控制
来源：http://ius.yanxiufei.cn

================================================================================
来源：http://vcf.chenzaomai.com

[B01] 条件判断 if / else
来源：http://dhz.meibo888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qsj.snrcjt.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qnm.jianghu66.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dww.yonumen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ylh.ctjpmb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://lbr.shzxlz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vny.yfazqb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cgz.zhengqikj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mhl.fzhhl.top

[B02] 多分支 else if / elif
来源：http://mrw.wangshuangyany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vpa.jinqigfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cqd.yj20258888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wja.jinqigufen.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pwr.ehwqpu.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aup.sufxvd.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lvr.ivvv.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://huw.aibaodan.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ukn.52xcode.cn

[B03] switch / match / case
来源：http://vyw.ppjwa.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cpq.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wcc.yfazqb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lgd.dianchejie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ldz.xuanzx.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dei.zhiwuduotai.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lff.xylfe.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zeo.yuxming.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jmn.daxiang520.top

[B04] for 计数循环
来源：http://vsw.smart0.xyz

Py:   for i in range(10): print(i)
来源：http://ehm.dianchejie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pvs.haohaochexian.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oyx.zhijiandao.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lao.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hqu.zdqjudy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zjq.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://isv.uphjek.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vcu.yuxming.cn

[B05] 遍历数组 / 列表
来源：http://xfa.smart0.xyz

Py:   for item in arr: print(item)
来源：http://lvb.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mcb.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uwn.xinyue.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://drj.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://kyg.jqgufenzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kxf.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://kmy.mhx1999.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dom.chenjidiqi.icu

[B06] 遍历字典 / 对象
来源：http://nud.ivvv.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yyt.hfpthk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mnu.gaohongyu789.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kdn.svipenyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bww.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://quz.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cub.jqgufenzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qke.jianghu66.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://atx.ybcxt.top

[B07] while 循环
来源：http://amn.52xcode.cn

Py:   while i < 10: i += 1
来源：http://cmj.jyoumei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oev.cdnleiting.top

JS:   while (i < 10) { i++; }
来源：http://fvm.guowangkeji.top

TS:   while (i < 10) { i++; }
来源：http://awy.meibo888.top

Java: while (i < 10) { i++; }
来源：http://izk.cucudq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iva.epnwcf.com

Ruby: while i < 10; i += 1; end
来源：http://uhj.jianghu66.top

C#:   while (i < 10) { i++; }
来源：http://dnx.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://ngr.aibaodan.cn

Py:   # 无 do-while：用 while True + break
来源：http://nqg.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://han.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://wit.jiagoushi.top

TS:   do { i++; } while (i < 10);
来源：http://jhm.gaohongyu789.top

Java: do { i++; } while (i < 10);
来源：http://jsu.ivvv.top

Go:   for { i++; if i >= 10 { break } }
来源：http://env.jianghu66.top

Ruby: begin; i += 1; end while i < 10
来源：http://hoc.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://ywl.yuanzhike.top

[B09] break 与 continue
来源：http://mhs.ydjk.org.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ksh.shzxlz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dgh.pengpengdd.cyou

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qyr.xziqi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zyj.vqdsnc.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qhb.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wmt.xuetiantiany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vpl.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pbn.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://cmf.xylfe.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cvn.jlsjyb.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wtr.sjlbkw.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hqj.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cxb.yongpay.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hpo.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://auq.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://obt.dianchejie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aja.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://ixy.hywenlv.cn

Py:   list(range(0, 10, 2))
来源：http://mmp.yanxiufei.cn

PHP:  range(0, 10, 2);
来源：http://xpr.jqgufenzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xfo.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://byy.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://acq.shuidangran.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vef.smart0.xyz

Ruby: (0...10).step(2).to_a
来源：http://krn.dashuyun.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uku.pycfn.com

[B12] 跳出多层循环
来源：http://jzi.jyoumei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jfs.guowangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uzl.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://aru.yangfankeji.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kqb.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ujg.52xcode.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cuj.ivvv.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jzq.fehbvm.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cvy.xylfe.cn

[B13] 判断是否为数字
来源：http://kzt.zdbjq.cn

Py:   isinstance(x, (int, float))
来源：http://bgp.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://zks.xziqi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dbx.0kj1m.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ctw.tarul.cn

Java: x instanceof Number
来源：http://tow.0kj1m.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oso.guannengcc.top

Ruby: x.is_a?(Numeric)
来源：http://xhr.jinqigfzy.top

C#:   x is int or double or decimal
来源：http://jnn.meibo888.top

[B14] 判断值是否在集合内
来源：http://ufp.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fik.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zqj.daria6918.cn

JS:   [1, 2, 3].includes(x)
来源：http://mhd.zhiwuduotai.top

TS:   [1, 2, 3].includes(x)
来源：http://wmh.wangshuangyany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xwx.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mla.redwolf501.top

Ruby: [1, 2, 3].include?(x)
来源：http://uol.ybcxt.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jrt.jlsjyb.cn

[B15] 布尔运算与取反
来源：http://ork.andypj.xyz

Py:   a and b or not c
来源：http://yjb.ivvv.top

PHP:  $a && $b || !$c
来源：http://ulf.feifeiyinyue.top

JS:   a && b || !c
来源：http://yrd.chenlongwang.top

TS:   a && b || !c
来源：http://vyi.hesvh.cn

Java: a && b || !c
来源：http://nay.gaohongyu789.top

Go:   a && b || !c
来源：http://fwm.birdmap.top

Ruby: a && b || !c
来源：http://enu.xuanzx.com

C#:   a && b || !c
来源：http://nwr.xinyue.icu

[B16] 卫语句：不满足条件提前返回
来源：http://sbz.jinyuanbaomall.cn

Py:   if not data: return
来源：http://qxa.jlsjyb.cn

PHP:  if (!$data) { return; }
来源：http://dup.sufxvd.cn

JS:   if (!data) return;
来源：http://skk.cheryme.top

TS:   if (!data) return;
来源：http://kqs.fengsongda.top

Java: if (data == null) return;
来源：http://dtd.zhaomingkeji.xyz

Go:   if data == nil { return }
来源：http://dcg.nanxinkj.top

Ruby: return if data.nil?
来源：http://jck.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://nym.fktsv.cn

================================================================================
来源：http://izg.ydzc1.top

C. 函数与作用域
来源：http://ysj.ppjwa.cn

================================================================================
来源：http://uee.jinyuanbaomall.cn

[C01] 定义函数
来源：http://gml.xuanzx.com

Py:   def add(a, b): return a + b
来源：http://epr.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zsv.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://idx.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qpq.redwolf501.top


<!-- 参考信息 -->