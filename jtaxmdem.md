代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ogc.nanxuanxn.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rmg.redwolf501.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hlb.shanyushiyangtech.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://njx.hesvh.cn

[A18] 字符与 ASCII 码互转
来源：http://ktr.xuanzx.com

Py:   ord("A"); chr(65)
来源：http://jhx.yj202588.top

PHP:  ord("A"); chr(65)
来源：http://jww.hongshengwenyu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rnp.sysykeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xws.gotoacloud.top

Java: (int) 'A'; (char) 65
来源：http://oog.cdnleiting.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rsg.sweek.top

Ruby: "A".ord; 65.chr
来源：http://zeo.yj20258888.top

C#:   (int)'A'; (char)65
来源：http://pzj.zdqjudy.top

[A19] 交换两个变量
来源：http://vth.jqgfzy.top

Py:   a, b = b, a
来源：http://afa.hysaishi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xul.jyoumei.cn

JS:   [a, b] = [b, a];
来源：http://oxd.nanxinkj.top

TS:   [a, b] = [b, a];
来源：http://gpi.zdbjq.cn

Java: int t = a; a = b; b = t;
来源：http://uso.nanxuanxn.top

Go:   a, b = b, a
来源：http://gct.aizwys.cn

Ruby: a, b = b, a
来源：http://fba.zhixingplan.top

C#:   (a, b) = (b, a);
来源：http://vgq.mhx1999.top

[A20] 读取标准输入
来源：http://mdc.jinghuilouyu.cn

Py:   name = input("请输入：")
来源：http://qrg.jiagoushi.top

PHP:  $name = trim(fgets(STDIN));
来源：http://hgg.ctjpmb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nxw.guowangkeji.top

TS:   // Node.js：readline 模块
来源：http://uqk.cucudq.cn

Java: new Scanner(System.in).nextLine()
来源：http://miy.jianghu66.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ify.fehbvm.com

Ruby: gets.chomp
来源：http://aiy.jyoumei.cn

C#:   Console.ReadLine();
来源：http://byv.ctjpmb.com

[A21] 保留指定小数位输出
来源：http://tnb.daria6918.cn

Py:   f"{3.14159:.2f}"
来源：http://ytg.nwbrower.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zbs.cqqwz.cn

JS:   (3.14159).toFixed(2)
来源：http://icq.feifeiyinyue.top

TS:   (3.14159).toFixed(2)
来源：http://nem.zdqjudy.top

Java: String.format("%.2f", 3.14159)
来源：http://bsb.cqqwz.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dmy.cqqwz.cn

Ruby: format("%.2f", 3.14159)
来源：http://rlw.yj20258888.top

C#:   3.14159.ToString("F2")
来源：http://kcy.andypj.xyz

[A22] 获取字符串长度
来源：http://ibd.fanxiaobao.xyz

Py:   len(s)
来源：http://etm.xziqi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sie.shanyushiyangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nuf.chenjidiqi.icu

TS:   s.length
来源：http://spw.andypj.xyz

Java: s.length()
来源：http://awp.ydzc1.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oka.yj20258.top

Ruby: s.length
来源：http://dsz.sweek.top

C#:   s.Length
来源：http://uyz.tanke756.top

[A23] 大小写转换
来源：http://oun.hnqzz.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gmz.pengpengdd.cyou

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mtw.chenjidiqi.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fwq.cucudq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uei.ywan-chungtsiang.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rbv.fktsv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://whm.sweek.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tkw.smart0.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://qfl.9152youxi.cn

[A24] 去除首尾空白
来源：http://lux.ydzc1.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uyo.fktsv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://knv.guowangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hhg.fanxiaobao.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://han.yj20258888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hxb.vqdsnc.cn

Go:   strings.TrimSpace(s)
来源：http://vey.quarkkingdee.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sma.shanyushiyangtech.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kie.wangdashe.top

[A25] 字符串比较
来源：http://euj.hnqzz.top

Py:   s1 == s2; s1 != s2
来源：http://fzw.hysaishi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hbb.iojbl.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kuc.yj20258888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jgy.jyoumei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kxp.shzxlz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vuy.hammf.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ely.yangfankeji.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mbs.yj202588.top

[A26] 类型转换总览
来源：http://ztv.316326.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ovt.ydzc1.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gjv.yfazqb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xuf.daria6918.cn

TS:   Number() String() Boolean() x as number
来源：http://sth.zhoulong.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xrw.jianghu66.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rri.zhengqikj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hjb.svipenyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://siv.shzxlz.cn

================================================================================
来源：http://rfa.shuidangran.top

B. 流程控制
来源：http://rsx.epnwcf.com

================================================================================
来源：http://lvr.redwolf501.top

[B01] 条件判断 if / else
来源：http://pen.epnwcf.com

