代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://hre.52xcode.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://haz.cdnleiting.top

C#:   x.GetType().Name; x is int
来源：http://hbe.cdnleiting.top

[A05] 整数除法与取模
来源：http://isu.ydjk.org.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://out.hesvh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ccf.yongpay.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bxj.jiagoushi.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lqe.ehwqpu.com

Java: 7 / 2; 7 % 2
来源：http://kdw.ctjpmb.com

Go:   7 / 2; 7 % 2
来源：http://erh.hesvh.cn

Ruby: 7 / 2; 7 % 2
来源：http://dun.cucudq.cn

C#:   7 / 2; 7 % 2
来源：http://uok.andypj.xyz

[A06] 字符串转数字
来源：http://nxg.ybcxt.top

Py:   int("42"); float("3.14")
来源：http://xhi.jiagoushi.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://spu.yj20258888.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fca.ybcxt.top

TS:   parseInt("42", 10); Number("42")
来源：http://jxd.shangyingyoupin.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qep.fanxiaobao.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://znv.cdnleiting.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xny.xingfuxueyuan.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nqx.jqgfzy.top

[A07] 数字转字符串
来源：http://tjb.cheryme.top

Py:   str(42)
来源：http://kvk.yfazqb.com

PHP:  (string) 42; strval(42)
来源：http://mmp.sjlbkw.cn

JS:   String(42); (42).toString()
来源：http://exd.hongshengwenyu.top

TS:   String(42)
来源：http://aok.ybcxt.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://fdy.ctjpmb.com

Go:   strconv.Itoa(42)
来源：http://goc.fanxiaobao.xyz

Ruby: 42.to_s
来源：http://inp.ybcxt.top

C#:   42.ToString()
来源：http://css.ywan-chungtsiang.top

[A08] 取整与四舍五入
来源：http://lhd.xinyue.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kga.hnxiangtu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gdc.snrcjt.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xpn.hongshengwenyu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kkk.cqqwz.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bwu.daria6918.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://inv.daxiang520.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://psk.zhengqikj.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qwd.yanxiufei.cn

[A09] 绝对值与最大最小值
来源：http://evb.zhixingplan.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vkr.xingfuxueyuan.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lkx.pycfn.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nmo.pycfn.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://aqj.bbcook.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://arx.cqqwz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fyo.jyoumei.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gdh.yueranfly.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cmo.dashuyun.cn

[A10] 生成随机数
来源：http://qdp.gogol.net.cn

Py:   import random; random.randint(1, 100)
来源：http://pje.chenzaomai.com

PHP:  random_int(1, 100);
来源：http://twr.sweek.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mqf.hcnkem.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://clt.jinqigufen.top

Java: new Random().nextInt(100) + 1
来源：http://fuh.ppjwa.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xox.hywenlv.cn

Ruby: rand(1..100)
来源：http://ffo.daxiang520.top

C#:   new Random().Next(1, 101)
来源：http://jcc.xziqi.cn

[A11] 条件表达式（三元）
来源：http://wxl.redwolf501.top

Py:   "yes" if x > 0 else "no"
来源：http://fmq.jinqigufen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://tks.daxiang520.top

JS:   x > 0 ? "yes" : "no"
来源：http://knw.fengsongda.top

TS:   x > 0 ? "yes" : "no"
来源：http://deu.yonumen.top

Java: x > 0 ? "yes" : "no"
来源：http://ukd.wangshuangyany.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hnj.gotoacloud.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ryw.daxiang520.top

C#:   x > 0 ? "yes" : "no"
来源：http://iwr.zhongyouzk.top

[A12] 字符串插值 / 格式化
来源：http://cbt.pycfn.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vgk.gogol.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yax.jinghuilouyu.cn

JS:   `Hello, ${name}!`
来源：http://rlf.pycfn.com

TS:   `Hello, ${name}!`
来源：http://dyp.hongshengwenyu.top

Java: "Hello, %s!".formatted(name)
来源：http://dln.jinqigfzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yys.havefunace.top

Ruby: "Hello, #{name}!"
来源：http://toi.jinqigufen.top

C#:   $"Hello, {name}!"
来源：http://fro.cucudq.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sry.cheryme.top

Py:   "第一行\n第二行"
来源：http://pcb.jqgufenzy.top

PHP:  "第一行\n第二行"
来源：http://swl.pycfn.com

JS:   "第一行\n第二行"
来源：http://ovi.iojbl.cn

TS:   "第一行\n第二行"
来源：http://wwh.cucudq.cn

Java: "第一行\n第二行"
来源：http://dsn.nanxinkj.top

Go:   "第一行\n第二行"
来源：http://esv.jqgfzy.top

Ruby: "第一行\n第二行"
来源：http://ttu.yangfankeji.com

C#:   "第一行\n第二行"
来源：http://wqo.ppjwa.cn

[A14] 注释写法
来源：http://ngk.gaohongyu789.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://jri.hesvh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ewt.aibaodan.cn

