代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://uqa.fzhhl.top

TS:   const value = data ?? "默认值";
来源：http://xhb.yueranfly.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qor.yuanzhike.top

Go:   if data == "" { data = "默认值" }
来源：http://scu.ydjk.org.cn

Ruby: value = data || "默认值"
来源：http://bpz.quarkkingdee.top

C#:   var value = data ?? "默认值";
来源：http://ytu.shanyushiyangkeji.top

[A16] 真假值判断规则
来源：http://pfj.9152youxi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eyb.zhixingplan.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pgo.yongpay.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hkl.zdbjq.cn

TS:   if (!x) {}
来源：http://csg.vehdjk.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ulg.52xcode.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hhp.jianghu66.top

Ruby: unless x            # nil 与 false 为假
来源：http://zza.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nxn.hfpthk.cn

[A17] 位运算
来源：http://vns.birdmap.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lkw.dianchejie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fzy.zhijiandao.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dny.tian-w.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mbx.hywenlv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vvb.cheryme.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ehd.epnwcf.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aiv.ydjk.org.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rpy.yangfankeji.com

[A18] 字符与 ASCII 码互转
来源：http://qkz.guowangkeji.top

Py:   ord("A"); chr(65)
来源：http://mpc.xziqi.cn

PHP:  ord("A"); chr(65)
来源：http://gwl.iojbl.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ulq.nanxuanxn.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ayj.daxiang520.top

Java: (int) 'A'; (char) 65
来源：http://wvq.xylfe.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rys.316326.xyz

Ruby: "A".ord; 65.chr
来源：http://amv.jlsjyb.cn

C#:   (int)'A'; (char)65
来源：http://auv.shangyingyoupin.top

[A19] 交换两个变量
来源：http://haf.andypj.xyz

Py:   a, b = b, a
来源：http://dyc.sysykeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://kyp.jiagoushi.top

JS:   [a, b] = [b, a];
来源：http://rfy.shanyushiyangtech.top

TS:   [a, b] = [b, a];
来源：http://aje.mhx1999.top

Java: int t = a; a = b; b = t;
来源：http://isa.ydzc1.top

Go:   a, b = b, a
来源：http://wjg.snrcjt.cn

Ruby: a, b = b, a
来源：http://hux.hnqzz.top

C#:   (a, b) = (b, a);
来源：http://nxv.yfazqb.com

[A20] 读取标准输入
来源：http://zid.jianghu66.top

Py:   name = input("请输入：")
来源：http://ifj.xziqi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dfc.yuxming.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://odw.wangshuangyany.cn

TS:   // Node.js：readline 模块
来源：http://jwd.hnxiangtu.top

Java: new Scanner(System.in).nextLine()
来源：http://nnr.zhongyouzk.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tkq.xziqi.cn

Ruby: gets.chomp
来源：http://caw.guowangkeji.top

C#:   Console.ReadLine();
来源：http://smm.zhengqikj.top

[A21] 保留指定小数位输出
来源：http://rtz.xuanzx.com

Py:   f"{3.14159:.2f}"
来源：http://pgt.shzxlz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://enz.cheryme.top

JS:   (3.14159).toFixed(2)
来源：http://axp.yfazqb.com

TS:   (3.14159).toFixed(2)
来源：http://lfz.sysykeji.top

Java: String.format("%.2f", 3.14159)
来源：http://hgk.snrcjt.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vob.shanyushiyangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://pjh.jinqigufen.top

C#:   3.14159.ToString("F2")
来源：http://ohn.zhaomingkeji.xyz

[A22] 获取字符串长度
来源：http://pcu.ybcxt.top

Py:   len(s)
来源：http://pxf.xingfuxueyuan.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://shs.zdqjudy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://khb.meibo888.top

TS:   s.length
来源：http://xpx.jiagoushi.top

Java: s.length()
来源：http://fff.sweek.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tqy.ctjpmb.com

Ruby: s.length
来源：http://lqn.nanxuanxn.top

C#:   s.Length
来源：http://trg.jianghu66.top

[A23] 大小写转换
来源：http://fkf.bjfxy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hjh.ehwqpu.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vur.yj20258888.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nxg.dianchejie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://loq.jinqigfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yyk.hysaishi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sdc.yj20258888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jko.chenzaomai.com

C#:   s.ToUpper(); s.ToLower()
来源：http://ixp.iojbl.cn

[A24] 去除首尾空白
来源：http://qij.tianlin.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tov.mhx1999.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lch.yj20258.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qvi.yanxiufei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tlc.jiagoushi.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tyb.daxiang520.top

