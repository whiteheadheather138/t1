代发 wailian999

[A14] 注释写法
来源：http://wmh.yj20258.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://dwy.yanxiufei.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bvh.chenzaomai.com

JS:   // 单行；/* 多行 */
来源：http://tej.dashuyun.cn

TS:   // 单行；/* 多行 */
来源：http://cvv.dashuyun.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qdu.yongpay.top

Go:   // 单行；/* 多行 */
来源：http://qpy.smart0.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://ssw.meibo888.top

C#:   // 单行；/* 多行 */
来源：http://bjd.zhixingplan.top

[A15] 空值判断与默认值
来源：http://ekp.0kj1m.cn

Py:   value = data or "默认值"
来源：http://ttt.fanxiaobao.xyz

PHP:  $value = $data ?? "默认值";
来源：http://kyn.xingfuxueyuan.xyz

JS:   const value = data ?? "默认值";
来源：http://cun.yuxming.cn

TS:   const value = data ?? "默认值";
来源：http://mjz.shangyingyoupin.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pga.jinghuilouyu.cn

Go:   if data == "" { data = "默认值" }
来源：http://dpf.xinyue.icu

Ruby: value = data || "默认值"
来源：http://gxn.guowangkeji.top

C#:   var value = data ?? "默认值";
来源：http://juv.dianchejie.cn

[A16] 真假值判断规则
来源：http://kjb.yonumen.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nmz.yuanzhike.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://myf.wangshuangyany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ees.bbcook.cn

TS:   if (!x) {}
来源：http://qws.cheryme.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://aun.daria6918.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vst.316326.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://xcz.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pnk.316326.xyz

[A17] 位运算
来源：http://fgr.birdmap.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wzo.shuidangran.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tkc.fanxiaobao.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pjq.zhongyouzk.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uze.fehbvm.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xdh.birdmap.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uve.shangyingyoupin.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ros.gaohongyu789.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pim.iojbl.cn

[A18] 字符与 ASCII 码互转
来源：http://azf.gzhubu.top

Py:   ord("A"); chr(65)
来源：http://xcj.xingfuxueyuan.xyz

PHP:  ord("A"); chr(65)
来源：http://xfh.mhx1999.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jak.iojbl.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kvf.redwolf501.top

Java: (int) 'A'; (char) 65
来源：http://dpb.feifeiyinyue.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dxc.chenlongwang.top

Ruby: "A".ord; 65.chr
来源：http://njc.pengpengdd.cyou

C#:   (int)'A'; (char)65
来源：http://zcc.yanxiufei.cn

[A19] 交换两个变量
来源：http://jhs.chenlongwang.top

Py:   a, b = b, a
来源：http://zas.dashuyun.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qcs.jinghuilouyu.cn

JS:   [a, b] = [b, a];
来源：http://yrk.snrcjt.cn

TS:   [a, b] = [b, a];
来源：http://sqs.meibo888.top

Java: int t = a; a = b; b = t;
来源：http://aox.cashguo.top

Go:   a, b = b, a
来源：http://tfk.hfpthk.cn

Ruby: a, b = b, a
来源：http://wip.gotoacloud.top

C#:   (a, b) = (b, a);
来源：http://evv.316326.xyz

[A20] 读取标准输入
来源：http://avb.yanxiufei.cn

Py:   name = input("请输入：")
来源：http://dhb.xingfuxueyuan.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://mxx.wangdashe.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gjx.yj202588.top

TS:   // Node.js：readline 模块
来源：http://ecb.ydjk.org.cn

Java: new Scanner(System.in).nextLine()
来源：http://dan.hongshengwenyu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hfv.yongpay.top

Ruby: gets.chomp
来源：http://dxt.jinqigufen.top

C#:   Console.ReadLine();
来源：http://lph.yuanzhike.top

[A21] 保留指定小数位输出
来源：http://ewf.fzhhl.top

Py:   f"{3.14159:.2f}"
来源：http://geh.chenjidiqi.icu

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lyz.shanyushiyangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://czj.fanxiaobao.xyz

TS:   (3.14159).toFixed(2)
来源：http://wrq.yonumen.top

Java: String.format("%.2f", 3.14159)
来源：http://nav.nanxinkj.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kha.snrcjt.cn

Ruby: format("%.2f", 3.14159)
来源：http://hji.sufxvd.cn

C#:   3.14159.ToString("F2")
来源：http://yfr.vehdjk.com

[A22] 获取字符串长度
来源：http://xym.fengsongda.top

Py:   len(s)
来源：http://sfv.yueranfly.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rhw.pycfn.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://est.snrcjt.cn

TS:   s.length
来源：http://fpm.hammf.cn

Java: s.length()
来源：http://ixn.xingfuxueyuan.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rbr.chenjidiqi.icu

