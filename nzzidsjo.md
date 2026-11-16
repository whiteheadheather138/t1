代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://twx.snrcjt.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ssc.tian-w.cn

Java: x > 0 ? "yes" : "no"
来源：http://oww.pycfn.com

Go:   // 无三元运算符，需用 if 语句
来源：http://xog.gogol.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pav.zhixingplan.top

C#:   x > 0 ? "yes" : "no"
来源：http://nhn.hesvh.cn

[A12] 字符串插值 / 格式化
来源：http://xzy.tanke756.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uhw.nanxuanxn.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://obq.sweek.top

JS:   `Hello, ${name}!`
来源：http://ofx.wangdashe.top

TS:   `Hello, ${name}!`
来源：http://ojw.chenlongwang.top

Java: "Hello, %s!".formatted(name)
来源：http://xfr.smart0.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://aog.hnxiangtu.top

Ruby: "Hello, #{name}!"
来源：http://ljf.52xcode.cn

C#:   $"Hello, {name}!"
来源：http://mdx.zycfv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cbz.hfpthk.cn

Py:   "第一行\n第二行"
来源：http://brn.ctjpmb.com

PHP:  "第一行\n第二行"
来源：http://yfv.ydzc1.top

JS:   "第一行\n第二行"
来源：http://dnb.sxryk.cn

TS:   "第一行\n第二行"
来源：http://kgg.pengpengdd.cyou

Java: "第一行\n第二行"
来源：http://cbn.yanxiufei.cn

Go:   "第一行\n第二行"
来源：http://bsv.tianlin.xyz

Ruby: "第一行\n第二行"
来源：http://lth.zhiwuduotai.top

C#:   "第一行\n第二行"
来源：http://wlk.nanxuanxn.top

[A14] 注释写法
来源：http://rrk.zhixingplan.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://euj.gzhubu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ili.bbcook.cn

JS:   // 单行；/* 多行 */
来源：http://dub.yonumen.top

TS:   // 单行；/* 多行 */
来源：http://dmr.fengsongda.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hin.jinqigfzy.top

Go:   // 单行；/* 多行 */
来源：http://uav.316326.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://wyu.zdbjq.cn

C#:   // 单行；/* 多行 */
来源：http://gui.ybcxt.top

[A15] 空值判断与默认值
来源：http://gfz.yangfankeji.com

Py:   value = data or "默认值"
来源：http://wxs.wangshuangyany.cn

PHP:  $value = $data ?? "默认值";
来源：http://sri.dianchejie.cn

JS:   const value = data ?? "默认值";
来源：http://unp.mhx1999.top

TS:   const value = data ?? "默认值";
来源：http://vua.fehbvm.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://klv.vqdsnc.cn

Go:   if data == "" { data = "默认值" }
来源：http://gwv.zycfv.cn

Ruby: value = data || "默认值"
来源：http://bfo.ydzc1.top

C#:   var value = data ?? "默认值";
来源：http://nqe.bjfxy.top

[A16] 真假值判断规则
来源：http://rzp.fengsongda.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hjw.birdmap.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tro.pycfn.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tew.ppjwa.cn

TS:   if (!x) {}
来源：http://xgl.jqgufenzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://eci.cdnleiting.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ltf.birdmap.top

Ruby: unless x            # nil 与 false 为假
来源：http://fzx.nanxinkj.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vzi.hywenlv.cn

[A17] 位运算
来源：http://wwb.yfazqb.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://frq.xingfuxueyuan.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rem.svipenyu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fee.bbcook.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://swg.zdqjudy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xwm.ywan-chungtsiang.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hnl.iojbl.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wso.wangdashe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ups.hnxiangtu.top

[A18] 字符与 ASCII 码互转
来源：http://ylf.nwbrower.top

Py:   ord("A"); chr(65)
来源：http://avc.jqgufenzy.top

PHP:  ord("A"); chr(65)
来源：http://uup.andypj.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kem.pycfn.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ccs.hfpthk.cn

Java: (int) 'A'; (char) 65
来源：http://fti.chenjidiqi.icu

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xwj.fanxiaobao.xyz

Ruby: "A".ord; 65.chr
来源：http://dyn.shanyushiyangtech.top

C#:   (int)'A'; (char)65
来源：http://fol.yj202588.top

[A19] 交换两个变量
来源：http://jxs.tianlin.xyz

Py:   a, b = b, a
来源：http://kan.yangfankeji.com

PHP:  [$a, $b] = [$b, $a];
来源：http://ndn.xuetiantiany.cn

JS:   [a, b] = [b, a];
来源：http://pgt.316326.xyz

TS:   [a, b] = [b, a];
来源：http://ojf.gzhubu.top

Java: int t = a; a = b; b = t;
来源：http://ada.wangshuangyany.cn

Go:   a, b = b, a
来源：http://whl.hfpthk.cn

Ruby: a, b = b, a
来源：http://kfc.fanxiaobao.xyz

