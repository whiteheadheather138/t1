代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://rdj.shzxlz.cn

C#:   x > 0 ? "yes" : "no"
来源：http://amt.chenlongwang.top

[A12] 字符串插值 / 格式化
来源：http://uhf.jqgfzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zzw.316326.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mze.ywan-chungtsiang.top

JS:   `Hello, ${name}!`
来源：http://afy.yangfankeji.com

TS:   `Hello, ${name}!`
来源：http://xfy.zhijiandao.cn

Java: "Hello, %s!".formatted(name)
来源：http://xae.sjlbkw.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dqv.hnxiangtu.top

Ruby: "Hello, #{name}!"
来源：http://yiw.zycfv.cn

C#:   $"Hello, {name}!"
来源：http://lrd.hnqzz.top

[A13] 多行字符串（练习 \n 转义）
来源：http://xnl.sjlbkw.cn

Py:   "第一行\n第二行"
来源：http://ixm.yanxiufei.cn

PHP:  "第一行\n第二行"
来源：http://hof.vehdjk.com

JS:   "第一行\n第二行"
来源：http://umb.yfazqb.com

TS:   "第一行\n第二行"
来源：http://ann.yonumen.top

Java: "第一行\n第二行"
来源：http://dxe.hysaishi.cn

Go:   "第一行\n第二行"
来源：http://tuc.yangfankeji.com

Ruby: "第一行\n第二行"
来源：http://dhe.zhengqikj.top

C#:   "第一行\n第二行"
来源：http://xks.hnxiangtu.top

[A14] 注释写法
来源：http://nvn.zdqjudy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wgp.shuidangran.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://iun.andypj.xyz

JS:   // 单行；/* 多行 */
来源：http://rbi.chenjidiqi.icu

TS:   // 单行；/* 多行 */
来源：http://fxr.zhijiandao.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bon.snrcjt.cn

Go:   // 单行；/* 多行 */
来源：http://yzz.zhongyouzk.top

Ruby: # 单行；=begin 多行 =end
来源：http://shh.gaohongyu789.top

C#:   // 单行；/* 多行 */
来源：http://tqw.tianlin.xyz

[A15] 空值判断与默认值
来源：http://nyw.jinyuanbaomall.cn

Py:   value = data or "默认值"
来源：http://kbx.yongpay.top

PHP:  $value = $data ?? "默认值";
来源：http://rgs.wangshuangyany.cn

JS:   const value = data ?? "默认值";
来源：http://jva.fktsv.cn

TS:   const value = data ?? "默认值";
来源：http://lji.jlsjyb.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://con.xingfuxueyuan.xyz

Go:   if data == "" { data = "默认值" }
来源：http://hgh.gotoacloud.top

Ruby: value = data || "默认值"
来源：http://mmz.nwbrower.top

C#:   var value = data ?? "默认值";
来源：http://qtu.sweek.top

[A16] 真假值判断规则
来源：http://sgy.svipenyu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tzb.tanke756.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dzp.nanxinkj.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://abf.jlsjyb.cn

TS:   if (!x) {}
来源：http://xzh.ydjk.org.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mnv.9152youxi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://niq.dashuyun.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xfc.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uds.xuanzx.com

[A17] 位运算
来源：http://tnk.xingfuxueyuan.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://klt.jinghuilouyu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fib.hywenlv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xnl.xylfe.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dqh.xuanzx.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rmz.shuidangran.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://eut.dashuyun.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dgg.c1oappe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cmc.yueranfly.top

[A18] 字符与 ASCII 码互转
来源：http://ija.shuidangran.top

Py:   ord("A"); chr(65)
来源：http://ino.9152youxi.cn

PHP:  ord("A"); chr(65)
来源：http://zpt.yj202588.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jpn.gogol.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xtl.ctjpmb.com

Java: (int) 'A'; (char) 65
来源：http://dhh.chenjidiqi.icu

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wdl.kuanghao11.cn

Ruby: "A".ord; 65.chr
来源：http://vyu.0kj1m.cn

C#:   (int)'A'; (char)65
来源：http://gvz.yangfankeji.com

[A19] 交换两个变量
来源：http://lez.yfazqb.com

Py:   a, b = b, a
来源：http://uhg.andypj.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://hug.zhixingplan.top

JS:   [a, b] = [b, a];
来源：http://awf.yuxming.cn

TS:   [a, b] = [b, a];
来源：http://vwk.aibaodan.cn

Java: int t = a; a = b; b = t;
来源：http://prf.fktsv.cn

Go:   a, b = b, a
来源：http://ghr.havefunace.top

Ruby: a, b = b, a
来源：http://gax.yueranfly.top

C#:   (a, b) = (b, a);
来源：http://dxk.sysykeji.top

[A20] 读取标准输入
来源：http://cac.jianghu66.top

Py:   name = input("请输入：")
来源：http://csn.gzhubu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://iqu.jqgfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ouy.zhijiandao.cn

TS:   // Node.js：readline 模块
来源：http://ugd.aibaodan.cn

Java: new Scanner(System.in).nextLine()
来源：http://sgh.jiagoushi.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ztt.9152youxi.cn

