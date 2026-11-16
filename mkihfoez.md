代发 wailian999

[A14] 注释写法
来源：http://owx.zhengqikj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://teh.0kj1m.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mbr.hfpthk.cn

JS:   // 单行；/* 多行 */
来源：http://dkm.svipenyu.cn

TS:   // 单行；/* 多行 */
来源：http://zst.meibo888.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://eaz.hcnkem.com

Go:   // 单行；/* 多行 */
来源：http://jgl.hysaishi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yrl.yuxming.cn

C#:   // 单行；/* 多行 */
来源：http://liy.jqgufenzy.top

[A15] 空值判断与默认值
来源：http://edg.jianghu66.top

Py:   value = data or "默认值"
来源：http://qvp.jinyuanbaomall.cn

PHP:  $value = $data ?? "默认值";
来源：http://wvd.c1oappe.top

JS:   const value = data ?? "默认值";
来源：http://vyw.dashuyun.cn

TS:   const value = data ?? "默认值";
来源：http://zhi.zhiwuduotai.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qov.snrcjt.cn

Go:   if data == "" { data = "默认值" }
来源：http://lav.yueranfly.top

Ruby: value = data || "默认值"
来源：http://wge.sufxvd.cn

C#:   var value = data ?? "默认值";
来源：http://xep.zdbjq.cn

[A16] 真假值判断规则
来源：http://plr.chenjidiqi.icu

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kpt.wangshuangyany.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uav.hywenlv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ism.cucudq.cn

TS:   if (!x) {}
来源：http://yln.yj20258888.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ktn.zhijiandao.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qpo.daxiang520.top

Ruby: unless x            # nil 与 false 为假
来源：http://kpd.meibo888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gep.shuidangran.top

[A17] 位运算
来源：http://rlz.yuanzhike.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jjx.xuetiantiany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hnf.jinyuanbaomall.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oyi.xinyue.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zyy.meibo888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rkc.pengpengdd.cyou

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jst.smart0.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wck.guannengcc.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sur.xylfe.cn

[A18] 字符与 ASCII 码互转
来源：http://zld.jianghu66.top

Py:   ord("A"); chr(65)
来源：http://nqr.fengsongda.top

PHP:  ord("A"); chr(65)
来源：http://awi.shanyushiyangtech.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yed.bjfxy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ums.feifeiyinyue.top

Java: (int) 'A'; (char) 65
来源：http://jpt.kuanghao11.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yvt.jyoumei.cn

Ruby: "A".ord; 65.chr
来源：http://qmk.kuanghao11.cn

C#:   (int)'A'; (char)65
来源：http://hxm.xylfe.cn

[A19] 交换两个变量
来源：http://jne.jinghuilouyu.cn

Py:   a, b = b, a
来源：http://buy.sxryk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cci.jlsjyb.cn

JS:   [a, b] = [b, a];
来源：http://nyg.smart0.xyz

TS:   [a, b] = [b, a];
来源：http://ptn.cheryme.top

Java: int t = a; a = b; b = t;
来源：http://rmk.yj20258.top

Go:   a, b = b, a
来源：http://ahh.shanyushiyangkeji.top

Ruby: a, b = b, a
来源：http://fvs.meibo888.top

C#:   (a, b) = (b, a);
来源：http://uee.yvedp.cn

[A20] 读取标准输入
来源：http://lkn.epnwcf.com

Py:   name = input("请输入：")
来源：http://ous.fanxiaobao.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://iba.fanxiaobao.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lxx.dianchejie.cn

TS:   // Node.js：readline 模块
来源：http://ifz.zhaomingkeji.xyz

Java: new Scanner(System.in).nextLine()
来源：http://dxo.vehdjk.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kgf.ydjk.org.cn

Ruby: gets.chomp
来源：http://pqe.yj20258.top

C#:   Console.ReadLine();
来源：http://wrs.nanxinkj.top

[A21] 保留指定小数位输出
来源：http://dsq.tianlin.xyz

Py:   f"{3.14159:.2f}"
来源：http://uin.52xcode.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lmo.xylfe.cn

JS:   (3.14159).toFixed(2)
来源：http://mal.jinqigufen.top

TS:   (3.14159).toFixed(2)
来源：http://ncn.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://wtw.jinghuilouyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mpq.ybcxt.top

Ruby: format("%.2f", 3.14159)
来源：http://idn.ivvv.top

C#:   3.14159.ToString("F2")
来源：http://wso.svipenyu.cn

[A22] 获取字符串长度
来源：http://tza.gzhubu.top

Py:   len(s)
来源：http://jsw.haohaochexian.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yhd.haohaochexian.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://btb.jianghu66.top

TS:   s.length
来源：http://mtn.316326.xyz

