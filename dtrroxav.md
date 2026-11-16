代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://lew.nanxinkj.top

JS:   arr.includes(x)
来源：http://ads.daxiang520.top

TS:   arr.includes(x)
来源：http://fnr.ydjk.org.cn

Java: list.contains(x)
来源：http://gzy.redwolf501.top

Go:   slices.Contains(arr, x)
来源：http://mmh.tanke756.top

Ruby: arr.include?(x)
来源：http://jlp.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://rzh.nwbrower.top

[D22] 复制数组（避免共享引用）
来源：http://qvj.uphjek.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qog.uphjek.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://emx.iojbl.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aha.jianghu66.top

TS:   [...arr];
来源：http://rwx.havefunace.top

Java: new ArrayList<>(list);
来源：http://xhk.daria6918.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wuw.hammf.cn

Ruby: arr.dup;  arr.clone
来源：http://dak.dashuyun.cn

C#:   new List<int>(list);
来源：http://pfu.c1oappe.top

[D23] reduce 累积计算
来源：http://arv.gogol.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yje.tarul.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fay.dashuyun.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wwv.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://etl.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://sqo.birdmap.top

Go:   // 手写循环
来源：http://dvh.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kdb.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://heo.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://rkb.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uie.yj20258.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pvy.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qjp.ybcxt.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vbc.xingfuxueyuan.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iwz.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dvk.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vdu.hywenlv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rjq.zdqjudy.top

[D25] Set 集合去重与交并差
来源：http://vex.zdbjq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lce.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sam.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ecb.jinqigufen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cws.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bou.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jpv.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kpb.uphjek.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zmy.gzhubu.top

[D26] 数组转字符串
来源：http://kvb.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://eaz.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://yyq.nanxuanxn.top

JS:   arr.join(", ")
来源：http://ccr.zhixingplan.top

TS:   arr.join(", ")
来源：http://kye.yuanzhike.top

Java: String.join(", ", list)
来源：http://zae.hcnkem.com

Go:   strings.Join(strs, ", ")
来源：http://oop.jiagoushi.top

Ruby: arr.join(", ")
来源：http://hqd.zdbjq.cn

C#:   string.Join(", ", list)
来源：http://gvb.aizwys.cn

================================================================================
来源：http://pmc.kuanghao11.cn

E. 字符串处理
来源：http://nvp.jinyuanbaomall.cn

================================================================================
来源：http://jhh.9152youxi.cn

[E01] 拼接字符串
来源：http://cqv.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wmh.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mdo.fehbvm.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yfm.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rtt.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hah.ywan-chungtsiang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vaq.hongshengwenyu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://awq.xingfuxueyuan.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://icr.xuanzx.com

[E02] 重复字符串
来源：http://cdt.fktsv.cn

Py:   "ab" * 3
来源：http://dzp.snrcjt.cn

PHP:  str_repeat("ab", 3);
来源：http://wni.yvedp.cn

JS:   "ab".repeat(3)
来源：http://ywb.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://afc.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://lhc.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://edo.dashuyun.cn

Ruby: "ab" * 3
来源：http://gji.ywan-chungtsiang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nqv.fengsongda.top

[E03] 截取子串
来源：http://fdb.9152youxi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rgq.zhoulong.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cbc.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qfs.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://kii.jinqigufen.top

Java: s.substring(1, 4)
来源：http://dwa.yanxiufei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qtm.fktsv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fmi.smart0.xyz

C#:   s.Substring(1, 3)
来源：http://sfv.aizwys.cn

[E04] 查找子串位置
来源：http://guv.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://eou.zycfv.cn

PHP:  strpos($s, "x");
来源：http://iuj.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uof.redwolf501.top

TS:   s.indexOf("x")
来源：http://ppj.havefunace.top

Java: s.indexOf("x")
来源：http://agn.jinqigfzy.top

Go:   strings.Index(s, "x")
来源：http://dna.yangfankeji.com

Ruby: s.index("x")
来源：http://git.shanyushiyangkeji.top

