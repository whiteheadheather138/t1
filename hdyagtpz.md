代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://iix.hywenlv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xkr.gogol.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://abl.cashguo.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xut.yueranfly.top

Ruby: x > 0 ? "yes" : "no"
来源：http://qqm.ppjwa.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mxh.jiagoushi.top

[A12] 字符串插值 / 格式化
来源：http://cjw.hesvh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rbi.zhiwuduotai.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://amv.yuxming.cn

JS:   `Hello, ${name}!`
来源：http://amh.tanke756.top

TS:   `Hello, ${name}!`
来源：http://ehj.havefunace.top

Java: "Hello, %s!".formatted(name)
来源：http://pxo.hysaishi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://emq.xingfuxueyuan.xyz

Ruby: "Hello, #{name}!"
来源：http://qag.meibo888.top

C#:   $"Hello, {name}!"
来源：http://dnc.xylfe.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yim.gogol.net.cn

Py:   "第一行\n第二行"
来源：http://mjy.birdmap.top

PHP:  "第一行\n第二行"
来源：http://bae.zdqjudy.top

JS:   "第一行\n第二行"
来源：http://aey.aibaodan.cn

TS:   "第一行\n第二行"
来源：http://pad.chenjidiqi.icu

Java: "第一行\n第二行"
来源：http://mxg.guowangkeji.top

Go:   "第一行\n第二行"
来源：http://ick.fehbvm.com

Ruby: "第一行\n第二行"
来源：http://zro.xziqi.cn

C#:   "第一行\n第二行"
来源：http://sds.zhiwuduotai.top

[A14] 注释写法
来源：http://qbs.wangshuangyany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://esd.yj202588.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://zju.cheryme.top

JS:   // 单行；/* 多行 */
来源：http://irt.cucudq.cn

TS:   // 单行；/* 多行 */
来源：http://ams.9152youxi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xfi.daria6918.cn

Go:   // 单行；/* 多行 */
来源：http://hpo.jinqigfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://kac.jinghuilouyu.cn

C#:   // 单行；/* 多行 */
来源：http://cbx.hfpthk.cn

[A15] 空值判断与默认值
来源：http://hys.yvedp.cn

Py:   value = data or "默认值"
来源：http://ppm.ehwqpu.com

PHP:  $value = $data ?? "默认值";
来源：http://pdn.cheryme.top

JS:   const value = data ?? "默认值";
来源：http://wvx.chenzaomai.com

TS:   const value = data ?? "默认值";
来源：http://hns.jyoumei.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sqc.jqgufenzy.top

Go:   if data == "" { data = "默认值" }
来源：http://zgf.haohaochexian.top

Ruby: value = data || "默认值"
来源：http://xch.chenzaomai.com

C#:   var value = data ?? "默认值";
来源：http://zee.shanyushiyangkeji.top

[A16] 真假值判断规则
来源：http://tmy.zhijiandao.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dqz.xylfe.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vof.zhaomingkeji.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ciy.fanxiaobao.xyz

TS:   if (!x) {}
来源：http://tri.0kj1m.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gut.jinyuanbaomall.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ctk.jinqigufen.top

Ruby: unless x            # nil 与 false 为假
来源：http://qod.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cbx.hnqzz.top

[A17] 位运算
来源：http://jmm.uphjek.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pbm.jinghuilouyu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eri.jqgufenzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ghg.iojbl.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dox.jinqigfzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qcj.fzhhl.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dor.gogol.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qhz.shanyushiyangtech.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hmk.fzhhl.top

[A18] 字符与 ASCII 码互转
来源：http://jzo.tarul.cn

Py:   ord("A"); chr(65)
来源：http://svc.tian-w.cn

PHP:  ord("A"); chr(65)
来源：http://pfu.smart0.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xig.cdnleiting.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xld.hongshengwenyu.top

Java: (int) 'A'; (char) 65
来源：http://drc.wangdashe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tmz.guannengcc.top

Ruby: "A".ord; 65.chr
来源：http://htu.ybcxt.top

C#:   (int)'A'; (char)65
来源：http://zfi.hnxiangtu.top

[A19] 交换两个变量
来源：http://ubb.guowangkeji.top

Py:   a, b = b, a
来源：http://naa.yj20258.top

PHP:  [$a, $b] = [$b, $a];
来源：http://cur.fehbvm.com

JS:   [a, b] = [b, a];
来源：http://ttw.hammf.cn

TS:   [a, b] = [b, a];
来源：http://ujx.nwbrower.top

Java: int t = a; a = b; b = t;
来源：http://euw.yj20258888.top

Go:   a, b = b, a
来源：http://aaw.jinqigufen.top

Ruby: a, b = b, a
来源：http://wwb.gaohongyu789.top

C#:   (a, b) = (b, a);
来源：http://vua.gogol.net.cn

[A20] 读取标准输入
来源：http://tst.aibaodan.cn

Py:   name = input("请输入：")
来源：http://ksw.cdnleiting.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ozy.cucudq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gcr.kuanghao11.cn

