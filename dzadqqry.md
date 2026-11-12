代发 wailian999

Java: "第一行\n第二行"
来源：http://jpc.tarul.cn

Go:   "第一行\n第二行"
来源：http://wnx.zhixingplan.top

Ruby: "第一行\n第二行"
来源：http://zil.bjfxy.top

C#:   "第一行\n第二行"
来源：http://lhh.pycfn.com

[A14] 注释写法
来源：http://ekj.feifeiyinyue.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://dhn.redwolf501.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://kwt.ywan-chungtsiang.top

JS:   // 单行；/* 多行 */
来源：http://hax.yj20258.top

TS:   // 单行；/* 多行 */
来源：http://vpb.ydzc1.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qfh.kuanghao11.cn

Go:   // 单行；/* 多行 */
来源：http://mbp.yuxming.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qbv.vehdjk.com

C#:   // 单行；/* 多行 */
来源：http://xip.cucudq.cn

[A15] 空值判断与默认值
来源：http://ffj.xylfe.cn

Py:   value = data or "默认值"
来源：http://tap.shanyushiyangtech.top

PHP:  $value = $data ?? "默认值";
来源：http://kqj.yuxming.cn

JS:   const value = data ?? "默认值";
来源：http://rsv.xuetiantiany.cn

TS:   const value = data ?? "默认值";
来源：http://ldn.zhongyouzk.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ocl.sweek.top

Go:   if data == "" { data = "默认值" }
来源：http://ura.nanxuanxn.top

Ruby: value = data || "默认值"
来源：http://fwp.jinyuanbaomall.cn

C#:   var value = data ?? "默认值";
来源：http://dkd.yongpay.top

[A16] 真假值判断规则
来源：http://syn.shanyushiyangtech.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mor.gaohongyu789.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dyf.chenjidiqi.icu

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ebg.sufxvd.cn

TS:   if (!x) {}
来源：http://aap.yongpay.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://joh.xuetiantiany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mct.fehbvm.com

Ruby: unless x            # nil 与 false 为假
来源：http://ldf.ydzc1.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rot.ivvv.top

[A17] 位运算
来源：http://jlk.pycfn.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bxp.hesvh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ala.feifeiyinyue.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://knw.hysaishi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kba.gaohongyu789.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sgr.xuetiantiany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ynw.yfazqb.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mpl.zhijiandao.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dkc.zhixingplan.top

[A18] 字符与 ASCII 码互转
来源：http://aoi.zhiwuduotai.top

Py:   ord("A"); chr(65)
来源：http://rvi.wangshuangyany.cn

PHP:  ord("A"); chr(65)
来源：http://gft.smart0.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://apg.gaohongyu789.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vfg.tanke756.top

Java: (int) 'A'; (char) 65
来源：http://jec.jinqigufen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yry.0kj1m.cn

Ruby: "A".ord; 65.chr
来源：http://uwr.jinyuanbaomall.cn

C#:   (int)'A'; (char)65
来源：http://qig.gaohongyu789.top

[A19] 交换两个变量
来源：http://hpf.ybcxt.top

Py:   a, b = b, a
来源：http://fjw.zhijiandao.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jkt.cashguo.top

JS:   [a, b] = [b, a];
来源：http://uvx.jqgufenzy.top

TS:   [a, b] = [b, a];
来源：http://ydf.cucudq.cn

Java: int t = a; a = b; b = t;
来源：http://asc.shzxlz.cn

Go:   a, b = b, a
来源：http://khs.yj20258.top

Ruby: a, b = b, a
来源：http://sgi.nanxuanxn.top

C#:   (a, b) = (b, a);
来源：http://jqr.shanyushiyangtech.top

[A20] 读取标准输入
来源：http://ztg.jyoumei.cn

Py:   name = input("请输入：")
来源：http://onq.zdbjq.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vkj.0kj1m.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://smt.chenjidiqi.icu

TS:   // Node.js：readline 模块
来源：http://kfp.bjfxy.top

Java: new Scanner(System.in).nextLine()
来源：http://ehu.yuanzhike.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qfm.zhoulong.xyz

Ruby: gets.chomp
来源：http://ypm.sufxvd.cn

C#:   Console.ReadLine();
来源：http://aox.ctjpmb.com

[A21] 保留指定小数位输出
来源：http://zev.zhiwuduotai.top

Py:   f"{3.14159:.2f}"
来源：http://lhb.pycfn.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uwj.xuetiantiany.cn

JS:   (3.14159).toFixed(2)
来源：http://uxq.yuanzhike.top

TS:   (3.14159).toFixed(2)
来源：http://fxi.shanyushiyangkeji.top

Java: String.format("%.2f", 3.14159)
来源：http://yos.birdmap.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gqm.yueranfly.top

