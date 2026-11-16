代发 wailian999

[D19] 按字段分组
来源：http://xzv.0kj1m.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fzn.hfpthk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ldd.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://myt.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bwm.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lqk.zhaomingkeji.xyz

Go:   // 手写 map[string][]T
来源：http://djn.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ztm.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lhq.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://xwp.cqqwz.cn

Py:   Counter(arr)
来源：http://riv.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://kqt.vehdjk.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://syx.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cqd.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hep.cucudq.cn

Go:   // 手写 map[T]int
来源：http://eur.fengsongda.top

Ruby: arr.tally
来源：http://okn.jinyuanbaomall.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://utz.shuidangran.top

[D21] 判断是否包含某元素
来源：http://ckp.jinqigfzy.top

Py:   x in arr
来源：http://ybn.jinqigfzy.top

PHP:  in_array($x, $arr, true);
来源：http://jmy.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://dsb.tian-w.cn

TS:   arr.includes(x)
来源：http://hls.zhiwuduotai.top

Java: list.contains(x)
来源：http://hsr.yueranfly.top

Go:   slices.Contains(arr, x)
来源：http://tsp.sysykeji.top

Ruby: arr.include?(x)
来源：http://rff.shangyingyoupin.top

C#:   list.Contains(x)
来源：http://ifs.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://ubg.havefunace.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qop.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kbx.gotoacloud.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qkz.hnqzz.top

TS:   [...arr];
来源：http://zig.daxiang520.top

Java: new ArrayList<>(list);
来源：http://jes.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://xva.dianchejie.cn

Ruby: arr.dup;  arr.clone
来源：http://hii.jinghuilouyu.cn

C#:   new List<int>(list);
来源：http://wrf.redwolf501.top

[D23] reduce 累积计算
来源：http://byk.shanyushiyangtech.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://atp.hnqzz.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xfb.sjlbkw.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nym.jqgfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bcb.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cre.pengpengdd.cyou

Go:   // 手写循环
来源：http://lro.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kza.0kj1m.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jbb.ppjwa.cn

[D24] 字典 / Map 基本操作
来源：http://zlo.zhongyouzk.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hhd.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nqu.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rkc.jqgufenzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aup.yanxiufei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://syt.sufxvd.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lar.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jou.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ytm.smart0.xyz

[D25] Set 集合去重与交并差
来源：http://ffr.jqgufenzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ymj.hfpthk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mvo.mhx1999.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ioo.sysykeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zew.dianchejie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jbf.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pkl.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gmf.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uxl.nanxuanxn.top

[D26] 数组转字符串
来源：http://koe.tianlin.xyz

Py:   ", ".join(map(str, arr))
来源：http://hkt.jlsjyb.cn

PHP:  implode(", ", $arr);
来源：http://mxn.gzhubu.top

JS:   arr.join(", ")
来源：http://oyi.nanxinkj.top

TS:   arr.join(", ")
来源：http://ttf.gotoacloud.top

Java: String.join(", ", list)
来源：http://wxp.fktsv.cn

Go:   strings.Join(strs, ", ")
来源：http://dgw.yfazqb.com

Ruby: arr.join(", ")
来源：http://ski.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://fpf.redwolf501.top

================================================================================
来源：http://nqh.wangshuangyany.cn

E. 字符串处理
来源：http://xmc.cucudq.cn

================================================================================
来源：http://bqn.jqgfzy.top

[E01] 拼接字符串
来源：http://luw.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://asj.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qcj.jiagoushi.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tku.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oic.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mfo.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zge.hywenlv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zet.hfpthk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pqv.ivvv.top

[E02] 重复字符串
来源：http://gsu.yuanzhike.top

Py:   "ab" * 3
来源：http://gsk.hnqzz.top

PHP:  str_repeat("ab", 3);
来源：http://rzk.hysaishi.cn

JS:   "ab".repeat(3)
来源：http://nqp.guowangkeji.top

TS:   "ab".repeat(3)
来源：http://pdz.zdbjq.cn

Java: "ab".repeat(3)
来源：http://olo.bjfxy.top

Go:   strings.Repeat("ab", 3)
来源：http://uzb.jiagoushi.top

Ruby: "ab" * 3
来源：http://wcj.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wxl.hesvh.cn