C#:   s.IndexOf("x")
来源：http://wkx.gzhubu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ang.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zjo.yonumen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://abx.ywan-chungtsiang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sok.cucudq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zau.zhixingplan.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hfv.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zne.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uyf.kuanghao11.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xfk.havefunace.top

[E06] 替换子串
来源：http://qbe.birdmap.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lpg.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://ogg.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nod.hnqzz.top

TS:   s.replaceAll("a", "b")
来源：http://ppo.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sld.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://idw.feifeiyinyue.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://idu.dashuyun.cn

C#:   s.Replace("a", "b")
来源：http://akk.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://hnx.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bwt.feifeiyinyue.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qgg.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://tem.ydjk.org.cn

TS:   s.split(",")
来源：http://wqk.xziqi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://aqi.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://abg.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://xjh.haohaochexian.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uio.redwolf501.top

[E08] 数组按分隔符合并
来源：http://njr.bjfxy.top

Py:   ",".join(items)
来源：http://nno.xinyue.icu

PHP:  implode(",", $items);
来源：http://zez.fehbvm.com

JS:   items.join(",")
来源：http://gvr.mhx1999.top

TS:   items.join(",")
来源：http://mxs.havefunace.top

Java: String.join(",", items)
来源：http://huy.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://hbt.yj20258888.top

Ruby: items.join(",")
来源：http://oda.hywenlv.cn

C#:   string.Join(",", items)
来源：http://eae.bbcook.cn

[E09] 去除所有空白字符
来源：http://mtm.shangyingyoupin.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://exo.9152youxi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bdg.52xcode.cn

JS:   s.replace(/\s+/g, "")
来源：http://pvn.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://bee.fengsongda.top

Java: s.replaceAll("\\s+", "")
来源：http://lnn.jlsjyb.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xga.guannengcc.top

Ruby: s.gsub(/\s+/, "")
来源：http://pvd.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lcm.vehdjk.com

[E10] 左侧补零 / 定长填充
来源：http://pcr.ivvv.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lsg.shuidangran.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ebh.xziqi.cn

JS:   "7".padStart(3, "0")
来源：http://fco.zhixingplan.top

TS:   "7".padStart(3, "0")
来源：http://tgq.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://rjt.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://peu.jyoumei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bnr.jlsjyb.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lwz.epnwcf.com

[E11] 反转字符串
来源：http://zyl.redwolf501.top

Py:   s[::-1]
来源：http://rks.nanxuanxn.top

PHP:  strrev($s);
来源：http://ylb.yuanzhike.top

JS:   [...s].reverse().join("")
来源：http://mmb.ydzc1.top

TS:   [...s].reverse().join("")
来源：http://csh.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wbs.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yte.chenzaomai.com

Ruby: s.reverse
来源：http://ywy.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vxi.vehdjk.com

[E12] 统计某字符出现次数
来源：http://qqc.ydjk.org.cn

Py:   s.count("a")
来源：http://rre.sufxvd.cn

PHP:  substr_count($s, "a");
来源：http://tto.smart0.xyz

JS:   s.split("a").length - 1
来源：http://xev.epnwcf.com

TS:   s.split("a").length - 1
来源：http://han.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iit.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://fko.cashguo.top

Ruby: s.count("a")
来源：http://jtn.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://lgy.zhixingplan.top

[E13] 逐字符遍历
来源：http://amc.zdbjq.cn

Py:   for ch in s: print(ch)
来源：http://uuc.dianchejie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zwu.yvedp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qhr.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sbd.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qbd.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eko.feifeiyinyue.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dfs.zhaomingkeji.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://emv.guowangkeji.top

[E14] URL 编码与 Base64
来源：http://wpc.tianlin.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dxh.xylfe.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://foh.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jnn.zhiwuduotai.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vhi.chenjidiqi.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ota.yj20258.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zoi.0kj1m.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zkx.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iet.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://kxq.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://phs.yongpay.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fkz.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bhe.aizwys.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xyz.xylfe.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jjw.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://usw.jinqigufen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zum.hnqzz.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yuo.wangshuangyany.cn