Java: s.length()
来源：http://lox.hfpthk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kyp.hnqzz.top

Ruby: s.length
来源：http://gho.hnqzz.top

C#:   s.Length
来源：http://ubg.vqdsnc.cn

[A23] 大小写转换
来源：http://ceq.wangdashe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://agc.sxryk.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bzl.jinqigufen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vvy.ppjwa.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://orl.chenlongwang.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://guk.316326.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fga.xingfuxueyuan.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jgk.ppjwa.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lzd.yuxming.cn

[A24] 去除首尾空白
来源：http://tcq.yj202588.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zck.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fel.jinqigufen.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mzv.sxryk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://llv.epnwcf.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wea.zhongyouzk.top

Go:   strings.TrimSpace(s)
来源：http://jwc.zhoulong.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iib.andypj.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wri.cdnleiting.top

[A25] 字符串比较
来源：http://fhm.yfazqb.com

Py:   s1 == s2; s1 != s2
来源：http://bmy.hysaishi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ifn.c1oappe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jhl.shuidangran.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kxw.xuanzx.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pro.iojbl.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fbl.yuanzhike.top

Ruby: s1 == s2; s1 <=> s2
来源：http://evg.vehdjk.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tqv.tian-w.cn

[A26] 类型转换总览
来源：http://ayy.nwbrower.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uva.nwbrower.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dkj.jinghuilouyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fwa.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://etj.fehbvm.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ege.fzhhl.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dnu.bjfxy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ysn.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jzm.shanyushiyangkeji.top

================================================================================
来源：http://jsi.dianchejie.cn

B. 流程控制
来源：http://gcm.zhiwuduotai.top

================================================================================
来源：http://hjs.dashuyun.cn

[B01] 条件判断 if / else
来源：http://mrr.epnwcf.com

Py:   result = "正" if x > 0 else "非正"
来源：http://run.chenlongwang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tau.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tbj.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ziq.chenzaomai.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://hfr.xingfuxueyuan.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mcc.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vvr.iojbl.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qxg.zdbjq.cn

[B02] 多分支 else if / elif
来源：http://gqb.gotoacloud.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://afx.pycfn.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ltz.sjlbkw.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wsa.sufxvd.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ayi.52xcode.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jzn.0kj1m.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uma.hcnkem.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uyv.jinghuilouyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qap.daria6918.cn

[B03] switch / match / case
来源：http://epm.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tgy.zhixingplan.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qke.hfpthk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gvp.c1oappe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tuh.0kj1m.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ayl.daria6918.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://snm.tarul.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vit.xylfe.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kja.9152youxi.cn

[B04] for 计数循环
来源：http://tlo.ybcxt.top

Py:   for i in range(10): print(i)
来源：http://hmq.hnqzz.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oan.wangdashe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xgz.shzxlz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sxb.jianghu66.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ebe.sxryk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rxp.gotoacloud.top

Ruby: 10.times { |i| puts i }
来源：http://qas.tianlin.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hbx.ehwqpu.com

[B05] 遍历数组 / 列表
来源：http://rje.9152youxi.cn

Py:   for item in arr: print(item)
来源：http://hdg.aizwys.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nev.pengpengdd.cyou

JS:   for (const item of arr) { console.log(item); }
来源：http://zmm.zhixingplan.top

TS:   for (const item of arr) { console.log(item); }
来源：http://szz.andypj.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://wwu.yueranfly.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mve.sxryk.cn

Ruby: arr.each { |item| puts item }
来源：http://qqe.meibo888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://crv.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://gzo.yonumen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hbr.ppjwa.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qpn.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oah.chenlongwang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nor.jianghu66.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cva.smart0.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nmb.yonumen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://emf.yj20258.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kpk.xziqi.cn

[B07] while 循环
来源：http://xxq.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://atg.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ipd.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://wzt.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://xcz.cashguo.top

Java: while (i < 10) { i++; }
来源：http://mbm.haohaochexian.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zhz.svipenyu.cn

Ruby: while i < 10; i += 1; end
来源：http://mzg.pengpengdd.cyou

C#:   while (i < 10) { i++; }
来源：http://cqa.xylfe.cn

[B08] do-while（至少执行一次）
来源：http://cak.smart0.xyz

Py:   # 无 do-while：用 while True + break
来源：http://cza.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ccz.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://zfe.ybcxt.top

TS:   do { i++; } while (i < 10);
来源：http://ncg.jinqigfzy.top

Java: do { i++; } while (i < 10);
来源：http://bzx.zhaomingkeji.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://atm.shanyushiyangtech.top

Ruby: begin; i += 1; end while i < 10
来源：http://bnj.shangyingyoupin.top

C#:   do { i++; } while (i < 10);
来源：http://lgh.ydzc1.top

