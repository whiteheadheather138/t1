代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://mdh.ehwqpu.com

[A15] 空值判断与默认值
来源：http://ojx.yvedp.cn

Py:   value = data or "默认值"
来源：http://stf.9152youxi.cn

PHP:  $value = $data ?? "默认值";
来源：http://qon.yj20258.top

JS:   const value = data ?? "默认值";
来源：http://ekt.dashuyun.cn

TS:   const value = data ?? "默认值";
来源：http://yki.haohaochexian.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bqv.wangshuangyany.cn

Go:   if data == "" { data = "默认值" }
来源：http://ony.meibo888.top

Ruby: value = data || "默认值"
来源：http://jxd.zdqjudy.top

C#:   var value = data ?? "默认值";
来源：http://zky.cucudq.cn

[A16] 真假值判断规则
来源：http://rjt.nanxuanxn.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cfl.aibaodan.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nyi.ybcxt.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qav.yonumen.top

TS:   if (!x) {}
来源：http://zaq.c1oappe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yrj.shangyingyoupin.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ajb.ivvv.top

Ruby: unless x            # nil 与 false 为假
来源：http://nwa.fengsongda.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nlc.dianchejie.cn

[A17] 位运算
来源：http://vwz.52xcode.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cda.yj20258.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mvh.yuxming.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tbv.yuxming.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://omx.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tve.xingfuxueyuan.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://une.sjlbkw.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vhq.yj202588.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://foh.dianchejie.cn

[A18] 字符与 ASCII 码互转
来源：http://vvt.yonumen.top

Py:   ord("A"); chr(65)
来源：http://lpd.kuanghao11.cn

PHP:  ord("A"); chr(65)
来源：http://slt.zhixingplan.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xrg.guannengcc.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qnt.pycfn.com

Java: (int) 'A'; (char) 65
来源：http://yoa.zhijiandao.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://apb.xuetiantiany.cn

Ruby: "A".ord; 65.chr
来源：http://aix.daxiang520.top

C#:   (int)'A'; (char)65
来源：http://qgd.gogol.net.cn

[A19] 交换两个变量
来源：http://aju.yuanzhike.top

Py:   a, b = b, a
来源：http://lbz.316326.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://yaa.yanxiufei.cn

JS:   [a, b] = [b, a];
来源：http://gsk.aizwys.cn

TS:   [a, b] = [b, a];
来源：http://juv.nanxinkj.top

Java: int t = a; a = b; b = t;
来源：http://lyu.xingfuxueyuan.xyz

Go:   a, b = b, a
来源：http://rhd.bjfxy.top

Ruby: a, b = b, a
来源：http://qqo.0kj1m.cn

C#:   (a, b) = (b, a);
来源：http://tbd.gogol.net.cn

[A20] 读取标准输入
来源：http://zcg.dashuyun.cn

Py:   name = input("请输入：")
来源：http://qtd.shanyushiyangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://oos.ydjk.org.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eef.iojbl.cn

TS:   // Node.js：readline 模块
来源：http://zby.bbcook.cn

Java: new Scanner(System.in).nextLine()
来源：http://hdi.yangfankeji.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xlv.sweek.top

Ruby: gets.chomp
来源：http://oux.sysykeji.top

C#:   Console.ReadLine();
来源：http://xuw.smart0.xyz

[A21] 保留指定小数位输出
来源：http://cpw.yonumen.top

Py:   f"{3.14159:.2f}"
来源：http://tqf.zhijiandao.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rrn.ydjk.org.cn

JS:   (3.14159).toFixed(2)
来源：http://alk.cdnleiting.top

TS:   (3.14159).toFixed(2)
来源：http://nxz.xylfe.cn

Java: String.format("%.2f", 3.14159)
来源：http://yze.yonumen.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://smw.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://jmp.fzhhl.top

C#:   3.14159.ToString("F2")
来源：http://jha.aizwys.cn

[A22] 获取字符串长度
来源：http://lre.cdnleiting.top

Py:   len(s)
来源：http://hql.tanke756.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xlu.sweek.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gbw.sweek.top

TS:   s.length
来源：http://ymr.0kj1m.cn

Java: s.length()
来源：http://zcr.guowangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tka.tanke756.top

Ruby: s.length
来源：http://bxz.xingfuxueyuan.xyz

C#:   s.Length
来源：http://chu.jlsjyb.cn

[A23] 大小写转换
来源：http://xcl.jqgfzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bqo.fanxiaobao.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pos.hcnkem.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gpo.hnqzz.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://byw.sufxvd.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://glb.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://twr.daria6918.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ust.xuetiantiany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hpj.bbcook.cn