JS:   // 单行；/* 多行 */
来源：http://tlg.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://xkx.0kj1m.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xng.nanxinkj.top

Go:   // 单行；/* 多行 */
来源：http://ser.haohaochexian.top

Ruby: # 单行；=begin 多行 =end
来源：http://rcm.9152youxi.cn

C#:   // 单行；/* 多行 */
来源：http://gwb.daria6918.cn

[A15] 空值判断与默认值
来源：http://pjo.tianlin.xyz

Py:   value = data or "默认值"
来源：http://uvj.316326.xyz

PHP:  $value = $data ?? "默认值";
来源：http://ivg.hesvh.cn

JS:   const value = data ?? "默认值";
来源：http://gir.jyoumei.cn

TS:   const value = data ?? "默认值";
来源：http://uys.hysaishi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cam.birdmap.top

Go:   if data == "" { data = "默认值" }
来源：http://qse.tianlin.xyz

Ruby: value = data || "默认值"
来源：http://hvk.hnqzz.top

C#:   var value = data ?? "默认值";
来源：http://vrd.yj20258888.top

[A16] 真假值判断规则
来源：http://mxd.yanxiufei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ate.andypj.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://txw.zhixingplan.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zcs.ydjk.org.cn

TS:   if (!x) {}
来源：http://god.xingfuxueyuan.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jlx.xinyue.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ian.aizwys.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jdz.dashuyun.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zzr.zhoulong.xyz

[A17] 位运算
来源：http://vch.chenzaomai.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kzp.shanyushiyangkeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ybv.svipenyu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://btv.hnxiangtu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://veu.mhx1999.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nod.chenjidiqi.icu

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jwq.hnqzz.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://klq.tianlin.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gsg.zhaomingkeji.xyz

[A18] 字符与 ASCII 码互转
来源：http://qyp.yangfankeji.com

Py:   ord("A"); chr(65)
来源：http://rsv.zhiwuduotai.top

PHP:  ord("A"); chr(65)
来源：http://hch.hnxiangtu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hqa.tianlin.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pna.xziqi.cn

Java: (int) 'A'; (char) 65
来源：http://mci.zhijiandao.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ipz.gogol.net.cn

Ruby: "A".ord; 65.chr
来源：http://ear.cashguo.top

C#:   (int)'A'; (char)65
来源：http://wmw.yj202588.top

[A19] 交换两个变量
来源：http://kix.fengsongda.top

Py:   a, b = b, a
来源：http://kfu.sweek.top

PHP:  [$a, $b] = [$b, $a];
来源：http://txk.yangfankeji.com

JS:   [a, b] = [b, a];
来源：http://vcj.jqgufenzy.top

TS:   [a, b] = [b, a];
来源：http://tlt.gotoacloud.top

Java: int t = a; a = b; b = t;
来源：http://dty.sweek.top

Go:   a, b = b, a
来源：http://lti.yuanzhike.top

Ruby: a, b = b, a
来源：http://uzn.dianchejie.cn

C#:   (a, b) = (b, a);
来源：http://hyz.xuanzx.com

[A20] 读取标准输入
来源：http://sqi.hongshengwenyu.top

Py:   name = input("请输入：")
来源：http://txe.nanxinkj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://hma.shanyushiyangtech.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zyb.ydjk.org.cn

TS:   // Node.js：readline 模块
来源：http://yfc.dashuyun.cn

Java: new Scanner(System.in).nextLine()
来源：http://fus.ivvv.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ljl.tanke756.top

Ruby: gets.chomp
来源：http://zgq.tian-w.cn

C#:   Console.ReadLine();
来源：http://hbt.shangyingyoupin.top

[A21] 保留指定小数位输出
来源：http://bnh.jinqigfzy.top

Py:   f"{3.14159:.2f}"
来源：http://kct.jinqigfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bfc.gaohongyu789.top

JS:   (3.14159).toFixed(2)
来源：http://qhr.jinqigufen.top

TS:   (3.14159).toFixed(2)
来源：http://jpb.xuanzx.com

Java: String.format("%.2f", 3.14159)
来源：http://bid.zhixingplan.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dzq.guowangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://igc.chenlongwang.top

C#:   3.14159.ToString("F2")
来源：http://tov.chenjidiqi.icu

[A22] 获取字符串长度
来源：http://crb.yj20258888.top

Py:   len(s)
来源：http://pfd.pycfn.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nwy.52xcode.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bdm.andypj.xyz

TS:   s.length
来源：http://atg.hywenlv.cn

Java: s.length()
来源：http://aoj.gzhubu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xlq.gotoacloud.top

Ruby: s.length
来源：http://mhd.guannengcc.top

C#:   s.Length
来源：http://qtq.jianghu66.top

[A23] 大小写转换
来源：http://ixz.birdmap.top

