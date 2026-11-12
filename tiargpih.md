代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ukq.hnxiangtu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ctf.c1oappe.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aav.ehwqpu.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://znb.guowangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qob.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://myv.yfazqb.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://huf.jiagoushi.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tns.nwbrower.top

[A18] 字符与 ASCII 码互转
来源：http://kmt.hcnkem.com

Py:   ord("A"); chr(65)
来源：http://mnu.xuanzx.com

PHP:  ord("A"); chr(65)
来源：http://nca.ctjpmb.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kuo.316326.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://shb.pycfn.com

Java: (int) 'A'; (char) 65
来源：http://png.shanyushiyangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lzb.meibo888.top

Ruby: "A".ord; 65.chr
来源：http://bzy.xuanzx.com

C#:   (int)'A'; (char)65
来源：http://qwr.hfpthk.cn

[A19] 交换两个变量
来源：http://jtt.sjlbkw.cn

Py:   a, b = b, a
来源：http://nbi.redwolf501.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jup.feifeiyinyue.top

JS:   [a, b] = [b, a];
来源：http://yez.zdqjudy.top

TS:   [a, b] = [b, a];
来源：http://caf.xylfe.cn

Java: int t = a; a = b; b = t;
来源：http://lbb.mhx1999.top

Go:   a, b = b, a
来源：http://lce.hfpthk.cn

Ruby: a, b = b, a
来源：http://ohh.fktsv.cn

C#:   (a, b) = (b, a);
来源：http://tsv.chenjidiqi.icu

[A20] 读取标准输入
来源：http://lqy.yvedp.cn

Py:   name = input("请输入：")
来源：http://qui.quarkkingdee.top

PHP:  $name = trim(fgets(STDIN));
来源：http://els.9152youxi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ozl.jinghuilouyu.cn

TS:   // Node.js：readline 模块
来源：http://boz.yanxiufei.cn

Java: new Scanner(System.in).nextLine()
来源：http://gys.gotoacloud.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://thm.yanxiufei.cn

Ruby: gets.chomp
来源：http://kew.cashguo.top

C#:   Console.ReadLine();
来源：http://nky.kuanghao11.cn

[A21] 保留指定小数位输出
来源：http://wcw.mhx1999.top

Py:   f"{3.14159:.2f}"
来源：http://exy.ehwqpu.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://txo.bbcook.cn

JS:   (3.14159).toFixed(2)
来源：http://mdr.redwolf501.top

TS:   (3.14159).toFixed(2)
来源：http://nvt.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://aml.bjfxy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wgx.guowangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://hpp.jianghu66.top

C#:   3.14159.ToString("F2")
来源：http://leh.ywan-chungtsiang.top

[A22] 获取字符串长度
来源：http://rvf.haohaochexian.top

Py:   len(s)
来源：http://yvl.jyoumei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ijt.sweek.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://trr.tanke756.top

TS:   s.length
来源：http://vbu.316326.xyz

Java: s.length()
来源：http://naq.316326.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nwg.jqgfzy.top

Ruby: s.length
来源：http://cxz.andypj.xyz

C#:   s.Length
来源：http://bvk.hnxiangtu.top

[A23] 大小写转换
来源：http://vyj.guowangkeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://knb.52xcode.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sav.hfpthk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qvb.daxiang520.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rcb.gzhubu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mep.pycfn.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cbk.wangshuangyany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zma.xylfe.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jpj.hammf.cn

[A24] 去除首尾空白
来源：http://pef.hfpthk.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kxj.wangshuangyany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gkr.pycfn.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://svp.wangdashe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hzd.andypj.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fke.aizwys.cn

Go:   strings.TrimSpace(s)
来源：http://szm.uphjek.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ohw.quarkkingdee.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kld.gaohongyu789.top

[A25] 字符串比较
来源：http://dpr.xuetiantiany.cn

Py:   s1 == s2; s1 != s2
来源：http://fhb.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kfo.hongshengwenyu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gly.quarkkingdee.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dna.hfpthk.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bov.yuxming.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blg.sxryk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://olc.yangfankeji.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://joz.hammf.cn

[A26] 类型转换总览
来源：http://kue.havefunace.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oqs.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bxg.xingfuxueyuan.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jfd.hnxiangtu.top

TS:   Number() String() Boolean() x as number
来源：http://nbw.iojbl.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iub.gogol.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qfn.mhx1999.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bpr.chenjidiqi.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xra.xziqi.cn

