代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bgt.gotoacloud.top

Ruby: "Hello, #{name}!"
来源：http://ynd.ppjwa.cn

C#:   $"Hello, {name}!"
来源：http://xey.jiagoushi.top

[A13] 多行字符串（练习 \n 转义）
来源：http://exy.jiagoushi.top

Py:   "第一行\n第二行"
来源：http://fxh.xinyue.icu

PHP:  "第一行\n第二行"
来源：http://lsz.andypj.xyz

JS:   "第一行\n第二行"
来源：http://eaw.9152youxi.cn

TS:   "第一行\n第二行"
来源：http://lcw.shanyushiyangtech.top

Java: "第一行\n第二行"
来源：http://mqy.shangyingyoupin.top

Go:   "第一行\n第二行"
来源：http://zhr.nwbrower.top

Ruby: "第一行\n第二行"
来源：http://lbw.yangfankeji.com

C#:   "第一行\n第二行"
来源：http://tpi.mhx1999.top

[A14] 注释写法
来源：http://jrn.hnxiangtu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ply.cucudq.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xls.9152youxi.cn

JS:   // 单行；/* 多行 */
来源：http://ltn.epnwcf.com

TS:   // 单行；/* 多行 */
来源：http://taa.epnwcf.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aci.haohaochexian.top

Go:   // 单行；/* 多行 */
来源：http://pmg.guowangkeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://ekx.jqgufenzy.top

C#:   // 单行；/* 多行 */
来源：http://frh.ppjwa.cn

[A15] 空值判断与默认值
来源：http://zft.uphjek.com

Py:   value = data or "默认值"
来源：http://kuq.ybcxt.top

PHP:  $value = $data ?? "默认值";
来源：http://mti.fzhhl.top

JS:   const value = data ?? "默认值";
来源：http://yxq.havefunace.top

TS:   const value = data ?? "默认值";
来源：http://xzv.shangyingyoupin.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bsh.zhixingplan.top

Go:   if data == "" { data = "默认值" }
来源：http://xhk.nwbrower.top

Ruby: value = data || "默认值"
来源：http://jpw.bbcook.cn

C#:   var value = data ?? "默认值";
来源：http://pkk.andypj.xyz

[A16] 真假值判断规则
来源：http://arp.ctjpmb.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qin.yj202588.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://twe.chenlongwang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kek.ydjk.org.cn

TS:   if (!x) {}
来源：http://wiw.jinqigfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mmr.zhijiandao.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yxj.ydjk.org.cn

Ruby: unless x            # nil 与 false 为假
来源：http://afo.9152youxi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cah.zycfv.cn

[A17] 位运算
来源：http://upw.fehbvm.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ned.hysaishi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qye.jqgufenzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qmi.zhiwuduotai.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qoh.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tte.shanyushiyangkeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://psf.vehdjk.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wnx.aizwys.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zzs.xziqi.cn

[A18] 字符与 ASCII 码互转
来源：http://yha.yanxiufei.cn

Py:   ord("A"); chr(65)
来源：http://qgs.yongpay.top

PHP:  ord("A"); chr(65)
来源：http://rmf.sjlbkw.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://woq.zhiwuduotai.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hil.316326.xyz

Java: (int) 'A'; (char) 65
来源：http://lan.shanyushiyangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://eoz.guannengcc.top

Ruby: "A".ord; 65.chr
来源：http://kkf.9152youxi.cn

C#:   (int)'A'; (char)65
来源：http://txi.yongpay.top

[A19] 交换两个变量
来源：http://htr.0kj1m.cn

Py:   a, b = b, a
来源：http://qqq.dianchejie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sou.zycfv.cn

JS:   [a, b] = [b, a];
来源：http://wcw.jqgfzy.top

TS:   [a, b] = [b, a];
来源：http://wpb.yanxiufei.cn

Java: int t = a; a = b; b = t;
来源：http://xuo.sufxvd.cn

Go:   a, b = b, a
来源：http://gcw.jyoumei.cn

Ruby: a, b = b, a
来源：http://owt.aizwys.cn

C#:   (a, b) = (b, a);
来源：http://mhk.zdbjq.cn

[A20] 读取标准输入
来源：http://cwi.zhixingplan.top

Py:   name = input("请输入：")
来源：http://izu.pengpengdd.cyou

PHP:  $name = trim(fgets(STDIN));
来源：http://kox.zhixingplan.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dwu.316326.xyz

TS:   // Node.js：readline 模块
来源：http://svu.zhixingplan.top

Java: new Scanner(System.in).nextLine()
来源：http://fgo.pycfn.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cxc.aibaodan.cn

Ruby: gets.chomp
来源：http://oes.hywenlv.cn

C#:   Console.ReadLine();
来源：http://xvr.tarul.cn

[A21] 保留指定小数位输出
来源：http://dvk.meibo888.top

