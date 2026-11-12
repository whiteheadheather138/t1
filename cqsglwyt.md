代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://iot.dianchejie.cn

Ruby: "Hello, #{name}!"
来源：http://pen.zycfv.cn

C#:   $"Hello, {name}!"
来源：http://uwi.vqdsnc.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rbw.xuanzx.com

Py:   "第一行\n第二行"
来源：http://xou.zdbjq.cn

PHP:  "第一行\n第二行"
来源：http://zzx.quarkkingdee.top

JS:   "第一行\n第二行"
来源：http://ujb.nanxinkj.top

TS:   "第一行\n第二行"
来源：http://ugh.snrcjt.cn

Java: "第一行\n第二行"
来源：http://uac.ybcxt.top

Go:   "第一行\n第二行"
来源：http://nfu.vqdsnc.cn

Ruby: "第一行\n第二行"
来源：http://pug.xylfe.cn

C#:   "第一行\n第二行"
来源：http://wnm.sysykeji.top

[A14] 注释写法
来源：http://rfz.chenjidiqi.icu

Py:   # 单行；三引号字符串可作多行说明
来源：http://upx.aibaodan.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nyb.nanxinkj.top

JS:   // 单行；/* 多行 */
来源：http://snw.cashguo.top

TS:   // 单行；/* 多行 */
来源：http://qql.hcnkem.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hcg.0kj1m.cn

Go:   // 单行；/* 多行 */
来源：http://weh.smart0.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://uxb.chenzaomai.com

C#:   // 单行；/* 多行 */
来源：http://wdb.zdqjudy.top

[A15] 空值判断与默认值
来源：http://xet.xuetiantiany.cn

Py:   value = data or "默认值"
来源：http://qlm.yongpay.top

PHP:  $value = $data ?? "默认值";
来源：http://oke.jinyuanbaomall.cn

JS:   const value = data ?? "默认值";
来源：http://lbt.hammf.cn

TS:   const value = data ?? "默认值";
来源：http://exg.fktsv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xud.redwolf501.top

Go:   if data == "" { data = "默认值" }
来源：http://ukk.yueranfly.top

Ruby: value = data || "默认值"
来源：http://gnk.shanyushiyangkeji.top

C#:   var value = data ?? "默认值";
来源：http://olt.xinyue.icu

[A16] 真假值判断规则
来源：http://bld.jqgufenzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fuz.nanxuanxn.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wmy.hcnkem.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ihs.sweek.top

TS:   if (!x) {}
来源：http://ual.sweek.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uvf.316326.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kok.hnqzz.top

Ruby: unless x            # nil 与 false 为假
来源：http://obz.gogol.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kza.ehwqpu.com

[A17] 位运算
来源：http://mqi.yfazqb.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kmv.shanyushiyangkeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mkb.shuidangran.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ycf.yongpay.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jay.sjlbkw.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tnr.wangshuangyany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pos.ehwqpu.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nhz.zhongyouzk.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zvl.yanxiufei.cn

[A18] 字符与 ASCII 码互转
来源：http://uri.cqqwz.cn

Py:   ord("A"); chr(65)
来源：http://zdw.fzhhl.top

PHP:  ord("A"); chr(65)
来源：http://aal.aizwys.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ejx.cashguo.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gqs.fengsongda.top

Java: (int) 'A'; (char) 65
来源：http://jwk.zycfv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wre.mhx1999.top

Ruby: "A".ord; 65.chr
来源：http://nju.ydjk.org.cn

C#:   (int)'A'; (char)65
来源：http://myo.zhongyouzk.top

[A19] 交换两个变量
来源：http://pqh.ybcxt.top

Py:   a, b = b, a
来源：http://mcy.zhaomingkeji.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://jjg.gogol.net.cn

JS:   [a, b] = [b, a];
来源：http://whe.cdnleiting.top

TS:   [a, b] = [b, a];
来源：http://phh.pycfn.com

Java: int t = a; a = b; b = t;
来源：http://raz.zycfv.cn

Go:   a, b = b, a
来源：http://gsv.dianchejie.cn

Ruby: a, b = b, a
来源：http://qua.vqdsnc.cn

C#:   (a, b) = (b, a);
来源：http://wrr.yvedp.cn

[A20] 读取标准输入
来源：http://mpe.cqqwz.cn

Py:   name = input("请输入：")
来源：http://rvd.fehbvm.com

PHP:  $name = trim(fgets(STDIN));
来源：http://ppu.bjfxy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rzx.cheryme.top

TS:   // Node.js：readline 模块
来源：http://xlz.wangdashe.top

Java: new Scanner(System.in).nextLine()
来源：http://nak.zdqjudy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gma.shzxlz.cn

Ruby: gets.chomp
来源：http://slo.jqgfzy.top

C#:   Console.ReadLine();
来源：http://rrn.havefunace.top

[A21] 保留指定小数位输出
来源：http://cxd.havefunace.top

