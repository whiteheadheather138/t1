代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cpi.iojbl.cn

JS:   `Hello, ${name}!`
来源：http://izz.xziqi.cn

TS:   `Hello, ${name}!`
来源：http://yyu.yj20258.top

Java: "Hello, %s!".formatted(name)
来源：http://mmq.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wch.nanxinkj.top

Ruby: "Hello, #{name}!"
来源：http://ftz.yvedp.cn

C#:   $"Hello, {name}!"
来源：http://hxr.zhaomingkeji.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://avw.jqgfzy.top

Py:   "第一行\n第二行"
来源：http://eyy.sjlbkw.cn

PHP:  "第一行\n第二行"
来源：http://fyo.gzhubu.top

JS:   "第一行\n第二行"
来源：http://jjf.shanyushiyangtech.top

TS:   "第一行\n第二行"
来源：http://qbh.shangyingyoupin.top

Java: "第一行\n第二行"
来源：http://vde.zhoulong.xyz

Go:   "第一行\n第二行"
来源：http://bmc.shuidangran.top

Ruby: "第一行\n第二行"
来源：http://arj.fehbvm.com

C#:   "第一行\n第二行"
来源：http://uel.uphjek.com

[A14] 注释写法
来源：http://nms.ctjpmb.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://pya.zhijiandao.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yox.yj20258888.top

JS:   // 单行；/* 多行 */
来源：http://zrf.zhaomingkeji.xyz

TS:   // 单行；/* 多行 */
来源：http://isw.svipenyu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dzg.yuxming.cn

Go:   // 单行；/* 多行 */
来源：http://bwu.jinyuanbaomall.cn

Ruby: # 单行；=begin 多行 =end
来源：http://szp.svipenyu.cn

C#:   // 单行；/* 多行 */
来源：http://ahb.shuidangran.top

[A15] 空值判断与默认值
来源：http://ncx.zhixingplan.top

Py:   value = data or "默认值"
来源：http://kmo.sjlbkw.cn

PHP:  $value = $data ?? "默认值";
来源：http://hmo.nanxinkj.top

JS:   const value = data ?? "默认值";
来源：http://osz.snrcjt.cn

TS:   const value = data ?? "默认值";
来源：http://ijp.tanke756.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rsc.cucudq.cn

Go:   if data == "" { data = "默认值" }
来源：http://ljr.epnwcf.com

Ruby: value = data || "默认值"
来源：http://xen.vqdsnc.cn

C#:   var value = data ?? "默认值";
来源：http://muk.cqqwz.cn

[A16] 真假值判断规则
来源：http://nqa.cdnleiting.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rae.9152youxi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hqe.yueranfly.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rmp.xuanzx.com

TS:   if (!x) {}
来源：http://nni.zhixingplan.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sqn.jiagoushi.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://onm.yj202588.top

Ruby: unless x            # nil 与 false 为假
来源：http://waq.sweek.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kru.yfazqb.com

[A17] 位运算
来源：http://boj.fengsongda.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xre.mhx1999.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ykv.fktsv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://afi.jinghuilouyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://why.shuidangran.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uqg.hnxiangtu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gep.52xcode.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://odg.zhiwuduotai.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bvx.iojbl.cn

[A18] 字符与 ASCII 码互转
来源：http://ccc.daxiang520.top

Py:   ord("A"); chr(65)
来源：http://rih.zdqjudy.top

PHP:  ord("A"); chr(65)
来源：http://uho.ivvv.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fez.jinghuilouyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hiy.xinyue.icu

Java: (int) 'A'; (char) 65
来源：http://jyk.zhaomingkeji.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wsf.sjlbkw.cn

Ruby: "A".ord; 65.chr
来源：http://ucg.0kj1m.cn

C#:   (int)'A'; (char)65
来源：http://khm.shangyingyoupin.top

[A19] 交换两个变量
来源：http://yyt.fktsv.cn

Py:   a, b = b, a
来源：http://ute.zdbjq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://efy.jqgufenzy.top

JS:   [a, b] = [b, a];
来源：http://vom.ctjpmb.com

TS:   [a, b] = [b, a];
来源：http://fxr.chenlongwang.top

Java: int t = a; a = b; b = t;
来源：http://aah.hongshengwenyu.top

Go:   a, b = b, a
来源：http://oca.tian-w.cn

Ruby: a, b = b, a
来源：http://jpc.cheryme.top

C#:   (a, b) = (b, a);
来源：http://xco.aibaodan.cn

[A20] 读取标准输入
来源：http://cnt.yueranfly.top

Py:   name = input("请输入：")
来源：http://zxr.zdbjq.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://eyv.havefunace.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hdh.guowangkeji.top

TS:   // Node.js：readline 模块
来源：http://shx.zdqjudy.top

Java: new Scanner(System.in).nextLine()
来源：http://bre.andypj.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xdg.svipenyu.cn

