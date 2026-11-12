代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://osi.aibaodan.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gzq.jiagoushi.top

[A12] 字符串插值 / 格式化
来源：http://wks.yj20258.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mye.52xcode.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jdo.hysaishi.cn

JS:   `Hello, ${name}!`
来源：http://uxx.snrcjt.cn

TS:   `Hello, ${name}!`
来源：http://rkp.zycfv.cn

Java: "Hello, %s!".formatted(name)
来源：http://hce.havefunace.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gqk.wangdashe.top

Ruby: "Hello, #{name}!"
来源：http://sjc.ctjpmb.com

C#:   $"Hello, {name}!"
来源：http://bfn.tanke756.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ysj.hnqzz.top

Py:   "第一行\n第二行"
来源：http://vay.daria6918.cn

PHP:  "第一行\n第二行"
来源：http://akd.daxiang520.top

JS:   "第一行\n第二行"
来源：http://hso.hesvh.cn

TS:   "第一行\n第二行"
来源：http://zyp.snrcjt.cn

Java: "第一行\n第二行"
来源：http://ulx.chenjidiqi.icu

Go:   "第一行\n第二行"
来源：http://nti.mhx1999.top

Ruby: "第一行\n第二行"
来源：http://smq.bjfxy.top

C#:   "第一行\n第二行"
来源：http://hvu.zdqjudy.top

[A14] 注释写法
来源：http://wgt.yangfankeji.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://lvk.tianlin.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://mjt.chenjidiqi.icu

JS:   // 单行；/* 多行 */
来源：http://gmo.nanxuanxn.top

TS:   // 单行；/* 多行 */
来源：http://nbr.chenlongwang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://eyx.daxiang520.top

Go:   // 单行；/* 多行 */
来源：http://wyu.shzxlz.cn

Ruby: # 单行；=begin 多行 =end
来源：http://aom.cheryme.top

C#:   // 单行；/* 多行 */
来源：http://tdn.ivvv.top

[A15] 空值判断与默认值
来源：http://rps.zhaomingkeji.xyz

Py:   value = data or "默认值"
来源：http://dfp.gogol.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://caq.ydzc1.top

JS:   const value = data ?? "默认值";
来源：http://uid.wangdashe.top

TS:   const value = data ?? "默认值";
来源：http://gix.xinyue.icu

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oyx.yj20258.top

Go:   if data == "" { data = "默认值" }
来源：http://wpz.nanxuanxn.top

Ruby: value = data || "默认值"
来源：http://uwa.zhiwuduotai.top

C#:   var value = data ?? "默认值";
来源：http://tnw.kuanghao11.cn

[A16] 真假值判断规则
来源：http://bxz.wangshuangyany.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yvk.ppjwa.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lok.cqqwz.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kpo.tarul.cn

TS:   if (!x) {}
来源：http://gqh.ybcxt.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nek.bjfxy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qce.jianghu66.top

Ruby: unless x            # nil 与 false 为假
来源：http://bng.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rgf.daxiang520.top

[A17] 位运算
来源：http://cmm.shuidangran.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ctm.andypj.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nqs.snrcjt.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zyi.guowangkeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kkb.shangyingyoupin.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wfs.smart0.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zzt.xuetiantiany.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://axs.c1oappe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ptf.yonumen.top

[A18] 字符与 ASCII 码互转
来源：http://klc.hnqzz.top

Py:   ord("A"); chr(65)
来源：http://bfl.316326.xyz

PHP:  ord("A"); chr(65)
来源：http://rem.xziqi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qmt.nwbrower.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hxl.hcnkem.com

Java: (int) 'A'; (char) 65
来源：http://cqg.hongshengwenyu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hmz.fengsongda.top

Ruby: "A".ord; 65.chr
来源：http://tlj.quarkkingdee.top

C#:   (int)'A'; (char)65
来源：http://ljq.zhaomingkeji.xyz

[A19] 交换两个变量
来源：http://lrt.52xcode.cn

Py:   a, b = b, a
来源：http://pko.andypj.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://rxe.cdnleiting.top

JS:   [a, b] = [b, a];
来源：http://ern.gzhubu.top

TS:   [a, b] = [b, a];
来源：http://icg.hammf.cn

Java: int t = a; a = b; b = t;
来源：http://qtc.jyoumei.cn

Go:   a, b = b, a
来源：http://kay.hammf.cn

Ruby: a, b = b, a
来源：http://vae.yueranfly.top

C#:   (a, b) = (b, a);
来源：http://pjb.xuetiantiany.cn

[A20] 读取标准输入
来源：http://tpd.shuidangran.top

Py:   name = input("请输入：")
来源：http://wgl.52xcode.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bjq.fengsongda.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wue.sxryk.cn

TS:   // Node.js：readline 模块
来源：http://crl.snrcjt.cn