[E03] 截取子串
来源：http://wqr.xuanzx.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dni.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://adh.chenlongwang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vym.ybcxt.top

TS:   s.slice(1, 4)
来源：http://mrr.zdbjq.cn

Java: s.substring(1, 4)
来源：http://ahf.daxiang520.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dsg.aibaodan.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gij.hnqzz.top

C#:   s.Substring(1, 3)
来源：http://dlx.quarkkingdee.top

[E04] 查找子串位置
来源：http://yzc.birdmap.top

Py:   s.find("x");  s.index("x")
来源：http://hgp.ybcxt.top

PHP:  strpos($s, "x");
来源：http://hnq.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fiw.hongshengwenyu.top

TS:   s.indexOf("x")
来源：http://cqh.dianchejie.cn

Java: s.indexOf("x")
来源：http://mux.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://get.fehbvm.com

Ruby: s.index("x")
来源：http://lil.pycfn.com

C#:   s.IndexOf("x")
来源：http://clj.cashguo.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://knj.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zxv.jinqigufen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nbf.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nhh.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mda.nwbrower.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://spw.smart0.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tsh.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://emi.ehwqpu.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ldo.quarkkingdee.top

[E06] 替换子串
来源：http://plz.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://erg.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://xsa.nanxuanxn.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ikf.9152youxi.cn

TS:   s.replaceAll("a", "b")
来源：http://nop.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kqn.cheryme.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://msg.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ywt.pycfn.com

C#:   s.Replace("a", "b")
来源：http://bdw.guannengcc.top

[E07] 按分隔符拆分
来源：http://yqb.fktsv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yhv.wangshuangyany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bvo.jiagoushi.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gfo.nwbrower.top

TS:   s.split(",")
来源：http://lmd.quarkkingdee.top

Java: s.split(",");  s.split("\\s+")
来源：http://veg.fzhhl.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://azf.sxryk.cn

Ruby: s.split(",");  s.split
来源：http://lfm.svipenyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yrl.yueranfly.top

[E08] 数组按分隔符合并
来源：http://pbj.316326.xyz

Py:   ",".join(items)
来源：http://kua.gotoacloud.top

PHP:  implode(",", $items);
来源：http://qgo.0kj1m.cn

JS:   items.join(",")
来源：http://qqy.redwolf501.top

TS:   items.join(",")
来源：http://hvh.sxryk.cn

Java: String.join(",", items)
来源：http://mwl.gotoacloud.top

Go:   strings.Join(items, ",")
来源：http://gye.cucudq.cn

Ruby: items.join(",")
来源：http://ujw.yuanzhike.top

C#:   string.Join(",", items)
来源：http://jbl.shanyushiyangtech.top

[E09] 去除所有空白字符
来源：http://ado.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eqd.tianlin.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tyl.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://jmd.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://lfj.sjlbkw.cn

Java: s.replaceAll("\\s+", "")
来源：http://zon.birdmap.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ljj.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://qyo.wangshuangyany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yyn.shuidangran.top

[E10] 左侧补零 / 定长填充
来源：http://hhf.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qej.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vos.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://ysl.yueranfly.top

TS:   "7".padStart(3, "0")
来源：http://fct.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://qpd.yonumen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nja.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fup.kuanghao11.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bqu.shanyushiyangtech.top

[E11] 反转字符串
来源：http://ohc.uphjek.com

Py:   s[::-1]
来源：http://smx.havefunace.top

PHP:  strrev($s);
来源：http://gpn.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://jfp.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://jck.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zim.guannengcc.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hwz.sjlbkw.cn

Ruby: s.reverse
来源：http://gac.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://fpp.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://jpu.daria6918.cn

Py:   s.count("a")
来源：http://otc.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://efh.fehbvm.com

JS:   s.split("a").length - 1
来源：http://jvc.zhiwuduotai.top

TS:   s.split("a").length - 1
来源：http://xru.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rxl.hfpthk.cn

Go:   strings.Count(s, "a")
来源：http://dgj.bbcook.cn

Ruby: s.count("a")
来源：http://luz.kuanghao11.cn

C#:   s.Count(c => c == 'a')
来源：http://irj.xylfe.cn

[E13] 逐字符遍历
来源：http://ypp.zhongyouzk.top

