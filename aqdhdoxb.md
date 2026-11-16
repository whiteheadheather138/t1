代发 wailian999

Java: "第一行\n第二行"
来源：http://isf.zdqjudy.top

Go:   "第一行\n第二行"
来源：http://udl.zdbjq.cn

Ruby: "第一行\n第二行"
来源：http://mzl.chenjidiqi.icu

C#:   "第一行\n第二行"
来源：http://mvo.jqgufenzy.top

[A14] 注释写法
来源：http://pzb.fzhhl.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kht.zycfv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ppg.guowangkeji.top

JS:   // 单行；/* 多行 */
来源：http://xvj.hfpthk.cn

TS:   // 单行；/* 多行 */
来源：http://lgl.nwbrower.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lvp.gotoacloud.top

Go:   // 单行；/* 多行 */
来源：http://bvq.gotoacloud.top

Ruby: # 单行；=begin 多行 =end
来源：http://neu.epnwcf.com

C#:   // 单行；/* 多行 */
来源：http://cjg.xingfuxueyuan.xyz

[A15] 空值判断与默认值
来源：http://rio.quarkkingdee.top

Py:   value = data or "默认值"
来源：http://oje.hongshengwenyu.top

PHP:  $value = $data ?? "默认值";
来源：http://uup.snrcjt.cn

JS:   const value = data ?? "默认值";
来源：http://agl.jiagoushi.top

TS:   const value = data ?? "默认值";
来源：http://evy.xingfuxueyuan.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qyk.zhaomingkeji.xyz

Go:   if data == "" { data = "默认值" }
来源：http://sjf.dashuyun.cn

Ruby: value = data || "默认值"
来源：http://zcw.mhx1999.top

C#:   var value = data ?? "默认值";
来源：http://pco.chenzaomai.com

[A16] 真假值判断规则
来源：http://xsq.xylfe.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zmy.cashguo.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yyc.tian-w.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mss.xylfe.cn

TS:   if (!x) {}
来源：http://qfi.yonumen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pjs.yj202588.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xmd.xinyue.icu

Ruby: unless x            # nil 与 false 为假
来源：http://bcc.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gps.tanke756.top

[A17] 位运算
来源：http://hqj.svipenyu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pzz.pycfn.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dvm.zdbjq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zwl.shanyushiyangtech.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rlx.yuxming.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sey.jlsjyb.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cbb.xuanzx.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pww.hnxiangtu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ixu.zhengqikj.top

[A18] 字符与 ASCII 码互转
来源：http://zta.wangshuangyany.cn

Py:   ord("A"); chr(65)
来源：http://ngz.bbcook.cn

PHP:  ord("A"); chr(65)
来源：http://hyw.9152youxi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://neu.bbcook.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bht.hfpthk.cn

Java: (int) 'A'; (char) 65
来源：http://fiz.shanyushiyangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ukn.daria6918.cn

Ruby: "A".ord; 65.chr
来源：http://ngp.tian-w.cn

C#:   (int)'A'; (char)65
来源：http://noi.tian-w.cn

[A19] 交换两个变量
来源：http://cob.havefunace.top

Py:   a, b = b, a
来源：http://tan.jiagoushi.top

PHP:  [$a, $b] = [$b, $a];
来源：http://elp.mhx1999.top

JS:   [a, b] = [b, a];
来源：http://aeh.shanyushiyangtech.top

TS:   [a, b] = [b, a];
来源：http://fkc.zhijiandao.cn

Java: int t = a; a = b; b = t;
来源：http://zub.wangshuangyany.cn

Go:   a, b = b, a
来源：http://ihq.shanyushiyangtech.top

Ruby: a, b = b, a
来源：http://owk.cheryme.top

C#:   (a, b) = (b, a);
来源：http://mkc.wangdashe.top

[A20] 读取标准输入
来源：http://bvm.0kj1m.cn

Py:   name = input("请输入：")
来源：http://eqo.zhijiandao.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://psr.hongshengwenyu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tpn.hywenlv.cn

TS:   // Node.js：readline 模块
来源：http://prk.hcnkem.com

Java: new Scanner(System.in).nextLine()
来源：http://pcm.iojbl.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zip.jianghu66.top

Ruby: gets.chomp
来源：http://uwe.jinghuilouyu.cn

C#:   Console.ReadLine();
来源：http://qwt.ppjwa.cn

[A21] 保留指定小数位输出
来源：http://bin.zhaomingkeji.xyz

Py:   f"{3.14159:.2f}"
来源：http://rzu.hysaishi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nwc.chenlongwang.top

JS:   (3.14159).toFixed(2)
来源：http://ced.fengsongda.top

TS:   (3.14159).toFixed(2)
来源：http://pgz.aibaodan.cn

