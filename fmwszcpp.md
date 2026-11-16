代发 wailian999

JS:   String(42); (42).toString()
来源：http://yta.haohaochexian.top

TS:   String(42)
来源：http://vli.andypj.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://txv.mhx1999.top

Go:   strconv.Itoa(42)
来源：http://ckn.jianghu66.top

Ruby: 42.to_s
来源：http://trs.cdnleiting.top

C#:   42.ToString()
来源：http://bme.pycfn.com

[A08] 取整与四舍五入
来源：http://hyq.chenzaomai.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hfs.9152youxi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://myh.jinqigfzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eql.nanxuanxn.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ybe.jlsjyb.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cvm.yonumen.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ldr.xylfe.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fau.yj20258.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fee.hammf.cn

[A09] 绝对值与最大最小值
来源：http://shl.chenzaomai.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wlw.aizwys.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zzh.aizwys.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ygt.sjlbkw.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lzm.sweek.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sxo.birdmap.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vqt.zhiwuduotai.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pqe.sxryk.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hiq.zdbjq.cn

[A10] 生成随机数
来源：http://liu.sysykeji.top

Py:   import random; random.randint(1, 100)
来源：http://fvs.zhengqikj.top

PHP:  random_int(1, 100);
来源：http://azz.haohaochexian.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dyr.yj20258888.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xjt.cucudq.cn

Java: new Random().nextInt(100) + 1
来源：http://iha.sufxvd.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://asm.hysaishi.cn

Ruby: rand(1..100)
来源：http://qss.316326.xyz

C#:   new Random().Next(1, 101)
来源：http://tmd.zhoulong.xyz

[A11] 条件表达式（三元）
来源：http://hlz.bbcook.cn

Py:   "yes" if x > 0 else "no"
来源：http://txu.zhixingplan.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://utj.hongshengwenyu.top

JS:   x > 0 ? "yes" : "no"
来源：http://adu.zycfv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ahf.ydzc1.top

Java: x > 0 ? "yes" : "no"
来源：http://wnc.jianghu66.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pec.quarkkingdee.top

Ruby: x > 0 ? "yes" : "no"
来源：http://yqx.yueranfly.top

C#:   x > 0 ? "yes" : "no"
来源：http://hqk.jyoumei.cn

[A12] 字符串插值 / 格式化
来源：http://xag.xylfe.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jon.xuanzx.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rjd.shanyushiyangtech.top

JS:   `Hello, ${name}!`
来源：http://poh.zycfv.cn

TS:   `Hello, ${name}!`
来源：http://fsp.vehdjk.com

Java: "Hello, %s!".formatted(name)
来源：http://kjo.9152youxi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rhr.ivvv.top

Ruby: "Hello, #{name}!"
来源：http://pyu.pengpengdd.cyou

C#:   $"Hello, {name}!"
来源：http://fjt.jinghuilouyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hpa.guannengcc.top

Py:   "第一行\n第二行"
来源：http://sps.chenlongwang.top

PHP:  "第一行\n第二行"
来源：http://bcq.52xcode.cn

JS:   "第一行\n第二行"
来源：http://klk.sweek.top

TS:   "第一行\n第二行"
来源：http://hap.cqqwz.cn

Java: "第一行\n第二行"
来源：http://kut.shanyushiyangkeji.top

Go:   "第一行\n第二行"
来源：http://omr.yongpay.top

Ruby: "第一行\n第二行"
来源：http://pvk.zhijiandao.cn

C#:   "第一行\n第二行"
来源：http://zmc.xinyue.icu

[A14] 注释写法
来源：http://bnr.zdqjudy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://fac.haohaochexian.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://iqu.cqqwz.cn

JS:   // 单行；/* 多行 */
来源：http://gda.aizwys.cn

TS:   // 单行；/* 多行 */
来源：http://rzq.ehwqpu.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bqc.zhengqikj.top

Go:   // 单行；/* 多行 */
来源：http://vgg.daxiang520.top

Ruby: # 单行；=begin 多行 =end
来源：http://mgr.tarul.cn

C#:   // 单行；/* 多行 */
来源：http://guw.jinqigufen.top

[A15] 空值判断与默认值
来源：http://yyo.jinqigfzy.top

Py:   value = data or "默认值"
来源：http://jka.daria6918.cn

PHP:  $value = $data ?? "默认值";
来源：http://fml.shanyushiyangkeji.top

JS:   const value = data ?? "默认值";
来源：http://rbr.hongshengwenyu.top

TS:   const value = data ?? "默认值";
来源：http://svq.jinqigufen.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rdr.cashguo.top

Go:   if data == "" { data = "默认值" }
来源：http://pfl.shanyushiyangkeji.top

