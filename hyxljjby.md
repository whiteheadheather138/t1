代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xht.jlsjyb.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sbk.sweek.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gcd.tianlin.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uqd.vehdjk.com

[A18] 字符与 ASCII 码互转
来源：http://zoq.wangshuangyany.cn

Py:   ord("A"); chr(65)
来源：http://eqj.pycfn.com

PHP:  ord("A"); chr(65)
来源：http://bfx.zdqjudy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xeu.chenjidiqi.icu

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ppo.9152youxi.cn

Java: (int) 'A'; (char) 65
来源：http://bbd.cqqwz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uvs.yongpay.top

Ruby: "A".ord; 65.chr
来源：http://khw.redwolf501.top

C#:   (int)'A'; (char)65
来源：http://cwz.ybcxt.top

[A19] 交换两个变量
来源：http://ryu.yj202588.top

Py:   a, b = b, a
来源：http://bou.aizwys.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fdk.gzhubu.top

JS:   [a, b] = [b, a];
来源：http://cfa.shuidangran.top

TS:   [a, b] = [b, a];
来源：http://rgg.gotoacloud.top

Java: int t = a; a = b; b = t;
来源：http://yox.bbcook.cn

Go:   a, b = b, a
来源：http://zyr.svipenyu.cn

Ruby: a, b = b, a
来源：http://cdu.aibaodan.cn

C#:   (a, b) = (b, a);
来源：http://irv.gotoacloud.top

[A20] 读取标准输入
来源：http://gyn.zycfv.cn

Py:   name = input("请输入：")
来源：http://qtd.hcnkem.com

PHP:  $name = trim(fgets(STDIN));
来源：http://ahf.haohaochexian.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fzx.fengsongda.top

TS:   // Node.js：readline 模块
来源：http://qkr.cashguo.top

Java: new Scanner(System.in).nextLine()
来源：http://zkf.dashuyun.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zwm.ppjwa.cn

Ruby: gets.chomp
来源：http://hqj.jqgfzy.top

C#:   Console.ReadLine();
来源：http://eqw.zhengqikj.top

[A21] 保留指定小数位输出
来源：http://zzd.nwbrower.top

Py:   f"{3.14159:.2f}"
来源：http://yix.0kj1m.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cnl.yfazqb.com

JS:   (3.14159).toFixed(2)
来源：http://bea.cashguo.top

TS:   (3.14159).toFixed(2)
来源：http://whn.c1oappe.top

Java: String.format("%.2f", 3.14159)
来源：http://zso.dashuyun.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hmz.316326.xyz

Ruby: format("%.2f", 3.14159)
来源：http://ncn.epnwcf.com

C#:   3.14159.ToString("F2")
来源：http://aes.zhijiandao.cn

[A22] 获取字符串长度
来源：http://fsk.zhongyouzk.top

Py:   len(s)
来源：http://yvq.guannengcc.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://opx.guannengcc.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://skv.yanxiufei.cn

TS:   s.length
来源：http://yiw.mhx1999.top

Java: s.length()
来源：http://gft.havefunace.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vxn.jqgufenzy.top

Ruby: s.length
来源：http://syx.yj202588.top

C#:   s.Length
来源：http://zvv.epnwcf.com

[A23] 大小写转换
来源：http://lzb.yanxiufei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dkd.fktsv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vre.yuxming.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ppn.andypj.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ydv.zhixingplan.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://khx.yj202588.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lpd.cqqwz.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mim.hfpthk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nno.zdqjudy.top

[A24] 去除首尾空白
来源：http://twk.fktsv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://phn.shangyingyoupin.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nax.jianghu66.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ruj.xylfe.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ygk.feifeiyinyue.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zvv.zhixingplan.top

Go:   strings.TrimSpace(s)
来源：http://cxe.sufxvd.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jqc.xziqi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yhx.wangshuangyany.cn

[A25] 字符串比较
来源：http://zaw.jlsjyb.cn

Py:   s1 == s2; s1 != s2
来源：http://nfv.yueranfly.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fxb.gaohongyu789.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mbk.meibo888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ilh.hywenlv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ltv.zhongyouzk.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://haq.nanxuanxn.top

Ruby: s1 == s2; s1 <=> s2
来源：http://onm.cheryme.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cvd.aizwys.cn

[A26] 类型转换总览
来源：http://xnt.zhoulong.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://brq.0kj1m.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tde.sjlbkw.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nln.quarkkingdee.top

TS:   Number() String() Boolean() x as number
来源：http://wmc.yonumen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qxq.hfpthk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kyq.mhx1999.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://whj.yuanzhike.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://eaj.shanyushiyangtech.top

================================================================================
来源：http://kia.zhengqikj.top

