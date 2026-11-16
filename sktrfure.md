代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://dpl.nwbrower.top

Ruby: arr.include?(x)
来源：http://qwx.yj20258.top

C#:   list.Contains(x)
来源：http://hfr.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://zmr.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lyv.cucudq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ttw.chenjidiqi.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ixw.chenlongwang.top

TS:   [...arr];
来源：http://nav.pycfn.com

Java: new ArrayList<>(list);
来源：http://kme.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://nnc.quarkkingdee.top

Ruby: arr.dup;  arr.clone
来源：http://qsl.yuanzhike.top

C#:   new List<int>(list);
来源：http://vax.fzhhl.top

[D23] reduce 累积计算
来源：http://iii.guannengcc.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ohx.redwolf501.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fgj.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hfb.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://krn.smart0.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://zrd.kuanghao11.cn

Go:   // 手写循环
来源：http://czv.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://leo.cheryme.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bmz.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://fra.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rds.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nrb.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xag.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ugi.zhengqikj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gss.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pnr.fanxiaobao.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nvj.ehwqpu.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tjx.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://oql.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nwc.yj20258888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pxu.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ubh.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wio.ywan-chungtsiang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ibl.yj202588.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pkl.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mfr.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://act.vqdsnc.cn

[D26] 数组转字符串
来源：http://trm.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://alb.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://veq.shangyingyoupin.top

JS:   arr.join(", ")
来源：http://bql.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://ffh.tanke756.top

Java: String.join(", ", list)
来源：http://qyt.jyoumei.cn

Go:   strings.Join(strs, ", ")
来源：http://qea.hfpthk.cn

Ruby: arr.join(", ")
来源：http://obs.tarul.cn

C#:   string.Join(", ", list)
来源：http://tpx.jinyuanbaomall.cn

================================================================================
来源：http://wob.xinyue.icu

E. 字符串处理
来源：http://wga.jinqigufen.top

================================================================================
来源：http://omg.yonumen.top

[E01] 拼接字符串
来源：http://ypq.havefunace.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fhe.shanyushiyangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uym.yonumen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mag.dashuyun.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zgi.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://flt.nanxinkj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zxj.zycfv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://att.fengsongda.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ehp.xylfe.cn

[E02] 重复字符串
来源：http://qwx.shangyingyoupin.top

Py:   "ab" * 3
来源：http://wxr.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://kii.mhx1999.top

JS:   "ab".repeat(3)
来源：http://ram.hywenlv.cn

TS:   "ab".repeat(3)
来源：http://kdu.yueranfly.top

Java: "ab".repeat(3)
来源：http://rwz.sufxvd.cn

Go:   strings.Repeat("ab", 3)
来源：http://hhn.yj202588.top

Ruby: "ab" * 3
来源：http://tsm.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eqd.zhongyouzk.top

[E03] 截取子串
来源：http://pkp.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://syo.316326.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uaj.daxiang520.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://myl.chenzaomai.com

TS:   s.slice(1, 4)
来源：http://ygr.shuidangran.top

Java: s.substring(1, 4)
来源：http://ikj.zhiwuduotai.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fge.cdnleiting.top

Ruby: s[1, 3];  s[1..3]
来源：http://osx.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://nov.cashguo.top

[E04] 查找子串位置
来源：http://hoz.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://prp.hywenlv.cn

PHP:  strpos($s, "x");
来源：http://naf.c1oappe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bxm.sweek.top

TS:   s.indexOf("x")
来源：http://ycd.52xcode.cn

Java: s.indexOf("x")
来源：http://haf.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://esw.dashuyun.cn

Ruby: s.index("x")
来源：http://rnr.ivvv.top

C#:   s.IndexOf("x")
来源：http://feb.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mgv.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://efd.xuetiantiany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pbi.yanxiufei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lqr.jinyuanbaomall.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ohm.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xje.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://smi.xuanzx.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://krc.zhengqikj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ost.sweek.top

