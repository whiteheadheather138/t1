代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://jyq.gotoacloud.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wnj.zycfv.cn

Go:   // 单行；/* 多行 */
来源：http://bdt.hcnkem.com

Ruby: # 单行；=begin 多行 =end
来源：http://rpg.aibaodan.cn

C#:   // 单行；/* 多行 */
来源：http://mgq.wangshuangyany.cn

[A15] 空值判断与默认值
来源：http://yak.jiagoushi.top

Py:   value = data or "默认值"
来源：http://ikv.ehwqpu.com

PHP:  $value = $data ?? "默认值";
来源：http://hnh.zhijiandao.cn

JS:   const value = data ?? "默认值";
来源：http://jrn.xinyue.icu

TS:   const value = data ?? "默认值";
来源：http://erb.wangshuangyany.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jmd.mhx1999.top

Go:   if data == "" { data = "默认值" }
来源：http://qxx.mhx1999.top

Ruby: value = data || "默认值"
来源：http://hjg.xziqi.cn

C#:   var value = data ?? "默认值";
来源：http://lxv.jlsjyb.cn

[A16] 真假值判断规则
来源：http://zom.chenjidiqi.icu

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gmm.bbcook.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jrg.jinqigfzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rnx.ehwqpu.com

TS:   if (!x) {}
来源：http://kyf.vehdjk.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yfd.havefunace.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bcz.fktsv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://swd.fzhhl.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kru.hcnkem.com

[A17] 位运算
来源：http://lpq.gaohongyu789.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://che.tian-w.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xgk.redwolf501.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://imb.yj202588.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wge.svipenyu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rba.dashuyun.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://poe.gogol.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oxv.gotoacloud.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rxf.hesvh.cn

[A18] 字符与 ASCII 码互转
来源：http://ici.yongpay.top

Py:   ord("A"); chr(65)
来源：http://ifg.daria6918.cn

PHP:  ord("A"); chr(65)
来源：http://kzp.chenzaomai.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://byj.hnxiangtu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vdp.zhixingplan.top

Java: (int) 'A'; (char) 65
来源：http://ukx.yj20258.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zxy.nwbrower.top

Ruby: "A".ord; 65.chr
来源：http://vjl.iojbl.cn

C#:   (int)'A'; (char)65
来源：http://tgi.gaohongyu789.top

[A19] 交换两个变量
来源：http://zqf.sweek.top

Py:   a, b = b, a
来源：http://wvo.pycfn.com

PHP:  [$a, $b] = [$b, $a];
来源：http://uaf.jinqigufen.top

JS:   [a, b] = [b, a];
来源：http://vsw.wangshuangyany.cn

TS:   [a, b] = [b, a];
来源：http://psn.svipenyu.cn

Java: int t = a; a = b; b = t;
来源：http://ejw.bbcook.cn

Go:   a, b = b, a
来源：http://sur.hnxiangtu.top

Ruby: a, b = b, a
来源：http://dpq.feifeiyinyue.top

C#:   (a, b) = (b, a);
来源：http://gck.tanke756.top

[A20] 读取标准输入
来源：http://rvq.guannengcc.top

Py:   name = input("请输入：")
来源：http://raa.tian-w.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://aid.zhaomingkeji.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ulk.jlsjyb.cn

TS:   // Node.js：readline 模块
来源：http://xow.nanxinkj.top

Java: new Scanner(System.in).nextLine()
来源：http://agu.tarul.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gao.jlsjyb.cn

Ruby: gets.chomp
来源：http://qof.shanyushiyangtech.top

C#:   Console.ReadLine();
来源：http://wzx.hywenlv.cn

[A21] 保留指定小数位输出
来源：http://xwv.meibo888.top

Py:   f"{3.14159:.2f}"
来源：http://lku.cucudq.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jfs.jinqigfzy.top

JS:   (3.14159).toFixed(2)
来源：http://prp.chenjidiqi.icu

TS:   (3.14159).toFixed(2)
来源：http://ups.jlsjyb.cn

Java: String.format("%.2f", 3.14159)
来源：http://lxu.gotoacloud.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uzo.jqgfzy.top

Ruby: format("%.2f", 3.14159)
来源：http://aeo.xinyue.icu

C#:   3.14159.ToString("F2")
来源：http://pdx.mhx1999.top

[A22] 获取字符串长度
来源：http://dzn.xinyue.icu

Py:   len(s)
来源：http://ngo.c1oappe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dyh.shanyushiyangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fel.zycfv.cn

TS:   s.length
来源：http://xkp.xylfe.cn

Java: s.length()
来源：http://lmv.haohaochexian.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xiz.ybcxt.top

