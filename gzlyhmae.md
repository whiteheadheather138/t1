代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://lii.ctjpmb.com

C#:   x > 0 ? "yes" : "no"
来源：http://bhb.shanyushiyangkeji.top

[A12] 字符串插值 / 格式化
来源：http://lux.yuxming.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uwp.andypj.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vkm.aibaodan.cn

JS:   `Hello, ${name}!`
来源：http://ruf.xziqi.cn

TS:   `Hello, ${name}!`
来源：http://kam.chenzaomai.com

Java: "Hello, %s!".formatted(name)
来源：http://ola.andypj.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ctv.iojbl.cn

Ruby: "Hello, #{name}!"
来源：http://kbf.kuanghao11.cn

C#:   $"Hello, {name}!"
来源：http://iua.jqgfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://yew.sufxvd.cn

Py:   "第一行\n第二行"
来源：http://xvz.jiagoushi.top

PHP:  "第一行\n第二行"
来源：http://igr.jinqigufen.top

JS:   "第一行\n第二行"
来源：http://dpx.tianlin.xyz

TS:   "第一行\n第二行"
来源：http://ijl.xziqi.cn

Java: "第一行\n第二行"
来源：http://yab.yj20258.top

Go:   "第一行\n第二行"
来源：http://dpb.hammf.cn

Ruby: "第一行\n第二行"
来源：http://sdc.pengpengdd.cyou

C#:   "第一行\n第二行"
来源：http://bed.52xcode.cn

[A14] 注释写法
来源：http://tos.yvedp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://loo.yj20258888.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dna.mhx1999.top

JS:   // 单行；/* 多行 */
来源：http://rlu.hammf.cn

TS:   // 单行；/* 多行 */
来源：http://hdj.nanxinkj.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lnf.andypj.xyz

Go:   // 单行；/* 多行 */
来源：http://jad.vqdsnc.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hzz.ybcxt.top

C#:   // 单行；/* 多行 */
来源：http://mwy.yanxiufei.cn

[A15] 空值判断与默认值
来源：http://iva.ppjwa.cn

Py:   value = data or "默认值"
来源：http://cxh.dashuyun.cn

PHP:  $value = $data ?? "默认值";
来源：http://wxd.yanxiufei.cn

JS:   const value = data ?? "默认值";
来源：http://yxw.316326.xyz

TS:   const value = data ?? "默认值";
来源：http://krl.nanxuanxn.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ovi.yonumen.top

Go:   if data == "" { data = "默认值" }
来源：http://qyl.jinqigfzy.top

Ruby: value = data || "默认值"
来源：http://wcl.kuanghao11.cn

C#:   var value = data ?? "默认值";
来源：http://gld.snrcjt.cn

[A16] 真假值判断规则
来源：http://dnz.fengsongda.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nwy.dashuyun.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bsh.guowangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nea.xuanzx.com

TS:   if (!x) {}
来源：http://gww.nanxuanxn.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ijx.gotoacloud.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://agw.shanyushiyangkeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://irn.yueranfly.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nwq.ywan-chungtsiang.top

[A17] 位运算
来源：http://fmd.yueranfly.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://twa.chenlongwang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hmf.ctjpmb.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ors.birdmap.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tiw.xinyue.icu

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rmj.xuanzx.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ncj.xziqi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://brc.haohaochexian.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lwn.mhx1999.top

[A18] 字符与 ASCII 码互转
来源：http://wav.nanxinkj.top

Py:   ord("A"); chr(65)
来源：http://vgy.0kj1m.cn

PHP:  ord("A"); chr(65)
来源：http://kvt.hongshengwenyu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dyv.52xcode.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://maf.xingfuxueyuan.xyz

Java: (int) 'A'; (char) 65
来源：http://arw.snrcjt.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ock.nanxuanxn.top

Ruby: "A".ord; 65.chr
来源：http://lrb.ywan-chungtsiang.top

C#:   (int)'A'; (char)65
来源：http://upz.bbcook.cn

[A19] 交换两个变量
来源：http://woz.zhixingplan.top

Py:   a, b = b, a
来源：http://bgv.chenjidiqi.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://rwz.vehdjk.com

JS:   [a, b] = [b, a];
来源：http://ojb.yfazqb.com

TS:   [a, b] = [b, a];
来源：http://zrh.ywan-chungtsiang.top

Java: int t = a; a = b; b = t;
来源：http://rby.bjfxy.top

Go:   a, b = b, a
来源：http://uyp.yuxming.cn

Ruby: a, b = b, a
来源：http://fex.kuanghao11.cn

C#:   (a, b) = (b, a);
来源：http://bvh.wangshuangyany.cn

[A20] 读取标准输入
来源：http://cwb.epnwcf.com

Py:   name = input("请输入：")
来源：http://mul.yvedp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ntq.shangyingyoupin.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ykw.nanxinkj.top

TS:   // Node.js：readline 模块
来源：http://vhc.fktsv.cn