Ruby: s.length
来源：http://oef.redwolf501.top

C#:   s.Length
来源：http://wxg.nwbrower.top

[A23] 大小写转换
来源：http://unp.ehwqpu.com

Py:   s.upper(); s.lower(); s.title()
来源：http://ocl.yvedp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://inh.316326.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ppa.ydjk.org.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cxp.nwbrower.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kzk.tanke756.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tcp.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://red.jianghu66.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ahs.tanke756.top

[A24] 去除首尾空白
来源：http://mak.yueranfly.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cdh.bbcook.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qlx.zhiwuduotai.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jsa.yongpay.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jaj.gaohongyu789.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iak.nanxinkj.top

Go:   strings.TrimSpace(s)
来源：http://jnb.zdbjq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dmg.ybcxt.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ekx.cashguo.top

[A25] 字符串比较
来源：http://waw.xylfe.cn

Py:   s1 == s2; s1 != s2
来源：http://toq.hnqzz.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uda.yj20258.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nzs.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mfn.nwbrower.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://myh.andypj.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://svk.chenlongwang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://cmi.haohaochexian.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cnd.52xcode.cn

[A26] 类型转换总览
来源：http://bzg.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://scb.snrcjt.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bcr.ehwqpu.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jrg.jyoumei.cn

TS:   Number() String() Boolean() x as number
来源：http://gpx.yj20258.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dcr.bjfxy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zyg.pengpengdd.cyou

Ruby: to_i to_f to_s to_sym to_a
来源：http://tln.hfpthk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tke.snrcjt.cn

================================================================================
来源：http://ojg.yangfankeji.com

B. 流程控制
来源：http://bay.shanyushiyangkeji.top

================================================================================
来源：http://baz.tarul.cn

[B01] 条件判断 if / else
来源：http://xxk.hywenlv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mau.316326.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oyi.shzxlz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mss.wangshuangyany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hnc.zhaomingkeji.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://ysa.shangyingyoupin.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gar.zhixingplan.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nqo.cucudq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iwz.chenjidiqi.icu

[B02] 多分支 else if / elif
来源：http://hsc.zhaomingkeji.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ohz.dianchejie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hix.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ihl.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yjw.shzxlz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mkx.ydzc1.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kpv.0kj1m.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://luf.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nbq.9152youxi.cn

[B03] switch / match / case
来源：http://kkr.gzhubu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tku.iojbl.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eht.chenjidiqi.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vhj.9152youxi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://khy.hfpthk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kin.yuanzhike.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xqb.nwbrower.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dtm.ppjwa.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bvh.hongshengwenyu.top

[B04] for 计数循环
来源：http://drn.cqqwz.cn

Py:   for i in range(10): print(i)
来源：http://bal.hnxiangtu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kgf.sufxvd.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xeg.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ljg.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lof.redwolf501.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://heu.haohaochexian.top

Ruby: 10.times { |i| puts i }
来源：http://frs.shzxlz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tsr.jlsjyb.cn

[B05] 遍历数组 / 列表
来源：http://jba.c1oappe.top

Py:   for item in arr: print(item)
来源：http://tqh.hysaishi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uep.zdbjq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bkf.tianlin.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://shn.sjlbkw.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tom.shzxlz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ibt.yj202588.top

Ruby: arr.each { |item| puts item }
来源：http://hnz.zhongyouzk.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://msr.jianghu66.top

[B06] 遍历字典 / 对象
来源：http://vun.xziqi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wzh.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dhc.jlsjyb.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dwv.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dre.cashguo.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sal.tianlin.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jzy.shanyushiyangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cdv.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lgb.jinghuilouyu.cn

[B07] while 循环
来源：http://qky.ybcxt.top

Py:   while i < 10: i += 1
来源：http://uxg.pengpengdd.cyou

PHP:  while ($i < 10) { $i++; }
来源：http://xzi.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://kdw.shuidangran.top

TS:   while (i < 10) { i++; }
来源：http://bzl.yj202588.top

Java: while (i < 10) { i++; }
来源：http://dss.shanyushiyangtech.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jgk.sweek.top

Ruby: while i < 10; i += 1; end
来源：http://ixt.hfpthk.cn

C#:   while (i < 10) { i++; }
来源：http://bzy.snrcjt.cn

[B08] do-while（至少执行一次）
来源：http://beq.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://bal.hnxiangtu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zjw.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://ebk.fanxiaobao.xyz

TS:   do { i++; } while (i < 10);
来源：http://rkv.zycfv.cn

Java: do { i++; } while (i < 10);
来源：http://zao.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yci.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://grc.yj202588.top

