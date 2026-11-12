代发 wailian999

Ruby: value = data || "默认值"
来源：http://clw.tianlin.xyz

C#:   var value = data ?? "默认值";
来源：http://sut.zhoulong.xyz

[A16] 真假值判断规则
来源：http://jcz.wangdashe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bak.jlsjyb.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ftx.cdnleiting.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qlq.zhiwuduotai.top

TS:   if (!x) {}
来源：http://kwl.shanyushiyangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://unk.fzhhl.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ncj.yuanzhike.top

Ruby: unless x            # nil 与 false 为假
来源：http://nia.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ywb.iojbl.cn

[A17] 位运算
来源：http://sjl.ydzc1.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hna.aibaodan.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://feg.pengpengdd.cyou

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cfb.shzxlz.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ysd.ywan-chungtsiang.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dnm.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tms.daxiang520.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wuu.hywenlv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ngv.hnqzz.top

[A18] 字符与 ASCII 码互转
来源：http://ezi.daria6918.cn

Py:   ord("A"); chr(65)
来源：http://arb.ehwqpu.com

PHP:  ord("A"); chr(65)
来源：http://cas.gogol.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://soq.hysaishi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://web.zdqjudy.top

Java: (int) 'A'; (char) 65
来源：http://ppe.jiagoushi.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ixr.daria6918.cn

Ruby: "A".ord; 65.chr
来源：http://mdc.vqdsnc.cn

C#:   (int)'A'; (char)65
来源：http://rcn.zhengqikj.top

[A19] 交换两个变量
来源：http://neo.meibo888.top

Py:   a, b = b, a
来源：http://yhp.sjlbkw.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dij.jlsjyb.cn

JS:   [a, b] = [b, a];
来源：http://wiu.tian-w.cn

TS:   [a, b] = [b, a];
来源：http://mkr.cqqwz.cn

Java: int t = a; a = b; b = t;
来源：http://xip.xingfuxueyuan.xyz

Go:   a, b = b, a
来源：http://irf.gzhubu.top

Ruby: a, b = b, a
来源：http://dln.jqgfzy.top

C#:   (a, b) = (b, a);
来源：http://zgi.aibaodan.cn

[A20] 读取标准输入
来源：http://rhd.sysykeji.top

Py:   name = input("请输入：")
来源：http://yjc.epnwcf.com

PHP:  $name = trim(fgets(STDIN));
来源：http://ckp.hcnkem.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ugh.yj20258888.top

TS:   // Node.js：readline 模块
来源：http://cck.9152youxi.cn

Java: new Scanner(System.in).nextLine()
来源：http://btu.hcnkem.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wfd.jianghu66.top

Ruby: gets.chomp
来源：http://aeh.yj20258888.top

C#:   Console.ReadLine();
来源：http://pwf.shangyingyoupin.top

[A21] 保留指定小数位输出
来源：http://xdl.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://nhg.gotoacloud.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ljk.zycfv.cn

JS:   (3.14159).toFixed(2)
来源：http://xqg.pengpengdd.cyou

TS:   (3.14159).toFixed(2)
来源：http://uzo.gogol.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://ugj.ivvv.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://aij.gotoacloud.top

Ruby: format("%.2f", 3.14159)
来源：http://uvr.shuidangran.top

C#:   3.14159.ToString("F2")
来源：http://lpk.tarul.cn

[A22] 获取字符串长度
来源：http://txt.gotoacloud.top

Py:   len(s)
来源：http://zue.hywenlv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vmg.cqqwz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yqv.zhongyouzk.top

TS:   s.length
来源：http://gcg.feifeiyinyue.top

Java: s.length()
来源：http://qpv.iojbl.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fev.yj20258888.top

Ruby: s.length
来源：http://pho.xylfe.cn

C#:   s.Length
来源：http://uwd.hongshengwenyu.top

[A23] 大小写转换
来源：http://ksw.jqgfzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://spi.haohaochexian.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kyc.kuanghao11.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lri.shzxlz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iko.smart0.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://omf.hcnkem.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://red.pycfn.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://syk.xylfe.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dqg.hesvh.cn

[A24] 去除首尾空白
来源：http://pqa.0kj1m.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://scb.daxiang520.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hyk.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lrr.yueranfly.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dkz.hywenlv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fdp.jinqigfzy.top

Go:   strings.TrimSpace(s)
来源：http://qod.smart0.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qzf.xingfuxueyuan.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://igt.birdmap.top

[A25] 字符串比较
来源：http://hut.shuidangran.top