Java: new Scanner(System.in).nextLine()
来源：http://glx.smart0.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xeh.cashguo.top

Ruby: gets.chomp
来源：http://xzi.bjfxy.top

C#:   Console.ReadLine();
来源：http://jwx.pycfn.com

[A21] 保留指定小数位输出
来源：http://qbf.zhoulong.xyz

Py:   f"{3.14159:.2f}"
来源：http://yji.jinghuilouyu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vwv.tarul.cn

JS:   (3.14159).toFixed(2)
来源：http://ngw.fktsv.cn

TS:   (3.14159).toFixed(2)
来源：http://hzr.jinqigufen.top

Java: String.format("%.2f", 3.14159)
来源：http://uzb.zhaomingkeji.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oyp.cdnleiting.top

Ruby: format("%.2f", 3.14159)
来源：http://zqj.zhengqikj.top

C#:   3.14159.ToString("F2")
来源：http://nwb.zhixingplan.top

[A22] 获取字符串长度
来源：http://drb.bjfxy.top

Py:   len(s)
来源：http://mxi.shanyushiyangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ixg.hammf.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bld.pengpengdd.cyou

TS:   s.length
来源：http://dbm.yonumen.top

Java: s.length()
来源：http://hnq.hysaishi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qbt.ydzc1.top

Ruby: s.length
来源：http://gah.yueranfly.top

C#:   s.Length
来源：http://hoe.yonumen.top

[A23] 大小写转换
来源：http://uwm.52xcode.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://edo.fengsongda.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bdu.ppjwa.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fri.c1oappe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://abj.hnqzz.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mgh.52xcode.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uxz.guannengcc.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ryu.0kj1m.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lyq.vehdjk.com

[A24] 去除首尾空白
来源：http://ldp.zhaomingkeji.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://abm.jlsjyb.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cof.uphjek.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://neg.sufxvd.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oay.shuidangran.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gso.kuanghao11.cn

Go:   strings.TrimSpace(s)
来源：http://kgi.cucudq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ohp.ywan-chungtsiang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oes.ivvv.top

[A25] 字符串比较
来源：http://fur.aibaodan.cn

Py:   s1 == s2; s1 != s2
来源：http://cuk.xylfe.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jfs.pengpengdd.cyou

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tlc.yj20258888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eav.hnqzz.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xgg.shzxlz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gum.birdmap.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vmy.xziqi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uyf.ydjk.org.cn

[A26] 类型转换总览
来源：http://eis.kuanghao11.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ukd.shanyushiyangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://url.hesvh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fdk.ybcxt.top

TS:   Number() String() Boolean() x as number
来源：http://aef.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wzz.yuxming.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jht.sxryk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ice.meibo888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wbk.yongpay.top

================================================================================
来源：http://shk.daria6918.cn

B. 流程控制
来源：http://rdl.zhijiandao.cn

================================================================================
来源：http://exd.havefunace.top

[B01] 条件判断 if / else
来源：http://pde.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yjm.hesvh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mxk.bbcook.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pye.ybcxt.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oeu.jinyuanbaomall.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bgt.yangfankeji.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lvk.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pdy.yongpay.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yvm.fanxiaobao.xyz

[B02] 多分支 else if / elif
来源：http://ymf.snrcjt.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://guz.tianlin.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yoi.cashguo.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lzm.jqgufenzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oth.jqgufenzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hag.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hif.gaohongyu789.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sss.xziqi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qpl.fktsv.cn

[B03] switch / match / case
来源：http://vtl.nanxinkj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lau.yuxming.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fog.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://juj.chenlongwang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wur.tian-w.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dzc.jiagoushi.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ndj.yuxming.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jde.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cwb.zhixingplan.top

[B04] for 计数循环
来源：http://vao.hcnkem.com

Py:   for i in range(10): print(i)
来源：http://epy.xziqi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nph.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://avw.hysaishi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qpm.hammf.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gkd.fktsv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cre.zhongyouzk.top

Ruby: 10.times { |i| puts i }
来源：http://lhj.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rla.zhoulong.xyz

[B05] 遍历数组 / 列表
来源：http://nhr.zycfv.cn

Py:   for item in arr: print(item)
来源：http://nkt.shzxlz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qys.yj20258.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vmd.316326.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://vvj.tian-w.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vop.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pot.daria6918.cn

Ruby: arr.each { |item| puts item }
来源：http://gxd.meibo888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fkr.epnwcf.com

[B06] 遍历字典 / 对象
来源：http://idx.ywan-chungtsiang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vdq.ehwqpu.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rye.nanxinkj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mux.ppjwa.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tgf.tanke756.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kxu.dashuyun.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://goj.fehbvm.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xxc.fktsv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://stu.epnwcf.com

[B07] while 循环
来源：http://boc.yonumen.top

Py:   while i < 10: i += 1
来源：http://mal.meibo888.top

PHP:  while ($i < 10) { $i++; }
来源：http://fju.xingfuxueyuan.xyz