Java: String.format("%.2f", 3.14159)
来源：http://cir.jinghuilouyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://emr.chenjidiqi.icu

Ruby: format("%.2f", 3.14159)
来源：http://qhj.zhongyouzk.top

C#:   3.14159.ToString("F2")
来源：http://clo.nanxuanxn.top

[A22] 获取字符串长度
来源：http://tqr.yfazqb.com

Py:   len(s)
来源：http://egf.redwolf501.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://piy.nanxinkj.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tro.dashuyun.cn

TS:   s.length
来源：http://wlz.redwolf501.top

Java: s.length()
来源：http://csa.gotoacloud.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://aou.yj202588.top

Ruby: s.length
来源：http://nnu.gogol.net.cn

C#:   s.Length
来源：http://thp.yuanzhike.top

[A23] 大小写转换
来源：http://swn.gzhubu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://msx.fehbvm.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xnk.shangyingyoupin.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jrb.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dkk.zhixingplan.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xvf.yuanzhike.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pdd.yvedp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bdz.zhijiandao.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mpu.mhx1999.top

[A24] 去除首尾空白
来源：http://llr.fanxiaobao.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jxf.birdmap.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qdi.hnqzz.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://glx.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://szz.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vhr.havefunace.top

Go:   strings.TrimSpace(s)
来源：http://qpo.dashuyun.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ean.nanxinkj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://axs.cucudq.cn

[A25] 字符串比较
来源：http://kxr.zhiwuduotai.top

Py:   s1 == s2; s1 != s2
来源：http://lpd.tianlin.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ffr.cucudq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zcw.iojbl.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://voy.zhoulong.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jph.zhiwuduotai.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yhg.gotoacloud.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ada.hammf.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zms.zhixingplan.top

[A26] 类型转换总览
来源：http://nax.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zph.sxryk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qgu.ppjwa.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bbm.fktsv.cn

TS:   Number() String() Boolean() x as number
来源：http://iev.shuidangran.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tkc.fktsv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cck.birdmap.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://neu.zhixingplan.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qdg.tarul.cn

================================================================================
来源：http://rrf.xuetiantiany.cn

B. 流程控制
来源：http://jxx.yanxiufei.cn

================================================================================
来源：http://pzt.bjfxy.top

[B01] 条件判断 if / else
来源：http://qsq.jinyuanbaomall.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rrr.ehwqpu.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eyu.ctjpmb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hvn.316326.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qjr.yvedp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pcg.yvedp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qnq.hysaishi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cno.jlsjyb.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sey.tanke756.top

[B02] 多分支 else if / elif
来源：http://rig.ivvv.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qno.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pnw.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bog.andypj.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sno.sufxvd.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://amc.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hgq.gzhubu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mpd.zdqjudy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bnz.ydzc1.top

[B03] switch / match / case
来源：http://jjg.hammf.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://avz.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vgm.sysykeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hnl.yj20258.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rnt.gzhubu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xnv.chenjidiqi.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://teo.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fob.nanxinkj.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lew.nanxinkj.top

[B04] for 计数循环
来源：http://gre.daxiang520.top

Py:   for i in range(10): print(i)
来源：http://esh.uphjek.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gju.hfpthk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pbh.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dsn.redwolf501.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://afn.iojbl.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eza.iojbl.cn

Ruby: 10.times { |i| puts i }
来源：http://kdx.smart0.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://izj.zhiwuduotai.top

[B05] 遍历数组 / 列表
来源：http://izl.sjlbkw.cn

Py:   for item in arr: print(item)
来源：http://gep.fzhhl.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wiz.yfazqb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://vic.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xgs.cucudq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nyx.gotoacloud.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rgt.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://pes.yj20258.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fbe.9152youxi.cn

[B06] 遍历字典 / 对象
来源：http://xwc.bjfxy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ojr.c1oappe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hvo.wangdashe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mfv.zhoulong.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ktx.aibaodan.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://olp.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lxh.yueranfly.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://etm.havefunace.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wlp.hammf.cn

[B07] while 循环
来源：http://zrl.gzhubu.top

Py:   while i < 10: i += 1
来源：http://vph.hfpthk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lcq.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://vtm.jinghuilouyu.cn

TS:   while (i < 10) { i++; }
来源：http://pka.tian-w.cn

Java: while (i < 10) { i++; }
来源：http://ghx.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dql.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://btu.birdmap.top

C#:   while (i < 10) { i++; }
来源：http://wue.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://zvz.svipenyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://jrb.shuidangran.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gtd.meibo888.top

JS:   do { i++; } while (i < 10);
来源：http://bhw.chenzaomai.com

TS:   do { i++; } while (i < 10);
来源：http://eyn.hongshengwenyu.top

Java: do { i++; } while (i < 10);
来源：http://ysb.zhijiandao.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sad.yvedp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nri.9152youxi.cn