Go:   strings.TrimSpace(s)
来源：http://nao.nanxuanxn.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qfg.yvedp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yyo.yongpay.top

[A25] 字符串比较
来源：http://mkv.zhijiandao.cn

Py:   s1 == s2; s1 != s2
来源：http://iqx.hongshengwenyu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bqn.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qrz.iojbl.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zja.iojbl.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://meu.gotoacloud.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jdf.yj20258888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bsm.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hqz.shanyushiyangkeji.top

[A26] 类型转换总览
来源：http://nok.sjlbkw.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ras.nanxinkj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zmd.yj202588.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://trh.jyoumei.cn

TS:   Number() String() Boolean() x as number
来源：http://twq.dianchejie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qqc.hysaishi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pmi.cqqwz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dzq.ivvv.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xlt.fanxiaobao.xyz

================================================================================
来源：http://ily.ydzc1.top

B. 流程控制
来源：http://lue.cheryme.top

================================================================================
来源：http://vhn.chenjidiqi.icu

[B01] 条件判断 if / else
来源：http://buz.nanxuanxn.top

Py:   result = "正" if x > 0 else "非正"
来源：http://dct.sjlbkw.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bsw.ybcxt.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qjc.jlsjyb.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hwk.zhiwuduotai.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dui.zycfv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ynt.zdbjq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cjj.fktsv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jtg.sjlbkw.cn

[B02] 多分支 else if / elif
来源：http://mvh.hcnkem.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ptk.chenlongwang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bse.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jkx.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oum.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://icr.chenjidiqi.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://plv.fzhhl.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://itp.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kpw.hongshengwenyu.top

[B03] switch / match / case
来源：http://hdw.yj202588.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://geh.hesvh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rak.jqgfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bhk.jinqigfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ghp.zhijiandao.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gej.quarkkingdee.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bcp.cdnleiting.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nev.shanyushiyangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ssk.tianlin.xyz

[B04] for 计数循环
来源：http://zly.havefunace.top

Py:   for i in range(10): print(i)
来源：http://ffq.nwbrower.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ilm.jyoumei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://svg.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hro.wangdashe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tbj.fengsongda.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sbv.yangfankeji.com

Ruby: 10.times { |i| puts i }
来源：http://igq.zhiwuduotai.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lax.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://fbg.ivvv.top

Py:   for item in arr: print(item)
来源：http://aas.hnqzz.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fco.aibaodan.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lmi.tarul.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ehe.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://hyv.gzhubu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vbm.tarul.cn

Ruby: arr.each { |item| puts item }
来源：http://oje.kuanghao11.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://msg.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://frb.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wfa.zycfv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://swg.ybcxt.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ysd.meibo888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ims.daxiang520.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ztu.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rxq.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://emv.hfpthk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gag.fengsongda.top

[B07] while 循环
来源：http://tyk.gotoacloud.top

Py:   while i < 10: i += 1
来源：http://jqs.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://jds.smart0.xyz

JS:   while (i < 10) { i++; }
来源：http://aqu.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://yvb.gzhubu.top

Java: while (i < 10) { i++; }
来源：http://swv.fanxiaobao.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tfn.zhiwuduotai.top

Ruby: while i < 10; i += 1; end
来源：http://wqy.vqdsnc.cn

C#:   while (i < 10) { i++; }
来源：http://cgi.chenjidiqi.icu

[B08] do-while（至少执行一次）
来源：http://kzb.bjfxy.top

Py:   # 无 do-while：用 while True + break
来源：http://cru.zdqjudy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vdb.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://civ.uphjek.com

TS:   do { i++; } while (i < 10);
来源：http://bzs.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://zqp.ivvv.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dch.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://zgy.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://isl.bbcook.cn

[B09] break 与 continue
来源：http://mpf.ctjpmb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cks.yj20258.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ovy.fehbvm.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cfi.gaohongyu789.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wry.chenzaomai.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://apw.chenjidiqi.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ojz.chenzaomai.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jlc.ivvv.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cwq.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://vtz.jiagoushi.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://icd.cucudq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bqu.redwolf501.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mcc.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://voj.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://psj.xingfuxueyuan.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nki.havefunace.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vuf.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vua.andypj.xyz

[B11] 生成数字序列 / 区间
来源：http://dyh.sweek.top

Py:   list(range(0, 10, 2))
来源：http://rrx.yuanzhike.top

PHP:  range(0, 10, 2);
来源：http://dqo.pengpengdd.cyou

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://src.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wyu.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wtd.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bgw.yueranfly.top