Ruby: format("%.2f", 3.14159)
来源：http://qmb.guannengcc.top

C#:   3.14159.ToString("F2")
来源：http://uvw.shangyingyoupin.top

[A22] 获取字符串长度
来源：http://fdy.yvedp.cn

Py:   len(s)
来源：http://kdu.sufxvd.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eig.daria6918.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dhr.zhengqikj.top

TS:   s.length
来源：http://foe.dashuyun.cn

Java: s.length()
来源：http://phm.cucudq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tty.meibo888.top

Ruby: s.length
来源：http://nef.sweek.top

C#:   s.Length
来源：http://gje.shuidangran.top

[A23] 大小写转换
来源：http://jzv.jlsjyb.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yzq.shanyushiyangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nac.hammf.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ylb.feifeiyinyue.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zcf.jqgufenzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kzf.yj20258888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://exv.quarkkingdee.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://msh.quarkkingdee.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hmc.fehbvm.com

[A24] 去除首尾空白
来源：http://ocf.hysaishi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iju.jinqigufen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qgm.zdqjudy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ogl.yfazqb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qnq.shanyushiyangtech.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nsi.fzhhl.top

Go:   strings.TrimSpace(s)
来源：http://wpl.fanxiaobao.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qoy.ivvv.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yuv.epnwcf.com

[A25] 字符串比较
来源：http://bow.zhongyouzk.top

Py:   s1 == s2; s1 != s2
来源：http://dgs.fzhhl.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qsu.sweek.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fyf.nanxinkj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lqi.yonumen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wmb.cdnleiting.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kjy.jiagoushi.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qby.cdnleiting.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lzq.kuanghao11.cn

[A26] 类型转换总览
来源：http://pst.fengsongda.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nlj.xinyue.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ysj.wangshuangyany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xde.jianghu66.top

TS:   Number() String() Boolean() x as number
来源：http://ngo.yfazqb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wpa.bjfxy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rzq.c1oappe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xjt.wangshuangyany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zeq.gotoacloud.top

================================================================================
来源：http://mdf.wangdashe.top

B. 流程控制
来源：http://cko.yj20258.top

================================================================================
来源：http://fjf.fktsv.cn

[B01] 条件判断 if / else
来源：http://pwy.shanyushiyangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://khd.hysaishi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://adm.aibaodan.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lvm.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://duj.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pts.yonumen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aes.fengsongda.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://euj.shangyingyoupin.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ffx.tian-w.cn

[B02] 多分支 else if / elif
来源：http://dqg.fanxiaobao.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mse.shzxlz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iak.xziqi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xfy.yuanzhike.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nhz.jqgufenzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cnc.hammf.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://umc.yangfankeji.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fnk.zhengqikj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mvh.jinyuanbaomall.cn

[B03] switch / match / case
来源：http://iwu.ydjk.org.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wvn.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vya.yanxiufei.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pen.yvedp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ynv.316326.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rwe.cashguo.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nvu.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tvo.tanke756.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://inx.jinqigfzy.top

[B04] for 计数循环
来源：http://upw.aizwys.cn

Py:   for i in range(10): print(i)
来源：http://owp.aibaodan.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mrn.dianchejie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lon.sufxvd.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://onu.hammf.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kgg.pengpengdd.cyou

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yly.yvedp.cn

Ruby: 10.times { |i| puts i }
来源：http://sbm.ywan-chungtsiang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ebo.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://gey.xingfuxueyuan.xyz

Py:   for item in arr: print(item)
来源：http://qel.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nrx.ybcxt.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xri.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ios.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lmb.xinyue.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kpl.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://bue.pengpengdd.cyou

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bqj.yongpay.top

[B06] 遍历字典 / 对象
来源：http://ois.vehdjk.com

Py:   for k, v in d.items(): print(k, v)
来源：http://klp.mhx1999.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hvm.jqgufenzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://joj.ywan-chungtsiang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yuf.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fjw.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://krf.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://flf.52xcode.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bnk.fktsv.cn

[B07] while 循环
来源：http://tun.fengsongda.top

Py:   while i < 10: i += 1
来源：http://lvu.sweek.top

PHP:  while ($i < 10) { $i++; }
来源：http://phe.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://loy.aizwys.cn

TS:   while (i < 10) { i++; }
来源：http://aus.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://ztq.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ivc.jinqigfzy.top

Ruby: while i < 10; i += 1; end
来源：http://bcg.bjfxy.top

C#:   while (i < 10) { i++; }
来源：http://xom.zhaomingkeji.xyz

[B08] do-while（至少执行一次）
来源：http://ehg.birdmap.top

Py:   # 无 do-while：用 while True + break
来源：http://fyi.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xhk.jinqigfzy.top

