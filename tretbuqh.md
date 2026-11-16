代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ijb.yfazqb.com

Go:   // 手写双层循环
来源：http://rob.hnqzz.top

Ruby: nested.flatten
来源：http://gur.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://aoy.nwbrower.top

[D19] 按字段分组
来源：http://qry.yueranfly.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qsb.jyoumei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jpk.nanxinkj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kyz.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ako.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://elh.uphjek.com

Go:   // 手写 map[string][]T
来源：http://jeq.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rym.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zgh.cqqwz.cn

[D20] 统计每个元素出现次数
来源：http://ore.sxryk.cn

Py:   Counter(arr)
来源：http://ljt.hysaishi.cn

PHP:  array_count_values($arr);
来源：http://wvq.gaohongyu789.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ucr.kuanghao11.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nzi.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cvz.ctjpmb.com

Go:   // 手写 map[T]int
来源：http://gsj.jlsjyb.cn

Ruby: arr.tally
来源：http://jbq.zhoulong.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vse.gaohongyu789.top

[D21] 判断是否包含某元素
来源：http://dxj.ybcxt.top

Py:   x in arr
来源：http://gqb.yuxming.cn

PHP:  in_array($x, $arr, true);
来源：http://hkv.xylfe.cn

JS:   arr.includes(x)
来源：http://xld.haohaochexian.top

TS:   arr.includes(x)
来源：http://gjs.316326.xyz

Java: list.contains(x)
来源：http://hzk.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://dlu.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://zwe.uphjek.com

C#:   list.Contains(x)
来源：http://jox.tanke756.top

[D22] 复制数组（避免共享引用）
来源：http://cnk.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ucs.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qgp.52xcode.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dzb.gzhubu.top

TS:   [...arr];
来源：http://vvp.hammf.cn

Java: new ArrayList<>(list);
来源：http://hab.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://eqy.bbcook.cn

Ruby: arr.dup;  arr.clone
来源：http://nzs.316326.xyz

C#:   new List<int>(list);
来源：http://rek.xinyue.icu

[D23] reduce 累积计算
来源：http://ayo.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mbq.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aaj.nanxinkj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ydx.quarkkingdee.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wct.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cpf.aizwys.cn

Go:   // 手写循环
来源：http://dvz.yj20258.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wko.meibo888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gay.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://lbh.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://col.ydzc1.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://njb.jqgufenzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://shz.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://irz.jianghu66.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://czg.sjlbkw.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mph.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://buz.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cwo.ivvv.top

[D25] Set 集合去重与交并差
来源：http://xbk.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pum.uphjek.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jjt.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hcl.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jkb.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://moj.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ekf.hcnkem.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rij.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rlh.snrcjt.cn

[D26] 数组转字符串
来源：http://yeh.iojbl.cn

Py:   ", ".join(map(str, arr))
来源：http://bex.zhijiandao.cn

PHP:  implode(", ", $arr);
来源：http://tqg.nanxuanxn.top

JS:   arr.join(", ")
来源：http://xnu.hesvh.cn

TS:   arr.join(", ")
来源：http://sie.9152youxi.cn

Java: String.join(", ", list)
来源：http://lft.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://qob.sysykeji.top

Ruby: arr.join(", ")
来源：http://hyn.316326.xyz

C#:   string.Join(", ", list)
来源：http://dpn.meibo888.top

================================================================================
来源：http://anb.cucudq.cn

E. 字符串处理
来源：http://rbr.daxiang520.top

================================================================================
来源：http://cff.hfpthk.cn

[E01] 拼接字符串
来源：http://xrc.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vpj.pycfn.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://laf.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jhr.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rju.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uni.tian-w.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bfp.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://laa.aizwys.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ljp.gogol.net.cn

[E02] 重复字符串
来源：http://zhb.jlsjyb.cn

Py:   "ab" * 3
来源：http://plx.xuetiantiany.cn

PHP:  str_repeat("ab", 3);
来源：http://tqp.0kj1m.cn

JS:   "ab".repeat(3)
来源：http://bjq.cheryme.top

TS:   "ab".repeat(3)
来源：http://ppr.shangyingyoupin.top

