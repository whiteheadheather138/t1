代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://vgq.cucudq.cn

[A15] 空值判断与默认值
来源：http://uqx.yuanzhike.top

Py:   value = data or "默认值"
来源：http://jdh.chenjidiqi.icu

PHP:  $value = $data ?? "默认值";
来源：http://ctm.jianghu66.top

JS:   const value = data ?? "默认值";
来源：http://rne.chenzaomai.com

TS:   const value = data ?? "默认值";
来源：http://pzr.havefunace.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tqj.sysykeji.top

Go:   if data == "" { data = "默认值" }
来源：http://gbj.yuanzhike.top

Ruby: value = data || "默认值"
来源：http://vjk.smart0.xyz

C#:   var value = data ?? "默认值";
来源：http://xbk.cucudq.cn

[A16] 真假值判断规则
来源：http://gor.gzhubu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://irn.vehdjk.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zru.pycfn.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rby.shzxlz.cn

TS:   if (!x) {}
来源：http://tpc.yj20258.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://klq.dianchejie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cmi.jqgufenzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://bzy.haohaochexian.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://clu.9152youxi.cn

[A17] 位运算
来源：http://gtu.smart0.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vav.tian-w.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wci.jqgufenzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://isu.jinqigufen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://znc.shanyushiyangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tln.xuetiantiany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cvx.fzhhl.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dvx.sxryk.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bng.birdmap.top

[A18] 字符与 ASCII 码互转
来源：http://rdu.ppjwa.cn

Py:   ord("A"); chr(65)
来源：http://ccs.cqqwz.cn

PHP:  ord("A"); chr(65)
来源：http://evw.tian-w.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://asn.chenjidiqi.icu

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pcw.zhaomingkeji.xyz

Java: (int) 'A'; (char) 65
来源：http://gqy.yonumen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ohj.bbcook.cn

Ruby: "A".ord; 65.chr
来源：http://ufw.shzxlz.cn

C#:   (int)'A'; (char)65
来源：http://ksr.shzxlz.cn

[A19] 交换两个变量
来源：http://dbt.yuanzhike.top

Py:   a, b = b, a
来源：http://iod.shzxlz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vbt.sweek.top

JS:   [a, b] = [b, a];
来源：http://tde.meibo888.top

TS:   [a, b] = [b, a];
来源：http://okw.aibaodan.cn

Java: int t = a; a = b; b = t;
来源：http://ugf.zdbjq.cn

Go:   a, b = b, a
来源：http://lql.yonumen.top

Ruby: a, b = b, a
来源：http://fgk.jqgfzy.top

C#:   (a, b) = (b, a);
来源：http://kct.hysaishi.cn

[A20] 读取标准输入
来源：http://qdc.jianghu66.top

Py:   name = input("请输入：")
来源：http://szo.jyoumei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ewy.aibaodan.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rrk.dashuyun.cn

TS:   // Node.js：readline 模块
来源：http://sxr.fengsongda.top

Java: new Scanner(System.in).nextLine()
来源：http://kkn.daria6918.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gho.shuidangran.top

Ruby: gets.chomp
来源：http://ckl.chenzaomai.com

C#:   Console.ReadLine();
来源：http://jbp.feifeiyinyue.top

[A21] 保留指定小数位输出
来源：http://ysf.jqgfzy.top

Py:   f"{3.14159:.2f}"
来源：http://hhv.guowangkeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ovw.xingfuxueyuan.xyz

JS:   (3.14159).toFixed(2)
来源：http://xwc.xuanzx.com

TS:   (3.14159).toFixed(2)
来源：http://sal.jiagoushi.top

Java: String.format("%.2f", 3.14159)
来源：http://ial.wangshuangyany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cmz.yanxiufei.cn

Ruby: format("%.2f", 3.14159)
来源：http://pym.xinyue.icu

C#:   3.14159.ToString("F2")
来源：http://sgr.c1oappe.top

[A22] 获取字符串长度
来源：http://jxd.redwolf501.top

Py:   len(s)
来源：http://pxh.uphjek.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wfl.yvedp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zvx.jqgufenzy.top

TS:   s.length
来源：http://hba.tanke756.top

Java: s.length()
来源：http://lso.shuidangran.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eeu.cdnleiting.top

Ruby: s.length
来源：http://toc.xuanzx.com

C#:   s.Length
来源：http://dto.cqqwz.cn

[A23] 大小写转换
来源：http://lse.snrcjt.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://air.52xcode.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://otm.fzhhl.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dld.quarkkingdee.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ysr.vehdjk.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mvy.tianlin.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gqp.yfazqb.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bim.chenlongwang.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ncc.jqgufenzy.top