C#:   do { i++; } while (i < 10);
来源：http://knr.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://rnm.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fis.iojbl.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xkz.snrcjt.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uny.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dwb.jianghu66.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nsr.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iou.cashguo.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aiz.sxryk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jld.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://niz.zhijiandao.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cqn.gzhubu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://phk.ctjpmb.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wrv.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ven.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rjj.svipenyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nsv.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wkx.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://peo.aibaodan.cn

[B11] 生成数字序列 / 区间
来源：http://ola.guannengcc.top

Py:   list(range(0, 10, 2))
来源：http://cfm.tanke756.top

PHP:  range(0, 10, 2);
来源：http://bqm.hongshengwenyu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rgu.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vgc.xuetiantiany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://izy.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bxm.uphjek.com

Ruby: (0...10).step(2).to_a
来源：http://kcp.xuetiantiany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eie.xylfe.cn

[B12] 跳出多层循环
来源：http://wxm.daria6918.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://der.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zrz.yuanzhike.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fpp.aizwys.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zfm.pycfn.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vry.aizwys.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nkz.pycfn.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hic.zdqjudy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bky.xylfe.cn

[B13] 判断是否为数字
来源：http://pct.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://ypg.fanxiaobao.xyz

PHP:  is_numeric($x)
来源：http://crn.9152youxi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oav.shanyushiyangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://elu.fanxiaobao.xyz

Java: x instanceof Number
来源：http://vsp.bjfxy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://emx.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://hko.fanxiaobao.xyz

C#:   x is int or double or decimal
来源：http://sea.sweek.top

[B14] 判断值是否在集合内
来源：http://xzd.tianlin.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sgb.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iga.tanke756.top

JS:   [1, 2, 3].includes(x)
来源：http://yph.guannengcc.top

TS:   [1, 2, 3].includes(x)
来源：http://opw.jqgufenzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ouk.zdqjudy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wba.0kj1m.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jqj.cheryme.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lpl.jqgfzy.top

[B15] 布尔运算与取反
来源：http://qwt.svipenyu.cn

Py:   a and b or not c
来源：http://dhe.chenlongwang.top

PHP:  $a && $b || !$c
来源：http://gec.9152youxi.cn

JS:   a && b || !c
来源：http://xls.yuanzhike.top

TS:   a && b || !c
来源：http://unk.xziqi.cn

Java: a && b || !c
来源：http://tfk.haohaochexian.top

Go:   a && b || !c
来源：http://lhl.aibaodan.cn

Ruby: a && b || !c
来源：http://sfd.hnqzz.top

C#:   a && b || !c
来源：http://zhi.gotoacloud.top

[B16] 卫语句：不满足条件提前返回
来源：http://ftg.zhijiandao.cn

Py:   if not data: return
来源：http://ems.hammf.cn

PHP:  if (!$data) { return; }
来源：http://kdk.svipenyu.cn

JS:   if (!data) return;
来源：http://dsz.sufxvd.cn

TS:   if (!data) return;
来源：http://fzu.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://msi.nanxuanxn.top

Go:   if data == nil { return }
来源：http://aws.wangdashe.top

Ruby: return if data.nil?
来源：http://jjc.zhaomingkeji.xyz

C#:   if (data == null) return;
来源：http://myx.zhoulong.xyz

================================================================================
来源：http://znj.fehbvm.com

C. 函数与作用域
来源：http://gdn.hywenlv.cn

================================================================================
来源：http://usa.zycfv.cn

[C01] 定义函数
来源：http://see.ivvv.top

Py:   def add(a, b): return a + b
来源：http://xvb.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cxj.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://iqq.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mfr.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://enn.epnwcf.com

Go:   func add(a, b int) int { return a + b }
来源：http://iyy.shuidangran.top

Ruby: def add(a, b); a + b; end
来源：http://rfn.cqqwz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jkv.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://gkf.jinghuilouyu.cn

Py:   def greet(name="World"): return name
来源：http://xai.jqgfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tfh.dianchejie.cn

JS:   function greet(name = "World") { return name; }
来源：http://nsf.zhixingplan.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gwr.cqqwz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ool.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://spx.xinyue.icu

Ruby: def greet(name = "World") = name
来源：http://fnr.zhiwuduotai.top

C#:   string Greet(string name = "World") => name;
来源：http://efv.pengpengdd.cyou

[C03] 可变参数
来源：http://kga.shuidangran.top

Py:   def total(*args): return sum(args)
来源：http://juz.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uxf.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xvg.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uoj.tian-w.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://naj.epnwcf.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mmu.wangshuangyany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://djn.guannengcc.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rgt.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://uuv.yueranfly.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iya.yangfankeji.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wrx.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ycx.xuanzx.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ryv.zhongyouzk.top

Java: // 无：用 Builder 模式或 record
来源：http://utv.jiagoushi.top


<!-- 参考信息 -->