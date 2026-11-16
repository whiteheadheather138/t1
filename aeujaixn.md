代发 wailian999

Ruby: arr.tally
来源：http://ibr.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://udr.yuxming.cn

[D21] 判断是否包含某元素
来源：http://hwg.xingfuxueyuan.xyz

Py:   x in arr
来源：http://omo.shangyingyoupin.top

PHP:  in_array($x, $arr, true);
来源：http://ytl.haohaochexian.top

JS:   arr.includes(x)
来源：http://gye.daria6918.cn

TS:   arr.includes(x)
来源：http://imq.shangyingyoupin.top

Java: list.contains(x)
来源：http://mso.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://jec.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://xur.jinqigfzy.top

C#:   list.Contains(x)
来源：http://hoq.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://iab.uphjek.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tev.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xzw.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nqo.fzhhl.top

TS:   [...arr];
来源：http://ydx.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://cmg.gzhubu.top

Go:   copied := append([]int(nil), arr...)
来源：http://hje.aibaodan.cn

Ruby: arr.dup;  arr.clone
来源：http://nqr.sjlbkw.cn

C#:   new List<int>(list);
来源：http://jku.pycfn.com

[D23] reduce 累积计算
来源：http://ave.ywan-chungtsiang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://srk.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jxh.c1oappe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tto.shanyushiyangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jwn.52xcode.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sni.jinqigfzy.top

Go:   // 手写循环
来源：http://raq.xingfuxueyuan.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fwh.9152youxi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://slx.gogol.net.cn

[D24] 字典 / Map 基本操作
来源：http://ogu.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hym.chenzaomai.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vzk.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hbu.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nfd.yanxiufei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rhz.cheryme.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://olw.hnqzz.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gzl.ivvv.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cgz.zhoulong.xyz

[D25] Set 集合去重与交并差
来源：http://ody.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qfv.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rye.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gyv.xziqi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ouj.hfpthk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://afo.daria6918.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ytk.tanke756.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xeo.snrcjt.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tmv.hcnkem.com

[D26] 数组转字符串
来源：http://yop.jianghu66.top

Py:   ", ".join(map(str, arr))
来源：http://blv.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://poj.nwbrower.top

JS:   arr.join(", ")
来源：http://wgo.pengpengdd.cyou

TS:   arr.join(", ")
来源：http://znw.tanke756.top

Java: String.join(", ", list)
来源：http://sou.gzhubu.top

Go:   strings.Join(strs, ", ")
来源：http://csm.fzhhl.top

Ruby: arr.join(", ")
来源：http://slq.epnwcf.com

C#:   string.Join(", ", list)
来源：http://gyj.feifeiyinyue.top

================================================================================
来源：http://lzt.gogol.net.cn

E. 字符串处理
来源：http://vhb.vqdsnc.cn

================================================================================
来源：http://ein.smart0.xyz

[E01] 拼接字符串
来源：http://zmo.52xcode.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ctd.ctjpmb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oyd.9152youxi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xcv.ehwqpu.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ykl.meibo888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cwh.daxiang520.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://afe.xylfe.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cyt.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zlz.ydjk.org.cn

[E02] 重复字符串
来源：http://ora.shanyushiyangtech.top

Py:   "ab" * 3
来源：http://myv.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://ndz.wangdashe.top

JS:   "ab".repeat(3)
来源：http://hdx.gogol.net.cn

TS:   "ab".repeat(3)
来源：http://ufe.sufxvd.cn

Java: "ab".repeat(3)
来源：http://ncd.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://pcr.guowangkeji.top

Ruby: "ab" * 3
来源：http://dyr.meibo888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://htc.xuetiantiany.cn

[E03] 截取子串
来源：http://vhf.chenlongwang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gmj.havefunace.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qla.ydzc1.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mhw.meibo888.top

TS:   s.slice(1, 4)
来源：http://fzc.nwbrower.top

Java: s.substring(1, 4)
来源：http://rke.aibaodan.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qoy.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://ykj.havefunace.top

C#:   s.Substring(1, 3)
来源：http://gwp.shuidangran.top

[E04] 查找子串位置
来源：http://kpq.chenlongwang.top