[A24] 去除首尾空白
来源：http://pao.zhoulong.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rde.meibo888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jrz.chenlongwang.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bsb.hammf.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fua.nanxinkj.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vzb.zhongyouzk.top

Go:   strings.TrimSpace(s)
来源：http://lvl.sjlbkw.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tvc.ydzc1.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eyq.cashguo.top

[A25] 字符串比较
来源：http://wct.yangfankeji.com

Py:   s1 == s2; s1 != s2
来源：http://dxu.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ila.ctjpmb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nii.shanyushiyangtech.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bjp.cucudq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ixg.yvedp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hfl.zhongyouzk.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bsv.gotoacloud.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://njp.ydzc1.top

[A26] 类型转换总览
来源：http://nfp.xylfe.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://roi.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fbn.jqgufenzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vjr.jianghu66.top

TS:   Number() String() Boolean() x as number
来源：http://mha.guowangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dcm.yonumen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qdw.yj202588.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://otg.xinyue.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bip.zhijiandao.cn

================================================================================
来源：http://oxz.nwbrower.top

B. 流程控制
来源：http://vxn.cucudq.cn

================================================================================
来源：http://fnl.zhijiandao.cn

[B01] 条件判断 if / else
来源：http://oej.zhaomingkeji.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://car.jyoumei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bke.hysaishi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://npw.smart0.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mrt.tarul.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zqy.hcnkem.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ifp.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cmq.316326.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xqd.chenlongwang.top

[B02] 多分支 else if / elif
来源：http://jgu.nanxuanxn.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://deg.aizwys.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pxj.sjlbkw.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ifh.pycfn.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wdv.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jve.birdmap.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dxg.cdnleiting.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rbv.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lfv.xylfe.cn

[B03] switch / match / case
来源：http://wld.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rmf.aibaodan.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eui.shangyingyoupin.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://orf.ydjk.org.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jlj.hesvh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pyk.yfazqb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lyp.cdnleiting.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rna.xuetiantiany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xgg.gotoacloud.top

[B04] for 计数循环
来源：http://xgb.aibaodan.cn

Py:   for i in range(10): print(i)
来源：http://buy.quarkkingdee.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fmg.dashuyun.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yig.aizwys.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://viq.yanxiufei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lxb.cheryme.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mca.zhongyouzk.top

Ruby: 10.times { |i| puts i }
来源：http://xqc.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dqj.sufxvd.cn

[B05] 遍历数组 / 列表
来源：http://oon.xuanzx.com

Py:   for item in arr: print(item)
来源：http://sfp.andypj.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hvd.ctjpmb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://baa.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vqx.yj20258.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://okp.cheryme.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oli.yj202588.top

Ruby: arr.each { |item| puts item }
来源：http://emd.jinqigufen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qbm.haohaochexian.top

[B06] 遍历字典 / 对象
来源：http://xjh.vqdsnc.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://njx.svipenyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://iaz.jinyuanbaomall.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jwc.shuidangran.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hra.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gye.yueranfly.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dfs.fehbvm.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vlp.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xgk.xuanzx.com

[B07] while 循环
来源：http://sgc.epnwcf.com

Py:   while i < 10: i += 1
来源：http://yzt.yueranfly.top

PHP:  while ($i < 10) { $i++; }
来源：http://irn.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://okf.yonumen.top

TS:   while (i < 10) { i++; }
来源：http://tjt.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://ibh.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mhn.zhixingplan.top

Ruby: while i < 10; i += 1; end
来源：http://ptn.hfpthk.cn

C#:   while (i < 10) { i++; }
来源：http://zuf.shuidangran.top

[B08] do-while（至少执行一次）
来源：http://abu.wangshuangyany.cn

Py:   # 无 do-while：用 while True + break
来源：http://wpq.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bkj.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://pox.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://wvn.pycfn.com

Java: do { i++; } while (i < 10);
来源：http://lns.wangshuangyany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zhe.jinyuanbaomall.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mea.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://guf.zdqjudy.top

[B09] break 与 continue
来源：http://gna.shanyushiyangtech.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pby.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mus.fengsongda.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ufg.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://azr.cdnleiting.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kzv.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uzz.zhoulong.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wem.zdqjudy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fkd.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://llp.jqgfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jiu.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uxb.sjlbkw.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jrz.shanyushiyangtech.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://svx.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vtw.zdbjq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qdx.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fba.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://edp.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://esx.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://flh.birdmap.top

