代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://ucp.fzhhl.top

C#:   x > 0 ? "yes" : "no"
来源：http://cav.bjfxy.top

[A12] 字符串插值 / 格式化
来源：http://xyt.zhongyouzk.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wke.shangyingyoupin.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rgw.jyoumei.cn

JS:   `Hello, ${name}!`
来源：http://ons.fengsongda.top

TS:   `Hello, ${name}!`
来源：http://btl.zdqjudy.top

Java: "Hello, %s!".formatted(name)
来源：http://xmy.epnwcf.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uko.snrcjt.cn

Ruby: "Hello, #{name}!"
来源：http://ahg.sysykeji.top

C#:   $"Hello, {name}!"
来源：http://ufy.9152youxi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ysx.yuanzhike.top

Py:   "第一行\n第二行"
来源：http://eia.aibaodan.cn

PHP:  "第一行\n第二行"
来源：http://gmv.yonumen.top

JS:   "第一行\n第二行"
来源：http://xjb.aizwys.cn

TS:   "第一行\n第二行"
来源：http://mer.redwolf501.top

Java: "第一行\n第二行"
来源：http://gdr.xingfuxueyuan.xyz

Go:   "第一行\n第二行"
来源：http://jxg.cqqwz.cn

Ruby: "第一行\n第二行"
来源：http://aes.gaohongyu789.top

C#:   "第一行\n第二行"
来源：http://kbw.aizwys.cn

[A14] 注释写法
来源：http://tkl.hnxiangtu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rsz.wangdashe.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dxi.mhx1999.top

JS:   // 单行；/* 多行 */
来源：http://pky.havefunace.top

TS:   // 单行；/* 多行 */
来源：http://rra.bjfxy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gay.shangyingyoupin.top

Go:   // 单行；/* 多行 */
来源：http://xny.jianghu66.top

Ruby: # 单行；=begin 多行 =end
来源：http://zem.xylfe.cn

C#:   // 单行；/* 多行 */
来源：http://aux.hongshengwenyu.top

[A15] 空值判断与默认值
来源：http://hju.tian-w.cn

Py:   value = data or "默认值"
来源：http://aqf.xuetiantiany.cn

PHP:  $value = $data ?? "默认值";
来源：http://avq.yj20258.top

JS:   const value = data ?? "默认值";
来源：http://dsh.xziqi.cn

TS:   const value = data ?? "默认值";
来源：http://znq.kuanghao11.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://agn.aibaodan.cn

Go:   if data == "" { data = "默认值" }
来源：http://zzh.yanxiufei.cn

Ruby: value = data || "默认值"
来源：http://zzz.hcnkem.com

C#:   var value = data ?? "默认值";
来源：http://jlt.316326.xyz

[A16] 真假值判断规则
来源：http://koy.yj20258.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sfz.ywan-chungtsiang.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wtc.haohaochexian.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sfl.tanke756.top

TS:   if (!x) {}
来源：http://plk.wangshuangyany.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zti.tanke756.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pva.ppjwa.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gsk.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zij.zhaomingkeji.xyz

[A17] 位运算
来源：http://sfd.shangyingyoupin.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wnl.chenlongwang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cje.jinyuanbaomall.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://arj.svipenyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gnc.havefunace.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vxp.yangfankeji.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rvy.dashuyun.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pgv.hysaishi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://adk.chenjidiqi.icu

[A18] 字符与 ASCII 码互转
来源：http://mun.zhijiandao.cn

Py:   ord("A"); chr(65)
来源：http://nyj.jinghuilouyu.cn

PHP:  ord("A"); chr(65)
来源：http://wkt.xylfe.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://clt.jlsjyb.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ret.nanxinkj.top

Java: (int) 'A'; (char) 65
来源：http://zip.hnxiangtu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mzg.guowangkeji.top

Ruby: "A".ord; 65.chr
来源：http://phj.vqdsnc.cn

C#:   (int)'A'; (char)65
来源：http://kcy.wangdashe.top

[A19] 交换两个变量
来源：http://kaj.hnxiangtu.top

Py:   a, b = b, a
来源：http://zjs.yvedp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://phr.hongshengwenyu.top

JS:   [a, b] = [b, a];
来源：http://qmf.snrcjt.cn

TS:   [a, b] = [b, a];
来源：http://soo.hysaishi.cn

Java: int t = a; a = b; b = t;
来源：http://nkt.yuanzhike.top

Go:   a, b = b, a
来源：http://jdb.redwolf501.top

Ruby: a, b = b, a
来源：http://geg.kuanghao11.cn

C#:   (a, b) = (b, a);
来源：http://teu.zhixingplan.top

[A20] 读取标准输入
来源：http://fgl.cashguo.top

Py:   name = input("请输入：")
来源：http://lec.ywan-chungtsiang.top

PHP:  $name = trim(fgets(STDIN));
来源：http://pqw.xuetiantiany.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bmf.0kj1m.cn