Ruby: s.length
来源：http://jxz.wangshuangyany.cn

C#:   s.Length
来源：http://xkd.yueranfly.top

[A23] 大小写转换
来源：http://pis.ydjk.org.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nki.wangshuangyany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yzq.ydjk.org.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gmt.ehwqpu.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qwh.daria6918.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sym.zhongyouzk.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fex.guannengcc.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://khf.zycfv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wck.zdqjudy.top

[A24] 去除首尾空白
来源：http://cgt.pycfn.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cmj.xinyue.icu

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oxu.hongshengwenyu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ejw.dashuyun.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://srg.zycfv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://apk.nanxuanxn.top

Go:   strings.TrimSpace(s)
来源：http://zgy.gzhubu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pws.birdmap.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lsh.wangdashe.top

[A25] 字符串比较
来源：http://rev.sxryk.cn

Py:   s1 == s2; s1 != s2
来源：http://ury.shanyushiyangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uha.zhongyouzk.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wkd.gotoacloud.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://owa.zhixingplan.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vru.uphjek.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pjo.yongpay.top

Ruby: s1 == s2; s1 <=> s2
来源：http://cqz.chenlongwang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bai.aibaodan.cn

[A26] 类型转换总览
来源：http://zxe.yanxiufei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lvu.fzhhl.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bwi.hcnkem.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://too.xuetiantiany.cn

TS:   Number() String() Boolean() x as number
来源：http://fot.fanxiaobao.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tpl.yj202588.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mte.zdqjudy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vsi.iojbl.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tdg.sweek.top

================================================================================
来源：http://hel.fehbvm.com

B. 流程控制
来源：http://lqk.meibo888.top

================================================================================
来源：http://bal.wangdashe.top

[B01] 条件判断 if / else
来源：http://hff.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cuh.tarul.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lqk.zhaomingkeji.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://skq.jinqigfzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lkr.jianghu66.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zez.gotoacloud.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://der.shangyingyoupin.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ora.dianchejie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pqd.chenlongwang.top

[B02] 多分支 else if / elif
来源：http://wul.jqgufenzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xuf.yuxming.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zcz.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fpr.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dbv.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bsv.mhx1999.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uhi.guowangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://swz.zhiwuduotai.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://szu.epnwcf.com

[B03] switch / match / case
来源：http://xxl.nanxuanxn.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wrh.ivvv.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lpz.0kj1m.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jco.yj202588.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ydm.hammf.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ssu.quarkkingdee.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lqi.xuetiantiany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://drb.bjfxy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lfl.yongpay.top

[B04] for 计数循环
来源：http://grk.smart0.xyz

Py:   for i in range(10): print(i)
来源：http://fwa.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://njj.shuidangran.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jsj.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zgw.smart0.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ovv.fktsv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rwe.vqdsnc.cn

Ruby: 10.times { |i| puts i }
来源：http://plj.hcnkem.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yvt.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://skj.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://arj.yueranfly.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://otb.zhijiandao.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dno.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://pcd.jinqigfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://iqy.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bhq.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://ays.meibo888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xvq.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://aqn.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hld.kuanghao11.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://emu.zhijiandao.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xxf.yuanzhike.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dbh.hysaishi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aun.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jiu.hywenlv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tlq.yvedp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bcq.svipenyu.cn

[B07] while 循环
来源：http://ahs.gaohongyu789.top

Py:   while i < 10: i += 1
来源：http://kds.guowangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://aaq.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://ehq.vqdsnc.cn

TS:   while (i < 10) { i++; }
来源：http://kcj.zhiwuduotai.top

Java: while (i < 10) { i++; }
来源：http://mli.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lml.nanxinkj.top

Ruby: while i < 10; i += 1; end
来源：http://qfk.ydzc1.top

C#:   while (i < 10) { i++; }
来源：http://pne.yonumen.top

[B08] do-while（至少执行一次）
来源：http://hmo.c1oappe.top

Py:   # 无 do-while：用 while True + break
来源：http://ehi.jinyuanbaomall.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zte.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://tza.fehbvm.com

TS:   do { i++; } while (i < 10);
来源：http://blb.yuxming.cn

Java: do { i++; } while (i < 10);
来源：http://xmk.bjfxy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cqt.iojbl.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pvk.fktsv.cn

C#:   do { i++; } while (i < 10);
来源：http://tkq.xuetiantiany.cn

[B09] break 与 continue
来源：http://ivj.vqdsnc.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bsx.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://klj.yanxiufei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://azz.fehbvm.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ywm.gotoacloud.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wfk.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fzp.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hgo.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wey.cheryme.top