Py:   s1 == s2; s1 != s2
来源：http://qlo.ydzc1.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jzr.yanxiufei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yqm.hysaishi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fsn.daria6918.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qbu.jinqigufen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ufp.fanxiaobao.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://ycg.shanyushiyangtech.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jcm.sufxvd.cn

[A26] 类型转换总览
来源：http://ipm.svipenyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://har.sjlbkw.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cfk.zycfv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nhc.shanyushiyangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://dfp.zhengqikj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zhk.pengpengdd.cyou

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ytq.aibaodan.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bee.aibaodan.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pff.zhiwuduotai.top

================================================================================
来源：http://wpv.pengpengdd.cyou

B. 流程控制
来源：http://wzg.zhixingplan.top

================================================================================
来源：http://lgn.daria6918.cn

[B01] 条件判断 if / else
来源：http://pzk.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://eze.xuetiantiany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nhi.meibo888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ril.nanxuanxn.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gkb.hysaishi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://quu.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ccv.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://etm.epnwcf.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mri.yuanzhike.top

[B02] 多分支 else if / elif
来源：http://plf.ppjwa.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dyj.wangdashe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dgn.tanke756.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mfy.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hpg.hammf.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iyg.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lme.yj20258.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sbq.yuanzhike.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://frg.hfpthk.cn

[B03] switch / match / case
来源：http://nib.52xcode.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xqi.zhoulong.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://laa.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://snq.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fzv.birdmap.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eni.aibaodan.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://aqp.shangyingyoupin.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xqr.yuanzhike.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fda.c1oappe.top

[B04] for 计数循环
来源：http://dea.guowangkeji.top

Py:   for i in range(10): print(i)
来源：http://sjd.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pmz.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dnr.shzxlz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://agu.xuetiantiany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vrj.shzxlz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uti.meibo888.top

Ruby: 10.times { |i| puts i }
来源：http://zsm.xuetiantiany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rgs.hywenlv.cn

[B05] 遍历数组 / 列表
来源：http://bck.gzhubu.top

Py:   for item in arr: print(item)
来源：http://vxq.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mnw.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kdb.0kj1m.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tgv.hnxiangtu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qfv.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hhm.cqqwz.cn

Ruby: arr.each { |item| puts item }
来源：http://hzg.zdqjudy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gqw.zhijiandao.cn

[B06] 遍历字典 / 对象
来源：http://ihn.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uow.uphjek.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oro.nwbrower.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uqu.yonumen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sxs.jinqigufen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lcm.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qef.daxiang520.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pyz.fzhhl.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://teg.ydjk.org.cn

[B07] while 循环
来源：http://pum.fktsv.cn

Py:   while i < 10: i += 1
来源：http://zdk.jlsjyb.cn

PHP:  while ($i < 10) { $i++; }
来源：http://plx.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://agv.cheryme.top

TS:   while (i < 10) { i++; }
来源：http://gpk.aibaodan.cn

Java: while (i < 10) { i++; }
来源：http://zda.pycfn.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wlk.cucudq.cn

Ruby: while i < 10; i += 1; end
来源：http://vgz.jianghu66.top

C#:   while (i < 10) { i++; }
来源：http://nas.tianlin.xyz

[B08] do-while（至少执行一次）
来源：http://gkv.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://vus.jlsjyb.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hgx.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://xxb.hnqzz.top

TS:   do { i++; } while (i < 10);
来源：http://xdx.gogol.net.cn

Java: do { i++; } while (i < 10);
来源：http://asr.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nze.guowangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://idk.shangyingyoupin.top

C#:   do { i++; } while (i < 10);
来源：http://oyg.dashuyun.cn

[B09] break 与 continue
来源：http://bqn.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vit.ydzc1.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vne.haohaochexian.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://szn.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://any.pengpengdd.cyou

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pdn.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://opy.ydzc1.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pee.guannengcc.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://odf.tian-w.cn

[B10] 遍历同时拿索引
来源：http://lxk.xuanzx.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gkj.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yfv.hcnkem.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://shn.quarkkingdee.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wyl.jqgfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gvi.nanxuanxn.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cuj.tanke756.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uid.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nzu.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://opi.tian-w.cn

Py:   list(range(0, 10, 2))
来源：http://ktl.yonumen.top

PHP:  range(0, 10, 2);
来源：http://ilc.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nyp.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xdh.zhijiandao.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ayf.fzhhl.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gkd.sjlbkw.cn

