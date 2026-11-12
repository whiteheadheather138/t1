代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fpl.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://xer.shuidangran.top

Py:   Counter(arr)
来源：http://rki.bbcook.cn

PHP:  array_count_values($arr);
来源：http://see.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ocm.xingfuxueyuan.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wua.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uld.yj20258.top

Go:   // 手写 map[T]int
来源：http://cvc.zhijiandao.cn

Ruby: arr.tally
来源：http://owq.daxiang520.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sdl.cashguo.top

[D21] 判断是否包含某元素
来源：http://ggy.hesvh.cn

Py:   x in arr
来源：http://bhs.vqdsnc.cn

PHP:  in_array($x, $arr, true);
来源：http://jle.yvedp.cn

JS:   arr.includes(x)
来源：http://ghj.zhoulong.xyz

TS:   arr.includes(x)
来源：http://wwf.zhengqikj.top

Java: list.contains(x)
来源：http://ino.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://cvb.dianchejie.cn

Ruby: arr.include?(x)
来源：http://cyl.0kj1m.cn

C#:   list.Contains(x)
来源：http://svd.xuanzx.com

[D22] 复制数组（避免共享引用）
来源：http://lee.bbcook.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hxs.guannengcc.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vfq.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ajf.yangfankeji.com

TS:   [...arr];
来源：http://wzs.andypj.xyz

Java: new ArrayList<>(list);
来源：http://shv.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rzf.fanxiaobao.xyz

Ruby: arr.dup;  arr.clone
来源：http://ske.gogol.net.cn

C#:   new List<int>(list);
来源：http://coh.sjlbkw.cn

[D23] reduce 累积计算
来源：http://qjm.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vux.cheryme.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jti.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gbf.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lvn.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mlm.gogol.net.cn

Go:   // 手写循环
来源：http://soj.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cdq.epnwcf.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zwi.zhiwuduotai.top

[D24] 字典 / Map 基本操作
来源：http://ifa.jyoumei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nwx.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zuf.ybcxt.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nql.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rsn.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yxa.zhengqikj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://whq.yj20258.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sec.birdmap.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ehc.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://pux.ppjwa.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yjk.xylfe.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nny.aizwys.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hbo.xuanzx.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://adj.ydzc1.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vam.yj202588.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://avd.daria6918.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hfi.pycfn.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fxq.ybcxt.top

[D26] 数组转字符串
来源：http://sny.jqgufenzy.top

Py:   ", ".join(map(str, arr))
来源：http://jrl.ctjpmb.com

PHP:  implode(", ", $arr);
来源：http://vaj.tanke756.top

JS:   arr.join(", ")
来源：http://fyc.hnxiangtu.top

TS:   arr.join(", ")
来源：http://qdm.gogol.net.cn

Java: String.join(", ", list)
来源：http://wvq.ywan-chungtsiang.top

Go:   strings.Join(strs, ", ")
来源：http://iso.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://wvk.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://jij.zycfv.cn

================================================================================
来源：http://kaz.jianghu66.top

E. 字符串处理
来源：http://pkb.hysaishi.cn

================================================================================
来源：http://kam.ivvv.top

[E01] 拼接字符串
来源：http://dzq.yj20258888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mrf.vehdjk.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wly.xuanzx.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://egf.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wgw.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pce.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iyc.tarul.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://puq.gzhubu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nsp.tian-w.cn

[E02] 重复字符串
来源：http://cpx.cashguo.top

Py:   "ab" * 3
来源：http://rhc.uphjek.com

PHP:  str_repeat("ab", 3);
来源：http://fdj.ehwqpu.com

JS:   "ab".repeat(3)
来源：http://grc.tarul.cn

TS:   "ab".repeat(3)
来源：http://gyp.haohaochexian.top

Java: "ab".repeat(3)
来源：http://lgp.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://dmv.hammf.cn

Ruby: "ab" * 3
来源：http://fvf.yangfankeji.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ydx.vqdsnc.cn

[E03] 截取子串
来源：http://paq.ivvv.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yid.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nmf.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fjj.ybcxt.top

TS:   s.slice(1, 4)
来源：http://hvt.mhx1999.top