[A24] 去除首尾空白
来源：http://uoi.chenjidiqi.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://who.pengpengdd.cyou

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ces.wangshuangyany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://you.yonumen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://brq.zhongyouzk.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://far.fktsv.cn

Go:   strings.TrimSpace(s)
来源：http://hsx.ydjk.org.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aue.sysykeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://psh.xingfuxueyuan.xyz

[A25] 字符串比较
来源：http://nss.hysaishi.cn

Py:   s1 == s2; s1 != s2
来源：http://aps.bbcook.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://slu.cdnleiting.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tnw.daxiang520.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jrg.hesvh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lrl.hesvh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://knt.ydjk.org.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ces.birdmap.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wtj.sufxvd.cn

[A26] 类型转换总览
来源：http://jho.tarul.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sjn.chenzaomai.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pda.ctjpmb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gyg.zhongyouzk.top

TS:   Number() String() Boolean() x as number
来源：http://ale.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tor.jiagoushi.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dio.yangfankeji.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://cmu.zycfv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ifp.hesvh.cn

================================================================================
来源：http://juc.guowangkeji.top

B. 流程控制
来源：http://ofa.jlsjyb.cn

================================================================================
来源：http://sqi.xylfe.cn

[B01] 条件判断 if / else
来源：http://qar.birdmap.top

Py:   result = "正" if x > 0 else "非正"
来源：http://glm.zdqjudy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vso.ybcxt.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lww.zhoulong.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fjw.yuxming.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uax.guannengcc.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://koj.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pza.guannengcc.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cvy.chenzaomai.com

[B02] 多分支 else if / elif
来源：http://pwn.tanke756.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://krt.jinghuilouyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mau.xinyue.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rmp.zhongyouzk.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ztn.zhixingplan.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bjv.haohaochexian.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lbp.meibo888.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uwm.dashuyun.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ecy.chenjidiqi.icu

[B03] switch / match / case
来源：http://vmw.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://abf.cqqwz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ker.yfazqb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wjk.meibo888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cfz.fktsv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lvm.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mna.zycfv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ajq.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://utk.havefunace.top

[B04] for 计数循环
来源：http://jzz.yj20258888.top

Py:   for i in range(10): print(i)
来源：http://rot.jinqigfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bnp.jlsjyb.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vsr.yj20258.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uqh.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lch.zdqjudy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rce.feifeiyinyue.top

Ruby: 10.times { |i| puts i }
来源：http://ilw.cheryme.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aqt.cashguo.top

[B05] 遍历数组 / 列表
来源：http://ply.nanxuanxn.top

Py:   for item in arr: print(item)
来源：http://pfy.jqgufenzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nbo.ctjpmb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://xel.yanxiufei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uqm.hongshengwenyu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jdg.shanyushiyangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bae.andypj.xyz

Ruby: arr.each { |item| puts item }
来源：http://bcn.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://erb.chenzaomai.com

[B06] 遍历字典 / 对象
来源：http://jms.gaohongyu789.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ybk.yj20258888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://quk.svipenyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mml.svipenyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eqd.hywenlv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hli.yfazqb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://trr.mhx1999.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pzx.fanxiaobao.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sis.ivvv.top

[B07] while 循环
来源：http://hwr.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://hjz.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://ogu.smart0.xyz

JS:   while (i < 10) { i++; }
来源：http://ali.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://fhl.bjfxy.top

Java: while (i < 10) { i++; }
来源：http://xno.fengsongda.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ckf.xuanzx.com

Ruby: while i < 10; i += 1; end
来源：http://qyw.gogol.net.cn

C#:   while (i < 10) { i++; }
来源：http://oqx.ydjk.org.cn

[B08] do-while（至少执行一次）
来源：http://gfu.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://sgi.cucudq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wfz.ydjk.org.cn

JS:   do { i++; } while (i < 10);
来源：http://yts.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://msb.hammf.cn

Java: do { i++; } while (i < 10);
来源：http://per.mhx1999.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lqb.cucudq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vmu.hfpthk.cn

C#:   do { i++; } while (i < 10);
来源：http://url.hnxiangtu.top

[B09] break 与 continue
来源：http://cko.yj20258888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nfh.sweek.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://isn.cheryme.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yso.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://esd.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ryu.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ydn.yfazqb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zdu.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cqh.zhongyouzk.top

[B10] 遍历同时拿索引
来源：http://xsi.zhixingplan.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://erf.hysaishi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bzp.svipenyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ewf.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nhz.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://igt.redwolf501.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iic.yuanzhike.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gol.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cpc.gogol.net.cn