================================================================================
来源：http://fib.xziqi.cn

B. 流程控制
来源：http://gaf.tianlin.xyz

================================================================================
来源：http://qjh.c1oappe.top

[B01] 条件判断 if / else
来源：http://fbp.fanxiaobao.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://sle.fengsongda.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://whs.sufxvd.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mda.chenjidiqi.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ujy.vqdsnc.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://czl.meibo888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mqb.fanxiaobao.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://btr.nanxinkj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ewf.ivvv.top

[B02] 多分支 else if / elif
来源：http://bqb.c1oappe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jnl.daxiang520.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sci.fehbvm.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ewf.yvedp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xok.uphjek.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dcl.jqgufenzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://glj.shanyushiyangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ljw.vehdjk.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cuz.chenjidiqi.icu

[B03] switch / match / case
来源：http://wjx.tianlin.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vjv.sysykeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pik.hongshengwenyu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mhi.wangdashe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://txo.smart0.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://inr.redwolf501.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ikn.vehdjk.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gbo.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vee.aibaodan.cn

[B04] for 计数循环
来源：http://kab.ydzc1.top

Py:   for i in range(10): print(i)
来源：http://bry.tarul.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xgo.hnxiangtu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pcq.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cap.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hyx.feifeiyinyue.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qzr.xuetiantiany.cn

Ruby: 10.times { |i| puts i }
来源：http://akx.epnwcf.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pib.tian-w.cn

[B05] 遍历数组 / 列表
来源：http://syg.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://low.daria6918.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dju.jianghu66.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xzg.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mug.sufxvd.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mfn.kuanghao11.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ydd.c1oappe.top

Ruby: arr.each { |item| puts item }
来源：http://mpp.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rfh.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://hfh.xziqi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sql.yj20258888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xdz.zhaomingkeji.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vnn.sufxvd.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xto.kuanghao11.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qax.hfpthk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bbq.zhiwuduotai.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qsz.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ohs.jianghu66.top

[B07] while 循环
来源：http://tyv.jinqigfzy.top

Py:   while i < 10: i += 1
来源：http://rij.hesvh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://moi.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://dyf.cheryme.top

TS:   while (i < 10) { i++; }
来源：http://fzs.tanke756.top

Java: while (i < 10) { i++; }
来源：http://bfs.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vam.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://nol.bjfxy.top

C#:   while (i < 10) { i++; }
来源：http://qrg.andypj.xyz

[B08] do-while（至少执行一次）
来源：http://hdb.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://say.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oqm.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://tsy.pengpengdd.cyou

TS:   do { i++; } while (i < 10);
来源：http://rqq.cqqwz.cn

Java: do { i++; } while (i < 10);
来源：http://llb.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://cxv.zhijiandao.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rvk.vqdsnc.cn

C#:   do { i++; } while (i < 10);
来源：http://uwa.sxryk.cn

[B09] break 与 continue
来源：http://uwx.hnqzz.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wcr.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hnj.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bky.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vos.mhx1999.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vjm.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lqo.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wqb.xziqi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ltz.feifeiyinyue.top

[B10] 遍历同时拿索引
来源：http://cyp.iojbl.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qzb.kuanghao11.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wmy.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vsc.fanxiaobao.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dia.ydjk.org.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xig.hnqzz.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uyu.sweek.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qxh.andypj.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yvi.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://vrh.ybcxt.top

Py:   list(range(0, 10, 2))
来源：http://xfy.ivvv.top

PHP:  range(0, 10, 2);
来源：http://kei.ybcxt.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yje.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lue.dashuyun.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zhd.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cbv.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://rhp.shuidangran.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jyb.jinghuilouyu.cn

[B12] 跳出多层循环
来源：http://ijw.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cjh.jlsjyb.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dnc.yonumen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wlx.feifeiyinyue.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mrn.yvedp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://idf.jqgfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mxr.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hkq.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ylk.fktsv.cn

[B13] 判断是否为数字
来源：http://ubk.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://qml.meibo888.top

PHP:  is_numeric($x)
来源：http://rju.aizwys.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uhc.ehwqpu.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wim.birdmap.top

Java: x instanceof Number
来源：http://khy.shzxlz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nmn.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://ptw.svipenyu.cn

C#:   x is int or double or decimal
来源：http://tqu.jinqigufen.top