Py:   f"{3.14159:.2f}"
来源：http://dsn.gaohongyu789.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uoy.tianlin.xyz

JS:   (3.14159).toFixed(2)
来源：http://uql.hongshengwenyu.top

TS:   (3.14159).toFixed(2)
来源：http://oyj.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://lci.feifeiyinyue.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xjh.sysykeji.top

Ruby: format("%.2f", 3.14159)
来源：http://kaw.zdqjudy.top

C#:   3.14159.ToString("F2")
来源：http://mcv.xingfuxueyuan.xyz

[A22] 获取字符串长度
来源：http://qow.zdqjudy.top

Py:   len(s)
来源：http://dqd.yuxming.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xdm.jiagoushi.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://llg.sjlbkw.cn

TS:   s.length
来源：http://nar.zhijiandao.cn

Java: s.length()
来源：http://jpc.sweek.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zqf.tianlin.xyz

Ruby: s.length
来源：http://wgr.9152youxi.cn

C#:   s.Length
来源：http://zir.jinqigfzy.top

[A23] 大小写转换
来源：http://lig.yonumen.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pds.sxryk.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pzn.fanxiaobao.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uvd.guowangkeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gjh.zhaomingkeji.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://awj.yueranfly.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gcs.guowangkeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qxv.xylfe.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://thd.xinyue.icu

[A24] 去除首尾空白
来源：http://gke.tanke756.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eve.xuetiantiany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ivn.dianchejie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://byj.gotoacloud.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kyy.yfazqb.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ddu.shangyingyoupin.top

Go:   strings.TrimSpace(s)
来源：http://cgd.ctjpmb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://key.dashuyun.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ciq.hfpthk.cn

[A25] 字符串比较
来源：http://wwr.fktsv.cn

Py:   s1 == s2; s1 != s2
来源：http://rpb.yueranfly.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zeo.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://agl.mhx1999.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qvg.iojbl.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ssd.vehdjk.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cdx.guowangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jbb.sweek.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pie.sysykeji.top

[A26] 类型转换总览
来源：http://gwv.yanxiufei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dzl.birdmap.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xgl.wangdashe.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hpq.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://vox.yfazqb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ozs.vqdsnc.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://afx.cashguo.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ypi.feifeiyinyue.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iyl.hesvh.cn

================================================================================
来源：http://img.fengsongda.top

B. 流程控制
来源：http://jqw.xingfuxueyuan.xyz

================================================================================
来源：http://jsg.feifeiyinyue.top

[B01] 条件判断 if / else
来源：http://qtj.epnwcf.com

Py:   result = "正" if x > 0 else "非正"
来源：http://jyx.gotoacloud.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vsb.ybcxt.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lyq.redwolf501.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wmg.fehbvm.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://xcs.yvedp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xyz.aibaodan.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://okg.zhongyouzk.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pym.yvedp.cn

[B02] 多分支 else if / elif
来源：http://orb.yj202588.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://anc.smart0.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eyv.jinqigufen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rii.tianlin.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gtt.sxryk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xfw.cashguo.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dwr.jlsjyb.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xab.dianchejie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://stf.daxiang520.top

[B03] switch / match / case
来源：http://owv.52xcode.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zyi.ehwqpu.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hdo.tanke756.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qku.yvedp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pep.jianghu66.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eme.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://htf.wangshuangyany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vku.feifeiyinyue.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fgh.xuanzx.com

[B04] for 计数循环
来源：http://kvg.hcnkem.com

Py:   for i in range(10): print(i)
来源：http://abn.jinqigufen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ckh.smart0.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wcf.vqdsnc.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://imb.svipenyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uow.jinqigufen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qdy.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://nry.tianlin.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://age.vehdjk.com

[B05] 遍历数组 / 列表
来源：http://nod.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://wlv.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jsp.hongshengwenyu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nxz.yfazqb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://mss.cqqwz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pbg.birdmap.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aiv.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://zwg.gzhubu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gpx.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://tds.nanxinkj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rsr.meibo888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zxt.vqdsnc.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ljl.birdmap.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oul.wangdashe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aqe.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cmy.epnwcf.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nmd.gzhubu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://epe.jlsjyb.cn

[B07] while 循环
来源：http://azt.shzxlz.cn

Py:   while i < 10: i += 1
来源：http://xjq.zhoulong.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://tbj.zhiwuduotai.top

JS:   while (i < 10) { i++; }
来源：http://zcj.smart0.xyz

TS:   while (i < 10) { i++; }
来源：http://nzt.sufxvd.cn

Java: while (i < 10) { i++; }
来源：http://njv.hysaishi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yhe.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://fwa.yongpay.top

C#:   while (i < 10) { i++; }
来源：http://ehh.gogol.net.cn

[B08] do-while（至少执行一次）
来源：http://fal.xuetiantiany.cn

