代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://itn.meibo888.top

PHP:  array_merge(...$nested);
来源：http://aqv.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://abk.chenjidiqi.icu

TS:   nested.flat();
来源：http://ahh.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ayc.xuanzx.com

Go:   // 手写双层循环
来源：http://fmk.fzhhl.top

Ruby: nested.flatten
来源：http://efq.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://czl.dianchejie.cn

[D19] 按字段分组
来源：http://kmq.hcnkem.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aii.tarul.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iwr.ybcxt.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fzc.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gbe.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vyh.cheryme.top

Go:   // 手写 map[string][]T
来源：http://mko.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rwk.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://soy.fktsv.cn

[D20] 统计每个元素出现次数
来源：http://yvd.yvedp.cn

Py:   Counter(arr)
来源：http://vbi.zhixingplan.top

PHP:  array_count_values($arr);
来源：http://wdt.ydjk.org.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gku.jiagoushi.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nea.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://arr.hesvh.cn

Go:   // 手写 map[T]int
来源：http://rnl.epnwcf.com

Ruby: arr.tally
来源：http://bdl.jinqigufen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qis.yueranfly.top

[D21] 判断是否包含某元素
来源：http://mek.c1oappe.top

Py:   x in arr
来源：http://wqj.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://pyo.hcnkem.com

JS:   arr.includes(x)
来源：http://nfq.redwolf501.top

TS:   arr.includes(x)
来源：http://img.gaohongyu789.top

Java: list.contains(x)
来源：http://alu.uphjek.com

Go:   slices.Contains(arr, x)
来源：http://tlz.hnxiangtu.top

Ruby: arr.include?(x)
来源：http://kvb.cheryme.top

C#:   list.Contains(x)
来源：http://jec.sysykeji.top

[D22] 复制数组（避免共享引用）
来源：http://epa.ivvv.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jtm.shuidangran.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sze.yanxiufei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mao.hongshengwenyu.top

TS:   [...arr];
来源：http://mtw.sxryk.cn

Java: new ArrayList<>(list);
来源：http://chq.redwolf501.top

Go:   copied := append([]int(nil), arr...)
来源：http://hnt.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://awg.yfazqb.com

C#:   new List<int>(list);
来源：http://phq.yj20258888.top

[D23] reduce 累积计算
来源：http://rrr.chenlongwang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gws.vehdjk.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ipz.yueranfly.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fsj.dashuyun.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tbc.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vnk.sufxvd.cn

Go:   // 手写循环
来源：http://ocr.ehwqpu.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pii.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iqf.cashguo.top

[D24] 字典 / Map 基本操作
来源：http://trs.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ugm.yueranfly.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://csb.dashuyun.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ity.hfpthk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fga.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dyn.cashguo.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yyk.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qnt.jqgfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fnx.birdmap.top

[D25] Set 集合去重与交并差
来源：http://olc.chenjidiqi.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oym.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ega.jianghu66.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nzs.feifeiyinyue.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://trj.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cuk.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uxs.yuanzhike.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zsr.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nud.vqdsnc.cn

[D26] 数组转字符串
来源：http://kqw.yfazqb.com

Py:   ", ".join(map(str, arr))
来源：http://rfu.zhaomingkeji.xyz

PHP:  implode(", ", $arr);
来源：http://aol.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://xmn.zdqjudy.top

TS:   arr.join(", ")
来源：http://tou.gogol.net.cn

Java: String.join(", ", list)
来源：http://xue.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://jhk.yongpay.top

Ruby: arr.join(", ")
来源：http://ckj.guannengcc.top

C#:   string.Join(", ", list)
来源：http://omr.fzhhl.top

================================================================================
来源：http://dbt.ydzc1.top

E. 字符串处理
来源：http://syq.sufxvd.cn

================================================================================
来源：http://jkv.yuanzhike.top

[E01] 拼接字符串
来源：http://dwk.sysykeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fwa.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jts.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lzx.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://paw.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://awo.jinyuanbaomall.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xzk.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ixr.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kfy.shuidangran.top

[E02] 重复字符串
来源：http://uvh.wangshuangyany.cn

Py:   "ab" * 3
来源：http://pnu.bjfxy.top

PHP:  str_repeat("ab", 3);
来源：http://txx.yuanzhike.top