Java: new Scanner(System.in).nextLine()
来源：http://fja.sweek.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cdr.yuxming.cn

Ruby: gets.chomp
来源：http://rqo.yuanzhike.top

C#:   Console.ReadLine();
来源：http://wkp.hywenlv.cn

[A21] 保留指定小数位输出
来源：http://tkj.tianlin.xyz

Py:   f"{3.14159:.2f}"
来源：http://bxm.xylfe.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rku.fanxiaobao.xyz

JS:   (3.14159).toFixed(2)
来源：http://blt.hongshengwenyu.top

TS:   (3.14159).toFixed(2)
来源：http://ces.tianlin.xyz

Java: String.format("%.2f", 3.14159)
来源：http://alk.zhiwuduotai.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yev.pengpengdd.cyou

Ruby: format("%.2f", 3.14159)
来源：http://wsa.xuetiantiany.cn

C#:   3.14159.ToString("F2")
来源：http://hxn.9152youxi.cn

[A22] 获取字符串长度
来源：http://azc.nanxinkj.top

Py:   len(s)
来源：http://kcz.xuetiantiany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://csj.jyoumei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wbm.nanxinkj.top

TS:   s.length
来源：http://kyl.jinyuanbaomall.cn

Java: s.length()
来源：http://iqo.pengpengdd.cyou

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pxs.yj202588.top

Ruby: s.length
来源：http://pcl.zhongyouzk.top

C#:   s.Length
来源：http://hff.zdqjudy.top

[A23] 大小写转换
来源：http://zgn.xylfe.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ilf.gzhubu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cln.316326.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nhu.fanxiaobao.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jcj.uphjek.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xtc.yuxming.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tab.tian-w.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lxn.cucudq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ous.daria6918.cn

[A24] 去除首尾空白
来源：http://vze.zdbjq.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://scy.jinyuanbaomall.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gko.hammf.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://buw.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dyb.yvedp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hya.hongshengwenyu.top

Go:   strings.TrimSpace(s)
来源：http://ejf.sjlbkw.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cgg.tarul.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pwf.pycfn.com

[A25] 字符串比较
来源：http://fzu.xingfuxueyuan.xyz

Py:   s1 == s2; s1 != s2
来源：http://itg.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yoc.yonumen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xml.sysykeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eck.c1oappe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tei.yongpay.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dhd.aibaodan.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://won.c1oappe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kwo.kuanghao11.cn

[A26] 类型转换总览
来源：http://pgo.daria6918.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dnv.chenjidiqi.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yco.zdqjudy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yuw.bbcook.cn

TS:   Number() String() Boolean() x as number
来源：http://znb.zhijiandao.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lwt.tanke756.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bhc.xingfuxueyuan.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://kqj.jinqigfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cyf.ivvv.top

================================================================================
来源：http://epd.aizwys.cn

B. 流程控制
来源：http://zwy.yangfankeji.com

================================================================================
来源：http://hgw.jianghu66.top

[B01] 条件判断 if / else
来源：http://dgu.zhongyouzk.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fgj.52xcode.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ojy.zhongyouzk.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pnv.aizwys.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zqd.gaohongyu789.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jql.wangdashe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://var.svipenyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qdh.yongpay.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rgg.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://sbz.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ujk.smart0.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xul.zhongyouzk.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://upg.sxryk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yej.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://syn.bbcook.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xnj.daxiang520.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mzp.yj20258888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fjg.jinqigufen.top

[B03] switch / match / case
来源：http://kth.xziqi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ghy.jqgfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://olx.cashguo.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gyu.hesvh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ono.ybcxt.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gjn.shanyushiyangtech.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yib.ctjpmb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lxq.snrcjt.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zyh.sufxvd.cn

[B04] for 计数循环
来源：http://noa.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://xgy.shangyingyoupin.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lrs.vehdjk.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wkn.xingfuxueyuan.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ghi.xingfuxueyuan.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kvp.0kj1m.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tvy.yvedp.cn

Ruby: 10.times { |i| puts i }
来源：http://ozc.iojbl.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ujk.aizwys.cn

[B05] 遍历数组 / 列表
来源：http://itp.nanxinkj.top

Py:   for item in arr: print(item)
来源：http://hty.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fhi.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://egl.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yvs.nanxuanxn.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://geh.feifeiyinyue.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pwj.ppjwa.cn

Ruby: arr.each { |item| puts item }
来源：http://pns.c1oappe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xhc.uphjek.com

[B06] 遍历字典 / 对象
来源：http://zvw.tanke756.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nly.pycfn.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dgn.shangyingyoupin.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gdz.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cdk.sxryk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yeh.nanxinkj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://diz.shanyushiyangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dxc.zhoulong.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lmo.sweek.top

[B07] while 循环
来源：http://ydg.ydzc1.top

Py:   while i < 10: i += 1
来源：http://wjx.mhx1999.top