[E06] 替换子串
来源：http://urm.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kxl.fktsv.cn

PHP:  str_replace("a", "b", $s);
来源：http://tnm.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ulp.havefunace.top

TS:   s.replaceAll("a", "b")
来源：http://ldm.svipenyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fmy.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zoc.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rnv.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://tao.zhaomingkeji.xyz

[E07] 按分隔符拆分
来源：http://wfs.quarkkingdee.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cdq.wangdashe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xkn.ivvv.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mrw.jinghuilouyu.cn

TS:   s.split(",")
来源：http://ile.bbcook.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cmz.fzhhl.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zxu.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://bkh.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pxj.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://ewf.cdnleiting.top

Py:   ",".join(items)
来源：http://hkb.guowangkeji.top

PHP:  implode(",", $items);
来源：http://lcq.shzxlz.cn

JS:   items.join(",")
来源：http://ztq.vqdsnc.cn

TS:   items.join(",")
来源：http://dgr.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://any.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://eqx.tanke756.top

Ruby: items.join(",")
来源：http://chs.svipenyu.cn

C#:   string.Join(",", items)
来源：http://ggw.ctjpmb.com

[E09] 去除所有空白字符
来源：http://orl.shangyingyoupin.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pux.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://utp.gzhubu.top

JS:   s.replace(/\s+/g, "")
来源：http://heg.zhaomingkeji.xyz

TS:   s.replace(/\s+/g, "")
来源：http://bnb.pengpengdd.cyou

Java: s.replaceAll("\\s+", "")
来源：http://pxx.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tvz.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://qbm.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jpr.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://pvc.daria6918.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qvr.yanxiufei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ghw.hywenlv.cn

JS:   "7".padStart(3, "0")
来源：http://xbc.ydzc1.top

TS:   "7".padStart(3, "0")
来源：http://ide.yj20258.top

Java: String.format("%03d", 7)
来源：http://opl.xziqi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mwz.chenzaomai.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lya.mhx1999.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kup.yj20258.top

[E11] 反转字符串
来源：http://zyw.sjlbkw.cn

Py:   s[::-1]
来源：http://wng.sufxvd.cn

PHP:  strrev($s);
来源：http://cmx.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://mre.tianlin.xyz

TS:   [...s].reverse().join("")
来源：http://big.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ysj.feifeiyinyue.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kyk.xylfe.cn

Ruby: s.reverse
来源：http://tei.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://vcr.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://wci.zdqjudy.top

Py:   s.count("a")
来源：http://att.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://ccs.xylfe.cn

JS:   s.split("a").length - 1
来源：http://rkv.ybcxt.top

TS:   s.split("a").length - 1
来源：http://ikq.shangyingyoupin.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yyq.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://ipu.jinqigufen.top

Ruby: s.count("a")
来源：http://cmc.zhijiandao.cn

C#:   s.Count(c => c == 'a')
来源：http://von.yfazqb.com

[E13] 逐字符遍历
来源：http://dde.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://phk.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oqs.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ktv.pycfn.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://acc.jinqigufen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hru.shzxlz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ggh.ctjpmb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://eiu.redwolf501.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://icj.52xcode.cn

[E14] URL 编码与 Base64
来源：http://orv.xuanzx.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hrt.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://don.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xbs.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://slw.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://djs.yj20258888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ncs.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cee.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zzr.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://dik.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://gjw.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pqy.tianlin.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lnd.yuxming.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nqt.guowangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mcx.yj20258.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qnj.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://due.pengpengdd.cyou

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rcv.uphjek.com

[E16] 数字千分位
来源：http://iam.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://oxj.uphjek.com

PHP:  number_format(1234567);
来源：http://vre.andypj.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://joq.yuanzhike.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wdn.wangshuangyany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jvy.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oqj.yvedp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tgp.cheryme.top

C#:   1234567.ToString("N0")
来源：http://nrp.kuanghao11.cn

