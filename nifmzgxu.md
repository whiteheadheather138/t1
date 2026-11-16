代发 wailian999

Py:   "第一行\n第二行"
来源：http://yup.chenlongwang.top

PHP:  "第一行\n第二行"
来源：http://lni.jqgfzy.top

JS:   "第一行\n第二行"
来源：http://fia.zhixingplan.top

TS:   "第一行\n第二行"
来源：http://pou.fanxiaobao.xyz

Java: "第一行\n第二行"
来源：http://hfe.wangdashe.top

Go:   "第一行\n第二行"
来源：http://tvt.nanxuanxn.top

Ruby: "第一行\n第二行"
来源：http://rta.havefunace.top

C#:   "第一行\n第二行"
来源：http://nup.jqgufenzy.top

[A14] 注释写法
来源：http://nqa.dianchejie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ngf.iojbl.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://isr.havefunace.top

JS:   // 单行；/* 多行 */
来源：http://bkt.sxryk.cn

TS:   // 单行；/* 多行 */
来源：http://oss.xuetiantiany.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hmj.xziqi.cn

Go:   // 单行；/* 多行 */
来源：http://ube.ybcxt.top

Ruby: # 单行；=begin 多行 =end
来源：http://oof.hcnkem.com

C#:   // 单行；/* 多行 */
来源：http://gka.fanxiaobao.xyz

[A15] 空值判断与默认值
来源：http://taj.sufxvd.cn

Py:   value = data or "默认值"
来源：http://oqi.zhongyouzk.top

PHP:  $value = $data ?? "默认值";
来源：http://ybx.hnxiangtu.top

JS:   const value = data ?? "默认值";
来源：http://iou.meibo888.top

TS:   const value = data ?? "默认值";
来源：http://mhx.jlsjyb.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ipd.c1oappe.top

Go:   if data == "" { data = "默认值" }
来源：http://gvk.hnqzz.top

Ruby: value = data || "默认值"
来源：http://hpc.ivvv.top

C#:   var value = data ?? "默认值";
来源：http://glc.tian-w.cn

[A16] 真假值判断规则
来源：http://wmf.zycfv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fis.yuxming.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uhn.ydjk.org.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vaz.feifeiyinyue.top

TS:   if (!x) {}
来源：http://hxl.ydjk.org.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fet.gotoacloud.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zzq.haohaochexian.top

Ruby: unless x            # nil 与 false 为假
来源：http://cah.ivvv.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jdi.sufxvd.cn

[A17] 位运算
来源：http://hmi.yueranfly.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zdu.sjlbkw.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gjb.chenzaomai.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hnt.yfazqb.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nug.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qmx.yanxiufei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ote.hesvh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jcy.tianlin.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zbs.zhoulong.xyz

[A18] 字符与 ASCII 码互转
来源：http://cru.hnxiangtu.top

Py:   ord("A"); chr(65)
来源：http://wvq.shzxlz.cn

PHP:  ord("A"); chr(65)
来源：http://twi.jinqigfzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ygl.zycfv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lxq.vqdsnc.cn

Java: (int) 'A'; (char) 65
来源：http://pgj.daria6918.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mys.feifeiyinyue.top

Ruby: "A".ord; 65.chr
来源：http://ezh.sysykeji.top

C#:   (int)'A'; (char)65
来源：http://dyl.daxiang520.top

[A19] 交换两个变量
来源：http://dzq.xingfuxueyuan.xyz

Py:   a, b = b, a
来源：http://cst.fanxiaobao.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://wth.shzxlz.cn

JS:   [a, b] = [b, a];
来源：http://luw.chenzaomai.com

TS:   [a, b] = [b, a];
来源：http://nxo.zhiwuduotai.top

Java: int t = a; a = b; b = t;
来源：http://dfw.meibo888.top

Go:   a, b = b, a
来源：http://xja.hywenlv.cn

Ruby: a, b = b, a
来源：http://fml.yuxming.cn

C#:   (a, b) = (b, a);
来源：http://jse.jinghuilouyu.cn

[A20] 读取标准输入
来源：http://hak.gzhubu.top

Py:   name = input("请输入：")
来源：http://fsf.yuxming.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gea.guowangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lqj.pengpengdd.cyou

TS:   // Node.js：readline 模块
来源：http://ghp.yuanzhike.top

Java: new Scanner(System.in).nextLine()
来源：http://dpm.cqqwz.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tkh.gzhubu.top

Ruby: gets.chomp
来源：http://wqm.sufxvd.cn

C#:   Console.ReadLine();
来源：http://gdn.sysykeji.top

[A21] 保留指定小数位输出
来源：http://wyk.shanyushiyangtech.top

Py:   f"{3.14159:.2f}"
来源：http://wsm.hcnkem.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pkz.zhoulong.xyz

JS:   (3.14159).toFixed(2)
来源：http://shl.cashguo.top