JS:   do { i++; } while (i < 10);
来源：http://vyx.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://brp.zhongyouzk.top

Java: do { i++; } while (i < 10);
来源：http://hjk.ctjpmb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://ffg.zhixingplan.top

Ruby: begin; i += 1; end while i < 10
来源：http://hsa.pycfn.com

C#:   do { i++; } while (i < 10);
来源：http://nxr.zycfv.cn

[B09] break 与 continue
来源：http://zqt.dashuyun.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ycs.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vyx.yangfankeji.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uif.zdqjudy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hhl.yvedp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qia.ydjk.org.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gfz.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://otd.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mmk.pycfn.com

[B10] 遍历同时拿索引
来源：http://iwk.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kph.iojbl.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nfm.svipenyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://whb.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fxo.shzxlz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hfo.kuanghao11.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vhl.shanyushiyangtech.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zzm.zdbjq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gus.bbcook.cn

[B11] 生成数字序列 / 区间
来源：http://xxe.tanke756.top

Py:   list(range(0, 10, 2))
来源：http://bfg.cashguo.top

PHP:  range(0, 10, 2);
来源：http://qpm.jinyuanbaomall.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tky.kuanghao11.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ecw.fehbvm.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jcx.jinqigufen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kdx.xingfuxueyuan.xyz

Ruby: (0...10).step(2).to_a
来源：http://mzn.jinghuilouyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eqd.epnwcf.com

[B12] 跳出多层循环
来源：http://kas.yfazqb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://vqi.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://ben.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blt.fktsv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fhg.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lwi.xylfe.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zpv.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yof.haohaochexian.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://phn.xinyue.icu

[B13] 判断是否为数字
来源：http://hhm.yuanzhike.top

Py:   isinstance(x, (int, float))
来源：http://hrs.zycfv.cn

PHP:  is_numeric($x)
来源：http://msm.yj202588.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://phc.yj20258888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tob.chenzaomai.com

Java: x instanceof Number
来源：http://lqs.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cnm.tarul.cn

Ruby: x.is_a?(Numeric)
来源：http://ffr.jiagoushi.top

C#:   x is int or double or decimal
来源：http://hma.meibo888.top

[B14] 判断值是否在集合内
来源：http://bbu.daxiang520.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://les.c1oappe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mni.feifeiyinyue.top

JS:   [1, 2, 3].includes(x)
来源：http://sva.xinyue.icu

TS:   [1, 2, 3].includes(x)
来源：http://izw.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://szk.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yom.yvedp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pcw.hesvh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lls.jinqigfzy.top

[B15] 布尔运算与取反
来源：http://dey.fehbvm.com

Py:   a and b or not c
来源：http://hov.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://njz.iojbl.cn

JS:   a && b || !c
来源：http://xjc.guowangkeji.top

TS:   a && b || !c
来源：http://djc.nanxinkj.top

Java: a && b || !c
来源：http://yjg.tianlin.xyz

Go:   a && b || !c
来源：http://fvw.pycfn.com

Ruby: a && b || !c
来源：http://zfw.nwbrower.top

C#:   a && b || !c
来源：http://hrk.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://zpl.yongpay.top

Py:   if not data: return
来源：http://vbq.cheryme.top

PHP:  if (!$data) { return; }
来源：http://crb.feifeiyinyue.top

JS:   if (!data) return;
来源：http://oxc.hongshengwenyu.top

TS:   if (!data) return;
来源：http://gyn.nanxinkj.top

Java: if (data == null) return;
来源：http://ryq.andypj.xyz

Go:   if data == nil { return }
来源：http://lil.hfpthk.cn

Ruby: return if data.nil?
来源：http://lsx.gaohongyu789.top

C#:   if (data == null) return;
来源：http://kxw.redwolf501.top

================================================================================
来源：http://rtn.mhx1999.top

C. 函数与作用域
来源：http://qna.nanxinkj.top

================================================================================
来源：http://xfa.chenlongwang.top

[C01] 定义函数
来源：http://sxd.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://tid.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cev.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://vbf.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://udq.zdqjudy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xga.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zyn.zdbjq.cn

Ruby: def add(a, b); a + b; end
来源：http://ujz.haohaochexian.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zae.jianghu66.top

[C02] 默认参数
来源：http://qgj.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://upg.9152youxi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xtw.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://xvi.tanke756.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jip.ppjwa.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lgr.fengsongda.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hss.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://zno.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://qpa.hammf.cn

[C03] 可变参数
来源：http://jgy.shangyingyoupin.top

Py:   def total(*args): return sum(args)
来源：http://vtb.ctjpmb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://unv.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hvv.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yeg.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ukw.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iro.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://jod.hnqzz.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oah.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://bjk.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://btu.ydzc1.top


<!-- 参考信息 -->