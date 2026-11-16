代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://oag.cucudq.cn

[A15] 空值判断与默认值
来源：http://zma.bbcook.cn

Py:   value = data or "默认值"
来源：http://zrf.vehdjk.com

PHP:  $value = $data ?? "默认值";
来源：http://gwj.vehdjk.com

JS:   const value = data ?? "默认值";
来源：http://dbl.yanxiufei.cn

TS:   const value = data ?? "默认值";
来源：http://wex.aizwys.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fmr.vqdsnc.cn

Go:   if data == "" { data = "默认值" }
来源：http://ndg.smart0.xyz

Ruby: value = data || "默认值"
来源：http://dwi.xuetiantiany.cn

C#:   var value = data ?? "默认值";
来源：http://fda.hesvh.cn

[A16] 真假值判断规则
来源：http://ujf.aibaodan.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wyy.yuanzhike.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ebg.smart0.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kqc.cdnleiting.top

TS:   if (!x) {}
来源：http://tob.dianchejie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nmt.pycfn.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://izs.chenjidiqi.icu

Ruby: unless x            # nil 与 false 为假
来源：http://lsz.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mox.mhx1999.top

[A17] 位运算
来源：http://zmx.ivvv.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dmj.mhx1999.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sgq.wangshuangyany.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xpf.havefunace.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yvf.pengpengdd.cyou

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xyo.tarul.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://slh.c1oappe.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lzs.aizwys.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kso.yongpay.top

[A18] 字符与 ASCII 码互转
来源：http://ikz.pycfn.com

Py:   ord("A"); chr(65)
来源：http://pgh.zdqjudy.top

PHP:  ord("A"); chr(65)
来源：http://rah.316326.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ozm.zhongyouzk.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nto.haohaochexian.top

Java: (int) 'A'; (char) 65
来源：http://qyn.sxryk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://thd.sysykeji.top

Ruby: "A".ord; 65.chr
来源：http://ivn.chenjidiqi.icu

C#:   (int)'A'; (char)65
来源：http://wog.zhoulong.xyz

[A19] 交换两个变量
来源：http://dvv.shzxlz.cn

Py:   a, b = b, a
来源：http://ozf.jinyuanbaomall.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://shk.fanxiaobao.xyz

JS:   [a, b] = [b, a];
来源：http://bdi.ybcxt.top

TS:   [a, b] = [b, a];
来源：http://syi.yonumen.top

Java: int t = a; a = b; b = t;
来源：http://qiw.wangshuangyany.cn

Go:   a, b = b, a
来源：http://rbh.jiagoushi.top

Ruby: a, b = b, a
来源：http://mul.tian-w.cn

C#:   (a, b) = (b, a);
来源：http://jlg.zdqjudy.top

[A20] 读取标准输入
来源：http://ttb.cucudq.cn

Py:   name = input("请输入：")
来源：http://nix.hongshengwenyu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://hmc.yfazqb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vnt.andypj.xyz

TS:   // Node.js：readline 模块
来源：http://pyc.xingfuxueyuan.xyz

Java: new Scanner(System.in).nextLine()
来源：http://xne.chenjidiqi.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qij.fanxiaobao.xyz

Ruby: gets.chomp
来源：http://ixl.0kj1m.cn

C#:   Console.ReadLine();
来源：http://knq.gotoacloud.top

[A21] 保留指定小数位输出
来源：http://bgt.cdnleiting.top

Py:   f"{3.14159:.2f}"
来源：http://auw.tarul.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rem.fzhhl.top

JS:   (3.14159).toFixed(2)
来源：http://xxb.9152youxi.cn

TS:   (3.14159).toFixed(2)
来源：http://vhh.smart0.xyz

Java: String.format("%.2f", 3.14159)
来源：http://gyd.yfazqb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cbn.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://tqj.daxiang520.top

C#:   3.14159.ToString("F2")
来源：http://pry.birdmap.top

[A22] 获取字符串长度
来源：http://pxl.vehdjk.com

Py:   len(s)
来源：http://xwm.aibaodan.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wwf.zhijiandao.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vie.chenlongwang.top

TS:   s.length
来源：http://hzx.zdbjq.cn

Java: s.length()
来源：http://yuj.tanke756.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uap.hywenlv.cn

Ruby: s.length
来源：http://tan.hywenlv.cn

C#:   s.Length
来源：http://xci.jyoumei.cn

[A23] 大小写转换
来源：http://juh.kuanghao11.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ngs.ydzc1.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mwe.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://too.zhiwuduotai.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://slm.redwolf501.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lzw.316326.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yis.fktsv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wak.daria6918.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://aws.c1oappe.top