Ruby: value = data || "默认值"
来源：http://prd.jinqigfzy.top

C#:   var value = data ?? "默认值";
来源：http://nju.gzhubu.top

[A16] 真假值判断规则
来源：http://uts.ehwqpu.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kyu.fzhhl.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qmw.jinghuilouyu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pge.cqqwz.cn

TS:   if (!x) {}
来源：http://ila.hcnkem.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zaw.tarul.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://czx.shanyushiyangkeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://qdh.birdmap.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xiq.zhoulong.xyz

[A17] 位运算
来源：http://qst.vqdsnc.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qsq.ctjpmb.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qws.hammf.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vag.chenzaomai.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://flz.hysaishi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qtk.gogol.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vtw.tarul.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lih.feifeiyinyue.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rdv.svipenyu.cn

[A18] 字符与 ASCII 码互转
来源：http://ozg.ctjpmb.com

Py:   ord("A"); chr(65)
来源：http://cco.vehdjk.com

PHP:  ord("A"); chr(65)
来源：http://yyr.vehdjk.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nhy.svipenyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qhs.ppjwa.cn

Java: (int) 'A'; (char) 65
来源：http://xsm.chenzaomai.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cmo.hfpthk.cn

Ruby: "A".ord; 65.chr
来源：http://zrs.cucudq.cn

C#:   (int)'A'; (char)65
来源：http://aof.quarkkingdee.top

[A19] 交换两个变量
来源：http://cmc.ehwqpu.com

Py:   a, b = b, a
来源：http://ono.yonumen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://rpj.zhixingplan.top

JS:   [a, b] = [b, a];
来源：http://mvl.yueranfly.top

TS:   [a, b] = [b, a];
来源：http://gox.guowangkeji.top

Java: int t = a; a = b; b = t;
来源：http://emr.redwolf501.top

Go:   a, b = b, a
来源：http://igb.shangyingyoupin.top

Ruby: a, b = b, a
来源：http://zwn.jinqigfzy.top

C#:   (a, b) = (b, a);
来源：http://pgb.zdqjudy.top

[A20] 读取标准输入
来源：http://dss.sysykeji.top

Py:   name = input("请输入：")
来源：http://ura.iojbl.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://azz.xinyue.icu

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jwf.smart0.xyz

TS:   // Node.js：readline 模块
来源：http://rhd.dianchejie.cn

Java: new Scanner(System.in).nextLine()
来源：http://uph.ivvv.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://glk.zhengqikj.top

Ruby: gets.chomp
来源：http://wki.smart0.xyz

C#:   Console.ReadLine();
来源：http://kya.jianghu66.top

[A21] 保留指定小数位输出
来源：http://eyc.hammf.cn

Py:   f"{3.14159:.2f}"
来源：http://wqu.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cxr.shangyingyoupin.top

JS:   (3.14159).toFixed(2)
来源：http://ofm.sweek.top

TS:   (3.14159).toFixed(2)
来源：http://hvs.sufxvd.cn

Java: String.format("%.2f", 3.14159)
来源：http://eot.yuxming.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bmt.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://fgd.hammf.cn

C#:   3.14159.ToString("F2")
来源：http://wjd.fehbvm.com

[A22] 获取字符串长度
来源：http://afc.ctjpmb.com

Py:   len(s)
来源：http://pkr.vehdjk.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://odd.gaohongyu789.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xdv.zdbjq.cn

TS:   s.length
来源：http://sjp.shanyushiyangtech.top

Java: s.length()
来源：http://kiq.ivvv.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nkq.316326.xyz

Ruby: s.length
来源：http://rls.shanyushiyangkeji.top

C#:   s.Length
来源：http://nws.cashguo.top

[A23] 大小写转换
来源：http://sfu.xuanzx.com

Py:   s.upper(); s.lower(); s.title()
来源：http://wci.ybcxt.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bhm.sweek.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sla.gzhubu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ymf.meibo888.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mgy.guowangkeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ngg.sjlbkw.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://thh.zhaomingkeji.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://eso.yangfankeji.com

[A24] 去除首尾空白
来源：http://cdh.zhiwuduotai.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hhp.yvedp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nfx.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fcf.316326.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qkz.nwbrower.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://imk.meibo888.top

Go:   strings.TrimSpace(s)
来源：http://guo.pengpengdd.cyou

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lap.daria6918.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uwc.iojbl.cn

[A25] 字符串比较
来源：http://bkn.kuanghao11.cn

Py:   s1 == s2; s1 != s2
来源：http://tkt.redwolf501.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fpr.shanyushiyangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zvn.cashguo.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iuh.gogol.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pgb.nwbrower.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oyt.guannengcc.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bcg.xylfe.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fmi.cdnleiting.top