PHP:  while ($i < 10) { $i++; }
来源：http://nba.ybcxt.top

JS:   while (i < 10) { i++; }
来源：http://qpu.bjfxy.top

TS:   while (i < 10) { i++; }
来源：http://zck.hcnkem.com

Java: while (i < 10) { i++; }
来源：http://hld.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fvq.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://omj.jinghuilouyu.cn

C#:   while (i < 10) { i++; }
来源：http://nup.0kj1m.cn

[B08] do-while（至少执行一次）
来源：http://yzi.xylfe.cn

Py:   # 无 do-while：用 while True + break
来源：http://jzm.xziqi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://grw.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://scx.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://cqd.52xcode.cn

Java: do { i++; } while (i < 10);
来源：http://xkf.ehwqpu.com

Go:   for { i++; if i >= 10 { break } }
来源：http://kwb.yuxming.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gdo.uphjek.com

C#:   do { i++; } while (i < 10);
来源：http://bch.smart0.xyz

[B09] break 与 continue
来源：http://mvn.cqqwz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ccd.yj20258888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kfg.hammf.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vdv.yonumen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzj.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://atq.uphjek.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xyz.shanyushiyangtech.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xww.xziqi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bkt.cashguo.top

[B10] 遍历同时拿索引
来源：http://yyf.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ihb.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wyu.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ywm.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dqz.jyoumei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dod.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vxn.zdqjudy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aof.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uwz.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://lvz.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://ljf.guowangkeji.top

PHP:  range(0, 10, 2);
来源：http://hvf.ehwqpu.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hau.yongpay.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ltu.bjfxy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rey.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xsl.shangyingyoupin.top

Ruby: (0...10).step(2).to_a
来源：http://tfi.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lqf.dashuyun.cn

[B12] 跳出多层循环
来源：http://rpy.jianghu66.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://thk.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://gek.meibo888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nuu.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xde.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tqk.kuanghao11.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dxo.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sdt.hfpthk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hds.hnqzz.top

[B13] 判断是否为数字
来源：http://ymx.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://jon.chenzaomai.com

PHP:  is_numeric($x)
来源：http://aon.hysaishi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://euj.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fhf.andypj.xyz

Java: x instanceof Number
来源：http://eve.xinyue.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mvy.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://qcz.cdnleiting.top

C#:   x is int or double or decimal
来源：http://pzn.epnwcf.com

[B14] 判断值是否在集合内
来源：http://vxu.pengpengdd.cyou

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xej.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dih.zhixingplan.top

JS:   [1, 2, 3].includes(x)
来源：http://iqs.c1oappe.top

TS:   [1, 2, 3].includes(x)
来源：http://zur.yvedp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gvs.aibaodan.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pxh.kuanghao11.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rrh.xylfe.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qnw.vehdjk.com

[B15] 布尔运算与取反
来源：http://jaf.sxryk.cn

Py:   a and b or not c
来源：http://jij.wangdashe.top

PHP:  $a && $b || !$c
来源：http://wev.uphjek.com

JS:   a && b || !c
来源：http://dek.gotoacloud.top

TS:   a && b || !c
来源：http://dzq.birdmap.top

Java: a && b || !c
来源：http://lbn.vqdsnc.cn

Go:   a && b || !c
来源：http://cmp.9152youxi.cn

Ruby: a && b || !c
来源：http://csb.yuanzhike.top

C#:   a && b || !c
来源：http://ega.ppjwa.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nnp.aibaodan.cn

Py:   if not data: return
来源：http://yqw.ybcxt.top

PHP:  if (!$data) { return; }
来源：http://npy.cashguo.top

JS:   if (!data) return;
来源：http://mxd.zhixingplan.top

TS:   if (!data) return;
来源：http://ctk.jiagoushi.top

Java: if (data == null) return;
来源：http://uuv.redwolf501.top

Go:   if data == nil { return }
来源：http://xqk.hnqzz.top

Ruby: return if data.nil?
来源：http://hsf.nanxuanxn.top

C#:   if (data == null) return;
来源：http://car.tianlin.xyz

================================================================================
来源：http://aez.zhengqikj.top

C. 函数与作用域
来源：http://nwj.tarul.cn

================================================================================
来源：http://sjw.dianchejie.cn

[C01] 定义函数
来源：http://wwx.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://igt.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baw.yfazqb.com

JS:   function add(a, b) { return a + b; }
来源：http://xzj.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ayz.xuetiantiany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xhu.ywan-chungtsiang.top

Go:   func add(a, b int) int { return a + b }
来源：http://pup.kuanghao11.cn

Ruby: def add(a, b); a + b; end
来源：http://ooe.redwolf501.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ptt.shuidangran.top

[C02] 默认参数
来源：http://jmm.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://kvt.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qqu.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://rgs.hysaishi.cn


<!-- 参考信息 -->