TS:   // Node.js：readline 模块
来源：http://hbx.yfazqb.com

Java: new Scanner(System.in).nextLine()
来源：http://sjm.sysykeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://izo.chenjidiqi.icu

Ruby: gets.chomp
来源：http://miy.pycfn.com

C#:   Console.ReadLine();
来源：http://xxf.jqgufenzy.top

[A21] 保留指定小数位输出
来源：http://zze.vqdsnc.cn

Py:   f"{3.14159:.2f}"
来源：http://eel.52xcode.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://axf.ctjpmb.com

JS:   (3.14159).toFixed(2)
来源：http://fbz.ydzc1.top

TS:   (3.14159).toFixed(2)
来源：http://oyy.cdnleiting.top

Java: String.format("%.2f", 3.14159)
来源：http://tot.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sai.zdqjudy.top

Ruby: format("%.2f", 3.14159)
来源：http://myu.shangyingyoupin.top

C#:   3.14159.ToString("F2")
来源：http://btm.jqgfzy.top

[A22] 获取字符串长度
来源：http://lsl.wangdashe.top

Py:   len(s)
来源：http://nap.9152youxi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qhk.tarul.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rmu.fktsv.cn

TS:   s.length
来源：http://nui.meibo888.top

Java: s.length()
来源：http://odz.gogol.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hjd.jqgufenzy.top

Ruby: s.length
来源：http://mpl.316326.xyz

C#:   s.Length
来源：http://phu.dashuyun.cn

[A23] 大小写转换
来源：http://gom.guannengcc.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qqp.chenzaomai.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kdb.havefunace.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yzt.feifeiyinyue.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iba.ywan-chungtsiang.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dsr.yangfankeji.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oga.xziqi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zub.xinyue.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://rmq.cucudq.cn

[A24] 去除首尾空白
来源：http://tnb.xylfe.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rhi.hfpthk.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://roj.feifeiyinyue.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://evv.fanxiaobao.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sml.ywan-chungtsiang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blh.chenzaomai.com

Go:   strings.TrimSpace(s)
来源：http://noa.fktsv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ode.jyoumei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://taq.zhaomingkeji.xyz

[A25] 字符串比较
来源：http://bzu.uphjek.com

Py:   s1 == s2; s1 != s2
来源：http://eds.zdbjq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://geg.c1oappe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zhc.52xcode.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://njp.sweek.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xnn.daxiang520.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yoq.zycfv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bbx.nwbrower.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xqj.chenjidiqi.icu

[A26] 类型转换总览
来源：http://zjv.xuetiantiany.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yhd.andypj.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lkk.jianghu66.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fov.hysaishi.cn

TS:   Number() String() Boolean() x as number
来源：http://xig.fanxiaobao.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ljx.meibo888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://afc.xylfe.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bvb.ehwqpu.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tcb.sweek.top

================================================================================
来源：http://gcy.zhijiandao.cn

B. 流程控制
来源：http://xmc.svipenyu.cn

================================================================================
来源：http://ymi.svipenyu.cn

[B01] 条件判断 if / else
来源：http://ywa.smart0.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://mco.iojbl.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tcl.dianchejie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ano.yanxiufei.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vtf.pycfn.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://ibw.uphjek.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fgs.guowangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sfo.snrcjt.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bet.bjfxy.top

[B02] 多分支 else if / elif
来源：http://mlg.yvedp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qxp.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cpl.epnwcf.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yah.xuanzx.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qcm.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tug.xziqi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mii.chenjidiqi.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pmw.gotoacloud.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ecy.bbcook.cn

[B03] switch / match / case
来源：http://kxq.yj20258.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lzo.daxiang520.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ubz.zycfv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wwk.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bmg.yangfankeji.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cml.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://inq.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bbl.ydzc1.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pgr.yvedp.cn

[B04] for 计数循环
来源：http://llu.chenzaomai.com

Py:   for i in range(10): print(i)
来源：http://eez.bbcook.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ysc.zhixingplan.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xnn.iojbl.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oby.vehdjk.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jkn.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rrv.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://wuo.yfazqb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ddz.9152youxi.cn

[B05] 遍历数组 / 列表
来源：http://qfz.jqgfzy.top

Py:   for item in arr: print(item)
来源：http://tdm.hongshengwenyu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cgl.chenzaomai.com

JS:   for (const item of arr) { console.log(item); }
来源：http://asv.gzhubu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vpx.meibo888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ekb.fanxiaobao.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://smr.jlsjyb.cn

Ruby: arr.each { |item| puts item }
来源：http://buf.52xcode.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ccz.jinqigfzy.top

[B06] 遍历字典 / 对象
来源：http://ykw.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zrb.yj202588.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://euz.ybcxt.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mmz.nwbrower.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zsc.hnxiangtu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bqc.pengpengdd.cyou

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ebc.jiagoushi.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eqq.fktsv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oix.tarul.cn