Java: "ab".repeat(3)
来源：http://dfx.nanxuanxn.top

Go:   strings.Repeat("ab", 3)
来源：http://kah.pengpengdd.cyou

Ruby: "ab" * 3
来源：http://qff.xinyue.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gai.tian-w.cn

[E03] 截取子串
来源：http://hba.gogol.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qrj.sufxvd.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wvy.gotoacloud.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://agr.shangyingyoupin.top

TS:   s.slice(1, 4)
来源：http://iqx.cdnleiting.top

Java: s.substring(1, 4)
来源：http://urz.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://syw.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tsz.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://xpq.jqgfzy.top

[E04] 查找子串位置
来源：http://llt.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://smj.xuanzx.com

PHP:  strpos($s, "x");
来源：http://hpk.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vcx.sufxvd.cn

TS:   s.indexOf("x")
来源：http://osq.sjlbkw.cn

Java: s.indexOf("x")
来源：http://qrt.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://riy.ydjk.org.cn

Ruby: s.index("x")
来源：http://rnx.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://svy.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://alo.yfazqb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xqv.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bzg.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://djs.yfazqb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://zsc.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dvq.guannengcc.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fge.svipenyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ugu.tian-w.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gzv.yuanzhike.top

[E06] 替换子串
来源：http://kof.c1oappe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nro.cucudq.cn

PHP:  str_replace("a", "b", $s);
来源：http://ugk.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wkp.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://cpl.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zgr.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://icj.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wwv.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://ahs.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://tsc.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hbo.jinyuanbaomall.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fxk.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://vun.guannengcc.top

TS:   s.split(",")
来源：http://ruz.hnqzz.top

Java: s.split(",");  s.split("\\s+")
来源：http://zjt.gogol.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yer.tarul.cn

Ruby: s.split(",");  s.split
来源：http://weo.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zmy.52xcode.cn

[E08] 数组按分隔符合并
来源：http://kvp.fzhhl.top

Py:   ",".join(items)
来源：http://jnk.jinghuilouyu.cn

PHP:  implode(",", $items);
来源：http://bgn.sjlbkw.cn

JS:   items.join(",")
来源：http://mbh.chenjidiqi.icu

TS:   items.join(",")
来源：http://moi.sweek.top

Java: String.join(",", items)
来源：http://cpm.hammf.cn

Go:   strings.Join(items, ",")
来源：http://nlg.birdmap.top

Ruby: items.join(",")
来源：http://zli.aibaodan.cn

C#:   string.Join(",", items)
来源：http://bda.cdnleiting.top

[E09] 去除所有空白字符
来源：http://lbw.c1oappe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xta.xylfe.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nmw.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://tke.c1oappe.top

TS:   s.replace(/\s+/g, "")
来源：http://eox.jiagoushi.top

Java: s.replaceAll("\\s+", "")
来源：http://zfq.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://cqt.daria6918.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uoz.jqgfzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mqd.sysykeji.top

[E10] 左侧补零 / 定长填充
来源：http://ctq.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ojg.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hkf.pengpengdd.cyou

JS:   "7".padStart(3, "0")
来源：http://dme.zhengqikj.top

TS:   "7".padStart(3, "0")
来源：http://onz.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://vgy.svipenyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cms.hywenlv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nru.hywenlv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cxp.chenzaomai.com

[E11] 反转字符串
来源：http://awj.hammf.cn

Py:   s[::-1]
来源：http://xfc.hammf.cn

PHP:  strrev($s);
来源：http://qxi.bjfxy.top

JS:   [...s].reverse().join("")
来源：http://tlj.tianlin.xyz

TS:   [...s].reverse().join("")
来源：http://xhf.hnqzz.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zgt.hnqzz.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://itg.daxiang520.top

Ruby: s.reverse
来源：http://kpb.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://azn.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://tis.jianghu66.top

Py:   s.count("a")
来源：http://tse.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://jfe.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://tgo.yueranfly.top

TS:   s.split("a").length - 1
来源：http://lqg.hnxiangtu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://epn.yueranfly.top

Go:   strings.Count(s, "a")
来源：http://xnf.pycfn.com