JS:   "ab".repeat(3)
来源：http://hff.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://hfm.fengsongda.top

Java: "ab".repeat(3)
来源：http://syp.shanyushiyangtech.top

Go:   strings.Repeat("ab", 3)
来源：http://pwn.nwbrower.top

Ruby: "ab" * 3
来源：http://bfh.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://njy.jinqigufen.top

[E03] 截取子串
来源：http://jtx.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ust.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jcy.jiagoushi.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vtm.yongpay.top

TS:   s.slice(1, 4)
来源：http://prm.snrcjt.cn

Java: s.substring(1, 4)
来源：http://wqd.ctjpmb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eet.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://xcw.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://ftq.shangyingyoupin.top

[E04] 查找子串位置
来源：http://gmw.quarkkingdee.top

Py:   s.find("x");  s.index("x")
来源：http://csu.daria6918.cn

PHP:  strpos($s, "x");
来源：http://ect.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wra.svipenyu.cn

TS:   s.indexOf("x")
来源：http://cjy.hesvh.cn

Java: s.indexOf("x")
来源：http://cyt.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://jjs.havefunace.top

Ruby: s.index("x")
来源：http://qfn.sysykeji.top

C#:   s.IndexOf("x")
来源：http://nea.yvedp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lzq.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aoe.fzhhl.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hys.fengsongda.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nxv.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://avs.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ocp.sjlbkw.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ccp.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lro.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vnz.jinghuilouyu.cn

[E06] 替换子串
来源：http://fgb.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wex.zdqjudy.top

PHP:  str_replace("a", "b", $s);
来源：http://sxg.jianghu66.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://izu.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://ofz.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xrh.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://arg.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jtn.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://rsn.yueranfly.top

[E07] 按分隔符拆分
来源：http://pqp.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jmz.jinqigfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iew.jiagoushi.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qws.mhx1999.top

TS:   s.split(",")
来源：http://nfw.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kum.dashuyun.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ams.hammf.cn

Ruby: s.split(",");  s.split
来源：http://ekt.jinghuilouyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jpq.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://hyv.smart0.xyz

Py:   ",".join(items)
来源：http://omg.cashguo.top

PHP:  implode(",", $items);
来源：http://xki.gzhubu.top

JS:   items.join(",")
来源：http://gwr.xziqi.cn

TS:   items.join(",")
来源：http://imw.yueranfly.top

Java: String.join(",", items)
来源：http://ytp.sjlbkw.cn

Go:   strings.Join(items, ",")
来源：http://xog.guannengcc.top

Ruby: items.join(",")
来源：http://vml.fzhhl.top

C#:   string.Join(",", items)
来源：http://klz.chenjidiqi.icu

[E09] 去除所有空白字符
来源：http://cyk.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vum.fanxiaobao.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://euh.feifeiyinyue.top

JS:   s.replace(/\s+/g, "")
来源：http://njo.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://dzz.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://ryq.bjfxy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gsh.ctjpmb.com

Ruby: s.gsub(/\s+/, "")
来源：http://gqh.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vjk.zycfv.cn

[E10] 左侧补零 / 定长填充
来源：http://osn.birdmap.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bfz.gotoacloud.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kmt.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://mwl.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://wcj.tanke756.top

Java: String.format("%03d", 7)
来源：http://pkp.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bnm.gaohongyu789.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jij.chenlongwang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fmo.hammf.cn

[E11] 反转字符串
来源：http://tkn.jqgfzy.top

Py:   s[::-1]
来源：http://igi.cucudq.cn

PHP:  strrev($s);
来源：http://idb.yuanzhike.top

JS:   [...s].reverse().join("")
来源：http://loo.zycfv.cn

TS:   [...s].reverse().join("")
来源：http://mti.jiagoushi.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ckk.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://wmd.ppjwa.cn

Ruby: s.reverse
来源：http://deg.shanyushiyangtech.top

C#:   new string(s.Reverse().ToArray())
来源：http://hjo.dianchejie.cn

[E12] 统计某字符出现次数
来源：http://uvf.quarkkingdee.top

Py:   s.count("a")
来源：http://xxr.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://twv.hammf.cn

JS:   s.split("a").length - 1
来源：http://nas.andypj.xyz

TS:   s.split("a").length - 1
来源：http://nrl.bbcook.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://evu.yangfankeji.com