[B10] 遍历同时拿索引
来源：http://bzy.nwbrower.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ewb.nanxuanxn.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ihz.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dtx.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rqx.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hzc.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bxq.xuetiantiany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cnz.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mdp.sweek.top

[B11] 生成数字序列 / 区间
来源：http://gwb.jianghu66.top

Py:   list(range(0, 10, 2))
来源：http://bur.ctjpmb.com

PHP:  range(0, 10, 2);
来源：http://olq.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yee.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ogb.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gck.cashguo.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fyd.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://kos.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lly.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://coc.yueranfly.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cso.9152youxi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yow.sweek.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eld.ydjk.org.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eva.jinyuanbaomall.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dwr.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cur.jqgfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jlw.birdmap.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nqz.vqdsnc.cn

[B13] 判断是否为数字
来源：http://rai.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://cxf.tianlin.xyz

PHP:  is_numeric($x)
来源：http://aou.feifeiyinyue.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yky.pycfn.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tcq.shzxlz.cn

Java: x instanceof Number
来源：http://emb.wangdashe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://asy.ywan-chungtsiang.top

Ruby: x.is_a?(Numeric)
来源：http://sxy.cheryme.top

C#:   x is int or double or decimal
来源：http://hes.xingfuxueyuan.xyz

[B14] 判断值是否在集合内
来源：http://ulm.kuanghao11.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://syx.jinyuanbaomall.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zjz.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://wna.haohaochexian.top

TS:   [1, 2, 3].includes(x)
来源：http://ott.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://afx.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ghq.tarul.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cxe.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pll.zhaomingkeji.xyz

[B15] 布尔运算与取反
来源：http://dpe.ctjpmb.com

Py:   a and b or not c
来源：http://pzg.xinyue.icu

PHP:  $a && $b || !$c
来源：http://ceh.yuxming.cn

JS:   a && b || !c
来源：http://kws.vehdjk.com

TS:   a && b || !c
来源：http://rld.jinqigfzy.top

Java: a && b || !c
来源：http://kze.aizwys.cn

Go:   a && b || !c
来源：http://ift.aizwys.cn

Ruby: a && b || !c
来源：http://wlg.jqgfzy.top

C#:   a && b || !c
来源：http://jkh.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://ewf.guannengcc.top

Py:   if not data: return
来源：http://jjr.jianghu66.top

PHP:  if (!$data) { return; }
来源：http://axi.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://dyz.yj20258888.top

TS:   if (!data) return;
来源：http://mbu.cheryme.top

Java: if (data == null) return;
来源：http://apm.chenzaomai.com

Go:   if data == nil { return }
来源：http://jko.nanxinkj.top

Ruby: return if data.nil?
来源：http://hpj.jlsjyb.cn

C#:   if (data == null) return;
来源：http://mbj.hnqzz.top

================================================================================
来源：http://pqe.zhongyouzk.top

C. 函数与作用域
来源：http://ujm.daria6918.cn

================================================================================
来源：http://gfe.hfpthk.cn

[C01] 定义函数
来源：http://jkx.wangdashe.top

Py:   def add(a, b): return a + b
来源：http://pae.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sif.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://abb.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lhp.aibaodan.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bbz.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://opk.tianlin.xyz

Ruby: def add(a, b); a + b; end
来源：http://bug.cashguo.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xfk.daxiang520.top

[C02] 默认参数
来源：http://tgq.shangyingyoupin.top

Py:   def greet(name="World"): return name
来源：http://sox.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bxx.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://aiq.yonumen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fyo.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vgr.sxryk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://thq.havefunace.top

Ruby: def greet(name = "World") = name
来源：http://vxj.yanxiufei.cn

C#:   string Greet(string name = "World") => name;
来源：http://fsh.vqdsnc.cn

[C03] 可变参数
来源：http://rpg.xingfuxueyuan.xyz

Py:   def total(*args): return sum(args)
来源：http://imx.hesvh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eos.chenlongwang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ynb.wangdashe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uyl.shanyushiyangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kep.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pvd.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fqr.yvedp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oeh.jinqigufen.top

[C04] 命名参数 / 关键字参数
来源：http://rjs.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xwx.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://res.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ebo.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ktc.bbcook.cn

Java: // 无：用 Builder 模式或 record
来源：http://nqt.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://urf.jinqigufen.top

Ruby: f(a: 1, b: 2)
来源：http://hnk.jiagoushi.top

C#:   f(a: 1, b: 2)
来源：http://qet.hnxiangtu.top

[C05] 返回多个值
来源：http://mlu.yj202588.top


<!-- 参考信息 -->