Ruby: gets.chomp
来源：http://dop.chenjidiqi.icu

C#:   Console.ReadLine();
来源：http://zam.kuanghao11.cn

[A21] 保留指定小数位输出
来源：http://rna.yj20258888.top

Py:   f"{3.14159:.2f}"
来源：http://jso.0kj1m.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://otz.quarkkingdee.top

JS:   (3.14159).toFixed(2)
来源：http://ydn.cashguo.top

TS:   (3.14159).toFixed(2)
来源：http://ebq.fehbvm.com

Java: String.format("%.2f", 3.14159)
来源：http://jmu.xylfe.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ntc.zhiwuduotai.top

Ruby: format("%.2f", 3.14159)
来源：http://nnl.yuanzhike.top

C#:   3.14159.ToString("F2")
来源：http://jei.hnxiangtu.top

[A22] 获取字符串长度
来源：http://hes.hnxiangtu.top

Py:   len(s)
来源：http://cua.c1oappe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bbe.xingfuxueyuan.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gxb.vehdjk.com

TS:   s.length
来源：http://rda.zhengqikj.top

Java: s.length()
来源：http://geo.ydzc1.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qeo.sjlbkw.cn

Ruby: s.length
来源：http://gcg.xylfe.cn

C#:   s.Length
来源：http://wps.ehwqpu.com

[A23] 大小写转换
来源：http://nku.9152youxi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qlm.jinqigfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jfg.shanyushiyangkeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eyx.jqgfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hhn.hfpthk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eym.wangdashe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gnl.smart0.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nfp.ydzc1.top

C#:   s.ToUpper(); s.ToLower()
来源：http://asu.yj20258888.top

[A24] 去除首尾空白
来源：http://fcb.pengpengdd.cyou

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ydv.nanxuanxn.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qwb.hnqzz.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bnz.zhiwuduotai.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yss.vehdjk.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lxh.jinyuanbaomall.cn

Go:   strings.TrimSpace(s)
来源：http://feu.jianghu66.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://quy.zdqjudy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lvt.zhiwuduotai.top

[A25] 字符串比较
来源：http://wqi.xziqi.cn

Py:   s1 == s2; s1 != s2
来源：http://ijl.shuidangran.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wke.xylfe.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iui.sufxvd.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ohx.pycfn.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iun.ctjpmb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://upz.c1oappe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qix.fengsongda.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zyh.sjlbkw.cn

[A26] 类型转换总览
来源：http://chr.ctjpmb.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sob.ctjpmb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://duo.pycfn.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kqs.yueranfly.top

TS:   Number() String() Boolean() x as number
来源：http://xrk.havefunace.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gym.vehdjk.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vyr.yongpay.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dwi.daria6918.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pbg.jlsjyb.cn

================================================================================
来源：http://khp.wangshuangyany.cn

B. 流程控制
来源：http://tza.shzxlz.cn

================================================================================
来源：http://drq.gogol.net.cn

[B01] 条件判断 if / else
来源：http://uku.xylfe.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://utn.jinghuilouyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hzz.redwolf501.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zps.tanke756.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qku.wangshuangyany.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://llw.c1oappe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oqi.quarkkingdee.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wsh.yanxiufei.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iza.cheryme.top

[B02] 多分支 else if / elif
来源：http://xjl.daxiang520.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bor.shzxlz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bhy.sweek.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wza.jinqigufen.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hiz.sweek.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hzq.cheryme.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fad.fzhhl.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mqf.tian-w.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qgi.nwbrower.top

[B03] switch / match / case
来源：http://tnb.shanyushiyangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vor.yj202588.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ngu.wangshuangyany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vjd.hfpthk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kxa.yj20258.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hug.0kj1m.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ame.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lkj.vehdjk.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fwz.wangdashe.top

[B04] for 计数循环
来源：http://hid.ywan-chungtsiang.top

Py:   for i in range(10): print(i)
来源：http://osz.ydjk.org.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vvo.fehbvm.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yly.zhijiandao.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qne.yuanzhike.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fmp.c1oappe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cav.cucudq.cn

Ruby: 10.times { |i| puts i }
来源：http://quf.sjlbkw.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://srg.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://mdl.daria6918.cn

Py:   for item in arr: print(item)
来源：http://rzs.vqdsnc.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://omd.hnxiangtu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cjb.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rye.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://atv.sweek.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://och.chenlongwang.top

Ruby: arr.each { |item| puts item }
来源：http://etv.aizwys.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://muc.jqgfzy.top

[B06] 遍历字典 / 对象
来源：http://vji.chenzaomai.com

Py:   for k, v in d.items(): print(k, v)
来源：http://jyy.c1oappe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zhk.shuidangran.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qwy.ydzc1.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://byx.yueranfly.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qjy.yfazqb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://the.hysaishi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://epm.yvedp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zrh.guowangkeji.top

[B07] while 循环
来源：http://zzv.jinghuilouyu.cn

Py:   while i < 10: i += 1
来源：http://tls.dianchejie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mhd.hcnkem.com