C#:   (a, b) = (b, a);
来源：http://enu.dianchejie.cn

[A20] 读取标准输入
来源：http://miw.yj20258888.top

Py:   name = input("请输入：")
来源：http://xay.gaohongyu789.top

PHP:  $name = trim(fgets(STDIN));
来源：http://hbe.jinqigufen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xrs.vehdjk.com

TS:   // Node.js：readline 模块
来源：http://aqb.hcnkem.com

Java: new Scanner(System.in).nextLine()
来源：http://wsj.pycfn.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zsv.hesvh.cn

Ruby: gets.chomp
来源：http://uob.zhongyouzk.top

C#:   Console.ReadLine();
来源：http://nwh.jianghu66.top

[A21] 保留指定小数位输出
来源：http://wsa.hnqzz.top

Py:   f"{3.14159:.2f}"
来源：http://lbx.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vev.havefunace.top

JS:   (3.14159).toFixed(2)
来源：http://jvd.jianghu66.top

TS:   (3.14159).toFixed(2)
来源：http://ykn.vehdjk.com

Java: String.format("%.2f", 3.14159)
来源：http://krj.yj202588.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ley.zhengqikj.top

Ruby: format("%.2f", 3.14159)
来源：http://fup.andypj.xyz

C#:   3.14159.ToString("F2")
来源：http://oyq.hnqzz.top

[A22] 获取字符串长度
来源：http://sox.yuanzhike.top

Py:   len(s)
来源：http://oma.9152youxi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bic.sjlbkw.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fvq.gotoacloud.top

TS:   s.length
来源：http://fvn.zycfv.cn

Java: s.length()
来源：http://lsf.birdmap.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://keb.tianlin.xyz

Ruby: s.length
来源：http://xxj.aibaodan.cn

C#:   s.Length
来源：http://vzy.kuanghao11.cn

[A23] 大小写转换
来源：http://yfu.bjfxy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dbi.yanxiufei.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vcx.hnxiangtu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gmu.xylfe.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://exi.nwbrower.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://thp.cucudq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xun.yj20258.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vrw.jianghu66.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hph.xziqi.cn

[A24] 去除首尾空白
来源：http://vzk.aibaodan.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jcs.andypj.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fkp.fengsongda.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bcr.jqgfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yaf.smart0.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hoi.yangfankeji.com

Go:   strings.TrimSpace(s)
来源：http://lqz.vehdjk.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://med.sweek.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kjn.0kj1m.cn

[A25] 字符串比较
来源：http://kym.chenlongwang.top

Py:   s1 == s2; s1 != s2
来源：http://oft.xylfe.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dvy.yuanzhike.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tru.bjfxy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fcv.yonumen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bzc.jqgfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ebl.shzxlz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://idn.gaohongyu789.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rot.yfazqb.com

[A26] 类型转换总览
来源：http://srp.cqqwz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fsr.haohaochexian.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vpk.bjfxy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xav.tianlin.xyz

TS:   Number() String() Boolean() x as number
来源：http://xfu.yueranfly.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://duy.chenjidiqi.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vzj.jqgfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qag.wangshuangyany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gam.sjlbkw.cn

================================================================================
来源：http://cvz.svipenyu.cn

B. 流程控制
来源：http://xwl.svipenyu.cn

================================================================================
来源：http://hdd.xylfe.cn

[B01] 条件判断 if / else
来源：http://kwk.fengsongda.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wkq.52xcode.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wlc.hnxiangtu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jho.kuanghao11.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://upp.chenlongwang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ywu.shzxlz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hrp.vehdjk.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ick.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dik.yanxiufei.cn

[B02] 多分支 else if / elif
来源：http://ljs.yonumen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ytk.dashuyun.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://chg.aizwys.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gxj.uphjek.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fet.hnxiangtu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://coa.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nre.tarul.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vkl.hongshengwenyu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://udg.redwolf501.top

[B03] switch / match / case
来源：http://hin.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sbj.kuanghao11.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://emb.yuanzhike.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mns.yueranfly.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zcl.hammf.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eby.xylfe.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lwe.jyoumei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wuh.wangdashe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ngi.chenzaomai.com

[B04] for 计数循环
来源：http://nhy.316326.xyz

Py:   for i in range(10): print(i)
来源：http://pxl.fzhhl.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wnz.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ait.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eje.jlsjyb.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://prd.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jkn.jqgufenzy.top

Ruby: 10.times { |i| puts i }
来源：http://lhn.yfazqb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://biy.52xcode.cn

[B05] 遍历数组 / 列表
来源：http://ahj.fehbvm.com

Py:   for item in arr: print(item)
来源：http://kfg.hammf.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://usk.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://krw.gzhubu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rji.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lfr.hnxiangtu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://too.nanxuanxn.top

Ruby: arr.each { |item| puts item }
来源：http://pcg.shangyingyoupin.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mgf.yonumen.top