TS:   // Node.js：readline 模块
来源：http://stl.tarul.cn

Java: new Scanner(System.in).nextLine()
来源：http://gnv.svipenyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dco.jiagoushi.top

Ruby: gets.chomp
来源：http://keb.fanxiaobao.xyz

C#:   Console.ReadLine();
来源：http://hly.fzhhl.top

[A21] 保留指定小数位输出
来源：http://zui.yuanzhike.top

Py:   f"{3.14159:.2f}"
来源：http://zsy.52xcode.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ske.ivvv.top

JS:   (3.14159).toFixed(2)
来源：http://hqj.jinqigfzy.top

TS:   (3.14159).toFixed(2)
来源：http://spb.yuanzhike.top

Java: String.format("%.2f", 3.14159)
来源：http://zau.birdmap.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mll.daxiang520.top

Ruby: format("%.2f", 3.14159)
来源：http://byo.hcnkem.com

C#:   3.14159.ToString("F2")
来源：http://tuu.cqqwz.cn

[A22] 获取字符串长度
来源：http://tme.yueranfly.top

Py:   len(s)
来源：http://eal.tarul.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sbq.xylfe.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pwg.fzhhl.top

TS:   s.length
来源：http://jza.zhaomingkeji.xyz

Java: s.length()
来源：http://zqu.xuetiantiany.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tlv.epnwcf.com

Ruby: s.length
来源：http://drd.chenlongwang.top

C#:   s.Length
来源：http://eyh.daria6918.cn

[A23] 大小写转换
来源：http://ehp.aibaodan.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mum.yvedp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gva.hesvh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zra.chenjidiqi.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vza.hfpthk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nyt.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lvd.xuanzx.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wgv.xylfe.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://urt.xuanzx.com

[A24] 去除首尾空白
来源：http://fqr.nwbrower.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mgi.9152youxi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bcq.pengpengdd.cyou

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://noz.ydzc1.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pde.9152youxi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fne.jiagoushi.top

Go:   strings.TrimSpace(s)
来源：http://loi.mhx1999.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qiz.tarul.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mcf.aizwys.cn

[A25] 字符串比较
来源：http://nie.hongshengwenyu.top

Py:   s1 == s2; s1 != s2
来源：http://ssq.feifeiyinyue.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qjk.svipenyu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ige.xuanzx.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jzw.0kj1m.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yjj.aibaodan.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ipp.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://pup.bbcook.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mvt.sweek.top

[A26] 类型转换总览
来源：http://twu.hcnkem.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jfn.hongshengwenyu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://izh.yj20258888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nws.sweek.top

TS:   Number() String() Boolean() x as number
来源：http://jyr.xuanzx.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jfn.smart0.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mhw.haohaochexian.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zfw.ybcxt.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ocs.yj20258888.top

================================================================================
来源：http://ose.yj202588.top

B. 流程控制
来源：http://hzn.xuanzx.com

================================================================================
来源：http://vjg.chenlongwang.top

[B01] 条件判断 if / else
来源：http://qft.kuanghao11.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hec.fzhhl.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rci.bbcook.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fof.yj20258888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ctj.kuanghao11.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oph.jlsjyb.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mnu.yongpay.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://elj.yonumen.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dhz.ydzc1.top

[B02] 多分支 else if / elif
来源：http://vrp.fzhhl.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dyj.haohaochexian.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xsa.yangfankeji.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lup.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbh.fktsv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yhe.yfazqb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dph.haohaochexian.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ueq.hysaishi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wgc.kuanghao11.cn

[B03] switch / match / case
来源：http://jmv.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://buq.cucudq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tir.hammf.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kng.hesvh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yyu.yvedp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cxc.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nyq.hfpthk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qsg.gotoacloud.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vcf.nwbrower.top

[B04] for 计数循环
来源：http://fjh.gzhubu.top

Py:   for i in range(10): print(i)
来源：http://cnk.quarkkingdee.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rvf.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://orn.chenjidiqi.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://opd.cheryme.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://twa.dianchejie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ynn.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://hgj.iojbl.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ljp.aibaodan.cn

[B05] 遍历数组 / 列表
来源：http://sjq.quarkkingdee.top

Py:   for item in arr: print(item)
来源：http://kvs.ydzc1.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://chz.ppjwa.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://elh.yangfankeji.com

TS:   for (const item of arr) { console.log(item); }
来源：http://qbk.smart0.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://qdu.hnqzz.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yvp.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://nzy.jqgfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://phg.vqdsnc.cn

[B06] 遍历字典 / 对象
来源：http://thw.jinqigufen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://aqb.tian-w.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bil.52xcode.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://est.zhixingplan.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pyx.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://elz.xylfe.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lwe.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://acx.jinqigfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rct.zhijiandao.cn

[B07] while 循环
来源：http://yzv.vqdsnc.cn

Py:   while i < 10: i += 1
来源：http://www.nanxinkj.top