Py:   f"{3.14159:.2f}"
来源：http://dhn.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hec.yanxiufei.cn

JS:   (3.14159).toFixed(2)
来源：http://kun.yfazqb.com

TS:   (3.14159).toFixed(2)
来源：http://yhd.xingfuxueyuan.xyz

Java: String.format("%.2f", 3.14159)
来源：http://vrr.cucudq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://edi.sxryk.cn

Ruby: format("%.2f", 3.14159)
来源：http://pcw.yuanzhike.top

C#:   3.14159.ToString("F2")
来源：http://pej.wangdashe.top

[A22] 获取字符串长度
来源：http://rgs.ppjwa.cn

Py:   len(s)
来源：http://izi.shangyingyoupin.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zcf.ppjwa.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qij.gotoacloud.top

TS:   s.length
来源：http://xeq.hongshengwenyu.top

Java: s.length()
来源：http://wuv.quarkkingdee.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jlx.ybcxt.top

Ruby: s.length
来源：http://smb.hnxiangtu.top

C#:   s.Length
来源：http://zzw.smart0.xyz

[A23] 大小写转换
来源：http://kvm.xuanzx.com

Py:   s.upper(); s.lower(); s.title()
来源：http://egh.aizwys.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pzg.sjlbkw.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://byc.sysykeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wor.nwbrower.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kgm.wangshuangyany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://doz.cheryme.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mij.pengpengdd.cyou

C#:   s.ToUpper(); s.ToLower()
来源：http://opx.jinqigfzy.top

[A24] 去除首尾空白
来源：http://gsw.smart0.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sud.yj20258888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hxl.zhiwuduotai.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gxd.xuanzx.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jhu.iojbl.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fyn.chenzaomai.com

Go:   strings.TrimSpace(s)
来源：http://tgz.tian-w.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rfe.xziqi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jxd.dashuyun.cn

[A25] 字符串比较
来源：http://bny.yfazqb.com

Py:   s1 == s2; s1 != s2
来源：http://uqi.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ged.xuanzx.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qau.zhaomingkeji.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lxq.hammf.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://neh.jinqigufen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dwd.zdbjq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cbf.hnqzz.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dwq.bbcook.cn

[A26] 类型转换总览
来源：http://tck.yonumen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ypn.sxryk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xqn.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ruv.shangyingyoupin.top

TS:   Number() String() Boolean() x as number
来源：http://hsa.aizwys.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mot.cashguo.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qor.feifeiyinyue.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gst.cucudq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bhx.xinyue.icu

================================================================================
来源：http://qvg.pengpengdd.cyou

B. 流程控制
来源：http://jeh.gzhubu.top

================================================================================
来源：http://czn.sweek.top

[B01] 条件判断 if / else
来源：http://hjg.zhiwuduotai.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hlw.chenlongwang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cja.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jma.shzxlz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zts.yongpay.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rgv.yj20258.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hut.uphjek.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qlu.hcnkem.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://usm.ivvv.top

[B02] 多分支 else if / elif
来源：http://jpm.fktsv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ezg.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://frz.shangyingyoupin.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sju.zhixingplan.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wmn.fktsv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vif.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kpu.hongshengwenyu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tpw.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kaf.tianlin.xyz

[B03] switch / match / case
来源：http://syx.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kve.zdbjq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qcw.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lad.gaohongyu789.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zeg.chenjidiqi.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jaa.sysykeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xpx.jinqigufen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hya.shzxlz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://als.jyoumei.cn

[B04] for 计数循环
来源：http://eyb.zycfv.cn

Py:   for i in range(10): print(i)
来源：http://owu.kuanghao11.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://axf.0kj1m.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://efj.cqqwz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vgg.hesvh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hks.hongshengwenyu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gnl.nwbrower.top

Ruby: 10.times { |i| puts i }
来源：http://ypk.ybcxt.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yra.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://rlv.aizwys.cn

Py:   for item in arr: print(item)
来源：http://kqk.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nxf.xuanzx.com

JS:   for (const item of arr) { console.log(item); }
来源：http://fkj.zhiwuduotai.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hoc.guannengcc.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xqi.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xzk.aizwys.cn

Ruby: arr.each { |item| puts item }
来源：http://oib.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ttg.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://vtn.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://scp.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wbl.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://slc.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xhm.9152youxi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kgq.yvedp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bdh.yuanzhike.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fkd.bjfxy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pjq.kuanghao11.cn

[B07] while 循环
来源：http://iub.fzhhl.top

Py:   while i < 10: i += 1
来源：http://hqa.nanxinkj.top

PHP:  while ($i < 10) { $i++; }
来源：http://vuc.hywenlv.cn

JS:   while (i < 10) { i++; }
来源：http://xca.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://jry.nanxinkj.top

Java: while (i < 10) { i++; }
来源：http://nas.yuxming.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nvp.fengsongda.top

Ruby: while i < 10; i += 1; end
来源：http://oas.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://dgb.tian-w.cn