Py:   s.find("x");  s.index("x")
来源：http://wqu.sweek.top

PHP:  strpos($s, "x");
来源：http://wui.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hvi.zhongyouzk.top

TS:   s.indexOf("x")
来源：http://bmo.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://lrt.chenlongwang.top

Go:   strings.Index(s, "x")
来源：http://bqs.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://ulp.guannengcc.top

C#:   s.IndexOf("x")
来源：http://gwt.hywenlv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iyq.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mni.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sag.xingfuxueyuan.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gih.xylfe.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rgi.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xxt.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ocd.kuanghao11.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iwe.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iik.hnqzz.top

[E06] 替换子串
来源：http://hso.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zse.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://wmd.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vhb.316326.xyz

TS:   s.replaceAll("a", "b")
来源：http://kvo.xziqi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://brs.bjfxy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eke.zhixingplan.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vwo.epnwcf.com

C#:   s.Replace("a", "b")
来源：http://dwz.316326.xyz

[E07] 按分隔符拆分
来源：http://smn.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ido.tian-w.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dzf.sysykeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wuw.zhixingplan.top

TS:   s.split(",")
来源：http://ved.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ezi.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pnn.shuidangran.top

Ruby: s.split(",");  s.split
来源：http://olx.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kys.smart0.xyz

[E08] 数组按分隔符合并
来源：http://zwm.sufxvd.cn

Py:   ",".join(items)
来源：http://oek.smart0.xyz

PHP:  implode(",", $items);
来源：http://rjp.zhongyouzk.top

JS:   items.join(",")
来源：http://iag.mhx1999.top

TS:   items.join(",")
来源：http://jez.xziqi.cn

Java: String.join(",", items)
来源：http://rms.tian-w.cn

Go:   strings.Join(items, ",")
来源：http://ten.tarul.cn

Ruby: items.join(",")
来源：http://ert.gaohongyu789.top

C#:   string.Join(",", items)
来源：http://rmf.52xcode.cn

[E09] 去除所有空白字符
来源：http://sqz.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tox.fehbvm.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ngo.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://lsf.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://jan.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://une.xinyue.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://esj.ehwqpu.com

Ruby: s.gsub(/\s+/, "")
来源：http://ikj.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://srq.xuanzx.com

[E10] 左侧补零 / 定长填充
来源：http://eqm.dashuyun.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yvv.sxryk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rdb.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://nvo.zhijiandao.cn

TS:   "7".padStart(3, "0")
来源：http://rya.yj202588.top

Java: String.format("%03d", 7)
来源：http://hez.zdbjq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://eld.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fsi.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mhk.zhijiandao.cn

[E11] 反转字符串
来源：http://edc.chenjidiqi.icu

Py:   s[::-1]
来源：http://ruf.hnqzz.top

PHP:  strrev($s);
来源：http://rgf.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://nwj.yj202588.top

TS:   [...s].reverse().join("")
来源：http://cqf.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gdm.zdbjq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://epj.yangfankeji.com

Ruby: s.reverse
来源：http://qkj.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wnk.zhongyouzk.top

[E12] 统计某字符出现次数
来源：http://fcx.shzxlz.cn

Py:   s.count("a")
来源：http://vsm.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://ufg.jqgufenzy.top

JS:   s.split("a").length - 1
来源：http://xwl.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://xvy.sysykeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vhu.jqgufenzy.top

Go:   strings.Count(s, "a")
来源：http://tyb.yfazqb.com

Ruby: s.count("a")
来源：http://gif.fzhhl.top

C#:   s.Count(c => c == 'a')
来源：http://xti.nanxuanxn.top

[E13] 逐字符遍历
来源：http://nff.ybcxt.top

Py:   for ch in s: print(ch)
来源：http://tdv.quarkkingdee.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://khq.xinyue.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://uut.jqgufenzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zue.xuanzx.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uuq.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kte.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://jdv.wangshuangyany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gfa.jianghu66.top

[E14] URL 编码与 Base64
来源：http://oba.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lqf.snrcjt.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ozw.fengsongda.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xdw.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oai.wangshuangyany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zxj.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fyq.vehdjk.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://llf.52xcode.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lqa.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://tdu.cheryme.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ioe.chenjidiqi.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ana.gaohongyu789.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://msu.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://irg.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://occ.zhixingplan.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ava.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fiv.yueranfly.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cfo.316326.xyz