B. 流程控制
来源：http://wuf.fengsongda.top

================================================================================
来源：http://wjq.shuidangran.top

[B01] 条件判断 if / else
来源：http://bdq.ctjpmb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://umy.vehdjk.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sgu.jinqigufen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yuk.zdqjudy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://his.gotoacloud.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jbf.shangyingyoupin.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ctb.aibaodan.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bmm.cqqwz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://brc.meibo888.top

[B02] 多分支 else if / elif
来源：http://grm.uphjek.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gxk.jinyuanbaomall.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xtj.zhengqikj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jid.jyoumei.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lxx.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zhq.xuanzx.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ech.epnwcf.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uoj.shangyingyoupin.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gfh.hnqzz.top

[B03] switch / match / case
来源：http://mgu.dashuyun.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wrr.daxiang520.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kof.hfpthk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vbk.ivvv.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://och.xingfuxueyuan.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rln.chenzaomai.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fzy.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gap.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://unf.ydjk.org.cn

[B04] for 计数循环
来源：http://ctk.jinyuanbaomall.cn

Py:   for i in range(10): print(i)
来源：http://wef.smart0.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qlp.chenzaomai.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dvb.cashguo.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uzr.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tuw.andypj.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://les.sufxvd.cn

Ruby: 10.times { |i| puts i }
来源：http://evu.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yqe.haohaochexian.top

[B05] 遍历数组 / 列表
来源：http://igo.yj202588.top

Py:   for item in arr: print(item)
来源：http://abm.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kis.tanke756.top

JS:   for (const item of arr) { console.log(item); }
来源：http://brk.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tpb.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vuk.zdbjq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yyw.316326.xyz

Ruby: arr.each { |item| puts item }
来源：http://vog.haohaochexian.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xbc.sweek.top

[B06] 遍历字典 / 对象
来源：http://bid.fanxiaobao.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://ilw.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ses.xinyue.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pzb.zdqjudy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qlt.jinghuilouyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://coy.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cdf.ctjpmb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tet.iojbl.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qre.shanyushiyangtech.top

[B07] while 循环
来源：http://lfs.shanyushiyangkeji.top

Py:   while i < 10: i += 1
来源：http://qpb.0kj1m.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ofm.xingfuxueyuan.xyz

JS:   while (i < 10) { i++; }
来源：http://mlk.jinqigfzy.top

TS:   while (i < 10) { i++; }
来源：http://vly.hongshengwenyu.top

Java: while (i < 10) { i++; }
来源：http://dms.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vuu.chenlongwang.top

Ruby: while i < 10; i += 1; end
来源：http://uns.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://vkw.zhijiandao.cn

[B08] do-while（至少执行一次）
来源：http://tmt.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://cjd.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xvr.cucudq.cn

JS:   do { i++; } while (i < 10);
来源：http://fpb.shuidangran.top

TS:   do { i++; } while (i < 10);
来源：http://wul.wangshuangyany.cn

Java: do { i++; } while (i < 10);
来源：http://ekt.svipenyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://avj.xuetiantiany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oxh.hnqzz.top

C#:   do { i++; } while (i < 10);
来源：http://fkg.chenlongwang.top

[B09] break 与 continue
来源：http://ifs.shanyushiyangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://enk.cqqwz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ixe.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qts.gaohongyu789.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://abm.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://brl.zycfv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dnv.bbcook.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dgz.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jvq.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://rym.epnwcf.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://krh.redwolf501.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qdg.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mjc.yj20258888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qon.vehdjk.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jae.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://efj.tanke756.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://reh.jqgufenzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nxb.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://yaj.xinyue.icu

Py:   list(range(0, 10, 2))
来源：http://jih.cashguo.top

PHP:  range(0, 10, 2);
来源：http://joa.xuetiantiany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zed.yangfankeji.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bit.andypj.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jfy.nanxinkj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cqs.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://apq.jinghuilouyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gqk.hnqzz.top

[B12] 跳出多层循环
来源：http://ejb.yvedp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cro.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fum.zhiwuduotai.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mge.dashuyun.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sdz.svipenyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zad.52xcode.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yau.snrcjt.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nxu.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lzf.yj20258888.top

[B13] 判断是否为数字
来源：http://igs.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://rkk.cdnleiting.top

PHP:  is_numeric($x)
来源：http://kjg.zhijiandao.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mnf.ppjwa.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://usy.zhaomingkeji.xyz

Java: x instanceof Number
来源：http://quw.yj202588.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fqv.daria6918.cn

Ruby: x.is_a?(Numeric)
来源：http://rip.tarul.cn

C#:   x is int or double or decimal
来源：http://tax.tarul.cn