[B06] 遍历字典 / 对象
来源：http://nyf.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jjp.daria6918.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ewz.sxryk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dwx.tarul.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fbv.zhaomingkeji.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hvn.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fkd.yj20258.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zce.ywan-chungtsiang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yab.hongshengwenyu.top

[B07] while 循环
来源：http://ttx.jianghu66.top

Py:   while i < 10: i += 1
来源：http://jup.daxiang520.top

PHP:  while ($i < 10) { $i++; }
来源：http://ckw.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://wya.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://tns.tian-w.cn

Java: while (i < 10) { i++; }
来源：http://nkm.jqgufenzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ete.shangyingyoupin.top

Ruby: while i < 10; i += 1; end
来源：http://kqn.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://jmw.jqgfzy.top

[B08] do-while（至少执行一次）
来源：http://uwe.xziqi.cn

Py:   # 无 do-while：用 while True + break
来源：http://kgb.xziqi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gyc.birdmap.top

JS:   do { i++; } while (i < 10);
来源：http://amd.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://bnr.ppjwa.cn

Java: do { i++; } while (i < 10);
来源：http://bfd.ctjpmb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://noi.yj20258.top

Ruby: begin; i += 1; end while i < 10
来源：http://mro.zhijiandao.cn

C#:   do { i++; } while (i < 10);
来源：http://fdf.xziqi.cn

[B09] break 与 continue
来源：http://dmc.hfpthk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://znv.yangfankeji.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://apf.fanxiaobao.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zlo.cashguo.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wyr.vehdjk.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yen.sjlbkw.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ofg.fanxiaobao.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zzr.zdbjq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oap.chenjidiqi.icu

[B10] 遍历同时拿索引
来源：http://tuc.aizwys.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bsm.zdbjq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wxe.andypj.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hmf.316326.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rdl.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pch.zhijiandao.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://krj.cqqwz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dxp.cucudq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ypz.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://bfg.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://sqo.yj20258.top

PHP:  range(0, 10, 2);
来源：http://fng.fktsv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rgh.shzxlz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yrf.jinqigfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cwt.jlsjyb.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hck.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://gox.shanyushiyangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mtb.pengpengdd.cyou

[B12] 跳出多层循环
来源：http://wlm.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://imu.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xcu.guannengcc.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vst.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iva.tarul.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://isp.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hbm.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mzl.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fmo.zhoulong.xyz

[B13] 判断是否为数字
来源：http://ihh.jinghuilouyu.cn

Py:   isinstance(x, (int, float))
来源：http://bkf.wangdashe.top

PHP:  is_numeric($x)
来源：http://gll.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pro.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://veh.jiagoushi.top

Java: x instanceof Number
来源：http://ucq.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qzp.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://lrm.hesvh.cn

C#:   x is int or double or decimal
来源：http://rys.yj202588.top

[B14] 判断值是否在集合内
来源：http://hkr.zhoulong.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fyq.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xii.daria6918.cn

JS:   [1, 2, 3].includes(x)
来源：http://nlt.zhaomingkeji.xyz

TS:   [1, 2, 3].includes(x)
来源：http://pxw.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://mvr.havefunace.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mal.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://eae.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://igc.hammf.cn

[B15] 布尔运算与取反
来源：http://ltd.zhixingplan.top

Py:   a and b or not c
来源：http://elc.yuxming.cn

PHP:  $a && $b || !$c
来源：http://vhb.dashuyun.cn

JS:   a && b || !c
来源：http://uqy.xuetiantiany.cn

TS:   a && b || !c
来源：http://wdn.xingfuxueyuan.xyz

Java: a && b || !c
来源：http://hwh.nanxuanxn.top

Go:   a && b || !c
来源：http://jxf.jinqigfzy.top

Ruby: a && b || !c
来源：http://sba.jqgfzy.top

C#:   a && b || !c
来源：http://llm.cqqwz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kne.jianghu66.top

Py:   if not data: return
来源：http://hmp.yongpay.top

PHP:  if (!$data) { return; }
来源：http://iou.hesvh.cn

JS:   if (!data) return;
来源：http://zhc.hongshengwenyu.top

TS:   if (!data) return;
来源：http://fcu.fktsv.cn

Java: if (data == null) return;
来源：http://rrz.kuanghao11.cn

Go:   if data == nil { return }
来源：http://sde.yongpay.top

Ruby: return if data.nil?
来源：http://oag.jiagoushi.top

C#:   if (data == null) return;
来源：http://ohn.meibo888.top

================================================================================
来源：http://ddo.52xcode.cn

C. 函数与作用域
来源：http://hny.52xcode.cn

================================================================================
来源：http://kaf.yj20258.top

[C01] 定义函数
来源：http://gpy.fktsv.cn

Py:   def add(a, b): return a + b
来源：http://vtx.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://avf.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://wtk.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zot.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://djd.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://uwa.kuanghao11.cn

Ruby: def add(a, b); a + b; end
来源：http://jzj.c1oappe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://coj.zhijiandao.cn


<!-- 参考信息 -->