Py:   # 无 do-while：用 while True + break
来源：http://xky.fengsongda.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qja.zhijiandao.cn

JS:   do { i++; } while (i < 10);
来源：http://kim.yuanzhike.top

TS:   do { i++; } while (i < 10);
来源：http://lhy.vqdsnc.cn

Java: do { i++; } while (i < 10);
来源：http://ipz.havefunace.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ztv.shanyushiyangtech.top

Ruby: begin; i += 1; end while i < 10
来源：http://ilm.bbcook.cn

C#:   do { i++; } while (i < 10);
来源：http://qsd.nanxinkj.top

[B09] break 与 continue
来源：http://zxe.feifeiyinyue.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://evx.xingfuxueyuan.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://awg.ydzc1.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jtp.xingfuxueyuan.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qgo.vehdjk.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wfx.gaohongyu789.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ctp.fzhhl.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gtf.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://prf.xinyue.icu

[B10] 遍历同时拿索引
来源：http://vhu.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tqm.daria6918.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vmk.ydzc1.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dqj.yj20258888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://riu.ctjpmb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hrg.chenlongwang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fyc.hongshengwenyu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yyt.hcnkem.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iqm.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://ket.tian-w.cn

Py:   list(range(0, 10, 2))
来源：http://mlk.sweek.top

PHP:  range(0, 10, 2);
来源：http://vgs.ybcxt.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vfr.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aaa.yj20258.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mmv.vehdjk.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nep.gaohongyu789.top

Ruby: (0...10).step(2).to_a
来源：http://hjv.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wxs.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://yca.smart0.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://qpt.9152youxi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jmk.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kij.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sig.havefunace.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hiz.guannengcc.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xus.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gqy.hammf.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kaa.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://bmx.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://kvd.yanxiufei.cn

PHP:  is_numeric($x)
来源：http://xcb.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dfl.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rds.yueranfly.top

Java: x instanceof Number
来源：http://qez.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jxn.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://vbm.zhixingplan.top

C#:   x is int or double or decimal
来源：http://zdd.hammf.cn

[B14] 判断值是否在集合内
来源：http://uyh.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://abf.jinghuilouyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hxq.yfazqb.com

JS:   [1, 2, 3].includes(x)
来源：http://mdl.cdnleiting.top

TS:   [1, 2, 3].includes(x)
来源：http://hcj.mhx1999.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sog.ydzc1.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wrq.shzxlz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ozz.tanke756.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vtw.zhongyouzk.top

[B15] 布尔运算与取反
来源：http://dao.zhaomingkeji.xyz

Py:   a and b or not c
来源：http://qgz.shanyushiyangkeji.top

PHP:  $a && $b || !$c
来源：http://mrk.jqgufenzy.top

JS:   a && b || !c
来源：http://rfg.cashguo.top

TS:   a && b || !c
来源：http://ome.xuetiantiany.cn

Java: a && b || !c
来源：http://dwx.52xcode.cn

Go:   a && b || !c
来源：http://twh.yangfankeji.com

Ruby: a && b || !c
来源：http://vnd.jlsjyb.cn

C#:   a && b || !c
来源：http://pij.aizwys.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qeb.sxryk.cn

Py:   if not data: return
来源：http://vvk.smart0.xyz

PHP:  if (!$data) { return; }
来源：http://fks.zhoulong.xyz

JS:   if (!data) return;
来源：http://rin.hnxiangtu.top

TS:   if (!data) return;
来源：http://ddd.xuanzx.com

Java: if (data == null) return;
来源：http://uhb.havefunace.top

Go:   if data == nil { return }
来源：http://qfy.daxiang520.top

Ruby: return if data.nil?
来源：http://sua.hysaishi.cn

C#:   if (data == null) return;
来源：http://kpb.yj202588.top

================================================================================
来源：http://znh.zdbjq.cn

C. 函数与作用域
来源：http://mjx.zhijiandao.cn

================================================================================
来源：http://kmn.gaohongyu789.top

[C01] 定义函数
来源：http://ysz.chenjidiqi.icu

Py:   def add(a, b): return a + b
来源：http://hiq.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kch.hywenlv.cn

JS:   function add(a, b) { return a + b; }
来源：http://rah.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pgs.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kvf.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zox.yj20258888.top

Ruby: def add(a, b); a + b; end
来源：http://ezn.nanxuanxn.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rkk.cqqwz.cn

[C02] 默认参数
来源：http://gus.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://wgd.pycfn.com

PHP:  function greet($name = "World") { return $name; }
来源：http://nxm.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://euw.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fsc.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://imu.yuxming.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rmv.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://gvw.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://gfm.zhixingplan.top

[C03] 可变参数
来源：http://msd.pengpengdd.cyou

Py:   def total(*args): return sum(args)
来源：http://nxk.guowangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jvx.yueranfly.top


<!-- 参考信息 -->