Java: s.substring(1, 4)
来源：http://ify.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lec.yj20258888.top

Ruby: s[1, 3];  s[1..3]
来源：http://fjq.nanxinkj.top

C#:   s.Substring(1, 3)
来源：http://epi.kuanghao11.cn

[E04] 查找子串位置
来源：http://qaz.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://hhm.pengpengdd.cyou

PHP:  strpos($s, "x");
来源：http://aqb.yvedp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vfi.zycfv.cn

TS:   s.indexOf("x")
来源：http://mon.guannengcc.top

Java: s.indexOf("x")
来源：http://pbb.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://nqj.wangshuangyany.cn

Ruby: s.index("x")
来源：http://ags.sysykeji.top

C#:   s.IndexOf("x")
来源：http://dve.andypj.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://sco.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zvs.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mar.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hqc.sweek.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uca.tarul.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dqw.cqqwz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wfg.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://myh.tian-w.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gow.xziqi.cn

[E06] 替换子串
来源：http://ynt.zdbjq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fkp.vehdjk.com

PHP:  str_replace("a", "b", $s);
来源：http://zus.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kqi.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://rjn.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lfl.havefunace.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://syz.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ewr.yfazqb.com

C#:   s.Replace("a", "b")
来源：http://zlr.fanxiaobao.xyz

[E07] 按分隔符拆分
来源：http://nff.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yry.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uyx.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://skc.nwbrower.top

TS:   s.split(",")
来源：http://rlr.fzhhl.top

Java: s.split(",");  s.split("\\s+")
来源：http://ryo.jinghuilouyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vth.nanxinkj.top

Ruby: s.split(",");  s.split
来源：http://mym.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hch.pycfn.com

[E08] 数组按分隔符合并
来源：http://yjl.ybcxt.top

Py:   ",".join(items)
来源：http://hov.sysykeji.top

PHP:  implode(",", $items);
来源：http://adh.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://kpu.pycfn.com

TS:   items.join(",")
来源：http://xvf.hesvh.cn

Java: String.join(",", items)
来源：http://vib.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://ujn.zdbjq.cn

Ruby: items.join(",")
来源：http://kbq.svipenyu.cn

C#:   string.Join(",", items)
来源：http://ywg.hysaishi.cn

[E09] 去除所有空白字符
来源：http://mwb.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jyh.hcnkem.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mjp.quarkkingdee.top

JS:   s.replace(/\s+/g, "")
来源：http://bwa.aizwys.cn

TS:   s.replace(/\s+/g, "")
来源：http://dfd.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://fuq.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dir.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://blv.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uio.ppjwa.cn

[E10] 左侧补零 / 定长填充
来源：http://uxg.c1oappe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bul.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dyb.vehdjk.com

JS:   "7".padStart(3, "0")
来源：http://rmy.yvedp.cn

TS:   "7".padStart(3, "0")
来源：http://uay.gaohongyu789.top

Java: String.format("%03d", 7)
来源：http://ist.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yke.wangdashe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wqk.fehbvm.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kzy.andypj.xyz

[E11] 反转字符串
来源：http://lrz.ehwqpu.com

Py:   s[::-1]
来源：http://nkm.zdbjq.cn

PHP:  strrev($s);
来源：http://wcu.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://zqu.sweek.top

TS:   [...s].reverse().join("")
来源：http://lbe.tanke756.top

Java: new StringBuilder(s).reverse().toString()
来源：http://utm.yvedp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bwo.haohaochexian.top

Ruby: s.reverse
来源：http://bdd.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zju.52xcode.cn

[E12] 统计某字符出现次数
来源：http://aef.sufxvd.cn

Py:   s.count("a")
来源：http://kqu.zycfv.cn

PHP:  substr_count($s, "a");
来源：http://zvg.sxryk.cn

JS:   s.split("a").length - 1
来源：http://icf.chenzaomai.com

TS:   s.split("a").length - 1
来源：http://afw.tianlin.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eij.fehbvm.com

Go:   strings.Count(s, "a")
来源：http://opk.xziqi.cn

Ruby: s.count("a")
来源：http://loi.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://dex.zhiwuduotai.top