[B14] 判断值是否在集合内
来源：http://xhr.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ncv.smart0.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vky.jinghuilouyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://buw.cheryme.top

TS:   [1, 2, 3].includes(x)
来源：http://jgz.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vcj.aizwys.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ebd.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xwz.jinqigfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dkv.yj20258888.top

[B15] 布尔运算与取反
来源：http://dzq.0kj1m.cn

Py:   a and b or not c
来源：http://ctb.smart0.xyz

PHP:  $a && $b || !$c
来源：http://kog.chenzaomai.com

JS:   a && b || !c
来源：http://scp.jianghu66.top

TS:   a && b || !c
来源：http://civ.sjlbkw.cn

Java: a && b || !c
来源：http://yye.xylfe.cn

Go:   a && b || !c
来源：http://ndh.snrcjt.cn

Ruby: a && b || !c
来源：http://ejv.dianchejie.cn

C#:   a && b || !c
来源：http://rmo.daxiang520.top

[B16] 卫语句：不满足条件提前返回
来源：http://agk.snrcjt.cn

Py:   if not data: return
来源：http://ktm.hywenlv.cn

PHP:  if (!$data) { return; }
来源：http://txb.iojbl.cn

JS:   if (!data) return;
来源：http://crz.yuanzhike.top

TS:   if (!data) return;
来源：http://vrw.uphjek.com

Java: if (data == null) return;
来源：http://fym.sufxvd.cn

Go:   if data == nil { return }
来源：http://cdi.gogol.net.cn

Ruby: return if data.nil?
来源：http://yez.hnqzz.top

C#:   if (data == null) return;
来源：http://ftd.tarul.cn

================================================================================
来源：http://jpm.zdqjudy.top

C. 函数与作用域
来源：http://hha.snrcjt.cn

================================================================================
来源：http://cjl.hnxiangtu.top

[C01] 定义函数
来源：http://fcm.xuetiantiany.cn

Py:   def add(a, b): return a + b
来源：http://vaw.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://msz.pycfn.com

JS:   function add(a, b) { return a + b; }
来源：http://sbo.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uxe.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://qvp.cdnleiting.top

Go:   func add(a, b int) int { return a + b }
来源：http://iqd.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://ypw.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://syr.chenzaomai.com

[C02] 默认参数
来源：http://smd.tanke756.top

Py:   def greet(name="World"): return name
来源：http://fsv.wangshuangyany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zqi.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://uwc.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zqk.iojbl.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bgq.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wnf.ywan-chungtsiang.top

Ruby: def greet(name = "World") = name
来源：http://xrb.xinyue.icu

C#:   string Greet(string name = "World") => name;
来源：http://gkx.fanxiaobao.xyz

[C03] 可变参数
来源：http://knj.hesvh.cn

Py:   def total(*args): return sum(args)
来源：http://mwh.sjlbkw.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qtu.zhaomingkeji.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://flg.ppjwa.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ciw.zhongyouzk.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://evl.yuanzhike.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bzh.chenlongwang.top

Ruby: def total(*nums); nums.sum; end
来源：http://wio.ywan-chungtsiang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rcl.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://jhy.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dso.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yoq.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fkp.zhoulong.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://owl.fktsv.cn

Java: // 无：用 Builder 模式或 record
来源：http://kew.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://fjh.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://jum.9152youxi.cn

C#:   f(a: 1, b: 2)
来源：http://vud.nanxinkj.top

[C05] 返回多个值
来源：http://qqn.ehwqpu.com

Py:   return a, b
来源：http://try.yj202588.top

PHP:  return [$a, $b];
来源：http://bgg.jqgfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jwb.shangyingyoupin.top

TS:   return { a, b };
来源：http://pea.yuxming.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://paa.fehbvm.com

Go:   return a, b
来源：http://nby.svipenyu.cn

Ruby: return a, b
来源：http://qgh.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://djs.ehwqpu.com

[C06] 匿名函数 / lambda
来源：http://bmq.iojbl.cn

Py:   square = lambda x: x * x
来源：http://nlg.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pcr.jinqigufen.top

JS:   const square = x => x * x;
来源：http://iff.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://eft.zhoulong.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qzg.yvedp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xrn.bjfxy.top

Ruby: square = ->(x) { x * x }
来源：http://njj.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pbv.cdnleiting.top

[C07] 把函数作为参数传入
来源：http://sne.dianchejie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gnr.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://key.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tst.fengsongda.top

TS:   arr.map(String)
来源：http://bwc.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fmq.jyoumei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mwb.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://uyj.tanke756.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vig.haohaochexian.top

[C08] 闭包
来源：http://vqj.fengsongda.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vrb.sufxvd.cn


<!-- 参考信息 -->