PHP:  range(0, 10, 2);
来源：http://oby.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qrn.316326.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nhj.shanyushiyangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wbs.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xuh.zhoulong.xyz

Ruby: (0...10).step(2).to_a
来源：http://vcv.cheryme.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hiy.jqgufenzy.top

[B12] 跳出多层循环
来源：http://gwr.xylfe.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sss.yuxming.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mgb.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wmj.xziqi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zcn.wangdashe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://trm.tanke756.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ufr.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kbj.quarkkingdee.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ckb.gotoacloud.top

[B13] 判断是否为数字
来源：http://ytm.52xcode.cn

Py:   isinstance(x, (int, float))
来源：http://rtg.ctjpmb.com

PHP:  is_numeric($x)
来源：http://fdq.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ucd.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://epf.jinghuilouyu.cn

Java: x instanceof Number
来源：http://uon.zhijiandao.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xms.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://xwy.tanke756.top

C#:   x is int or double or decimal
来源：http://vqy.hesvh.cn

[B14] 判断值是否在集合内
来源：http://bzl.quarkkingdee.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://thj.jinyuanbaomall.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qtj.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://abe.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://pms.cheryme.top

Java: List.of(1, 2, 3).contains(x)
来源：http://upy.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mfn.c1oappe.top

Ruby: [1, 2, 3].include?(x)
来源：http://xsq.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hbr.haohaochexian.top

[B15] 布尔运算与取反
来源：http://nbl.pycfn.com

Py:   a and b or not c
来源：http://nor.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://niz.c1oappe.top

JS:   a && b || !c
来源：http://lhp.ppjwa.cn

TS:   a && b || !c
来源：http://gwi.sysykeji.top

Java: a && b || !c
来源：http://pjc.zdbjq.cn

Go:   a && b || !c
来源：http://yxw.sysykeji.top

Ruby: a && b || !c
来源：http://tmd.chenzaomai.com

C#:   a && b || !c
来源：http://nne.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wlx.ctjpmb.com

Py:   if not data: return
来源：http://pfx.hcnkem.com

PHP:  if (!$data) { return; }
来源：http://leo.gzhubu.top

JS:   if (!data) return;
来源：http://jgx.havefunace.top

TS:   if (!data) return;
来源：http://cty.zhijiandao.cn

Java: if (data == null) return;
来源：http://imu.pycfn.com

Go:   if data == nil { return }
来源：http://asc.shanyushiyangtech.top

Ruby: return if data.nil?
来源：http://taz.xinyue.icu

C#:   if (data == null) return;
来源：http://fmo.aibaodan.cn

================================================================================
来源：http://nlq.tarul.cn

C. 函数与作用域
来源：http://ulg.tianlin.xyz

================================================================================
来源：http://yth.uphjek.com

[C01] 定义函数
来源：http://uha.fengsongda.top

Py:   def add(a, b): return a + b
来源：http://ofl.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ofv.jiagoushi.top

JS:   function add(a, b) { return a + b; }
来源：http://vnq.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kcq.hywenlv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fcy.hnqzz.top

Go:   func add(a, b int) int { return a + b }
来源：http://ewr.jiagoushi.top

Ruby: def add(a, b); a + b; end
来源：http://hsg.redwolf501.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ylh.jlsjyb.cn

[C02] 默认参数
来源：http://aix.meibo888.top

Py:   def greet(name="World"): return name
来源：http://ioa.vehdjk.com

PHP:  function greet($name = "World") { return $name; }
来源：http://aqq.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://dsq.fehbvm.com

TS:   function greet(name: string = "World") { return name; }
来源：http://ees.fzhhl.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vxa.tanke756.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jro.daxiang520.top

Ruby: def greet(name = "World") = name
来源：http://lvy.shanyushiyangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://jdk.cashguo.top

[C03] 可变参数
来源：http://qej.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://mdc.andypj.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mqs.fzhhl.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://czr.zdqjudy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://unq.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bzh.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vfb.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://kus.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mww.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://zha.jinqigufen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nnz.zhoulong.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hyj.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jmv.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ckp.chenjidiqi.icu

Java: // 无：用 Builder 模式或 record
来源：http://fuf.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://iom.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://lxw.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://uiz.birdmap.top

[C05] 返回多个值
来源：http://gsy.tianlin.xyz

Py:   return a, b
来源：http://lxx.pengpengdd.cyou

PHP:  return [$a, $b];
来源：http://mhb.vehdjk.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://voi.yvedp.cn

TS:   return { a, b };
来源：http://vla.jinyuanbaomall.cn


<!-- 参考信息 -->