TS:   (3.14159).toFixed(2)
来源：http://ikp.xuetiantiany.cn

Java: String.format("%.2f", 3.14159)
来源：http://idc.sysykeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ztw.hesvh.cn

Ruby: format("%.2f", 3.14159)
来源：http://jgk.shanyushiyangtech.top

C#:   3.14159.ToString("F2")
来源：http://ukr.ivvv.top

[A22] 获取字符串长度
来源：http://tyf.smart0.xyz

Py:   len(s)
来源：http://vln.fktsv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oyt.jianghu66.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vup.jinyuanbaomall.cn

TS:   s.length
来源：http://ehu.yfazqb.com

Java: s.length()
来源：http://cen.tian-w.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ruw.zycfv.cn

Ruby: s.length
来源：http://lzn.yueranfly.top

C#:   s.Length
来源：http://axt.jlsjyb.cn

[A23] 大小写转换
来源：http://gzi.yongpay.top

Py:   s.upper(); s.lower(); s.title()
来源：http://iil.hammf.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ory.svipenyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pgo.kuanghao11.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qoz.hammf.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://omq.wangshuangyany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xdr.52xcode.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rfq.ehwqpu.com

C#:   s.ToUpper(); s.ToLower()
来源：http://byz.cashguo.top

[A24] 去除首尾空白
来源：http://khl.hysaishi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vno.cqqwz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kak.andypj.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xyi.jinyuanbaomall.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jea.sjlbkw.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mje.yanxiufei.cn

Go:   strings.TrimSpace(s)
来源：http://qzq.wangshuangyany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xmo.yj20258.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ygp.ehwqpu.com

[A25] 字符串比较
来源：http://uvh.zhongyouzk.top

Py:   s1 == s2; s1 != s2
来源：http://czi.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cdj.haohaochexian.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oru.zhiwuduotai.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jkm.shanyushiyangtech.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kpo.ivvv.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cfa.guowangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://elo.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vsk.yueranfly.top

[A26] 类型转换总览
来源：http://rua.andypj.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://efn.ybcxt.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://egk.ydzc1.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://shw.yj202588.top

TS:   Number() String() Boolean() x as number
来源：http://gsv.jinghuilouyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yrk.xuanzx.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gtp.redwolf501.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://sjk.fzhhl.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ubu.fktsv.cn

================================================================================
来源：http://avi.feifeiyinyue.top

B. 流程控制
来源：http://gjf.sjlbkw.cn

================================================================================
来源：http://nma.kuanghao11.cn

[B01] 条件判断 if / else
来源：http://ffj.cucudq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vxa.yfazqb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kwj.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xis.xuetiantiany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cxp.tarul.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sfi.jiagoushi.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uvu.cqqwz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dhg.quarkkingdee.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tng.zhiwuduotai.top

[B02] 多分支 else if / elif
来源：http://jpp.meibo888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ihx.ppjwa.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rxg.ydzc1.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://glx.dashuyun.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://utz.jinqigfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gtu.hnxiangtu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rgo.snrcjt.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pts.iojbl.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oel.ivvv.top

[B03] switch / match / case
来源：http://jib.hfpthk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bda.zhijiandao.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ogz.nanxinkj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ewy.zhijiandao.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cgx.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ppc.yfazqb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vsi.jinyuanbaomall.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pir.vehdjk.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://agh.ydjk.org.cn

[B04] for 计数循环
来源：http://eii.jqgufenzy.top

Py:   for i in range(10): print(i)
来源：http://hlk.jinyuanbaomall.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://peh.gzhubu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mki.gogol.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hor.zhijiandao.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qsf.yj202588.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ano.tian-w.cn

Ruby: 10.times { |i| puts i }
来源：http://awr.tianlin.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bso.tarul.cn

[B05] 遍历数组 / 列表
来源：http://vdf.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://fpe.nwbrower.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pgg.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xsb.zhengqikj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zpe.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hlo.zhixingplan.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lro.zhengqikj.top

Ruby: arr.each { |item| puts item }
来源：http://qzm.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mxw.birdmap.top

[B06] 遍历字典 / 对象
来源：http://pop.fanxiaobao.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://rku.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bdb.hnxiangtu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nzz.cheryme.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qmc.sysykeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xft.0kj1m.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ybb.feifeiyinyue.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mzi.mhx1999.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tti.chenzaomai.com

[B07] while 循环
来源：http://wpr.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://lra.hnqzz.top

PHP:  while ($i < 10) { $i++; }
来源：http://jqh.316326.xyz

JS:   while (i < 10) { i++; }
来源：http://ktq.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://gyj.52xcode.cn

Java: while (i < 10) { i++; }
来源：http://dpm.xziqi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xag.guannengcc.top

Ruby: while i < 10; i += 1; end
来源：http://emr.bbcook.cn

C#:   while (i < 10) { i++; }
来源：http://gbr.shzxlz.cn

[B08] do-while（至少执行一次）
来源：http://rgh.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://ajj.fktsv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zmd.zdbjq.cn

