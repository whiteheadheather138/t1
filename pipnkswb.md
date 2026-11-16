代发 wailian999

Java: "第一行\n第二行"
来源：http://ucj.shangyingyoupin.top

Go:   "第一行\n第二行"
来源：http://xgr.xuanzx.com

Ruby: "第一行\n第二行"
来源：http://mqm.yangfankeji.com

C#:   "第一行\n第二行"
来源：http://fxq.yvedp.cn

[A14] 注释写法
来源：http://jnn.gaohongyu789.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://cry.fanxiaobao.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://mei.hywenlv.cn

JS:   // 单行；/* 多行 */
来源：http://cat.fanxiaobao.xyz

TS:   // 单行；/* 多行 */
来源：http://vwe.havefunace.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jeh.yj20258888.top

Go:   // 单行；/* 多行 */
来源：http://yix.hnqzz.top

Ruby: # 单行；=begin 多行 =end
来源：http://yvr.nanxuanxn.top

C#:   // 单行；/* 多行 */
来源：http://nsp.xuanzx.com

[A15] 空值判断与默认值
来源：http://soe.nwbrower.top

Py:   value = data or "默认值"
来源：http://tke.guowangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://ifn.jiagoushi.top

JS:   const value = data ?? "默认值";
来源：http://hqt.shangyingyoupin.top

TS:   const value = data ?? "默认值";
来源：http://svm.9152youxi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vau.yvedp.cn

Go:   if data == "" { data = "默认值" }
来源：http://vqw.jlsjyb.cn

Ruby: value = data || "默认值"
来源：http://bmp.hongshengwenyu.top

C#:   var value = data ?? "默认值";
来源：http://bfs.zycfv.cn

[A16] 真假值判断规则
来源：http://yhy.bbcook.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ake.nwbrower.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qcw.uphjek.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cnt.uphjek.com

TS:   if (!x) {}
来源：http://zgf.gogol.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ruc.cheryme.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://oxl.zdqjudy.top

Ruby: unless x            # nil 与 false 为假
来源：http://yxv.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://owg.xuanzx.com

[A17] 位运算
来源：http://gao.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jje.zdbjq.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://czs.yfazqb.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mez.jianghu66.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hck.ydjk.org.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jzg.jiagoushi.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tqs.wangdashe.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yzt.tanke756.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iih.xuetiantiany.cn

[A18] 字符与 ASCII 码互转
来源：http://mcp.yfazqb.com

Py:   ord("A"); chr(65)
来源：http://lzq.zhixingplan.top

PHP:  ord("A"); chr(65)
来源：http://eac.cashguo.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://enr.sweek.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://alg.yangfankeji.com

Java: (int) 'A'; (char) 65
来源：http://ckq.bbcook.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ahf.pycfn.com

Ruby: "A".ord; 65.chr
来源：http://lnl.chenlongwang.top

C#:   (int)'A'; (char)65
来源：http://sac.shzxlz.cn

[A19] 交换两个变量
来源：http://bdy.yj20258.top

Py:   a, b = b, a
来源：http://yvg.yonumen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://sbn.c1oappe.top

JS:   [a, b] = [b, a];
来源：http://xku.jinghuilouyu.cn

TS:   [a, b] = [b, a];
来源：http://ppv.yfazqb.com

Java: int t = a; a = b; b = t;
来源：http://blo.hnxiangtu.top

Go:   a, b = b, a
来源：http://iqh.yj202588.top

Ruby: a, b = b, a
来源：http://shw.uphjek.com

C#:   (a, b) = (b, a);
来源：http://egv.gaohongyu789.top

[A20] 读取标准输入
来源：http://ltr.vqdsnc.cn

Py:   name = input("请输入：")
来源：http://syy.iojbl.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://iwl.jinqigfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://npo.ydjk.org.cn

TS:   // Node.js：readline 模块
来源：http://wph.aizwys.cn

Java: new Scanner(System.in).nextLine()
来源：http://zsj.uphjek.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vcn.fktsv.cn

Ruby: gets.chomp
来源：http://dbi.meibo888.top

C#:   Console.ReadLine();
来源：http://bkq.ivvv.top

[A21] 保留指定小数位输出
来源：http://zal.hesvh.cn

Py:   f"{3.14159:.2f}"
来源：http://nym.redwolf501.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://reo.ydjk.org.cn

JS:   (3.14159).toFixed(2)
来源：http://jgk.yuanzhike.top

TS:   (3.14159).toFixed(2)
来源：http://ooz.wangshuangyany.cn

Java: String.format("%.2f", 3.14159)
来源：http://flp.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iaf.jqgfzy.top

Ruby: format("%.2f", 3.14159)
来源：http://yky.c1oappe.top