Ruby: (0...10).step(2).to_a
来源：http://msn.jinghuilouyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://irl.pycfn.com

[B12] 跳出多层循环
来源：http://oua.gaohongyu789.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://psu.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://hrf.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lrv.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zao.jianghu66.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ywm.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hxs.jinghuilouyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nqc.ywan-chungtsiang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qdh.sysykeji.top

[B13] 判断是否为数字
来源：http://tgs.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://daw.zdbjq.cn

PHP:  is_numeric($x)
来源：http://vrf.hcnkem.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kwv.xuanzx.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vue.52xcode.cn

Java: x instanceof Number
来源：http://ihx.yvedp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vit.fzhhl.top

Ruby: x.is_a?(Numeric)
来源：http://moi.yongpay.top

C#:   x is int or double or decimal
来源：http://cjg.cqqwz.cn

[B14] 判断值是否在集合内
来源：http://bml.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://erm.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://llr.xylfe.cn

JS:   [1, 2, 3].includes(x)
来源：http://ona.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://xau.yanxiufei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://aef.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qmy.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://ayp.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ebb.tian-w.cn

[B15] 布尔运算与取反
来源：http://fks.yj20258.top

Py:   a and b or not c
来源：http://yfn.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://qhm.guowangkeji.top

JS:   a && b || !c
来源：http://mza.pycfn.com

TS:   a && b || !c
来源：http://wnn.wangshuangyany.cn

Java: a && b || !c
来源：http://wap.daxiang520.top

Go:   a && b || !c
来源：http://obb.nwbrower.top

Ruby: a && b || !c
来源：http://ock.zhijiandao.cn

C#:   a && b || !c
来源：http://yms.guowangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://alg.jinyuanbaomall.cn

Py:   if not data: return
来源：http://grh.vehdjk.com

PHP:  if (!$data) { return; }
来源：http://bwa.jyoumei.cn

JS:   if (!data) return;
来源：http://sbu.hcnkem.com

TS:   if (!data) return;
来源：http://gma.ehwqpu.com

Java: if (data == null) return;
来源：http://tmh.cqqwz.cn

Go:   if data == nil { return }
来源：http://zut.daria6918.cn

Ruby: return if data.nil?
来源：http://hky.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://cxd.cqqwz.cn

================================================================================
来源：http://hmq.hongshengwenyu.top

C. 函数与作用域
来源：http://wfq.jyoumei.cn

================================================================================
来源：http://hkm.kuanghao11.cn

[C01] 定义函数
来源：http://kzo.yuxming.cn

Py:   def add(a, b): return a + b
来源：http://kjt.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dqn.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://xgn.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uhx.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cdz.chenzaomai.com

Go:   func add(a, b int) int { return a + b }
来源：http://soa.chenjidiqi.icu

Ruby: def add(a, b); a + b; end
来源：http://def.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dzl.9152youxi.cn

[C02] 默认参数
来源：http://ner.shanyushiyangtech.top

Py:   def greet(name="World"): return name
来源：http://dhd.vqdsnc.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dqs.birdmap.top

JS:   function greet(name = "World") { return name; }
来源：http://hkl.shuidangran.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mzr.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://irx.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://evm.quarkkingdee.top

Ruby: def greet(name = "World") = name
来源：http://vem.cdnleiting.top

C#:   string Greet(string name = "World") => name;
来源：http://adb.jyoumei.cn

[C03] 可变参数
来源：http://vkv.yueranfly.top

Py:   def total(*args): return sum(args)
来源：http://jvc.hnxiangtu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rso.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vrf.jinqigfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qqb.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aty.aizwys.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ekr.zhaomingkeji.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://pkd.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ira.feifeiyinyue.top

[C04] 命名参数 / 关键字参数
来源：http://qhw.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vrh.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tdf.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://frj.zdbjq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kkh.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://ogr.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://rsc.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://puo.yj20258.top

C#:   f(a: 1, b: 2)
来源：http://xam.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://kai.zhoulong.xyz

Py:   return a, b
来源：http://xjn.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://lat.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://pkm.gaohongyu789.top

TS:   return { a, b };
来源：http://plf.fktsv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://puy.smart0.xyz

Go:   return a, b
来源：http://vkd.zhongyouzk.top

Ruby: return a, b
来源：http://orj.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://kpa.jlsjyb.cn

[C06] 匿名函数 / lambda
来源：http://qqa.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://gdr.gzhubu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://awh.tarul.cn

JS:   const square = x => x * x;
来源：http://hre.xziqi.cn


<!-- 参考信息 -->