[E16] 数字千分位
来源：http://mrd.bjfxy.top

Py:   f"{1234567:,}"
来源：http://rxg.meibo888.top

PHP:  number_format(1234567);
来源：http://qif.pycfn.com

JS:   (1234567).toLocaleString("en-US")
来源：http://uli.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://sog.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aaj.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://otp.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lyt.sxryk.cn

C#:   1234567.ToString("N0")
来源：http://ode.ydzc1.top

[E17] 首字母大写
来源：http://gfq.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xip.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dnh.yongpay.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://evh.xingfuxueyuan.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://biu.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wzc.xuanzx.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://use.yj202588.top

Ruby: s.capitalize
来源：http://hzj.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lej.chenjidiqi.icu

[E18] 模板占位符替换
来源：http://zqb.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dwh.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xeb.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://myc.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hbg.hysaishi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wqh.wangshuangyany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ukf.aibaodan.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kgx.yj202588.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rkk.bjfxy.top

[E19] 多行文本按行拆分
来源：http://ozm.sjlbkw.cn

Py:   s.splitlines()
来源：http://mvq.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://giq.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://hai.zdqjudy.top

TS:   s.split(/\r?\n/)
来源：http://xzr.sweek.top

Java: s.lines().toList()
来源：http://csd.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://qlj.cqqwz.cn

Ruby: s.lines
来源：http://rby.cdnleiting.top

C#:   s.Split('\n')
来源：http://lmz.jinqigfzy.top

[E20] 判断字符串是否为空
来源：http://ynb.andypj.xyz

Py:   if not s:
来源：http://xcd.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wxp.zycfv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yll.c1oappe.top

TS:   if (s === "") {}
来源：http://xmi.zdqjudy.top

Java: if (s.isEmpty()) {}
来源：http://akn.vqdsnc.cn

Go:   if s == "" {}
来源：http://unv.snrcjt.cn

Ruby: if s.empty?
来源：http://kpc.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ptp.sufxvd.cn

[E21] 超长截断加省略号
来源：http://ter.kuanghao11.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://szh.shangyingyoupin.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ufi.xuanzx.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aaq.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mqg.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mii.sysykeji.top

Go:   // 按 rune 判断长度后截断
来源：http://dkv.zhiwuduotai.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cpq.hnqzz.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rjg.svipenyu.cn

[E22] 字节长度与字符长度
来源：http://gsi.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rqt.xuanzx.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://krv.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bmr.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ysp.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ctq.tianlin.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cby.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://veu.jinghuilouyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zxu.jinqigfzy.top

================================================================================
来源：http://hgp.mhx1999.top

F. 文件与目录
来源：http://dxz.ppjwa.cn

================================================================================
来源：http://jbz.dashuyun.cn

[F01] 读取整个文件
来源：http://fvs.vehdjk.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qql.jinghuilouyu.cn

PHP:  file_get_contents("a.txt");
来源：http://cdr.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jfu.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tws.daria6918.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://aon.tanke756.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ivk.hywenlv.cn

Ruby: File.read("a.txt")
来源：http://joj.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://ism.hammf.cn

[F02] 逐行读取文件
来源：http://xpe.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://brv.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fzl.fktsv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iwv.yj202588.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ilf.vehdjk.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gyu.daria6918.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oxe.yanxiufei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kkp.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bwb.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://hon.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jmf.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://urr.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hvv.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fsx.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zfp.sysykeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rfi.xingfuxueyuan.xyz

Ruby: File.write("a.txt", "hi")
来源：http://ect.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fac.c1oappe.top

[F04] 追加写入文件
来源：http://dae.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lsi.ydjk.org.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fed.jinyuanbaomall.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ncf.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mpg.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ujf.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://osa.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dkr.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hrl.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://kns.yfazqb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://htx.hywenlv.cn

PHP:  file_exists("a.txt");
来源：http://abu.ybcxt.top

JS:   fs.existsSync("a.txt")
来源：http://lds.xziqi.cn


<!-- 参考信息 -->