[E16] 数字千分位
来源：http://qol.yuxming.cn

Py:   f"{1234567:,}"
来源：http://yeh.hnqzz.top

PHP:  number_format(1234567);
来源：http://xcr.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mdd.zhijiandao.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zhf.zhengqikj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fcb.bjfxy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ecn.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dbf.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://dip.chenjidiqi.icu

[E17] 首字母大写
来源：http://qeh.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jop.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pgp.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jqy.gotoacloud.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pjy.hesvh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zae.wangdashe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dsi.jinghuilouyu.cn

Ruby: s.capitalize
来源：http://uzm.jinqigufen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://utg.yj20258888.top

[E18] 模板占位符替换
来源：http://obz.yonumen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gdu.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jxf.xingfuxueyuan.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://dhl.dianchejie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cmn.uphjek.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uzv.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://btx.tianlin.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ezq.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gni.jqgufenzy.top

[E19] 多行文本按行拆分
来源：http://xhw.0kj1m.cn

Py:   s.splitlines()
来源：http://ppp.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://grm.cheryme.top

JS:   s.split(/\r?\n/)
来源：http://syd.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://ssu.wangshuangyany.cn

Java: s.lines().toList()
来源：http://gpu.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://cya.jinghuilouyu.cn

Ruby: s.lines
来源：http://snp.daria6918.cn

C#:   s.Split('\n')
来源：http://mop.smart0.xyz

[E20] 判断字符串是否为空
来源：http://dim.zhijiandao.cn

Py:   if not s:
来源：http://ejp.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://epz.wangdashe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pww.yuxming.cn

TS:   if (s === "") {}
来源：http://jmq.gotoacloud.top

Java: if (s.isEmpty()) {}
来源：http://ajm.hesvh.cn

Go:   if s == "" {}
来源：http://yvw.zdbjq.cn

Ruby: if s.empty?
来源：http://frk.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hji.yuxming.cn

[E21] 超长截断加省略号
来源：http://xfh.guannengcc.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aln.fktsv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ict.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nlq.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yrz.hcnkem.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://geh.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://yvj.gaohongyu789.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oqc.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ikt.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://vep.daxiang520.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://skf.nanxuanxn.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uoa.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bca.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://don.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://otd.yongpay.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dvr.birdmap.top

Ruby: s.bytesize;  s.length
来源：http://ltr.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cdx.mhx1999.top

================================================================================
来源：http://ptx.ehwqpu.com

F. 文件与目录
来源：http://jlx.cqqwz.cn

================================================================================
来源：http://ver.feifeiyinyue.top

[F01] 读取整个文件
来源：http://txh.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uwt.gotoacloud.top

PHP:  file_get_contents("a.txt");
来源：http://xac.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zyb.fehbvm.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://seg.fengsongda.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yqc.yangfankeji.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zad.quarkkingdee.top

Ruby: File.read("a.txt")
来源：http://ncb.xziqi.cn

C#:   File.ReadAllText("a.txt");
来源：http://zix.hnxiangtu.top

[F02] 逐行读取文件
来源：http://kab.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://upu.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pwb.svipenyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dgv.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ybt.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pnd.shanyushiyangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zpc.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zkm.jinyuanbaomall.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fjw.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://cgb.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uwm.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jhp.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://enk.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wvf.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ahd.jlsjyb.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gbi.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://aib.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kpa.svipenyu.cn

[F04] 追加写入文件
来源：http://fxk.9152youxi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qcs.hywenlv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zea.shanyushiyangtech.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lhk.xingfuxueyuan.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dwt.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wah.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fva.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://szj.jqgufenzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kkt.chenjidiqi.icu

[F05] 判断文件或目录是否存在
来源：http://nth.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ydc.vehdjk.com

PHP:  file_exists("a.txt");
来源：http://fsb.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://cwj.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://fum.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dxm.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://twc.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://hxh.fzhhl.top


<!-- 参考信息 -->