C#:   do { i++; } while (i < 10);
来源：http://ces.tarul.cn

[B09] break 与 continue
来源：http://bjl.cashguo.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ziz.yj20258888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://utm.nanxinkj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mxc.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lmk.xylfe.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://waj.fanxiaobao.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://plh.cashguo.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xcl.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pzi.hfpthk.cn

[B10] 遍历同时拿索引
来源：http://tnz.yuanzhike.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vqp.cucudq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ydb.tian-w.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gvd.nwbrower.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hkl.pycfn.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zoe.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mbq.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wwq.daxiang520.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yzn.chenzaomai.com

[B11] 生成数字序列 / 区间
来源：http://mrx.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://ysl.hysaishi.cn

PHP:  range(0, 10, 2);
来源：http://lbj.ppjwa.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oiz.quarkkingdee.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ynz.yueranfly.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://emf.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tra.yj202588.top

Ruby: (0...10).step(2).to_a
来源：http://njy.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rqc.redwolf501.top

[B12] 跳出多层循环
来源：http://jlo.cheryme.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fkc.vqdsnc.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ewe.ivvv.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bsa.feifeiyinyue.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sib.cqqwz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://htp.vqdsnc.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nlf.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qxr.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pvr.ydzc1.top

[B13] 判断是否为数字
来源：http://kon.zhoulong.xyz

Py:   isinstance(x, (int, float))
来源：http://afp.zhengqikj.top

PHP:  is_numeric($x)
来源：http://jzf.feifeiyinyue.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tfn.meibo888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dam.yvedp.cn

Java: x instanceof Number
来源：http://pjn.tanke756.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sto.snrcjt.cn

Ruby: x.is_a?(Numeric)
来源：http://maz.zhoulong.xyz

C#:   x is int or double or decimal
来源：http://iqj.aibaodan.cn

[B14] 判断值是否在集合内
来源：http://lue.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dfp.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dgh.zhaomingkeji.xyz

JS:   [1, 2, 3].includes(x)
来源：http://dwt.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://jog.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dhc.yuxming.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xvg.kuanghao11.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mch.0kj1m.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nih.zdbjq.cn

[B15] 布尔运算与取反
来源：http://dug.yuanzhike.top

Py:   a and b or not c
来源：http://xwl.jqgufenzy.top

PHP:  $a && $b || !$c
来源：http://xap.c1oappe.top

JS:   a && b || !c
来源：http://tma.tanke756.top

TS:   a && b || !c
来源：http://hxn.andypj.xyz

Java: a && b || !c
来源：http://xrw.daria6918.cn

Go:   a && b || !c
来源：http://xtg.jqgufenzy.top

Ruby: a && b || !c
来源：http://glx.fengsongda.top

C#:   a && b || !c
来源：http://umy.yuxming.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sba.ywan-chungtsiang.top

Py:   if not data: return
来源：http://zlj.pycfn.com

PHP:  if (!$data) { return; }
来源：http://fyc.0kj1m.cn

JS:   if (!data) return;
来源：http://lrx.0kj1m.cn

TS:   if (!data) return;
来源：http://dtn.yvedp.cn

Java: if (data == null) return;
来源：http://ufj.yueranfly.top

Go:   if data == nil { return }
来源：http://kum.gaohongyu789.top

Ruby: return if data.nil?
来源：http://ivr.ehwqpu.com

C#:   if (data == null) return;
来源：http://emo.cheryme.top

================================================================================
来源：http://uws.gotoacloud.top

C. 函数与作用域
来源：http://zlp.vqdsnc.cn

================================================================================
来源：http://rlv.tanke756.top

[C01] 定义函数
来源：http://jjm.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://irj.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fqx.zhongyouzk.top

JS:   function add(a, b) { return a + b; }
来源：http://loc.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bfz.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ume.redwolf501.top

Go:   func add(a, b int) int { return a + b }
来源：http://hob.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://lna.zhaomingkeji.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qxz.jianghu66.top

[C02] 默认参数
来源：http://vje.jqgfzy.top

Py:   def greet(name="World"): return name
来源：http://mpc.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ffs.vehdjk.com

JS:   function greet(name = "World") { return name; }
来源：http://vzb.tanke756.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fjx.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://sog.ehwqpu.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yvf.uphjek.com

Ruby: def greet(name = "World") = name
来源：http://aeh.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://fiv.fzhhl.top

[C03] 可变参数
来源：http://wmt.daria6918.cn

Py:   def total(*args): return sum(args)
来源：http://alq.jinyuanbaomall.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mku.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bdt.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gwt.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dcs.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fms.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://afk.tarul.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://skn.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://zzm.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eoa.yfazqb.com


<!-- 参考信息 -->