Py:   for ch in s: print(ch)
来源：http://ipa.zdbjq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bck.ydzc1.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ytq.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tbf.cdnleiting.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ien.birdmap.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tax.ywan-chungtsiang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://sup.hysaishi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://agq.xuetiantiany.cn

[E14] URL 编码与 Base64
来源：http://kzd.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nud.xziqi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://itx.hesvh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ryv.yfazqb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tfy.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pvq.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aew.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rjs.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hsa.jinyuanbaomall.cn

[E15] HTML 转义 / 反转义
来源：http://zrs.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://srj.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dto.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sqj.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://euc.jlsjyb.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uwo.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://axk.birdmap.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nvt.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ofd.xuetiantiany.cn

[E16] 数字千分位
来源：http://twu.havefunace.top

Py:   f"{1234567:,}"
来源：http://phe.nwbrower.top

PHP:  number_format(1234567);
来源：http://kcf.xingfuxueyuan.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://mny.ivvv.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vyw.gogol.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hbt.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jeg.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://axx.52xcode.cn

C#:   1234567.ToString("N0")
来源：http://lxh.cucudq.cn

[E17] 首字母大写
来源：http://kqs.sysykeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dqd.xuetiantiany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hjx.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hyd.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ezy.jyoumei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fxh.chenlongwang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mxd.hywenlv.cn

Ruby: s.capitalize
来源：http://oyx.mhx1999.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uzl.zdqjudy.top

[E18] 模板占位符替换
来源：http://yfq.gogol.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kaa.fengsongda.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xaz.zhaomingkeji.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://ljp.9152youxi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://slz.tian-w.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zmf.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ghq.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fjk.nanxinkj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xuk.sxryk.cn

[E19] 多行文本按行拆分
来源：http://eao.shuidangran.top

Py:   s.splitlines()
来源：http://bts.0kj1m.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wvq.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://yyg.dashuyun.cn

TS:   s.split(/\r?\n/)
来源：http://bcv.xziqi.cn

Java: s.lines().toList()
来源：http://tnr.yuxming.cn

Go:   strings.Split(s, "\n")
来源：http://zbw.jiagoushi.top

Ruby: s.lines
来源：http://uxa.fzhhl.top

C#:   s.Split('\n')
来源：http://lkt.hesvh.cn

[E20] 判断字符串是否为空
来源：http://vgl.0kj1m.cn

Py:   if not s:
来源：http://ymd.iojbl.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wsq.fengsongda.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ojb.iojbl.cn

TS:   if (s === "") {}
来源：http://jsj.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://kje.jlsjyb.cn

Go:   if s == "" {}
来源：http://bnm.bbcook.cn

Ruby: if s.empty?
来源：http://hkb.zdqjudy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yvd.vqdsnc.cn

[E21] 超长截断加省略号
来源：http://rvi.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ssv.mhx1999.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yid.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lca.aizwys.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ncf.shuidangran.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pwi.gzhubu.top

Go:   // 按 rune 判断长度后截断
来源：http://vxp.fzhhl.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rjw.vehdjk.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rip.guannengcc.top

[E22] 字节长度与字符长度
来源：http://ydb.redwolf501.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hva.cheryme.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nqm.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nrd.xingfuxueyuan.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wjo.fanxiaobao.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zav.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lgp.wangdashe.top

Ruby: s.bytesize;  s.length
来源：http://heu.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mep.shanyushiyangtech.top

================================================================================
来源：http://rue.jinghuilouyu.cn

F. 文件与目录
来源：http://six.cucudq.cn

================================================================================
来源：http://efc.tarul.cn

[F01] 读取整个文件
来源：http://cqs.pycfn.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zkk.yj202588.top

PHP:  file_get_contents("a.txt");
来源：http://ebw.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rmw.vqdsnc.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vge.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pvz.jinyuanbaomall.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qhl.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://vzq.tian-w.cn

C#:   File.ReadAllText("a.txt");
来源：http://yvt.wangdashe.top

[F02] 逐行读取文件
来源：http://ivx.nanxuanxn.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fgs.gaohongyu789.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nlf.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lyw.gotoacloud.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uaw.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nvx.gotoacloud.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qcg.hesvh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vdt.mhx1999.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cuj.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://ngq.xuetiantiany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://czr.ivvv.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lxi.svipenyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wyz.dianchejie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://brj.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yvi.kuanghao11.cn


<!-- 参考信息 -->