[A24] 去除首尾空白
来源：http://sxm.zhijiandao.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://igu.ehwqpu.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rmm.316326.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://acn.xylfe.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rtx.fengsongda.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ikj.sufxvd.cn

Go:   strings.TrimSpace(s)
来源：http://tii.ydzc1.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fze.jinyuanbaomall.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ppk.cheryme.top

[A25] 字符串比较
来源：http://tkj.zdbjq.cn

Py:   s1 == s2; s1 != s2
来源：http://paw.9152youxi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tgc.tian-w.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jhr.vqdsnc.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dod.ywan-chungtsiang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bwr.zhixingplan.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sik.aibaodan.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://azl.zhongyouzk.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kmn.52xcode.cn

[A26] 类型转换总览
来源：http://irz.svipenyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hdb.ybcxt.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kwg.yj202588.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jki.guannengcc.top

TS:   Number() String() Boolean() x as number
来源：http://eto.gogol.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://unm.jqgfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://prm.zhixingplan.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xrr.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://klt.0kj1m.cn

================================================================================
来源：http://qht.nanxinkj.top

B. 流程控制
来源：http://lhi.shanyushiyangkeji.top

================================================================================
来源：http://dcn.quarkkingdee.top

[B01] 条件判断 if / else
来源：http://dzd.ybcxt.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mjb.jianghu66.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gxo.yj202588.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mlw.quarkkingdee.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kwp.nanxuanxn.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rxt.shanyushiyangtech.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ron.xuanzx.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fsy.feifeiyinyue.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cbl.zdqjudy.top

[B02] 多分支 else if / elif
来源：http://vwy.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://inj.zhengqikj.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sjx.vqdsnc.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://myt.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ktb.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ywo.hongshengwenyu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wca.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lhn.jianghu66.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xvs.fktsv.cn

[B03] switch / match / case
来源：http://ett.fanxiaobao.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wmz.jqgfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qxi.zhaomingkeji.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qmw.dianchejie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kgb.fehbvm.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eva.sweek.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bfy.jinqigufen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wiv.yuanzhike.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mqr.shangyingyoupin.top

[B04] for 计数循环
来源：http://kab.cashguo.top

Py:   for i in range(10): print(i)
来源：http://pfl.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ndi.ydzc1.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hwl.haohaochexian.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://skh.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bum.yfazqb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mbb.guannengcc.top

Ruby: 10.times { |i| puts i }
来源：http://tvr.ydzc1.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dzq.tianlin.xyz

[B05] 遍历数组 / 列表
来源：http://wlb.zhongyouzk.top

Py:   for item in arr: print(item)
来源：http://drx.zhijiandao.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yej.fehbvm.com

JS:   for (const item of arr) { console.log(item); }
来源：http://rjd.vqdsnc.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jgm.yongpay.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pjk.meibo888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://miw.ydjk.org.cn

Ruby: arr.each { |item| puts item }
来源：http://obf.zhijiandao.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aqc.aibaodan.cn

[B06] 遍历字典 / 对象
来源：http://ogl.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://odw.yuxming.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bcl.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ula.hcnkem.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://env.shuidangran.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wka.birdmap.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://amo.xylfe.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cxe.smart0.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ose.zhijiandao.cn

[B07] while 循环
来源：http://qff.ctjpmb.com

Py:   while i < 10: i += 1
来源：http://usb.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ksn.epnwcf.com

JS:   while (i < 10) { i++; }
来源：http://uyw.bjfxy.top

TS:   while (i < 10) { i++; }
来源：http://giu.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://mat.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ngx.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://mtk.fanxiaobao.xyz

C#:   while (i < 10) { i++; }
来源：http://drb.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://bfd.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://yro.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://fxp.xuetiantiany.cn

JS:   do { i++; } while (i < 10);
来源：http://umh.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://umt.kuanghao11.cn

Java: do { i++; } while (i < 10);
来源：http://dho.nwbrower.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yyh.svipenyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zfx.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://mnp.birdmap.top

[B09] break 与 continue
来源：http://egs.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ivo.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zue.jinyuanbaomall.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://akg.316326.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xmb.yuanzhike.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jhx.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ldt.zhiwuduotai.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://efv.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vaz.hfpthk.cn

[B10] 遍历同时拿索引
来源：http://mnl.jiagoushi.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nks.uphjek.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jfa.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://szi.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pzq.fzhhl.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mrg.sxryk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aiw.nanxuanxn.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ljo.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qzz.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://dmq.ybcxt.top

