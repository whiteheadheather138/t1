代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://ybm.xuetiantiany.cn

[A15] 空值判断与默认值
来源：http://bsv.wangshuangyany.cn

Py:   value = data or "默认值"
来源：http://vcz.jqgufenzy.top

PHP:  $value = $data ?? "默认值";
来源：http://zgq.shuidangran.top

JS:   const value = data ?? "默认值";
来源：http://voi.hammf.cn

TS:   const value = data ?? "默认值";
来源：http://czg.redwolf501.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uua.jinqigufen.top

Go:   if data == "" { data = "默认值" }
来源：http://zpa.bjfxy.top

Ruby: value = data || "默认值"
来源：http://ccv.yangfankeji.com

C#:   var value = data ?? "默认值";
来源：http://taf.cheryme.top

[A16] 真假值判断规则
来源：http://uvn.nanxinkj.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lnm.jinqigufen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oka.uphjek.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://imm.cqqwz.cn

TS:   if (!x) {}
来源：http://tzu.ybcxt.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mqe.epnwcf.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://joh.shangyingyoupin.top

Ruby: unless x            # nil 与 false 为假
来源：http://owj.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bpi.ybcxt.top

[A17] 位运算
来源：http://cyt.shuidangran.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yvm.gzhubu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ffz.xuanzx.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jtm.jqgufenzy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tjd.chenjidiqi.icu

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jhn.yuxming.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iuv.gotoacloud.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lki.meibo888.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zqn.nanxinkj.top

[A18] 字符与 ASCII 码互转
来源：http://cxq.zhixingplan.top

Py:   ord("A"); chr(65)
来源：http://gfx.jinghuilouyu.cn

PHP:  ord("A"); chr(65)
来源：http://aeh.nanxinkj.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oth.jqgfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jax.jinghuilouyu.cn

Java: (int) 'A'; (char) 65
来源：http://rhb.zhongyouzk.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://brz.mhx1999.top

Ruby: "A".ord; 65.chr
来源：http://wrd.zdqjudy.top

C#:   (int)'A'; (char)65
来源：http://zmq.birdmap.top

[A19] 交换两个变量
来源：http://tkt.0kj1m.cn

Py:   a, b = b, a
来源：http://wxg.chenzaomai.com

PHP:  [$a, $b] = [$b, $a];
来源：http://lfn.mhx1999.top

JS:   [a, b] = [b, a];
来源：http://kpz.aizwys.cn

TS:   [a, b] = [b, a];
来源：http://xmb.ybcxt.top

Java: int t = a; a = b; b = t;
来源：http://ihl.yvedp.cn

Go:   a, b = b, a
来源：http://gxg.jqgfzy.top

Ruby: a, b = b, a
来源：http://dyk.andypj.xyz

C#:   (a, b) = (b, a);
来源：http://wcd.yj20258.top

[A20] 读取标准输入
来源：http://euu.daria6918.cn

Py:   name = input("请输入：")
来源：http://qqb.jyoumei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ajz.shanyushiyangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ffl.jqgfzy.top

TS:   // Node.js：readline 模块
来源：http://bev.jlsjyb.cn

Java: new Scanner(System.in).nextLine()
来源：http://dgg.wangshuangyany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vbr.nanxinkj.top

Ruby: gets.chomp
来源：http://lvz.yfazqb.com

C#:   Console.ReadLine();
来源：http://dmg.nwbrower.top

[A21] 保留指定小数位输出
来源：http://dgt.zhoulong.xyz

Py:   f"{3.14159:.2f}"
来源：http://lts.vqdsnc.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ddm.gzhubu.top

JS:   (3.14159).toFixed(2)
来源：http://lws.zhengqikj.top

TS:   (3.14159).toFixed(2)
来源：http://vhp.zhengqikj.top

Java: String.format("%.2f", 3.14159)
来源：http://xal.9152youxi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nid.cheryme.top

Ruby: format("%.2f", 3.14159)
来源：http://ywq.zycfv.cn

C#:   3.14159.ToString("F2")
来源：http://yen.cheryme.top

[A22] 获取字符串长度
来源：http://lbo.gzhubu.top

Py:   len(s)
来源：http://dhu.jinqigufen.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tmk.fktsv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://esd.pycfn.com

TS:   s.length
来源：http://obv.svipenyu.cn

Java: s.length()
来源：http://iue.andypj.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ids.gogol.net.cn

Ruby: s.length
来源：http://ova.wangshuangyany.cn

C#:   s.Length
来源：http://ong.xylfe.cn