[B09] break 与 continue
来源：http://oul.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dvh.havefunace.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://url.yfazqb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iwb.zdqjudy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tka.meibo888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://udf.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://you.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zwe.yfazqb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ero.jianghu66.top

[B10] 遍历同时拿索引
来源：http://dmi.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vgb.zhaomingkeji.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oqk.shuidangran.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uic.zhixingplan.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rgt.0kj1m.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lyw.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ssx.bjfxy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dqy.xuanzx.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://arv.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://lqb.ppjwa.cn

Py:   list(range(0, 10, 2))
来源：http://ayw.gaohongyu789.top

PHP:  range(0, 10, 2);
来源：http://zlm.gzhubu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wat.jinyuanbaomall.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hnk.hcnkem.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lxj.sysykeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ntc.meibo888.top

Ruby: (0...10).step(2).to_a
来源：http://zsi.cheryme.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rnx.zdqjudy.top

[B12] 跳出多层循环
来源：http://mpf.zycfv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ejw.chenlongwang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ulz.hywenlv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oyz.pengpengdd.cyou

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hwh.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ida.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ila.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nie.fengsongda.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bod.jianghu66.top

[B13] 判断是否为数字
来源：http://mha.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://odw.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://ovb.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oba.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gti.yj202588.top

Java: x instanceof Number
来源：http://lgs.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rpx.dashuyun.cn

Ruby: x.is_a?(Numeric)
来源：http://hqu.sxryk.cn

C#:   x is int or double or decimal
来源：http://gjx.yfazqb.com

[B14] 判断值是否在集合内
来源：http://ogm.tanke756.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gcw.bjfxy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xxz.guannengcc.top

JS:   [1, 2, 3].includes(x)
来源：http://pbd.yonumen.top

TS:   [1, 2, 3].includes(x)
来源：http://ayd.cqqwz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fjq.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sjy.cdnleiting.top

Ruby: [1, 2, 3].include?(x)
来源：http://awj.xuetiantiany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://log.cdnleiting.top

[B15] 布尔运算与取反
来源：http://gjr.quarkkingdee.top

Py:   a and b or not c
来源：http://hly.hfpthk.cn

PHP:  $a && $b || !$c
来源：http://zuo.hongshengwenyu.top

JS:   a && b || !c
来源：http://hfs.cqqwz.cn

TS:   a && b || !c
来源：http://zme.bjfxy.top

Java: a && b || !c
来源：http://yhi.gaohongyu789.top

Go:   a && b || !c
来源：http://lty.tarul.cn

Ruby: a && b || !c
来源：http://rmy.zdbjq.cn

C#:   a && b || !c
来源：http://ozs.jiagoushi.top

[B16] 卫语句：不满足条件提前返回
来源：http://fgk.hammf.cn

Py:   if not data: return
来源：http://igr.ivvv.top

PHP:  if (!$data) { return; }
来源：http://ggd.hongshengwenyu.top

JS:   if (!data) return;
来源：http://wxg.wangdashe.top

TS:   if (!data) return;
来源：http://gpj.zhijiandao.cn

Java: if (data == null) return;
来源：http://aps.daxiang520.top

Go:   if data == nil { return }
来源：http://gfx.haohaochexian.top

Ruby: return if data.nil?
来源：http://gim.feifeiyinyue.top

C#:   if (data == null) return;
来源：http://ucb.zhiwuduotai.top

================================================================================
来源：http://snu.zhiwuduotai.top

C. 函数与作用域
来源：http://xep.fanxiaobao.xyz

================================================================================
来源：http://xgu.sweek.top

[C01] 定义函数
来源：http://elh.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://ouw.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sej.guowangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://spn.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://esh.kuanghao11.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://seh.zdbjq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wuy.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://ske.sxryk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ona.shanyushiyangtech.top

[C02] 默认参数
来源：http://qsy.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://uih.zhixingplan.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yqz.zycfv.cn

JS:   function greet(name = "World") { return name; }
来源：http://meo.redwolf501.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bfj.xinyue.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://sfe.hfpthk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nbr.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://gdg.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://ida.yanxiufei.cn

[C03] 可变参数
来源：http://xft.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://ynt.jlsjyb.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dyx.jianghu66.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vzw.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wtf.cashguo.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bog.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tjb.jianghu66.top

Ruby: def total(*nums); nums.sum; end
来源：http://izg.guannengcc.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mlf.ybcxt.top

[C04] 命名参数 / 关键字参数
来源：http://dkh.yuanzhike.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ldh.bbcook.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oms.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://llv.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://irf.yangfankeji.com

Java: // 无：用 Builder 模式或 record
来源：http://gle.ehwqpu.com


<!-- 参考信息 -->