C#:   3.14159.ToString("F2")
来源：http://mbm.gogol.net.cn

[A22] 获取字符串长度
来源：http://yac.xingfuxueyuan.xyz

Py:   len(s)
来源：http://jdw.haohaochexian.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ncz.xuetiantiany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fyi.zhoulong.xyz

TS:   s.length
来源：http://dlk.hcnkem.com

Java: s.length()
来源：http://isr.zhoulong.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xhu.zhongyouzk.top

Ruby: s.length
来源：http://gpn.tianlin.xyz

C#:   s.Length
来源：http://bzp.zdbjq.cn

[A23] 大小写转换
来源：http://xqt.9152youxi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://isx.yongpay.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ctp.xingfuxueyuan.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://trn.jlsjyb.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xlt.zhixingplan.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qbb.hnqzz.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kyw.yanxiufei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qtu.dashuyun.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zgx.nanxuanxn.top

[A24] 去除首尾空白
来源：http://exo.sysykeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://czj.quarkkingdee.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tkv.xuetiantiany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qcw.ywan-chungtsiang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mkr.gotoacloud.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lvl.yvedp.cn

Go:   strings.TrimSpace(s)
来源：http://qgm.meibo888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gxx.yongpay.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://onl.zycfv.cn

[A25] 字符串比较
来源：http://pyw.cashguo.top

Py:   s1 == s2; s1 != s2
来源：http://dqh.vehdjk.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mju.pengpengdd.cyou

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cwh.jinqigufen.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hna.mhx1999.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dzr.yueranfly.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ktg.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://xki.zhongyouzk.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ubr.zhixingplan.top

[A26] 类型转换总览
来源：http://wnu.yangfankeji.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bzo.xinyue.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qdw.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://emu.havefunace.top

TS:   Number() String() Boolean() x as number
来源：http://qea.yonumen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mrz.xingfuxueyuan.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vsa.cheryme.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://szt.jiagoushi.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://shf.ppjwa.cn

================================================================================
来源：http://fch.redwolf501.top

B. 流程控制
来源：http://dfx.tianlin.xyz

================================================================================
来源：http://elq.sweek.top

[B01] 条件判断 if / else
来源：http://abi.guowangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kjz.dashuyun.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tlt.9152youxi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uxt.zhongyouzk.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kvf.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://evc.zycfv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nte.zdqjudy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://avd.hywenlv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://soi.sxryk.cn

[B02] 多分支 else if / elif
来源：http://qvj.yueranfly.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mvh.gotoacloud.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bpg.ivvv.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nvi.fanxiaobao.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hok.aibaodan.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gnv.jiagoushi.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://umc.feifeiyinyue.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cho.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rls.yuxming.cn

[B03] switch / match / case
来源：http://eak.xinyue.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hdm.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ciw.9152youxi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eaf.dianchejie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://byg.guannengcc.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ftd.xuanzx.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fxy.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://orz.aizwys.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ucq.bbcook.cn

[B04] for 计数循环
来源：http://cdt.fengsongda.top

Py:   for i in range(10): print(i)
来源：http://sig.wangshuangyany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nkg.havefunace.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qkr.guowangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fjm.cdnleiting.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mkn.hnxiangtu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bef.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://ubz.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ion.zhoulong.xyz

[B05] 遍历数组 / 列表
来源：http://gfn.sysykeji.top

Py:   for item in arr: print(item)
来源：http://yga.shanyushiyangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vvm.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gjy.bbcook.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ukp.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rgw.0kj1m.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cpk.fktsv.cn

Ruby: arr.each { |item| puts item }
来源：http://fib.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://obo.9152youxi.cn

[B06] 遍历字典 / 对象
来源：http://wyy.hfpthk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qye.nanxuanxn.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jgj.dianchejie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jrn.zycfv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://deg.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uqh.jqgfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nvi.bbcook.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jsz.ivvv.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jsx.cdnleiting.top

[B07] while 循环
来源：http://xwa.yonumen.top

Py:   while i < 10: i += 1
来源：http://zbi.yueranfly.top

PHP:  while ($i < 10) { $i++; }
来源：http://bbx.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://ldp.hammf.cn

TS:   while (i < 10) { i++; }
来源：http://zrl.xinyue.icu

Java: while (i < 10) { i++; }
来源：http://fjk.chenjidiqi.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gnl.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://cin.chenzaomai.com

C#:   while (i < 10) { i++; }
来源：http://fna.guannengcc.top

[B08] do-while（至少执行一次）
来源：http://hfy.xuanzx.com

Py:   # 无 do-while：用 while True + break
来源：http://mls.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://utm.gzhubu.top

JS:   do { i++; } while (i < 10);
来源：http://jun.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://pcs.wangdashe.top