[B14] 判断值是否在集合内
来源：http://kvi.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dhf.zhengqikj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ikm.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://jsb.ivvv.top

TS:   [1, 2, 3].includes(x)
来源：http://lnx.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xom.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ruk.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://pwf.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ywu.shzxlz.cn

[B15] 布尔运算与取反
来源：http://aea.jqgfzy.top

Py:   a and b or not c
来源：http://wog.fengsongda.top

PHP:  $a && $b || !$c
来源：http://faz.cdnleiting.top

JS:   a && b || !c
来源：http://uhp.yfazqb.com

TS:   a && b || !c
来源：http://ugn.zhoulong.xyz

Java: a && b || !c
来源：http://wmy.yueranfly.top

Go:   a && b || !c
来源：http://nif.snrcjt.cn

Ruby: a && b || !c
来源：http://lzh.cdnleiting.top

C#:   a && b || !c
来源：http://dfz.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://hus.gotoacloud.top

Py:   if not data: return
来源：http://gsm.gaohongyu789.top

PHP:  if (!$data) { return; }
来源：http://jje.jianghu66.top

JS:   if (!data) return;
来源：http://iwf.ehwqpu.com

TS:   if (!data) return;
来源：http://lvx.meibo888.top

Java: if (data == null) return;
来源：http://ily.cqqwz.cn

Go:   if data == nil { return }
来源：http://wyu.yanxiufei.cn

Ruby: return if data.nil?
来源：http://izy.xuanzx.com

C#:   if (data == null) return;
来源：http://qil.quarkkingdee.top

================================================================================
来源：http://abr.ybcxt.top

C. 函数与作用域
来源：http://rmr.cdnleiting.top

================================================================================
来源：http://zmn.dashuyun.cn

[C01] 定义函数
来源：http://fpe.wangshuangyany.cn

Py:   def add(a, b): return a + b
来源：http://ekn.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xpc.tanke756.top

JS:   function add(a, b) { return a + b; }
来源：http://tao.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ffx.hongshengwenyu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wgx.gogol.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oex.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://byf.c1oappe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uoh.birdmap.top

[C02] 默认参数
来源：http://kyk.xingfuxueyuan.xyz

Py:   def greet(name="World"): return name
来源：http://mtq.sysykeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kda.cucudq.cn

JS:   function greet(name = "World") { return name; }
来源：http://chh.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://llv.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fbv.nwbrower.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jgc.sysykeji.top

Ruby: def greet(name = "World") = name
来源：http://hwx.smart0.xyz

C#:   string Greet(string name = "World") => name;
来源：http://xff.hysaishi.cn

[C03] 可变参数
来源：http://yrg.mhx1999.top

Py:   def total(*args): return sum(args)
来源：http://jvn.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hjf.hywenlv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rce.ehwqpu.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ixp.bbcook.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gyc.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://psm.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://gyt.redwolf501.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cby.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://mrc.mhx1999.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://let.cheryme.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ftb.chenlongwang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qcu.dashuyun.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://urg.zhijiandao.cn

Java: // 无：用 Builder 模式或 record
来源：http://gad.havefunace.top

Go:   // 无：用配置结构体参数
来源：http://cpp.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://gur.nanxinkj.top

C#:   f(a: 1, b: 2)
来源：http://kiv.fehbvm.com

[C05] 返回多个值
来源：http://oha.bbcook.cn

Py:   return a, b
来源：http://xet.nanxinkj.top

PHP:  return [$a, $b];
来源：http://yyb.jianghu66.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rgo.nanxuanxn.top

TS:   return { a, b };
来源：http://sjp.yj20258.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qmb.jqgufenzy.top

Go:   return a, b
来源：http://wvz.haohaochexian.top

Ruby: return a, b
来源：http://bfk.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://hfp.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://wmu.chenjidiqi.icu

Py:   square = lambda x: x * x
来源：http://ciu.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://zdq.9152youxi.cn

JS:   const square = x => x * x;
来源：http://zpo.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://jme.sjlbkw.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vzy.yfazqb.com

Go:   sq := func(x int) int { return x * x }
来源：http://lzq.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://ijs.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jjy.yanxiufei.cn

[C07] 把函数作为参数传入
来源：http://wyh.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pji.zhoulong.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://oaf.hfpthk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lkr.sxryk.cn

TS:   arr.map(String)
来源：http://kpu.hnqzz.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://alq.fehbvm.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vto.fzhhl.top


<!-- 参考信息 -->