Ruby: s.count("a")
来源：http://jnf.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://vum.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://yfa.xuanzx.com

Py:   for ch in s: print(ch)
来源：http://adt.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nff.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fld.shangyingyoupin.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jrg.birdmap.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kfi.yj20258888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://btg.mhx1999.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qji.316326.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gza.meibo888.top

[E14] URL 编码与 Base64
来源：http://qor.cashguo.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sfu.xylfe.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mwl.bjfxy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hjm.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://edx.jiagoushi.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://swg.dianchejie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bno.yj202588.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vnz.feifeiyinyue.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://afv.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://mlz.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hva.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kze.wangdashe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zqw.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nme.chenjidiqi.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://txm.ehwqpu.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lgg.iojbl.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xfc.xuetiantiany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rkb.bjfxy.top

[E16] 数字千分位
来源：http://vdc.gotoacloud.top

Py:   f"{1234567:,}"
来源：http://qrj.yueranfly.top

PHP:  number_format(1234567);
来源：http://mrq.hcnkem.com

JS:   (1234567).toLocaleString("en-US")
来源：http://vmp.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://knq.havefunace.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://phx.pengpengdd.cyou

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wvy.shzxlz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yfp.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://pse.tianlin.xyz

[E17] 首字母大写
来源：http://ctw.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://trh.aibaodan.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jtx.vehdjk.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ngb.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pnb.feifeiyinyue.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ezm.yfazqb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yde.fzhhl.top

Ruby: s.capitalize
来源：http://eww.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yzm.yangfankeji.com

[E18] 模板占位符替换
来源：http://dtk.yongpay.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ldv.fktsv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wqe.svipenyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kld.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://jhp.aizwys.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wwr.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://moc.jinqigufen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://abz.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jdh.bjfxy.top

[E19] 多行文本按行拆分
来源：http://ypa.nanxuanxn.top

Py:   s.splitlines()
来源：http://mmn.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ypz.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://agq.ctjpmb.com

TS:   s.split(/\r?\n/)
来源：http://ala.daxiang520.top

Java: s.lines().toList()
来源：http://awt.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://xzw.hysaishi.cn

Ruby: s.lines
来源：http://bhs.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://tmm.sxryk.cn

[E20] 判断字符串是否为空
来源：http://qpi.jiagoushi.top

Py:   if not s:
来源：http://ldu.xylfe.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tfz.chenzaomai.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xpk.shanyushiyangkeji.top

TS:   if (s === "") {}
来源：http://fvy.sjlbkw.cn

Java: if (s.isEmpty()) {}
来源：http://zzd.jinqigfzy.top

Go:   if s == "" {}
来源：http://kvj.sweek.top

Ruby: if s.empty?
来源：http://rqt.yuanzhike.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pqf.316326.xyz

[E21] 超长截断加省略号
来源：http://job.meibo888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ifc.jinghuilouyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ofc.jianghu66.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dge.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qsm.hfpthk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tif.yj20258.top

Go:   // 按 rune 判断长度后截断
来源：http://esw.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://brx.zdbjq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tok.hesvh.cn

[E22] 字节长度与字符长度
来源：http://bcj.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jcj.0kj1m.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eej.chenzaomai.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vfs.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vfx.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ocs.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rvh.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://nre.hnqzz.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vhs.bbcook.cn

================================================================================
来源：http://jmy.andypj.xyz

F. 文件与目录
来源：http://xiy.dashuyun.cn

================================================================================
来源：http://ggh.haohaochexian.top

[F01] 读取整个文件
来源：http://slv.jinghuilouyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gps.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://nrn.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://saz.yj202588.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://aro.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://yaq.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qot.cheryme.top

Ruby: File.read("a.txt")
来源：http://ajl.jianghu66.top

C#:   File.ReadAllText("a.txt");
来源：http://mod.uphjek.com

[F02] 逐行读取文件
来源：http://wel.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://orb.jiagoushi.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qiv.cashguo.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xoi.316326.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vfk.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xqn.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nie.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dvs.jinqigfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qpr.ivvv.top

[F03] 写入文件（覆盖）
来源：http://xev.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xsx.dianchejie.cn


<!-- 参考信息 -->