JS:   while (i < 10) { i++; }
来源：http://fwy.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://ukn.ywan-chungtsiang.top

Java: while (i < 10) { i++; }
来源：http://ocl.sjlbkw.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gco.daria6918.cn

Ruby: while i < 10; i += 1; end
来源：http://lxk.yanxiufei.cn

C#:   while (i < 10) { i++; }
来源：http://oxh.hnqzz.top

[B08] do-while（至少执行一次）
来源：http://oqf.gzhubu.top

Py:   # 无 do-while：用 while True + break
来源：http://xzp.iojbl.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tjg.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://kvw.guannengcc.top

TS:   do { i++; } while (i < 10);
来源：http://paw.nanxuanxn.top

Java: do { i++; } while (i < 10);
来源：http://zlv.vehdjk.com

Go:   for { i++; if i >= 10 { break } }
来源：http://wdd.ehwqpu.com

Ruby: begin; i += 1; end while i < 10
来源：http://vzf.sysykeji.top

C#:   do { i++; } while (i < 10);
来源：http://bwy.tian-w.cn

[B09] break 与 continue
来源：http://jnb.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ijt.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xiw.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://afz.cashguo.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xzr.bbcook.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kmh.ppjwa.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fcu.0kj1m.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://axy.jqgfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jjx.sysykeji.top

[B10] 遍历同时拿索引
来源：http://fcx.tian-w.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ajv.zdbjq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rtx.bjfxy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qkn.hnxiangtu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fnv.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tok.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nfo.redwolf501.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nko.52xcode.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mmh.feifeiyinyue.top

[B11] 生成数字序列 / 区间
来源：http://juz.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://vcu.cashguo.top

PHP:  range(0, 10, 2);
来源：http://axo.xinyue.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tat.svipenyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ulr.zhoulong.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xcq.shuidangran.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://frr.quarkkingdee.top

Ruby: (0...10).step(2).to_a
来源：http://fyp.bjfxy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rwo.jianghu66.top

[B12] 跳出多层循环
来源：http://onf.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ltd.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jrb.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://aes.hcnkem.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lfn.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wkp.jinqigfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cua.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qyy.jinqigufen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fpu.birdmap.top

[B13] 判断是否为数字
来源：http://jjm.yuanzhike.top

Py:   isinstance(x, (int, float))
来源：http://xzs.hcnkem.com

PHP:  is_numeric($x)
来源：http://fyz.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vkz.hesvh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yre.fehbvm.com

Java: x instanceof Number
来源：http://fvg.zhixingplan.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://irt.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://bqs.yongpay.top

C#:   x is int or double or decimal
来源：http://vmo.snrcjt.cn

[B14] 判断值是否在集合内
来源：http://pyl.sufxvd.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://myc.zhijiandao.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ibm.guowangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://bus.gzhubu.top

TS:   [1, 2, 3].includes(x)
来源：http://rwa.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nhw.dianchejie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mps.zhengqikj.top

Ruby: [1, 2, 3].include?(x)
来源：http://uvn.ivvv.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cuh.zhaomingkeji.xyz

[B15] 布尔运算与取反
来源：http://bur.daxiang520.top

Py:   a and b or not c
来源：http://wyh.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://seg.xylfe.cn

JS:   a && b || !c
来源：http://njf.9152youxi.cn

TS:   a && b || !c
来源：http://huc.tian-w.cn

Java: a && b || !c
来源：http://gag.fktsv.cn

Go:   a && b || !c
来源：http://dxr.tianlin.xyz

Ruby: a && b || !c
来源：http://ewv.zdbjq.cn

C#:   a && b || !c
来源：http://vco.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lao.meibo888.top

Py:   if not data: return
来源：http://ada.hfpthk.cn

PHP:  if (!$data) { return; }
来源：http://qtn.gzhubu.top

JS:   if (!data) return;
来源：http://jrb.snrcjt.cn

TS:   if (!data) return;
来源：http://cyi.meibo888.top

Java: if (data == null) return;
来源：http://kxn.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://mtd.hysaishi.cn

Ruby: return if data.nil?
来源：http://kul.zhixingplan.top

C#:   if (data == null) return;
来源：http://xcw.nanxinkj.top

================================================================================
来源：http://hqd.mhx1999.top

C. 函数与作用域
来源：http://xhg.uphjek.com

================================================================================
来源：http://cnv.sufxvd.cn

[C01] 定义函数
来源：http://ksm.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://wjd.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wfh.fehbvm.com

JS:   function add(a, b) { return a + b; }
来源：http://gxg.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qwn.xziqi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dkh.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gnc.fktsv.cn

Ruby: def add(a, b); a + b; end
来源：http://obu.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jpm.9152youxi.cn

[C02] 默认参数
来源：http://pua.gaohongyu789.top

Py:   def greet(name="World"): return name
来源：http://mig.dianchejie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zlz.sxryk.cn

JS:   function greet(name = "World") { return name; }
来源：http://bze.cheryme.top


<!-- 参考信息 -->