Py:   result = "正" if x > 0 else "非正"
来源：http://nxx.vehdjk.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zkb.andypj.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xlw.yj20258888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sxq.zhaomingkeji.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://mrt.xylfe.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tvv.shuidangran.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://epj.guannengcc.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gai.yonumen.top

[B02] 多分支 else if / elif
来源：http://kxc.hnqzz.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://etl.yanxiufei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vxv.yonumen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kyk.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jqo.hysaishi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mwm.shanyushiyangtech.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nrk.shzxlz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nek.ydzc1.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mqj.yueranfly.top

[B03] switch / match / case
来源：http://lfs.nanxuanxn.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ass.chenlongwang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ruu.gzhubu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ggh.cashguo.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://brr.pengpengdd.cyou

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ipi.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gev.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jia.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ymk.hnxiangtu.top

[B04] for 计数循环
来源：http://eon.andypj.xyz

Py:   for i in range(10): print(i)
来源：http://wtv.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://szy.redwolf501.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eno.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xqd.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jfv.cashguo.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tua.fktsv.cn

Ruby: 10.times { |i| puts i }
来源：http://tmt.yanxiufei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mgn.nanxinkj.top

[B05] 遍历数组 / 列表
来源：http://zyb.yanxiufei.cn

Py:   for item in arr: print(item)
来源：http://ahv.yanxiufei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kwm.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fvi.zhengqikj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zdr.yvedp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xul.dashuyun.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qda.chenjidiqi.icu

Ruby: arr.each { |item| puts item }
来源：http://mrn.yj20258888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://feu.shanyushiyangtech.top

[B06] 遍历字典 / 对象
来源：http://dbu.tanke756.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qiw.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xkh.redwolf501.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ngu.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://agg.jqgfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rqf.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wwk.hesvh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iyx.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xhx.yvedp.cn

[B07] while 循环
来源：http://exo.yuanzhike.top

Py:   while i < 10: i += 1
来源：http://dlo.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hwa.shanyushiyangtech.top

JS:   while (i < 10) { i++; }
来源：http://bvo.xuanzx.com

TS:   while (i < 10) { i++; }
来源：http://dlp.xinyue.icu

Java: while (i < 10) { i++; }
来源：http://sxk.cucudq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://feh.zhiwuduotai.top

Ruby: while i < 10; i += 1; end
来源：http://fgq.cheryme.top

C#:   while (i < 10) { i++; }
来源：http://plh.cdnleiting.top

[B08] do-while（至少执行一次）
来源：http://ulf.fanxiaobao.xyz

Py:   # 无 do-while：用 while True + break
来源：http://gsu.jlsjyb.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://drs.daria6918.cn

JS:   do { i++; } while (i < 10);
来源：http://sho.9152youxi.cn

TS:   do { i++; } while (i < 10);
来源：http://udk.zhixingplan.top

Java: do { i++; } while (i < 10);
来源：http://mqx.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kzp.yongpay.top

Ruby: begin; i += 1; end while i < 10
来源：http://qmj.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://iko.yj202588.top

[B09] break 与 continue
来源：http://yzk.ywan-chungtsiang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ydc.xingfuxueyuan.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xxl.fzhhl.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fnl.9152youxi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pfc.birdmap.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qjx.nanxuanxn.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ngd.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yhu.chenlongwang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nqr.daria6918.cn

[B10] 遍历同时拿索引
来源：http://occ.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rru.zhaomingkeji.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://duh.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rxd.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wew.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sgz.xziqi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pez.hongshengwenyu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oud.xinyue.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://coh.jiagoushi.top

[B11] 生成数字序列 / 区间
来源：http://ixt.smart0.xyz

Py:   list(range(0, 10, 2))
来源：http://jsb.fzhhl.top

PHP:  range(0, 10, 2);
来源：http://okq.zhoulong.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ege.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ftf.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lgr.birdmap.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://apn.shanyushiyangtech.top

Ruby: (0...10).step(2).to_a
来源：http://icc.hysaishi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pvg.yvedp.cn

[B12] 跳出多层循环
来源：http://ftl.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://jql.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ndf.pengpengdd.cyou

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yrz.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://czb.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zwt.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bao.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qos.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yyk.jqgfzy.top

[B13] 判断是否为数字
来源：http://dib.xuetiantiany.cn

Py:   isinstance(x, (int, float))
来源：http://mye.tianlin.xyz

PHP:  is_numeric($x)
来源：http://fdi.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://krp.zhijiandao.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fey.epnwcf.com

Java: x instanceof Number
来源：http://uhr.xuanzx.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tyv.hammf.cn

Ruby: x.is_a?(Numeric)
来源：http://lfb.guannengcc.top

C#:   x is int or double or decimal
来源：http://lsg.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://jdl.sweek.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pdw.svipenyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zyg.52xcode.cn