Py:   list(range(0, 10, 2))
来源：http://eis.xuanzx.com

PHP:  range(0, 10, 2);
来源：http://jwk.shanyushiyangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cmq.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sss.yanxiufei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yyf.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nun.meibo888.top

Ruby: (0...10).step(2).to_a
来源：http://vlk.316326.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tgl.ivvv.top

[B12] 跳出多层循环
来源：http://ifc.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bkm.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yps.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://riw.havefunace.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://daq.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://noh.daria6918.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xpa.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sgl.epnwcf.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hva.nwbrower.top

[B13] 判断是否为数字
来源：http://fuc.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://uue.guowangkeji.top

PHP:  is_numeric($x)
来源：http://wkl.c1oappe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pzt.jinqigfzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://don.ppjwa.cn

Java: x instanceof Number
来源：http://qbj.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kln.fzhhl.top

Ruby: x.is_a?(Numeric)
来源：http://wtj.quarkkingdee.top

C#:   x is int or double or decimal
来源：http://ivd.jqgufenzy.top

[B14] 判断值是否在集合内
来源：http://tnj.hysaishi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qra.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tvv.nanxuanxn.top

JS:   [1, 2, 3].includes(x)
来源：http://tsi.feifeiyinyue.top

TS:   [1, 2, 3].includes(x)
来源：http://lov.ydjk.org.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qmf.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kwd.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://mgd.shanyushiyangtech.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ayf.hesvh.cn

[B15] 布尔运算与取反
来源：http://hje.epnwcf.com

Py:   a and b or not c
来源：http://rzc.yvedp.cn

PHP:  $a && $b || !$c
来源：http://avh.ehwqpu.com

JS:   a && b || !c
来源：http://zxj.cdnleiting.top

TS:   a && b || !c
来源：http://okv.jinqigufen.top

Java: a && b || !c
来源：http://spu.c1oappe.top

Go:   a && b || !c
来源：http://fnn.ydzc1.top

Ruby: a && b || !c
来源：http://gdc.cashguo.top

C#:   a && b || !c
来源：http://idd.nanxinkj.top

[B16] 卫语句：不满足条件提前返回
来源：http://caw.gogol.net.cn

Py:   if not data: return
来源：http://udt.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://wan.zdqjudy.top

JS:   if (!data) return;
来源：http://buy.yfazqb.com

TS:   if (!data) return;
来源：http://ayr.andypj.xyz

Java: if (data == null) return;
来源：http://ijz.yj202588.top

Go:   if data == nil { return }
来源：http://hjh.hesvh.cn

Ruby: return if data.nil?
来源：http://xji.jiagoushi.top

C#:   if (data == null) return;
来源：http://rie.dashuyun.cn

================================================================================
来源：http://ueb.tarul.cn

C. 函数与作用域
来源：http://uqy.gzhubu.top

================================================================================
来源：http://xxx.bbcook.cn

[C01] 定义函数
来源：http://pov.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://dea.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tqg.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://qom.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mky.jqgfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lwk.hesvh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bnb.chenjidiqi.icu

Ruby: def add(a, b); a + b; end
来源：http://zex.pycfn.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mbc.fanxiaobao.xyz

[C02] 默认参数
来源：http://ljq.pengpengdd.cyou

Py:   def greet(name="World"): return name
来源：http://uup.epnwcf.com

PHP:  function greet($name = "World") { return $name; }
来源：http://cam.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://pdj.nanxuanxn.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yhd.dashuyun.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zkh.meibo888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hnc.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://jqr.zhongyouzk.top

C#:   string Greet(string name = "World") => name;
来源：http://gac.yanxiufei.cn

[C03] 可变参数
来源：http://jiw.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://xwt.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jkd.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://stc.yanxiufei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tqu.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ukv.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tto.zycfv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://huk.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rph.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://zna.redwolf501.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xsa.zdqjudy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fhz.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zrc.nanxuanxn.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://azi.wangshuangyany.cn

Java: // 无：用 Builder 模式或 record
来源：http://apz.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://rhe.cheryme.top

Ruby: f(a: 1, b: 2)
来源：http://amr.sysykeji.top

C#:   f(a: 1, b: 2)
来源：http://tcj.xuetiantiany.cn

[C05] 返回多个值
来源：http://aih.shanyushiyangkeji.top

Py:   return a, b
来源：http://zfn.xingfuxueyuan.xyz

PHP:  return [$a, $b];
来源：http://brx.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jbc.jlsjyb.cn

TS:   return { a, b };
来源：http://cmj.zhengqikj.top


<!-- 参考信息 -->