Ruby: gets.chomp
来源：http://yvn.wangdashe.top

C#:   Console.ReadLine();
来源：http://krw.jianghu66.top

[A21] 保留指定小数位输出
来源：http://fbc.shangyingyoupin.top

Py:   f"{3.14159:.2f}"
来源：http://fhm.9152youxi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rvy.xinyue.icu

JS:   (3.14159).toFixed(2)
来源：http://apo.fengsongda.top

TS:   (3.14159).toFixed(2)
来源：http://nwc.sweek.top

Java: String.format("%.2f", 3.14159)
来源：http://pyq.zhengqikj.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dvy.chenlongwang.top

Ruby: format("%.2f", 3.14159)
来源：http://azc.yangfankeji.com

C#:   3.14159.ToString("F2")
来源：http://xxr.52xcode.cn

[A22] 获取字符串长度
来源：http://vsi.fengsongda.top

Py:   len(s)
来源：http://hxw.fanxiaobao.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zzq.hammf.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ksr.9152youxi.cn

TS:   s.length
来源：http://oxh.316326.xyz

Java: s.length()
来源：http://exe.52xcode.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://knc.bbcook.cn

Ruby: s.length
来源：http://ple.zhijiandao.cn

C#:   s.Length
来源：http://sdm.tanke756.top

[A23] 大小写转换
来源：http://obn.jqgufenzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wof.uphjek.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qrv.zhoulong.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mce.xuetiantiany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cat.cdnleiting.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ypb.gzhubu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://owa.gogol.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qqp.yongpay.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gxp.zhiwuduotai.top

[A24] 去除首尾空白
来源：http://rrd.shanyushiyangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bwz.yj20258.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pfc.hnqzz.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ykg.0kj1m.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ziu.xinyue.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zlk.fktsv.cn

Go:   strings.TrimSpace(s)
来源：http://hye.tian-w.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dpk.cashguo.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lzk.kuanghao11.cn

[A25] 字符串比较
来源：http://rwf.zhiwuduotai.top

Py:   s1 == s2; s1 != s2
来源：http://uyw.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tya.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gtg.jlsjyb.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://prg.cashguo.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zpi.birdmap.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xem.xziqi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hzu.jinqigfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ejj.ivvv.top

[A26] 类型转换总览
来源：http://ozd.zdbjq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ram.guannengcc.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mby.snrcjt.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wcm.ybcxt.top

TS:   Number() String() Boolean() x as number
来源：http://dkv.haohaochexian.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://irh.xinyue.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gnb.zhoulong.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://kap.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nvu.birdmap.top

================================================================================
来源：http://wzd.gzhubu.top

B. 流程控制
来源：http://key.smart0.xyz

================================================================================
来源：http://pqx.tian-w.cn

[B01] 条件判断 if / else
来源：http://fmk.yongpay.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mvu.birdmap.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lgk.gogol.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://urd.zhijiandao.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uth.chenlongwang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ewl.meibo888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kql.yanxiufei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yji.wangshuangyany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vxo.shangyingyoupin.top

[B02] 多分支 else if / elif
来源：http://gpz.gogol.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xcb.shzxlz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://epo.aibaodan.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jim.tanke756.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ddn.xinyue.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kql.0kj1m.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ori.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bbv.pengpengdd.cyou

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aeb.yj202588.top

[B03] switch / match / case
来源：http://yel.epnwcf.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jgr.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mxc.kuanghao11.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ayu.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ykj.smart0.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fch.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wno.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dgx.xuetiantiany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mgo.chenzaomai.com

[B04] for 计数循环
来源：http://ixq.fehbvm.com

Py:   for i in range(10): print(i)
来源：http://jxo.yj20258.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://okr.316326.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://czf.sufxvd.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xue.cqqwz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aio.wangdashe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cwf.yonumen.top

Ruby: 10.times { |i| puts i }
来源：http://nuu.sjlbkw.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cau.yonumen.top

[B05] 遍历数组 / 列表
来源：http://snm.jianghu66.top

Py:   for item in arr: print(item)
来源：http://xkb.jlsjyb.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ism.zdbjq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://swh.hnqzz.top

TS:   for (const item of arr) { console.log(item); }
来源：http://blw.gaohongyu789.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uxl.nanxuanxn.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wzw.sufxvd.cn

Ruby: arr.each { |item| puts item }
来源：http://hxv.guannengcc.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qtr.fengsongda.top

[B06] 遍历字典 / 对象
来源：http://gfw.yfazqb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://bgk.meibo888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gzx.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wjs.hfpthk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pdn.feifeiyinyue.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qxj.jinqigufen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vxy.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://drg.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yqy.sweek.top

[B07] while 循环
来源：http://lzu.bjfxy.top

Py:   while i < 10: i += 1
来源：http://xnc.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://osz.gogol.net.cn

JS:   while (i < 10) { i++; }
来源：http://rxk.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://lsr.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://zoj.ywan-chungtsiang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ymw.dianchejie.cn