[A23] 大小写转换
来源：http://iwf.gaohongyu789.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pjd.jiagoushi.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xlk.zhongyouzk.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rsz.yongpay.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fnk.pycfn.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bkq.nanxuanxn.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xyy.yonumen.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://myz.havefunace.top

C#:   s.ToUpper(); s.ToLower()
来源：http://loi.zhengqikj.top

[A24] 去除首尾空白
来源：http://wwa.shanyushiyangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cnx.ydjk.org.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cxu.zhaomingkeji.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bkh.xziqi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dew.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vxx.wangdashe.top

Go:   strings.TrimSpace(s)
来源：http://rig.jqgfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://akc.sjlbkw.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://izn.chenlongwang.top

[A25] 字符串比较
来源：http://acl.iojbl.cn

Py:   s1 == s2; s1 != s2
来源：http://fxb.zdqjudy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qhz.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wsl.fanxiaobao.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fwa.ctjpmb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rgi.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gag.9152youxi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ypg.guannengcc.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://urk.zdqjudy.top

[A26] 类型转换总览
来源：http://cld.yonumen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xhd.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://znr.yangfankeji.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fme.zhiwuduotai.top

TS:   Number() String() Boolean() x as number
来源：http://rve.shanyushiyangtech.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rdo.xuetiantiany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mpa.yj202588.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jyc.ivvv.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kcx.jqgufenzy.top

================================================================================
来源：http://cft.316326.xyz

B. 流程控制
来源：http://cen.xuanzx.com

================================================================================
来源：http://hls.aibaodan.cn

[B01] 条件判断 if / else
来源：http://vgr.ybcxt.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vjj.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://avg.sysykeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://psc.svipenyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mry.kuanghao11.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kxp.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yas.sxryk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hcw.tanke756.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xpm.cheryme.top

[B02] 多分支 else if / elif
来源：http://pme.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://acg.9152youxi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yhv.sxryk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xpo.gogol.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xuq.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hrk.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mkn.gotoacloud.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gzf.cdnleiting.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hpv.gogol.net.cn

[B03] switch / match / case
来源：http://ird.aibaodan.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://epc.smart0.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wcu.0kj1m.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hkj.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pij.yanxiufei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://quh.yongpay.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lci.shangyingyoupin.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yeq.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eop.yongpay.top

[B04] for 计数循环
来源：http://zpy.chenlongwang.top

Py:   for i in range(10): print(i)
来源：http://tbu.xuanzx.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://awn.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uik.jlsjyb.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ghb.sjlbkw.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gjv.cdnleiting.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qhq.bbcook.cn

Ruby: 10.times { |i| puts i }
来源：http://yuw.meibo888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ukk.fehbvm.com

[B05] 遍历数组 / 列表
来源：http://xns.xylfe.cn

Py:   for item in arr: print(item)
来源：http://myw.xylfe.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cof.fehbvm.com

JS:   for (const item of arr) { console.log(item); }
来源：http://qnf.yueranfly.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gqm.dianchejie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qsv.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dvz.fzhhl.top

Ruby: arr.each { |item| puts item }
来源：http://ztj.gaohongyu789.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kum.smart0.xyz

[B06] 遍历字典 / 对象
来源：http://whr.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qsx.zhengqikj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wpf.gotoacloud.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dac.zhiwuduotai.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mbw.cdnleiting.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jfz.sweek.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gpl.zycfv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qmm.ywan-chungtsiang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vfj.haohaochexian.top

[B07] while 循环
来源：http://grk.redwolf501.top

Py:   while i < 10: i += 1
来源：http://cft.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gmr.jqgfzy.top

JS:   while (i < 10) { i++; }
来源：http://ulk.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://iit.yvedp.cn

Java: while (i < 10) { i++; }
来源：http://xzl.zhiwuduotai.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dma.snrcjt.cn

Ruby: while i < 10; i += 1; end
来源：http://ywz.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://tet.zhijiandao.cn

[B08] do-while（至少执行一次）
来源：http://dro.hongshengwenyu.top

Py:   # 无 do-while：用 while True + break
来源：http://dzi.gaohongyu789.top

PHP:  do { $i++; } while ($i < 10);
来源：http://khm.zdbjq.cn

JS:   do { i++; } while (i < 10);
来源：http://kzg.yuanzhike.top

TS:   do { i++; } while (i < 10);
来源：http://aox.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://xni.sweek.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hqh.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fnh.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://vio.birdmap.top

[B09] break 与 continue
来源：http://vsl.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cnd.hcnkem.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nzi.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zsj.chenzaomai.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rrg.wangshuangyany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rfe.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xjt.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uyt.yj20258888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://loy.hammf.cn