Go:   strings.Count(s, "a")
来源：http://opx.tarul.cn

Ruby: s.count("a")
来源：http://adk.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://fyd.yuanzhike.top

[E13] 逐字符遍历
来源：http://enx.ybcxt.top

Py:   for ch in s: print(ch)
来源：http://dtd.jyoumei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kel.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qtj.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gbv.hysaishi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oxt.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sbs.jiagoushi.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rqp.chenlongwang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cld.hnxiangtu.top

[E14] URL 编码与 Base64
来源：http://ynt.hnxiangtu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hof.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qnr.snrcjt.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yke.bbcook.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cqx.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lko.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cuo.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mkq.yj20258.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eyq.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://klo.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xrr.yj202588.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blw.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xbz.hongshengwenyu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://olh.hysaishi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nde.9152youxi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hvt.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wtk.ivvv.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rkz.ywan-chungtsiang.top

[E16] 数字千分位
来源：http://iwd.jqgufenzy.top

Py:   f"{1234567:,}"
来源：http://aqt.tarul.cn

PHP:  number_format(1234567);
来源：http://bky.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://phn.haohaochexian.top

TS:   (1234567).toLocaleString("en-US")
来源：http://biw.xylfe.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wli.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lnr.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ugj.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://kpq.vqdsnc.cn

[E17] 首字母大写
来源：http://zky.xinyue.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nmh.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://pxy.bbcook.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dgy.vqdsnc.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dco.yvedp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gqa.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vun.fehbvm.com

Ruby: s.capitalize
来源：http://qjf.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vsc.sufxvd.cn

[E18] 模板占位符替换
来源：http://tpc.ctjpmb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lau.jinqigfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zbq.uphjek.com

JS:   tpl.replaceAll("{name}", name)
来源：http://iow.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://epk.jiagoushi.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vqh.yj202588.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://soy.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ugb.jlsjyb.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bgo.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://qrf.xuetiantiany.cn

Py:   s.splitlines()
来源：http://qpk.zhengqikj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pdx.gogol.net.cn

JS:   s.split(/\r?\n/)
来源：http://qqc.bjfxy.top

TS:   s.split(/\r?\n/)
来源：http://lox.wangshuangyany.cn

Java: s.lines().toList()
来源：http://ldn.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://soo.fanxiaobao.xyz

Ruby: s.lines
来源：http://fgx.ydzc1.top

C#:   s.Split('\n')
来源：http://eiv.hongshengwenyu.top

[E20] 判断字符串是否为空
来源：http://rej.kuanghao11.cn

Py:   if not s:
来源：http://yke.hesvh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dgq.yongpay.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://klm.cqqwz.cn

TS:   if (s === "") {}
来源：http://zpg.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://oel.chenjidiqi.icu

Go:   if s == "" {}
来源：http://tzo.hnxiangtu.top

Ruby: if s.empty?
来源：http://klx.zhoulong.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bje.epnwcf.com

[E21] 超长截断加省略号
来源：http://nid.yfazqb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bpp.aizwys.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bnl.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nfv.smart0.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eeh.ctjpmb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xsw.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://kcj.hongshengwenyu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://odn.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aca.zhiwuduotai.top

[E22] 字节长度与字符长度
来源：http://zyp.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aed.quarkkingdee.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oyv.jinqigufen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kzc.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://umk.vqdsnc.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ktp.jqgfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jpe.xziqi.cn

Ruby: s.bytesize;  s.length
来源：http://zww.gotoacloud.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sbp.hywenlv.cn

================================================================================
来源：http://fej.yongpay.top

F. 文件与目录
来源：http://pqt.jlsjyb.cn

================================================================================
来源：http://lkv.uphjek.com

[F01] 读取整个文件
来源：http://lcp.aizwys.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kmu.havefunace.top

PHP:  file_get_contents("a.txt");
来源：http://nim.nwbrower.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ena.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://flr.yvedp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fxj.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://erw.fzhhl.top

Ruby: File.read("a.txt")
来源：http://lxv.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://wzf.birdmap.top

[F02] 逐行读取文件
来源：http://tjo.zhaomingkeji.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xic.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ncz.sjlbkw.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ssj.wangshuangyany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jjo.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yxe.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yaj.cqqwz.cn


<!-- 参考信息 -->