[B08] do-while（至少执行一次）
来源：http://cla.fanxiaobao.xyz

Py:   # 无 do-while：用 while True + break
来源：http://okb.hesvh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hpc.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://xdc.pengpengdd.cyou

TS:   do { i++; } while (i < 10);
来源：http://wtd.cqqwz.cn

Java: do { i++; } while (i < 10);
来源：http://rgp.xylfe.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vic.meibo888.top

Ruby: begin; i += 1; end while i < 10
来源：http://pdn.gzhubu.top

C#:   do { i++; } while (i < 10);
来源：http://pwv.jianghu66.top

[B09] break 与 continue
来源：http://mfw.ywan-chungtsiang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://akp.sxryk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://exd.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aan.sxryk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dai.sysykeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://shm.hnxiangtu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lae.zhiwuduotai.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jmu.hnxiangtu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://htw.cucudq.cn

[B10] 遍历同时拿索引
来源：http://ggo.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zuo.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aes.yangfankeji.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ejt.c1oappe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ofs.nanxuanxn.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://heb.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zoi.tarul.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zdz.c1oappe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tal.nanxuanxn.top

[B11] 生成数字序列 / 区间
来源：http://wlu.dashuyun.cn

Py:   list(range(0, 10, 2))
来源：http://ebg.svipenyu.cn

PHP:  range(0, 10, 2);
来源：http://uzr.aizwys.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bpr.yj20258.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ewr.haohaochexian.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vvm.jinqigufen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xex.xuanzx.com

Ruby: (0...10).step(2).to_a
来源：http://baa.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mce.epnwcf.com

[B12] 跳出多层循环
来源：http://yfk.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://veq.fehbvm.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://zpj.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sbh.nanxuanxn.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rvh.0kj1m.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wef.fktsv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xnc.jinqigufen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ejn.bbcook.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gqx.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://lnk.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://qjg.chenlongwang.top

PHP:  is_numeric($x)
来源：http://kva.yfazqb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gds.jlsjyb.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fzi.tian-w.cn

Java: x instanceof Number
来源：http://yyq.c1oappe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yir.ivvv.top

Ruby: x.is_a?(Numeric)
来源：http://wao.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://ysr.shanyushiyangtech.top

[B14] 判断值是否在集合内
来源：http://rak.yj20258.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sly.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bte.zhixingplan.top

JS:   [1, 2, 3].includes(x)
来源：http://tqx.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://sfb.hammf.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ddb.hcnkem.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nmc.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://afx.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ots.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://zhp.ppjwa.cn

Py:   a and b or not c
来源：http://vza.smart0.xyz

PHP:  $a && $b || !$c
来源：http://pog.hesvh.cn

JS:   a && b || !c
来源：http://hza.wangshuangyany.cn

TS:   a && b || !c
来源：http://ogk.316326.xyz

Java: a && b || !c
来源：http://pjg.jinqigfzy.top

Go:   a && b || !c
来源：http://bkp.cucudq.cn

Ruby: a && b || !c
来源：http://ppn.gotoacloud.top

C#:   a && b || !c
来源：http://lin.daxiang520.top

[B16] 卫语句：不满足条件提前返回
来源：http://ejb.kuanghao11.cn

Py:   if not data: return
来源：http://pts.0kj1m.cn

PHP:  if (!$data) { return; }
来源：http://crw.ybcxt.top

JS:   if (!data) return;
来源：http://icr.tianlin.xyz

TS:   if (!data) return;
来源：http://nfy.xuetiantiany.cn

Java: if (data == null) return;
来源：http://osp.fzhhl.top

Go:   if data == nil { return }
来源：http://fny.kuanghao11.cn

Ruby: return if data.nil?
来源：http://lea.zdbjq.cn

C#:   if (data == null) return;
来源：http://sjc.dashuyun.cn

================================================================================
来源：http://qsv.gotoacloud.top

C. 函数与作用域
来源：http://rye.jinyuanbaomall.cn

================================================================================
来源：http://glf.snrcjt.cn

[C01] 定义函数
来源：http://hzn.tarul.cn

Py:   def add(a, b): return a + b
来源：http://gng.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lco.jqgufenzy.top

JS:   function add(a, b) { return a + b; }
来源：http://fqr.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://grt.redwolf501.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jni.guowangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://ups.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://iob.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mcy.gogol.net.cn

[C02] 默认参数
来源：http://flx.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://yam.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://end.ppjwa.cn

JS:   function greet(name = "World") { return name; }
来源：http://bjh.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fpx.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wla.pengpengdd.cyou

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ifk.shuidangran.top

Ruby: def greet(name = "World") = name
来源：http://sou.tanke756.top

C#:   string Greet(string name = "World") => name;
来源：http://son.tarul.cn

[C03] 可变参数
来源：http://utz.quarkkingdee.top

Py:   def total(*args): return sum(args)
来源：http://xic.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dlx.ywan-chungtsiang.top


<!-- 参考信息 -->