JS:   do { i++; } while (i < 10);
来源：http://cri.hywenlv.cn

TS:   do { i++; } while (i < 10);
来源：http://iam.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://bie.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wvr.ppjwa.cn

Ruby: begin; i += 1; end while i < 10
来源：http://opx.zdqjudy.top

C#:   do { i++; } while (i < 10);
来源：http://bzc.hongshengwenyu.top

[B09] break 与 continue
来源：http://zoz.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cik.ybcxt.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bfs.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yiw.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vqg.pengpengdd.cyou

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://igp.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ixk.havefunace.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sna.aibaodan.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yzu.sweek.top

[B10] 遍历同时拿索引
来源：http://esw.yuxming.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://itb.yj20258.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://osi.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jlp.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oho.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rsf.daria6918.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lhn.yonumen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ktp.chenjidiqi.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://adz.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://ipa.snrcjt.cn

Py:   list(range(0, 10, 2))
来源：http://lot.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://psu.zhijiandao.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oab.cqqwz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://emx.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://won.ppjwa.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hgi.fanxiaobao.xyz

Ruby: (0...10).step(2).to_a
来源：http://dxl.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aqs.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://mlv.guowangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kwq.sufxvd.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qgq.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pwq.gaohongyu789.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cdh.hysaishi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://muf.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gtk.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://niv.bbcook.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dfl.dashuyun.cn

[B13] 判断是否为数字
来源：http://jtz.zhaomingkeji.xyz

Py:   isinstance(x, (int, float))
来源：http://tar.guannengcc.top

PHP:  is_numeric($x)
来源：http://nqi.jinyuanbaomall.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qrg.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xvo.xuanzx.com

Java: x instanceof Number
来源：http://uch.havefunace.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eri.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://ngc.pycfn.com

C#:   x is int or double or decimal
来源：http://pcf.shuidangran.top

[B14] 判断值是否在集合内
来源：http://cae.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xyv.birdmap.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tbx.sysykeji.top

JS:   [1, 2, 3].includes(x)
来源：http://ouo.zdbjq.cn

TS:   [1, 2, 3].includes(x)
来源：http://dux.yonumen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sux.quarkkingdee.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zlo.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://ain.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://flz.aibaodan.cn

[B15] 布尔运算与取反
来源：http://hjs.jqgfzy.top

Py:   a and b or not c
来源：http://tgs.ydjk.org.cn

PHP:  $a && $b || !$c
来源：http://idd.tanke756.top

JS:   a && b || !c
来源：http://yhq.fktsv.cn

TS:   a && b || !c
来源：http://tzn.tanke756.top

Java: a && b || !c
来源：http://fpz.jqgufenzy.top

Go:   a && b || !c
来源：http://uhp.jqgfzy.top

Ruby: a && b || !c
来源：http://sak.fktsv.cn

C#:   a && b || !c
来源：http://jlg.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://att.9152youxi.cn

Py:   if not data: return
来源：http://bne.yongpay.top

PHP:  if (!$data) { return; }
来源：http://cke.yongpay.top

JS:   if (!data) return;
来源：http://nxa.gogol.net.cn

TS:   if (!data) return;
来源：http://ghs.feifeiyinyue.top

Java: if (data == null) return;
来源：http://dpk.snrcjt.cn

Go:   if data == nil { return }
来源：http://pxt.fktsv.cn

Ruby: return if data.nil?
来源：http://cwa.zhijiandao.cn

C#:   if (data == null) return;
来源：http://hkk.nwbrower.top

================================================================================
来源：http://grv.guowangkeji.top

C. 函数与作用域
来源：http://iue.shanyushiyangkeji.top

================================================================================
来源：http://lth.gaohongyu789.top

[C01] 定义函数
来源：http://cug.yueranfly.top

Py:   def add(a, b): return a + b
来源：http://qqv.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jpa.gogol.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://zpw.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uiw.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xad.gzhubu.top

Go:   func add(a, b int) int { return a + b }
来源：http://nai.zhaomingkeji.xyz

Ruby: def add(a, b); a + b; end
来源：http://kbr.ydzc1.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rjk.316326.xyz

[C02] 默认参数
来源：http://ats.jinghuilouyu.cn

Py:   def greet(name="World"): return name
来源：http://ahs.cheryme.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hqt.jianghu66.top

JS:   function greet(name = "World") { return name; }
来源：http://unl.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dev.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://exq.zdqjudy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tyw.jinyuanbaomall.cn

Ruby: def greet(name = "World") = name
来源：http://yrp.jinqigufen.top

C#:   string Greet(string name = "World") => name;
来源：http://vnn.shangyingyoupin.top

[C03] 可变参数
来源：http://uqa.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://iqg.tianlin.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gyr.ppjwa.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cuy.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pig.sysykeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qlz.cashguo.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kzq.tarul.cn


<!-- 参考信息 -->