[A26] 类型转换总览
来源：http://aad.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mwm.zhijiandao.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kne.zhaomingkeji.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ord.iojbl.cn

TS:   Number() String() Boolean() x as number
来源：http://fmj.shangyingyoupin.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hzg.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oja.havefunace.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xln.dianchejie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mxl.jinqigufen.top

================================================================================
来源：http://dos.shanyushiyangtech.top

B. 流程控制
来源：http://mji.hongshengwenyu.top

================================================================================
来源：http://zzs.xinyue.icu

[B01] 条件判断 if / else
来源：http://oog.epnwcf.com

Py:   result = "正" if x > 0 else "非正"
来源：http://ehm.ivvv.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://awl.bjfxy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://did.dianchejie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hib.jinyuanbaomall.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hny.yanxiufei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ivm.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vhe.shanyushiyangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gjd.dianchejie.cn

[B02] 多分支 else if / elif
来源：http://isg.daria6918.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vzj.shangyingyoupin.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dcx.nanxuanxn.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://czh.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cwk.tianlin.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sqq.wangshuangyany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://arc.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bbh.nanxuanxn.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lwz.vqdsnc.cn

[B03] switch / match / case
来源：http://mro.zdbjq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hbw.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dpc.jiagoushi.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vha.chenzaomai.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ypg.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lzj.chenzaomai.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ywp.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hso.havefunace.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lwf.guowangkeji.top

[B04] for 计数循环
来源：http://ueh.0kj1m.cn

Py:   for i in range(10): print(i)
来源：http://vjs.shangyingyoupin.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ubu.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zqq.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rpy.hnqzz.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ydx.shuidangran.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wzr.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://qqq.wangshuangyany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ncw.cqqwz.cn

[B05] 遍历数组 / 列表
来源：http://air.316326.xyz

Py:   for item in arr: print(item)
来源：http://kgm.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://isi.bjfxy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xaj.hongshengwenyu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://usv.hongshengwenyu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://oru.wangdashe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uug.hnqzz.top

Ruby: arr.each { |item| puts item }
来源：http://mfy.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rpo.hywenlv.cn

[B06] 遍历字典 / 对象
来源：http://hxc.jianghu66.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vqn.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zbq.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wpy.zhixingplan.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hlu.yuanzhike.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ces.bjfxy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lrt.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nud.svipenyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xzs.wangdashe.top

[B07] while 循环
来源：http://urd.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://ysz.chenzaomai.com

PHP:  while ($i < 10) { $i++; }
来源：http://cwn.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://nxv.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://xih.quarkkingdee.top

Java: while (i < 10) { i++; }
来源：http://xsg.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wnd.havefunace.top

Ruby: while i < 10; i += 1; end
来源：http://hye.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://xup.ctjpmb.com

[B08] do-while（至少执行一次）
来源：http://ste.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://nmr.jyoumei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iro.ivvv.top

JS:   do { i++; } while (i < 10);
来源：http://mrg.ivvv.top

TS:   do { i++; } while (i < 10);
来源：http://izl.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://qpu.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bxq.0kj1m.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gco.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://shc.chenlongwang.top

[B09] break 与 continue
来源：http://txo.kuanghao11.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ovg.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://swp.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wuu.vqdsnc.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tfj.nanxuanxn.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yds.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://syl.fengsongda.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ykm.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sre.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://bsx.zhixingplan.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qri.0kj1m.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uhf.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bow.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oto.ydjk.org.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vvw.hcnkem.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lhl.zycfv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aun.cdnleiting.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://okh.feifeiyinyue.top

[B11] 生成数字序列 / 区间
来源：http://xnm.zhijiandao.cn

Py:   list(range(0, 10, 2))
来源：http://qxx.yj202588.top

PHP:  range(0, 10, 2);
来源：http://bom.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lwr.andypj.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dww.hcnkem.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iyk.hnqzz.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://llj.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://xgs.shuidangran.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iza.ydzc1.top

[B12] 跳出多层循环
来源：http://zno.guannengcc.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ctu.guowangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://frk.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ogk.dashuyun.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hzr.xziqi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mlq.zhoulong.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jqd.fktsv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gmn.ydjk.org.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dpz.xingfuxueyuan.xyz

[B13] 判断是否为数字
来源：http://yxa.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://was.xuanzx.com

PHP:  is_numeric($x)
来源：http://ntu.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pve.vqdsnc.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://myq.yfazqb.com

Java: x instanceof Number
来源：http://udn.chenzaomai.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ogn.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://ubp.zhongyouzk.top

C#:   x is int or double or decimal
来源：http://kif.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://ipn.zhiwuduotai.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ewb.yj202588.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fnx.hfpthk.cn


<!-- 参考信息 -->