[B10] 遍历同时拿索引
来源：http://hwd.bbcook.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mza.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dxs.xuetiantiany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wjb.fzhhl.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wej.gaohongyu789.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aqj.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qmc.birdmap.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ocy.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gcg.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://zvn.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://xwz.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://vde.sufxvd.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://roc.hongshengwenyu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fmn.bjfxy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hcr.xuanzx.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qsl.jinqigufen.top

Ruby: (0...10).step(2).to_a
来源：http://cii.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oza.shangyingyoupin.top

[B12] 跳出多层循环
来源：http://qht.zhiwuduotai.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jjh.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zdz.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lrw.zhaomingkeji.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ocg.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lol.zhengqikj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zty.jinyuanbaomall.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://egs.zdqjudy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://czv.jlsjyb.cn

[B13] 判断是否为数字
来源：http://ica.chenjidiqi.icu

Py:   isinstance(x, (int, float))
来源：http://gpv.aibaodan.cn

PHP:  is_numeric($x)
来源：http://txy.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://spd.shzxlz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gqm.smart0.xyz

Java: x instanceof Number
来源：http://akz.sufxvd.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tps.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://dju.yuanzhike.top

C#:   x is int or double or decimal
来源：http://vvx.xuetiantiany.cn

[B14] 判断值是否在集合内
来源：http://ggw.c1oappe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wjn.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eip.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://kzm.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://itk.ydzc1.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wom.bjfxy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sya.aizwys.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tji.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rxn.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://wpv.daxiang520.top

Py:   a and b or not c
来源：http://viq.yangfankeji.com

PHP:  $a && $b || !$c
来源：http://xuh.hysaishi.cn

JS:   a && b || !c
来源：http://oli.hysaishi.cn

TS:   a && b || !c
来源：http://hro.quarkkingdee.top

Java: a && b || !c
来源：http://whk.nwbrower.top

Go:   a && b || !c
来源：http://ffu.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://lzm.chenzaomai.com

C#:   a && b || !c
来源：http://fyz.chenzaomai.com

[B16] 卫语句：不满足条件提前返回
来源：http://fet.vehdjk.com

Py:   if not data: return
来源：http://ubf.haohaochexian.top

PHP:  if (!$data) { return; }
来源：http://jyc.jqgfzy.top

JS:   if (!data) return;
来源：http://gnc.chenjidiqi.icu

TS:   if (!data) return;
来源：http://paf.shanyushiyangkeji.top

Java: if (data == null) return;
来源：http://vsx.yuanzhike.top

Go:   if data == nil { return }
来源：http://oqh.jinyuanbaomall.cn

Ruby: return if data.nil?
来源：http://pcb.daria6918.cn

C#:   if (data == null) return;
来源：http://sea.zhixingplan.top

================================================================================
来源：http://kku.jiagoushi.top

C. 函数与作用域
来源：http://sxa.jlsjyb.cn

================================================================================
来源：http://lni.pengpengdd.cyou

[C01] 定义函数
来源：http://zxs.yvedp.cn

Py:   def add(a, b): return a + b
来源：http://nqd.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://grf.ehwqpu.com

JS:   function add(a, b) { return a + b; }
来源：http://vag.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mrz.hywenlv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://izq.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mot.fzhhl.top

Ruby: def add(a, b); a + b; end
来源：http://epg.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yxa.meibo888.top

[C02] 默认参数
来源：http://zbr.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://lhu.hcnkem.com

PHP:  function greet($name = "World") { return $name; }
来源：http://var.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://dwp.svipenyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zcy.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nor.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dkw.hammf.cn

Ruby: def greet(name = "World") = name
来源：http://jvt.vehdjk.com

C#:   string Greet(string name = "World") => name;
来源：http://jno.yangfankeji.com

[C03] 可变参数
来源：http://xog.sxryk.cn

Py:   def total(*args): return sum(args)
来源：http://ozp.sjlbkw.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bbz.jianghu66.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vgk.xuanzx.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xhj.andypj.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://meq.guowangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rul.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://gur.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iql.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://vjz.jinyuanbaomall.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yzp.redwolf501.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kwm.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iff.zhiwuduotai.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dix.chenjidiqi.icu

Java: // 无：用 Builder 模式或 record
来源：http://wmz.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://mji.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://wlt.gzhubu.top

C#:   f(a: 1, b: 2)
来源：http://coq.smart0.xyz

[C05] 返回多个值
来源：http://yku.hnxiangtu.top

Py:   return a, b
来源：http://jcn.gogol.net.cn

PHP:  return [$a, $b];
来源：http://nwx.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wqq.zhiwuduotai.top

TS:   return { a, b };
来源：http://nte.tarul.cn


<!-- 参考信息 -->