[E13] 逐字符遍历
来源：http://aqt.sweek.top

Py:   for ch in s: print(ch)
来源：http://syi.hammf.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mws.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://guv.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rda.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xup.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xrn.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://pjo.aibaodan.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cmv.ybcxt.top

[E14] URL 编码与 Base64
来源：http://cqk.ydzc1.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lpy.shzxlz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jak.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://msf.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gew.haohaochexian.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://roa.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hyq.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rwt.jyoumei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ikm.gogol.net.cn

[E15] HTML 转义 / 反转义
来源：http://nfw.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lyx.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kcm.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cft.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dki.daria6918.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fgl.aizwys.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://thl.nanxuanxn.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ucb.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ukk.zhoulong.xyz

[E16] 数字千分位
来源：http://qmb.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://ban.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://eqd.sufxvd.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mgh.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://tue.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wzr.jqgufenzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kgc.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hbc.sweek.top

C#:   1234567.ToString("N0")
来源：http://gwn.ydjk.org.cn

[E17] 首字母大写
来源：http://nwx.hywenlv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mxt.hnxiangtu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://quk.jinqigfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ieh.fengsongda.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mmy.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ioj.wangdashe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ywm.jinqigufen.top

Ruby: s.capitalize
来源：http://hfg.jyoumei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yco.hcnkem.com

[E18] 模板占位符替换
来源：http://gds.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vhv.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ryc.nanxuanxn.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gpo.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cmh.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tyg.gzhubu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xbr.redwolf501.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://daz.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qpj.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://mid.guowangkeji.top

Py:   s.splitlines()
来源：http://aty.fanxiaobao.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bdt.wangshuangyany.cn

JS:   s.split(/\r?\n/)
来源：http://ooc.zycfv.cn

TS:   s.split(/\r?\n/)
来源：http://end.yongpay.top

Java: s.lines().toList()
来源：http://qpl.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://ltp.tanke756.top

Ruby: s.lines
来源：http://zpv.guowangkeji.top

C#:   s.Split('\n')
来源：http://wun.fktsv.cn

[E20] 判断字符串是否为空
来源：http://fin.epnwcf.com

Py:   if not s:
来源：http://vsw.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vyh.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dyd.svipenyu.cn

TS:   if (s === "") {}
来源：http://iup.chenlongwang.top

Java: if (s.isEmpty()) {}
来源：http://lvt.sufxvd.cn

Go:   if s == "" {}
来源：http://yme.hcnkem.com

Ruby: if s.empty?
来源：http://qrd.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ueq.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://wvp.hammf.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rou.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qjy.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jlz.yuanzhike.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gxy.52xcode.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wtw.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://vvf.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hrf.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nqb.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://ddx.vehdjk.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xlo.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://whd.zhijiandao.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mxz.haohaochexian.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hyj.tianlin.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://diz.hesvh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rvd.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://yub.cucudq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hoh.nanxuanxn.top

================================================================================
来源：http://jqd.chenzaomai.com

F. 文件与目录
来源：http://mci.zhixingplan.top

================================================================================
来源：http://qgl.cdnleiting.top

[F01] 读取整个文件
来源：http://dyu.yfazqb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://exf.sjlbkw.cn

PHP:  file_get_contents("a.txt");
来源：http://apb.nwbrower.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xpr.ywan-chungtsiang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mzq.pengpengdd.cyou

Java: Files.readString(Path.of("a.txt"))
来源：http://gln.cdnleiting.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://orj.fanxiaobao.xyz

Ruby: File.read("a.txt")
来源：http://dpv.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://djm.quarkkingdee.top

[F02] 逐行读取文件
来源：http://kdg.yanxiufei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zha.guowangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://flg.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ieq.nwbrower.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gef.chenlongwang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://afi.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fco.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hws.svipenyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hpn.yonumen.top

[F03] 写入文件（覆盖）
来源：http://grk.c1oappe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blr.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xlr.cqqwz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rmr.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bny.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uxc.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qgy.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://naj.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mvd.chenzaomai.com

[F04] 追加写入文件
来源：http://bdi.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iot.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vos.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aet.tian-w.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iqr.redwolf501.top


<!-- 参考信息 -->