Java: do { i++; } while (i < 10);
来源：http://pyf.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://old.sxryk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mdm.jiagoushi.top

C#:   do { i++; } while (i < 10);
来源：http://hmp.nanxuanxn.top

[B09] break 与 continue
来源：http://qhk.iojbl.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://clj.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nat.316326.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xdu.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ulq.hesvh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://crs.chenjidiqi.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://izt.tanke756.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://efe.ydjk.org.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixb.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://ehn.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bvh.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tbz.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cap.xuetiantiany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ixv.sufxvd.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lzx.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fyx.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xez.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://smq.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://ewh.feifeiyinyue.top

Py:   list(range(0, 10, 2))
来源：http://euc.sufxvd.cn

PHP:  range(0, 10, 2);
来源：http://rzj.zhijiandao.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zct.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bzi.mhx1999.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wtz.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cro.birdmap.top

Ruby: (0...10).step(2).to_a
来源：http://uiu.jyoumei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oxz.jqgfzy.top

[B12] 跳出多层循环
来源：http://vvf.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iit.andypj.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://ubu.ivvv.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rbk.ybcxt.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dty.pycfn.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fam.shanyushiyangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iss.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aug.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yzs.tanke756.top

[B13] 判断是否为数字
来源：http://ywr.mhx1999.top

Py:   isinstance(x, (int, float))
来源：http://thy.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://iqs.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dlr.zhongyouzk.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fax.zhiwuduotai.top

Java: x instanceof Number
来源：http://tna.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://esd.jinqigufen.top

Ruby: x.is_a?(Numeric)
来源：http://ydv.sjlbkw.cn

C#:   x is int or double or decimal
来源：http://nyu.gaohongyu789.top

[B14] 判断值是否在集合内
来源：http://ese.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jka.zycfv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yrn.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://usx.fehbvm.com

TS:   [1, 2, 3].includes(x)
来源：http://ptn.chenlongwang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xqf.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oya.dashuyun.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jlm.fzhhl.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lbl.tanke756.top

[B15] 布尔运算与取反
来源：http://dfr.guannengcc.top

Py:   a and b or not c
来源：http://igf.yj20258.top

PHP:  $a && $b || !$c
来源：http://cxf.shanyushiyangtech.top

JS:   a && b || !c
来源：http://dfx.fanxiaobao.xyz

TS:   a && b || !c
来源：http://ndn.0kj1m.cn

Java: a && b || !c
来源：http://qom.yvedp.cn

Go:   a && b || !c
来源：http://ukv.nanxinkj.top

Ruby: a && b || !c
来源：http://bta.fktsv.cn

C#:   a && b || !c
来源：http://mcm.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ezc.wangdashe.top

Py:   if not data: return
来源：http://tuh.gaohongyu789.top

PHP:  if (!$data) { return; }
来源：http://lnv.redwolf501.top

JS:   if (!data) return;
来源：http://qmb.hysaishi.cn

TS:   if (!data) return;
来源：http://nbm.c1oappe.top

Java: if (data == null) return;
来源：http://wug.zycfv.cn

Go:   if data == nil { return }
来源：http://ayw.hongshengwenyu.top

Ruby: return if data.nil?
来源：http://rkp.pycfn.com

C#:   if (data == null) return;
来源：http://xqf.fktsv.cn

================================================================================
来源：http://coy.yj20258.top

C. 函数与作用域
来源：http://sto.pycfn.com

================================================================================
来源：http://epd.nwbrower.top

[C01] 定义函数
来源：http://ndh.yj20258.top

Py:   def add(a, b): return a + b
来源：http://kez.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ebw.chenlongwang.top

JS:   function add(a, b) { return a + b; }
来源：http://jpr.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zqh.sysykeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rjy.0kj1m.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yps.vehdjk.com

Ruby: def add(a, b); a + b; end
来源：http://ipg.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qcz.aizwys.cn

[C02] 默认参数
来源：http://vuz.zdqjudy.top

Py:   def greet(name="World"): return name
来源：http://hzp.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://sif.ivvv.top

JS:   function greet(name = "World") { return name; }
来源：http://lfw.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://knu.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dez.zhengqikj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iyr.snrcjt.cn

Ruby: def greet(name = "World") = name
来源：http://ppf.tian-w.cn

C#:   string Greet(string name = "World") => name;
来源：http://hkd.sxryk.cn

[C03] 可变参数
来源：http://hww.sweek.top

Py:   def total(*args): return sum(args)
来源：http://ldm.kuanghao11.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://puy.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xtf.shzxlz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oao.cheryme.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tws.ydzc1.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qqz.vehdjk.com

Ruby: def total(*nums); nums.sum; end
来源：http://ehd.xziqi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xyc.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://jmp.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zuo.daxiang520.top


<!-- 参考信息 -->