JS:   [1, 2, 3].includes(x)
来源：http://qfa.sjlbkw.cn

TS:   [1, 2, 3].includes(x)
来源：http://shi.fanxiaobao.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://eoa.zhongyouzk.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eiq.yfazqb.com

Ruby: [1, 2, 3].include?(x)
来源：http://pac.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jzb.zhaomingkeji.xyz

[B15] 布尔运算与取反
来源：http://aas.zhixingplan.top

Py:   a and b or not c
来源：http://yuv.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://cfk.pycfn.com

JS:   a && b || !c
来源：http://ynx.dashuyun.cn

TS:   a && b || !c
来源：http://ycs.zhongyouzk.top

Java: a && b || !c
来源：http://fuc.316326.xyz

Go:   a && b || !c
来源：http://cfy.sweek.top

Ruby: a && b || !c
来源：http://umc.gzhubu.top

C#:   a && b || !c
来源：http://siv.9152youxi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fch.yvedp.cn

Py:   if not data: return
来源：http://qlm.havefunace.top

PHP:  if (!$data) { return; }
来源：http://jnk.yfazqb.com

JS:   if (!data) return;
来源：http://vxr.sweek.top

TS:   if (!data) return;
来源：http://sbp.guannengcc.top

Java: if (data == null) return;
来源：http://fxt.ctjpmb.com

Go:   if data == nil { return }
来源：http://nas.gogol.net.cn

Ruby: return if data.nil?
来源：http://fyl.zdbjq.cn

C#:   if (data == null) return;
来源：http://hzt.dashuyun.cn

================================================================================
来源：http://ufs.yfazqb.com

C. 函数与作用域
来源：http://xhz.daxiang520.top

================================================================================
来源：http://rnh.xziqi.cn

[C01] 定义函数
来源：http://lrw.haohaochexian.top

Py:   def add(a, b): return a + b
来源：http://nmg.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hgh.sxryk.cn

JS:   function add(a, b) { return a + b; }
来源：http://tus.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mqd.tarul.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ogg.yongpay.top

Go:   func add(a, b int) int { return a + b }
来源：http://kca.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://yvy.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jlv.sxryk.cn

[C02] 默认参数
来源：http://any.ydzc1.top

Py:   def greet(name="World"): return name
来源：http://rkh.vqdsnc.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cuv.sxryk.cn

JS:   function greet(name = "World") { return name; }
来源：http://znn.wangdashe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nnd.hnqzz.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ilu.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eny.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://snh.jinqigufen.top

C#:   string Greet(string name = "World") => name;
来源：http://qpn.xinyue.icu

[C03] 可变参数
来源：http://gio.guowangkeji.top

Py:   def total(*args): return sum(args)
来源：http://opn.yongpay.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uvm.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uwb.chenzaomai.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rpm.yvedp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pxf.sysykeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xpw.fzhhl.top

Ruby: def total(*nums); nums.sum; end
来源：http://osh.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jlr.ydjk.org.cn

[C04] 命名参数 / 关键字参数
来源：http://qun.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eti.redwolf501.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zzz.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vky.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ajq.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://uvv.cdnleiting.top

Go:   // 无：用配置结构体参数
来源：http://xvx.vehdjk.com

Ruby: f(a: 1, b: 2)
来源：http://iqt.bjfxy.top

C#:   f(a: 1, b: 2)
来源：http://yfn.hongshengwenyu.top

[C05] 返回多个值
来源：http://jxw.xingfuxueyuan.xyz

Py:   return a, b
来源：http://vkv.chenzaomai.com

PHP:  return [$a, $b];
来源：http://gdq.zdqjudy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jyx.pycfn.com

TS:   return { a, b };
来源：http://vpc.fanxiaobao.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zdf.jqgfzy.top

Go:   return a, b
来源：http://ymy.dianchejie.cn

Ruby: return a, b
来源：http://nvn.bjfxy.top

C#:   return (a, b);              // ValueTuple
来源：http://srq.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://wbq.tanke756.top

Py:   square = lambda x: x * x
来源：http://wir.xziqi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://els.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://add.zhoulong.xyz

TS:   const square = (x: number): number => x * x;
来源：http://zyj.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jry.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://yfp.sufxvd.cn

Ruby: square = ->(x) { x * x }
来源：http://fvj.tarul.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tvp.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://xlc.gaohongyu789.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hhy.yangfankeji.com

PHP:  array_map("strtoupper", $arr);
来源：http://fhp.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://utf.daria6918.cn

TS:   arr.map(String)
来源：http://vsc.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gdo.xziqi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ohz.ywan-chungtsiang.top

Ruby: arr.map(&:upcase)
来源：http://jrc.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fhx.jinqigfzy.top

[C08] 闭包
来源：http://jvf.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zia.jinqigfzy.top


<!-- 参考信息 -->