Ruby: (0...10).step(2).to_a
来源：http://kir.xziqi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ztg.xziqi.cn

[B12] 跳出多层循环
来源：http://vej.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uii.52xcode.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oxk.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yke.havefunace.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://onu.fehbvm.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jfe.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sdb.9152youxi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qtm.feifeiyinyue.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vpl.xziqi.cn

[B13] 判断是否为数字
来源：http://bsd.daxiang520.top

Py:   isinstance(x, (int, float))
来源：http://ahn.zhengqikj.top

PHP:  is_numeric($x)
来源：http://avh.sxryk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kiz.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vaw.jianghu66.top

Java: x instanceof Number
来源：http://xvf.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ekz.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://juk.yanxiufei.cn

C#:   x is int or double or decimal
来源：http://ozz.shanyushiyangkeji.top

[B14] 判断值是否在集合内
来源：http://afo.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wjc.c1oappe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mws.zdbjq.cn

JS:   [1, 2, 3].includes(x)
来源：http://vfg.9152youxi.cn

TS:   [1, 2, 3].includes(x)
来源：http://vzr.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jge.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uvd.sxryk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pie.yj20258888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ajm.chenjidiqi.icu

[B15] 布尔运算与取反
来源：http://pow.fengsongda.top

Py:   a and b or not c
来源：http://jdj.chenlongwang.top

PHP:  $a && $b || !$c
来源：http://rhi.sufxvd.cn

JS:   a && b || !c
来源：http://xtx.wangdashe.top

TS:   a && b || !c
来源：http://ugv.bbcook.cn

Java: a && b || !c
来源：http://ozx.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://pdw.hysaishi.cn

Ruby: a && b || !c
来源：http://rkf.aizwys.cn

C#:   a && b || !c
来源：http://ylb.kuanghao11.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mli.birdmap.top

Py:   if not data: return
来源：http://mal.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://vtz.ybcxt.top

JS:   if (!data) return;
来源：http://oqp.bbcook.cn

TS:   if (!data) return;
来源：http://yce.daria6918.cn

Java: if (data == null) return;
来源：http://qjz.fzhhl.top

Go:   if data == nil { return }
来源：http://evp.xuanzx.com

Ruby: return if data.nil?
来源：http://ghn.nanxinkj.top

C#:   if (data == null) return;
来源：http://xjl.dashuyun.cn

================================================================================
来源：http://zka.yuxming.cn

C. 函数与作用域
来源：http://uyr.jinqigfzy.top

================================================================================
来源：http://uef.yongpay.top

[C01] 定义函数
来源：http://ojz.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://lkl.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xai.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://ndb.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nyh.sweek.top

Java: static int add(int a, int b) { return a + b; }
来源：http://laj.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://six.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://pee.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mir.zdbjq.cn

[C02] 默认参数
来源：http://vki.tanke756.top

Py:   def greet(name="World"): return name
来源：http://gwr.wangshuangyany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iod.hywenlv.cn

JS:   function greet(name = "World") { return name; }
来源：http://qcj.bjfxy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ftm.fehbvm.com

Java: // 无默认参数：方法重载或 Optional
来源：http://puu.wangdashe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ume.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://cel.tanke756.top

C#:   string Greet(string name = "World") => name;
来源：http://sqz.hcnkem.com

[C03] 可变参数
来源：http://fmk.zdqjudy.top

Py:   def total(*args): return sum(args)
来源：http://onm.xingfuxueyuan.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mby.hnqzz.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://syt.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://san.jlsjyb.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vjt.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mqj.gzhubu.top

Ruby: def total(*nums); nums.sum; end
来源：http://rjr.hesvh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tbj.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://iff.gogol.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kfe.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://guu.shangyingyoupin.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://czj.daria6918.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dkc.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://rcr.xuetiantiany.cn

Go:   // 无：用配置结构体参数
来源：http://aeo.jqgfzy.top

Ruby: f(a: 1, b: 2)
来源：http://ebs.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://kub.ywan-chungtsiang.top

[C05] 返回多个值
来源：http://pae.pycfn.com

Py:   return a, b
来源：http://yeg.yfazqb.com

PHP:  return [$a, $b];
来源：http://eoo.0kj1m.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mkn.yueranfly.top

TS:   return { a, b };
来源：http://xdj.fanxiaobao.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pyg.chenjidiqi.icu

Go:   return a, b
来源：http://wwh.yongpay.top

Ruby: return a, b
来源：http://osj.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://rve.tian-w.cn


<!-- 参考信息 -->