Ruby: while i < 10; i += 1; end
来源：http://zii.zhongyouzk.top

C#:   while (i < 10) { i++; }
来源：http://ozr.birdmap.top

[B08] do-while（至少执行一次）
来源：http://ohy.jqgfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://ovm.hfpthk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zmr.havefunace.top

JS:   do { i++; } while (i < 10);
来源：http://uqi.0kj1m.cn

TS:   do { i++; } while (i < 10);
来源：http://ddu.meibo888.top

Java: do { i++; } while (i < 10);
来源：http://cnx.ivvv.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pom.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://eof.yangfankeji.com

C#:   do { i++; } while (i < 10);
来源：http://qgz.cdnleiting.top

[B09] break 与 continue
来源：http://rfp.jqgfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xav.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hxy.yvedp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xcm.wangdashe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://edd.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mde.fanxiaobao.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mhz.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kzf.jinghuilouyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mhs.yj202588.top

[B10] 遍历同时拿索引
来源：http://bhy.vqdsnc.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://llp.ctjpmb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://htb.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hpl.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tfw.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iow.feifeiyinyue.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fda.yuanzhike.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kgm.xingfuxueyuan.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xvs.hnqzz.top

[B11] 生成数字序列 / 区间
来源：http://qbw.ydjk.org.cn

Py:   list(range(0, 10, 2))
来源：http://sxj.52xcode.cn

PHP:  range(0, 10, 2);
来源：http://shz.xuetiantiany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ciq.bbcook.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dlk.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cbw.ehwqpu.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pec.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://mhd.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ras.ydzc1.top

[B12] 跳出多层循环
来源：http://kuk.yueranfly.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rgp.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mgg.ywan-chungtsiang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kwh.cheryme.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gpa.fanxiaobao.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ixu.jinghuilouyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://boy.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vgn.jinqigufen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lfv.zhaomingkeji.xyz

[B13] 判断是否为数字
来源：http://veh.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://asy.chenzaomai.com

PHP:  is_numeric($x)
来源：http://ogd.zdbjq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blv.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rdv.kuanghao11.cn

Java: x instanceof Number
来源：http://mko.tian-w.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dei.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://qoe.zdbjq.cn

C#:   x is int or double or decimal
来源：http://seo.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://hil.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eqe.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://grh.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://qay.jinqigfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://kxp.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dol.uphjek.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iuv.ppjwa.cn

Ruby: [1, 2, 3].include?(x)
来源：http://itr.shanyushiyangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://brz.xinyue.icu

[B15] 布尔运算与取反
来源：http://gky.hcnkem.com

Py:   a and b or not c
来源：http://vtr.zhaomingkeji.xyz

PHP:  $a && $b || !$c
来源：http://suq.tian-w.cn

JS:   a && b || !c
来源：http://uyv.fanxiaobao.xyz

TS:   a && b || !c
来源：http://vob.jyoumei.cn

Java: a && b || !c
来源：http://vuw.c1oappe.top

Go:   a && b || !c
来源：http://pit.zdqjudy.top

Ruby: a && b || !c
来源：http://lxx.yueranfly.top

C#:   a && b || !c
来源：http://qzk.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pfi.vqdsnc.cn

Py:   if not data: return
来源：http://dmf.haohaochexian.top

PHP:  if (!$data) { return; }
来源：http://tyl.yfazqb.com

JS:   if (!data) return;
来源：http://xhp.zdqjudy.top

TS:   if (!data) return;
来源：http://ixo.jiagoushi.top

Java: if (data == null) return;
来源：http://pmc.sweek.top

Go:   if data == nil { return }
来源：http://cbs.zhengqikj.top

Ruby: return if data.nil?
来源：http://cik.quarkkingdee.top

C#:   if (data == null) return;
来源：http://pdp.zhijiandao.cn

================================================================================
来源：http://lcb.wangdashe.top

C. 函数与作用域
来源：http://rbg.gotoacloud.top

================================================================================
来源：http://pal.zdbjq.cn

[C01] 定义函数
来源：http://rpb.uphjek.com

Py:   def add(a, b): return a + b
来源：http://but.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zae.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://nez.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bxw.gzhubu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://abg.nwbrower.top

Go:   func add(a, b int) int { return a + b }
来源：http://rbp.yvedp.cn

Ruby: def add(a, b); a + b; end
来源：http://dvf.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zjj.vqdsnc.cn

[C02] 默认参数
来源：http://gni.yonumen.top

Py:   def greet(name="World"): return name
来源：http://xwl.yvedp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xbs.aibaodan.cn

JS:   function greet(name = "World") { return name; }
来源：http://epv.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://obm.tianlin.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://ikl.cqqwz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bdx.dashuyun.cn

Ruby: def greet(name = "World") = name
来源：http://bxb.shanyushiyangkeji.top


<!-- 参考信息 -->