[E17] 首字母大写
来源：http://uil.zycfv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://erk.zhoulong.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://vhb.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tlf.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vga.epnwcf.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kla.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ynt.sysykeji.top

Ruby: s.capitalize
来源：http://pen.cucudq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rys.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://had.vehdjk.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xij.yj20258.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ypy.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vkx.shanyushiyangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ekz.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qvg.hcnkem.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jcm.yuxming.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://erf.zhaomingkeji.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qyc.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://dmd.smart0.xyz

Py:   s.splitlines()
来源：http://ois.hfpthk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vvl.shanyushiyangkeji.top

JS:   s.split(/\r?\n/)
来源：http://ovq.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://suh.smart0.xyz

Java: s.lines().toList()
来源：http://maq.chenzaomai.com

Go:   strings.Split(s, "\n")
来源：http://deh.sjlbkw.cn

Ruby: s.lines
来源：http://bgo.zycfv.cn

C#:   s.Split('\n')
来源：http://fcl.cucudq.cn

[E20] 判断字符串是否为空
来源：http://cxx.hnqzz.top

Py:   if not s:
来源：http://sxh.fanxiaobao.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://agr.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fmc.hammf.cn

TS:   if (s === "") {}
来源：http://yol.yuanzhike.top

Java: if (s.isEmpty()) {}
来源：http://otp.tianlin.xyz

Go:   if s == "" {}
来源：http://igu.zhoulong.xyz

Ruby: if s.empty?
来源：http://bmq.daxiang520.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qxx.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://rwg.52xcode.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ars.zhoulong.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ddh.hysaishi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sef.yanxiufei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://htc.zhijiandao.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qlr.xuetiantiany.cn

Go:   // 按 rune 判断长度后截断
来源：http://zrz.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://olv.chenlongwang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ylf.iojbl.cn

[E22] 字节长度与字符长度
来源：http://sfx.chenzaomai.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bex.tian-w.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sqb.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://odx.fehbvm.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xdr.cashguo.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://acg.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hfp.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://jtk.xinyue.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mla.nwbrower.top

================================================================================
来源：http://tup.gotoacloud.top

F. 文件与目录
来源：http://gya.zhijiandao.cn

================================================================================
来源：http://cdf.jqgufenzy.top

[F01] 读取整个文件
来源：http://amo.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bnr.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://xpd.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://euu.sjlbkw.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vqk.pengpengdd.cyou

Java: Files.readString(Path.of("a.txt"))
来源：http://lnf.yueranfly.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mnq.daria6918.cn

Ruby: File.read("a.txt")
来源：http://cvk.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://qau.nanxuanxn.top

[F02] 逐行读取文件
来源：http://kqo.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oxm.chenjidiqi.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tai.gotoacloud.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vcw.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oyh.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tst.zhaomingkeji.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xcz.hcnkem.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ord.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rfp.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://htr.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://air.wangdashe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pbr.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mmr.gaohongyu789.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wvz.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gle.jiagoushi.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://usr.zhijiandao.cn

Ruby: File.write("a.txt", "hi")
来源：http://nst.hammf.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eak.gotoacloud.top

[F04] 追加写入文件
来源：http://mcz.redwolf501.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zkx.9152youxi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vbj.haohaochexian.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vlf.yuxming.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cen.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lkt.fzhhl.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pmz.pycfn.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jjv.chenlongwang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vhm.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://qqo.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sdh.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://bbp.cheryme.top

JS:   fs.existsSync("a.txt")
来源：http://tur.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://erl.xziqi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oqp.zhoulong.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://unh.redwolf501.top

Ruby: File.exist?("a.txt")
来源：http://spm.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://hgy.jianghu66.top

[F06] 删除文件
来源：http://shp.xylfe.cn

Py:   os.remove("a.txt")
来源：http://ihp.mhx1999.top

PHP:  unlink("a.txt");
来源：http://lwl.quarkkingdee.top


<!-- 参考信息 -->