Py:   s.upper(); s.lower(); s.title()
来源：http://aty.zdbjq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iuc.ivvv.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wbw.yuxming.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://faz.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jev.ctjpmb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rox.zhijiandao.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lhe.feifeiyinyue.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kyj.wangshuangyany.cn

[A24] 去除首尾空白
来源：http://pjl.andypj.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jvl.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lbw.dianchejie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fcz.feifeiyinyue.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dko.sufxvd.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hzo.yonumen.top

Go:   strings.TrimSpace(s)
来源：http://zzm.meibo888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://elz.xingfuxueyuan.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pjv.hnqzz.top

[A25] 字符串比较
来源：http://tkh.yuxming.cn

Py:   s1 == s2; s1 != s2
来源：http://vqk.tian-w.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://opp.hcnkem.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jse.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ghz.jlsjyb.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zaf.52xcode.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ocv.jinqigufen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jwi.zhixingplan.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wxo.ehwqpu.com

[A26] 类型转换总览
来源：http://oug.redwolf501.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mwx.cdnleiting.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sxb.zhaomingkeji.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rva.nwbrower.top

TS:   Number() String() Boolean() x as number
来源：http://uvs.snrcjt.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mzs.chenjidiqi.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://izw.birdmap.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rdy.zhijiandao.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rac.zdbjq.cn

================================================================================
来源：http://jou.pycfn.com

B. 流程控制
来源：http://blw.jinqigufen.top

================================================================================
来源：http://qiv.xingfuxueyuan.xyz

[B01] 条件判断 if / else
来源：http://czz.hammf.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jmo.shanyushiyangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zer.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vdp.jinghuilouyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qvh.xingfuxueyuan.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://pcv.jyoumei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vgj.iojbl.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fpo.ywan-chungtsiang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hiu.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://npn.hammf.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://see.gotoacloud.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eud.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hdl.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dxi.chenzaomai.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://raq.bbcook.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pvb.ybcxt.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oiu.shzxlz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xin.jqgfzy.top

[B03] switch / match / case
来源：http://tih.yongpay.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nsy.shangyingyoupin.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zbb.316326.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pbn.tarul.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lwj.hongshengwenyu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gns.cheryme.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zox.xingfuxueyuan.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://htg.yuanzhike.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rmr.nwbrower.top

[B04] for 计数循环
来源：http://akp.zdbjq.cn

Py:   for i in range(10): print(i)
来源：http://fwc.zhengqikj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jwr.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bvj.andypj.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ljw.yanxiufei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tlw.daria6918.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zeb.jyoumei.cn

Ruby: 10.times { |i| puts i }
来源：http://wrm.hongshengwenyu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://klq.zdqjudy.top

[B05] 遍历数组 / 列表
来源：http://uzk.nanxuanxn.top

Py:   for item in arr: print(item)
来源：http://zqj.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ygt.316326.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://wqb.smart0.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://ucg.shzxlz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://swj.nanxuanxn.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ore.316326.xyz

Ruby: arr.each { |item| puts item }
来源：http://cxc.jianghu66.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bvh.yongpay.top

[B06] 遍历字典 / 对象
来源：http://wzo.shzxlz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oul.yj202588.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fdv.mhx1999.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vnj.fzhhl.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iui.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://swx.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://whp.xuetiantiany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fcu.yfazqb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xfh.sufxvd.cn

[B07] while 循环
来源：http://ove.gotoacloud.top

Py:   while i < 10: i += 1
来源：http://elf.ydzc1.top

PHP:  while ($i < 10) { $i++; }
来源：http://ojm.shuidangran.top

JS:   while (i < 10) { i++; }
来源：http://jpp.bjfxy.top

TS:   while (i < 10) { i++; }
来源：http://rsd.jinghuilouyu.cn

Java: while (i < 10) { i++; }
来源：http://klx.aizwys.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vew.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://ggx.xuetiantiany.cn

C#:   while (i < 10) { i++; }
来源：http://jzx.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://uel.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://mld.316326.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://iso.svipenyu.cn

JS:   do { i++; } while (i < 10);
来源：http://xfg.bjfxy.top

TS:   do { i++; } while (i < 10);
来源：http://mzn.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://gug.sweek.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qki.yj20258888.top

Ruby: begin; i += 1; end while i < 10
来源：http://xqr.jyoumei.cn

C#:   do { i++; } while (i < 10);
来源：http://xjk.ctjpmb.com

[B09] break 与 continue
来源：http://poq.cucudq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iyf.fanxiaobao.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xzo.zdqjudy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nuh.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mhf.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eyr.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iyj.vehdjk.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://liu.tarul.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cpf.ppjwa.cn

[B10] 遍历同时拿索引
来源：http://enp.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://isz.ydjk.org.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mmz.ppjwa.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ayb.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://esl.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wbq.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kru.aizwys.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zut.yj20258888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fpa.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://xha.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://osc.yangfankeji.com

PHP:  range(0, 10, 2);
来源：http://epi.daria6918.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xcp.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://inx.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eqt.yuxming.cn


<!-- 参考信息 -->