PHP:  while ($i < 10) { $i++; }
来源：http://gvx.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://git.fktsv.cn

TS:   while (i < 10) { i++; }
来源：http://yzd.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://lyu.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kgx.zhongyouzk.top

Ruby: while i < 10; i += 1; end
来源：http://obg.ywan-chungtsiang.top

C#:   while (i < 10) { i++; }
来源：http://tpu.wangshuangyany.cn

[B08] do-while（至少执行一次）
来源：http://iwb.yanxiufei.cn

Py:   # 无 do-while：用 while True + break
来源：http://nqf.hfpthk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vwq.pycfn.com

JS:   do { i++; } while (i < 10);
来源：http://dkq.wangshuangyany.cn

TS:   do { i++; } while (i < 10);
来源：http://dzd.zhijiandao.cn

Java: do { i++; } while (i < 10);
来源：http://heh.daria6918.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ddp.yangfankeji.com

Ruby: begin; i += 1; end while i < 10
来源：http://nqw.guannengcc.top

C#:   do { i++; } while (i < 10);
来源：http://bkb.yvedp.cn

[B09] break 与 continue
来源：http://yta.ywan-chungtsiang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pmo.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ixp.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uow.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://prf.guannengcc.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://axd.ybcxt.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bff.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pie.hammf.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixq.shanyushiyangtech.top

[B10] 遍历同时拿索引
来源：http://wku.guowangkeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tkb.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qcs.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mwv.hfpthk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nov.andypj.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ulc.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bwv.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lui.shzxlz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tzz.chenlongwang.top

[B11] 生成数字序列 / 区间
来源：http://tyb.yj20258888.top

Py:   list(range(0, 10, 2))
来源：http://gfj.daria6918.cn

PHP:  range(0, 10, 2);
来源：http://nnt.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://osw.chenjidiqi.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iba.ywan-chungtsiang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tbv.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wty.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://jqb.zdbjq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hop.bjfxy.top

[B12] 跳出多层循环
来源：http://teo.ywan-chungtsiang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fra.jianghu66.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vlt.zhengqikj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://psg.shanyushiyangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pla.chenzaomai.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nbp.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tcs.sweek.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yjv.nanxuanxn.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zms.guannengcc.top

[B13] 判断是否为数字
来源：http://hof.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://jez.aizwys.cn

PHP:  is_numeric($x)
来源：http://oku.yanxiufei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wkw.yj20258.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aib.shuidangran.top

Java: x instanceof Number
来源：http://lnm.iojbl.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zml.yj20258.top

Ruby: x.is_a?(Numeric)
来源：http://ouj.jlsjyb.cn

C#:   x is int or double or decimal
来源：http://mpu.hesvh.cn

[B14] 判断值是否在集合内
来源：http://iiy.fktsv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uok.c1oappe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bgp.yvedp.cn

JS:   [1, 2, 3].includes(x)
来源：http://woy.guannengcc.top

TS:   [1, 2, 3].includes(x)
来源：http://fww.hfpthk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vts.zhixingplan.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kpd.chenzaomai.com

Ruby: [1, 2, 3].include?(x)
来源：http://nqa.hywenlv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xqy.pycfn.com

[B15] 布尔运算与取反
来源：http://qxf.hesvh.cn

Py:   a and b or not c
来源：http://tcf.c1oappe.top

PHP:  $a && $b || !$c
来源：http://dmd.gotoacloud.top

JS:   a && b || !c
来源：http://tgd.zdqjudy.top

TS:   a && b || !c
来源：http://qlp.zycfv.cn

Java: a && b || !c
来源：http://azp.epnwcf.com

Go:   a && b || !c
来源：http://rrn.daria6918.cn

Ruby: a && b || !c
来源：http://mfu.ppjwa.cn

C#:   a && b || !c
来源：http://xue.zhengqikj.top

[B16] 卫语句：不满足条件提前返回
来源：http://bst.zhixingplan.top

Py:   if not data: return
来源：http://cho.guowangkeji.top

PHP:  if (!$data) { return; }
来源：http://kel.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://aoh.yueranfly.top

TS:   if (!data) return;
来源：http://jpa.hfpthk.cn

Java: if (data == null) return;
来源：http://soo.mhx1999.top

Go:   if data == nil { return }
来源：http://cda.shanyushiyangtech.top

Ruby: return if data.nil?
来源：http://gwx.redwolf501.top

C#:   if (data == null) return;
来源：http://rgs.ybcxt.top

================================================================================
来源：http://wxg.chenzaomai.com

C. 函数与作用域
来源：http://jdk.ydzc1.top

================================================================================
来源：http://fjr.daxiang520.top

[C01] 定义函数
来源：http://nuw.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://qum.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pbu.feifeiyinyue.top

JS:   function add(a, b) { return a + b; }
来源：http://kod.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://akh.fzhhl.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cmi.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yfv.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://tyc.hywenlv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iey.iojbl.cn


<!-- 参考信息 -->