[B11] 生成数字序列 / 区间
来源：http://pxn.hnqzz.top

Py:   list(range(0, 10, 2))
来源：http://cxb.cheryme.top

PHP:  range(0, 10, 2);
来源：http://nxq.52xcode.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://apz.nanxuanxn.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vky.dianchejie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jgh.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dww.zdbjq.cn

Ruby: (0...10).step(2).to_a
来源：http://wnm.chenzaomai.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://psd.xinyue.icu

[B12] 跳出多层循环
来源：http://axl.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ndh.pengpengdd.cyou

PHP:  # 无标签：用 goto 或函数返回
来源：http://mfn.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tly.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nmn.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fgu.jinqigfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wyy.9152youxi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nmw.yangfankeji.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dqm.yj20258888.top

[B13] 判断是否为数字
来源：http://kyf.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://cfd.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://erf.quarkkingdee.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://asf.fehbvm.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pnw.aibaodan.cn

Java: x instanceof Number
来源：http://xah.sjlbkw.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ebw.feifeiyinyue.top

Ruby: x.is_a?(Numeric)
来源：http://dsh.zhongyouzk.top

C#:   x is int or double or decimal
来源：http://xss.cheryme.top

[B14] 判断值是否在集合内
来源：http://zgj.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jws.zdbjq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zvx.jinqigfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://zco.xziqi.cn

TS:   [1, 2, 3].includes(x)
来源：http://hlb.gaohongyu789.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fjj.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xau.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qdr.daxiang520.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jrw.shzxlz.cn

[B15] 布尔运算与取反
来源：http://cct.jianghu66.top

Py:   a and b or not c
来源：http://wvu.pycfn.com

PHP:  $a && $b || !$c
来源：http://ccm.0kj1m.cn

JS:   a && b || !c
来源：http://pdy.vqdsnc.cn

TS:   a && b || !c
来源：http://fdg.jqgfzy.top

Java: a && b || !c
来源：http://tre.chenzaomai.com

Go:   a && b || !c
来源：http://owy.chenzaomai.com

Ruby: a && b || !c
来源：http://nub.svipenyu.cn

C#:   a && b || !c
来源：http://epe.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://smq.cqqwz.cn

Py:   if not data: return
来源：http://gsx.gzhubu.top

PHP:  if (!$data) { return; }
来源：http://crw.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://zee.nanxuanxn.top

TS:   if (!data) return;
来源：http://ssl.bjfxy.top

Java: if (data == null) return;
来源：http://uav.cheryme.top

Go:   if data == nil { return }
来源：http://xwq.jinqigfzy.top

Ruby: return if data.nil?
来源：http://ifx.yj20258888.top

C#:   if (data == null) return;
来源：http://ijx.iojbl.cn

================================================================================
来源：http://brj.jianghu66.top

C. 函数与作用域
来源：http://lss.zhijiandao.cn

================================================================================
来源：http://ibm.vqdsnc.cn

[C01] 定义函数
来源：http://ins.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://kkt.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hmg.xinyue.icu

JS:   function add(a, b) { return a + b; }
来源：http://ivb.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://udv.xziqi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gee.jinqigufen.top

Go:   func add(a, b int) int { return a + b }
来源：http://pio.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://zmz.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ryg.yuxming.cn

[C02] 默认参数
来源：http://lmx.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://knc.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fzw.aibaodan.cn

JS:   function greet(name = "World") { return name; }
来源：http://pix.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cto.ydzc1.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dsn.pycfn.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ydl.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://vvx.guannengcc.top

C#:   string Greet(string name = "World") => name;
来源：http://scu.zhiwuduotai.top

[C03] 可变参数
来源：http://igb.guannengcc.top

Py:   def total(*args): return sum(args)
来源：http://wfs.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qrt.chenjidiqi.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yjo.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ptc.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xjb.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rpr.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lkj.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://los.gzhubu.top

[C04] 命名参数 / 关键字参数
来源：http://dcp.xuetiantiany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jvb.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iws.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kxy.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gbr.wangshuangyany.cn

Java: // 无：用 Builder 模式或 record
来源：http://hnq.9152youxi.cn

Go:   // 无：用配置结构体参数
来源：http://szm.cdnleiting.top

Ruby: f(a: 1, b: 2)
来源：http://xpp.hammf.cn

C#:   f(a: 1, b: 2)
来源：http://rhq.xylfe.cn

[C05] 返回多个值
来源：http://ams.tarul.cn

Py:   return a, b
来源：http://bcg.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://wki.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qql.vqdsnc.cn

TS:   return { a, b };
来源：http://shx.andypj.xyz


<!-- 参考信息 -->