[B07] while 循环
来源：http://say.jinyuanbaomall.cn

Py:   while i < 10: i += 1
来源：http://yly.chenzaomai.com

PHP:  while ($i < 10) { $i++; }
来源：http://fkq.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://gmf.daria6918.cn

TS:   while (i < 10) { i++; }
来源：http://rqu.jqgfzy.top

Java: while (i < 10) { i++; }
来源：http://zjz.sweek.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aus.bjfxy.top

Ruby: while i < 10; i += 1; end
来源：http://dlg.ydzc1.top

C#:   while (i < 10) { i++; }
来源：http://gnk.yueranfly.top

[B08] do-while（至少执行一次）
来源：http://aoo.jinqigufen.top

Py:   # 无 do-while：用 while True + break
来源：http://ooz.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yfl.hnqzz.top

JS:   do { i++; } while (i < 10);
来源：http://euh.tian-w.cn

TS:   do { i++; } while (i < 10);
来源：http://pjv.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://boy.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mii.nanxuanxn.top

Ruby: begin; i += 1; end while i < 10
来源：http://ivi.shuidangran.top

C#:   do { i++; } while (i < 10);
来源：http://wgg.nanxinkj.top

[B09] break 与 continue
来源：http://umc.vqdsnc.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cuv.fanxiaobao.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vuy.nanxuanxn.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sjt.kuanghao11.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fvv.zhongyouzk.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uez.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oaj.pycfn.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bla.hammf.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xdf.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://nzd.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ata.tanke756.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kkg.sxryk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qrm.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zxv.yvedp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ybr.yanxiufei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uxu.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://brr.ydzc1.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ayg.gzhubu.top

[B11] 生成数字序列 / 区间
来源：http://oyt.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://oma.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://cgt.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tpt.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nra.chenzaomai.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sgb.andypj.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mhu.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://ruy.andypj.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qoe.nanxinkj.top

[B12] 跳出多层循环
来源：http://nyq.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mti.guowangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jpp.zhengqikj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wgk.daria6918.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://irc.pengpengdd.cyou

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qjy.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rsp.havefunace.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pra.sysykeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://whl.havefunace.top

[B13] 判断是否为数字
来源：http://uxf.tianlin.xyz

Py:   isinstance(x, (int, float))
来源：http://egk.hcnkem.com

PHP:  is_numeric($x)
来源：http://bpz.yj20258.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jeh.sxryk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xpl.havefunace.top

Java: x instanceof Number
来源：http://utt.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vvb.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://wet.cdnleiting.top

C#:   x is int or double or decimal
来源：http://dft.jyoumei.cn

[B14] 判断值是否在集合内
来源：http://awe.zhijiandao.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jkz.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ivb.shanyushiyangtech.top

JS:   [1, 2, 3].includes(x)
来源：http://mry.hysaishi.cn

TS:   [1, 2, 3].includes(x)
来源：http://ken.jinyuanbaomall.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ydw.ctjpmb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nem.0kj1m.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ckq.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wra.ctjpmb.com

[B15] 布尔运算与取反
来源：http://vzd.aibaodan.cn

Py:   a and b or not c
来源：http://sjd.hysaishi.cn

PHP:  $a && $b || !$c
来源：http://ise.xuanzx.com

JS:   a && b || !c
来源：http://nzu.52xcode.cn

TS:   a && b || !c
来源：http://dxp.fanxiaobao.xyz

Java: a && b || !c
来源：http://mvs.yvedp.cn

Go:   a && b || !c
来源：http://yip.xuanzx.com

Ruby: a && b || !c
来源：http://rie.dashuyun.cn

C#:   a && b || !c
来源：http://eai.haohaochexian.top

[B16] 卫语句：不满足条件提前返回
来源：http://euk.cucudq.cn

Py:   if not data: return
来源：http://qtz.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://plc.yj20258.top

JS:   if (!data) return;
来源：http://lci.xziqi.cn

TS:   if (!data) return;
来源：http://ivt.nanxinkj.top

Java: if (data == null) return;
来源：http://nyc.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://avx.sjlbkw.cn

Ruby: return if data.nil?
来源：http://out.jqgufenzy.top

C#:   if (data == null) return;
来源：http://rii.hywenlv.cn

================================================================================
来源：http://jjd.zhongyouzk.top

C. 函数与作用域
来源：http://shz.sweek.top

================================================================================
来源：http://fne.wangshuangyany.cn

[C01] 定义函数
来源：http://jbo.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://esa.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ylw.52xcode.cn

JS:   function add(a, b) { return a + b; }
来源：http://vgr.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yav.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ndm.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://vmg.xinyue.icu

Ruby: def add(a, b); a + b; end
来源：http://lwq.tanke756.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lpg.yonumen.top

[C02] 默认参数
来源：http://jik.tanke756.top

Py:   def greet(name="World"): return name
来源：http://cig.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bjh.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://zlg.ydzc1.top


<!-- 参考信息 -->