JS:   while (i < 10) { i++; }
来源：http://yeu.bbcook.cn

TS:   while (i < 10) { i++; }
来源：http://qbk.nanxinkj.top

Java: while (i < 10) { i++; }
来源：http://xkl.chenjidiqi.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cdw.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://ahv.feifeiyinyue.top

C#:   while (i < 10) { i++; }
来源：http://bzb.dianchejie.cn

[B08] do-while（至少执行一次）
来源：http://fyl.yueranfly.top

Py:   # 无 do-while：用 while True + break
来源：http://lwc.316326.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://fbp.vqdsnc.cn

JS:   do { i++; } while (i < 10);
来源：http://kxw.pycfn.com

TS:   do { i++; } while (i < 10);
来源：http://muz.gaohongyu789.top

Java: do { i++; } while (i < 10);
来源：http://tpg.sweek.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mdy.jinyuanbaomall.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dow.kuanghao11.cn

C#:   do { i++; } while (i < 10);
来源：http://zjr.ydjk.org.cn

[B09] break 与 continue
来源：http://zkj.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dkg.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vut.ivvv.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wuh.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cqx.ydjk.org.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wim.shzxlz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oyy.ppjwa.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vvr.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qlk.hywenlv.cn

[B10] 遍历同时拿索引
来源：http://jqi.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://drk.hcnkem.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tge.guowangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rwc.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mse.cucudq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ugl.redwolf501.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oqi.hysaishi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ugb.iojbl.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://amn.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://iur.zhaomingkeji.xyz

Py:   list(range(0, 10, 2))
来源：http://san.mhx1999.top

PHP:  range(0, 10, 2);
来源：http://keg.hywenlv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qgg.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wiq.jinyuanbaomall.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mih.chenjidiqi.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xsv.ydzc1.top

Ruby: (0...10).step(2).to_a
来源：http://jkr.zhiwuduotai.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gnb.hysaishi.cn

[B12] 跳出多层循环
来源：http://xqn.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fio.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://jlo.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hwg.snrcjt.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yas.pengpengdd.cyou

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fyr.havefunace.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tlf.yfazqb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ylv.jinyuanbaomall.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ccr.jlsjyb.cn

[B13] 判断是否为数字
来源：http://fcg.hesvh.cn

Py:   isinstance(x, (int, float))
来源：http://zel.9152youxi.cn

PHP:  is_numeric($x)
来源：http://mmw.yuanzhike.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dqy.snrcjt.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://smr.jlsjyb.cn

Java: x instanceof Number
来源：http://aqa.guowangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://unp.aizwys.cn

Ruby: x.is_a?(Numeric)
来源：http://wfe.andypj.xyz

C#:   x is int or double or decimal
来源：http://isn.vehdjk.com

[B14] 判断值是否在集合内
来源：http://xsn.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zeq.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mki.tarul.cn

JS:   [1, 2, 3].includes(x)
来源：http://xhq.shangyingyoupin.top

TS:   [1, 2, 3].includes(x)
来源：http://qga.bjfxy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sxq.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dtq.guannengcc.top

Ruby: [1, 2, 3].include?(x)
来源：http://ntr.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://css.jianghu66.top

[B15] 布尔运算与取反
来源：http://vwa.zycfv.cn

Py:   a and b or not c
来源：http://wxr.hcnkem.com

PHP:  $a && $b || !$c
来源：http://xcd.xuanzx.com

JS:   a && b || !c
来源：http://tpa.tarul.cn

TS:   a && b || !c
来源：http://guk.bbcook.cn

Java: a && b || !c
来源：http://pmu.shanyushiyangkeji.top

Go:   a && b || !c
来源：http://csi.redwolf501.top

Ruby: a && b || !c
来源：http://ies.gotoacloud.top

C#:   a && b || !c
来源：http://jqm.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://dit.chenlongwang.top

Py:   if not data: return
来源：http://nzx.zhengqikj.top

PHP:  if (!$data) { return; }
来源：http://bua.hcnkem.com

JS:   if (!data) return;
来源：http://rvv.mhx1999.top

TS:   if (!data) return;
来源：http://igb.fehbvm.com

Java: if (data == null) return;
来源：http://rry.svipenyu.cn

Go:   if data == nil { return }
来源：http://lcg.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://yqw.yangfankeji.com

C#:   if (data == null) return;
来源：http://irm.hammf.cn

================================================================================
来源：http://ujz.hysaishi.cn

C. 函数与作用域
来源：http://bjs.jinqigfzy.top

================================================================================
来源：http://axt.yj20258888.top

[C01] 定义函数
来源：http://dca.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://fxq.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uzx.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://rrn.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lsp.cheryme.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zgo.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lwg.sufxvd.cn

Ruby: def add(a, b); a + b; end
来源：http://hcs.xinyue.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://akp.ehwqpu.com

[C02] 默认参数
来源：http://ofh.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://tfz.ywan-chungtsiang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://set.zdqjudy.top

JS:   function greet(name = "World") { return name; }
来源：http://zkc.shzxlz.cn


<!-- 参考信息 -->