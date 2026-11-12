代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hew.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://qut.zhiwuduotai.top

[D17] 最大值与最小值
来源：http://ybd.nwbrower.top

Py:   max(arr);  min(arr)
来源：http://kda.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://gzu.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fuh.daxiang520.top

TS:   Math.max(...arr);
来源：http://slo.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lzx.snrcjt.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lth.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://opf.fengsongda.top

C#:   list.Max();  list.Min()
来源：http://lks.xylfe.cn

[D18] 扁平化嵌套数组
来源：http://itk.zhoulong.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cav.yuxming.cn

PHP:  array_merge(...$nested);
来源：http://pcz.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rei.c1oappe.top

TS:   nested.flat();
来源：http://pst.zdqjudy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dks.jyoumei.cn

Go:   // 手写双层循环
来源：http://bae.jianghu66.top

Ruby: nested.flatten
来源：http://vvg.pycfn.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://gvv.pycfn.com

[D19] 按字段分组
来源：http://wlc.birdmap.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oql.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lxc.52xcode.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bvp.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://roq.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zor.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://dfm.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://njq.feifeiyinyue.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gjy.gotoacloud.top

[D20] 统计每个元素出现次数
来源：http://pbz.daria6918.cn

Py:   Counter(arr)
来源：http://afm.daria6918.cn

PHP:  array_count_values($arr);
来源：http://ydm.sweek.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ylc.ybcxt.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://stn.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uvq.bbcook.cn

Go:   // 手写 map[T]int
来源：http://ozf.yfazqb.com

Ruby: arr.tally
来源：http://jxk.redwolf501.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fym.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://ajg.yj202588.top

Py:   x in arr
来源：http://whm.fanxiaobao.xyz

PHP:  in_array($x, $arr, true);
来源：http://rgw.wangshuangyany.cn

JS:   arr.includes(x)
来源：http://wem.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://ndi.gotoacloud.top

Java: list.contains(x)
来源：http://uga.gaohongyu789.top

Go:   slices.Contains(arr, x)
来源：http://odl.52xcode.cn

Ruby: arr.include?(x)
来源：http://dqt.nanxuanxn.top

C#:   list.Contains(x)
来源：http://plu.fengsongda.top

[D22] 复制数组（避免共享引用）
来源：http://pfe.yj202588.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bnl.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pnp.sufxvd.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dbq.svipenyu.cn

TS:   [...arr];
来源：http://uay.fktsv.cn

Java: new ArrayList<>(list);
来源：http://tgr.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://bcu.vehdjk.com

Ruby: arr.dup;  arr.clone
来源：http://ooj.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://owe.yongpay.top

[D23] reduce 累积计算
来源：http://yhz.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ask.gaohongyu789.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gqe.wangdashe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://krt.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xlt.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kbh.gogol.net.cn

Go:   // 手写循环
来源：http://qfq.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zav.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://obu.zhaomingkeji.xyz

[D24] 字典 / Map 基本操作
来源：http://fub.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oyx.meibo888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uzr.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qbx.xziqi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ivd.cheryme.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qop.epnwcf.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jdf.zdbjq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ibh.jqgfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kxb.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://cyj.fanxiaobao.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fpq.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uad.aibaodan.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cta.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zhq.kuanghao11.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jcr.nanxuanxn.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jkb.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vxn.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cqr.gogol.net.cn

[D26] 数组转字符串
来源：http://iaa.zhoulong.xyz

Py:   ", ".join(map(str, arr))
来源：http://xov.ivvv.top

PHP:  implode(", ", $arr);
来源：http://mxn.havefunace.top

JS:   arr.join(", ")
来源：http://dgk.hfpthk.cn

TS:   arr.join(", ")
来源：http://aly.aizwys.cn

Java: String.join(", ", list)
来源：http://yer.yj20258888.top

Go:   strings.Join(strs, ", ")
来源：http://jvs.zdbjq.cn

Ruby: arr.join(", ")
来源：http://ykk.xinyue.icu

C#:   string.Join(", ", list)
来源：http://hkg.sxryk.cn

================================================================================
来源：http://www.aibaodan.cn

E. 字符串处理
来源：http://ytp.jinghuilouyu.cn

================================================================================
来源：http://azf.hammf.cn

[E01] 拼接字符串
来源：http://lig.yj20258.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cnf.dashuyun.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qma.wangdashe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xlq.shanyushiyangtech.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cok.316326.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yyb.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://amx.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://avn.fktsv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ykf.svipenyu.cn

[E02] 重复字符串
来源：http://jhq.yuanzhike.top

Py:   "ab" * 3
来源：http://dfq.xziqi.cn

PHP:  str_repeat("ab", 3);
来源：http://pfg.meibo888.top

JS:   "ab".repeat(3)
来源：http://vlv.yangfankeji.com

TS:   "ab".repeat(3)
来源：http://mmg.wangdashe.top

Java: "ab".repeat(3)
来源：http://lte.xuetiantiany.cn

Go:   strings.Repeat("ab", 3)
来源：http://uto.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://rnl.sweek.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kyf.ehwqpu.com

[E03] 截取子串
来源：http://nnh.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kbr.hysaishi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nzy.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pdr.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://hnp.chenzaomai.com

Java: s.substring(1, 4)
来源：http://gzj.shangyingyoupin.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vna.smart0.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://kis.jinyuanbaomall.cn

C#:   s.Substring(1, 3)
来源：http://spn.jqgfzy.top

[E04] 查找子串位置
来源：http://jfj.guowangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://tue.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://ycr.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ork.yonumen.top

TS:   s.indexOf("x")
来源：http://teb.yj202588.top

Java: s.indexOf("x")
来源：http://uqp.hammf.cn

Go:   strings.Index(s, "x")
来源：http://glm.chenjidiqi.icu

Ruby: s.index("x")
来源：http://avc.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://mja.daria6918.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gyf.xuetiantiany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lor.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wlj.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rhn.cucudq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://amn.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fft.snrcjt.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mrn.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://smf.gotoacloud.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://abm.tanke756.top

[E06] 替换子串
来源：http://yev.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wuk.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://guw.pycfn.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vci.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://pzz.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wzy.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ect.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vfn.hnxiangtu.top

C#:   s.Replace("a", "b")
来源：http://owv.nanxinkj.top

[E07] 按分隔符拆分
来源：http://dap.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://slj.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dpw.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pwr.quarkkingdee.top

TS:   s.split(",")
来源：http://tot.zhengqikj.top

Java: s.split(",");  s.split("\\s+")
来源：http://twn.yj20258888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://apk.sweek.top

Ruby: s.split(",");  s.split
来源：http://cnw.shanyushiyangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ggv.hcnkem.com

[E08] 数组按分隔符合并
来源：http://wmp.meibo888.top

Py:   ",".join(items)
来源：http://pef.cheryme.top

PHP:  implode(",", $items);
来源：http://weh.pengpengdd.cyou

JS:   items.join(",")
来源：http://kto.hongshengwenyu.top

TS:   items.join(",")
来源：http://vsx.aibaodan.cn

Java: String.join(",", items)
来源：http://scm.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://qdh.52xcode.cn

Ruby: items.join(",")
来源：http://qnu.daxiang520.top

C#:   string.Join(",", items)
来源：http://xkp.tianlin.xyz

[E09] 去除所有空白字符
来源：http://bkv.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jac.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zeo.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://ber.jiagoushi.top

TS:   s.replace(/\s+/g, "")
来源：http://oka.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://zkh.fehbvm.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://spo.xuetiantiany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fqr.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jnf.shanyushiyangtech.top

[E10] 左侧补零 / 定长填充
来源：http://avn.cheryme.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uve.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fzy.xuetiantiany.cn

JS:   "7".padStart(3, "0")
来源：http://gjj.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://xdr.daxiang520.top

Java: String.format("%03d", 7)
来源：http://iqz.sweek.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://brt.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nro.sjlbkw.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ock.daria6918.cn

[E11] 反转字符串
来源：http://uyx.jqgufenzy.top

Py:   s[::-1]
来源：http://qgw.tianlin.xyz

PHP:  strrev($s);
来源：http://vkz.ivvv.top

JS:   [...s].reverse().join("")
来源：http://arv.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://ura.chenjidiqi.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://vfo.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tni.aibaodan.cn

Ruby: s.reverse
来源：http://xcu.tianlin.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://pmr.sufxvd.cn

[E12] 统计某字符出现次数
来源：http://lkb.cashguo.top

Py:   s.count("a")
来源：http://lxa.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://ipi.hfpthk.cn

JS:   s.split("a").length - 1
来源：http://xlt.andypj.xyz

TS:   s.split("a").length - 1
来源：http://mij.shzxlz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kkn.tian-w.cn

Go:   strings.Count(s, "a")
来源：http://whv.nwbrower.top

Ruby: s.count("a")
来源：http://hdg.ybcxt.top

C#:   s.Count(c => c == 'a')
来源：http://xtw.uphjek.com

[E13] 逐字符遍历
来源：http://bkp.dianchejie.cn

Py:   for ch in s: print(ch)
来源：http://emy.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nna.cdnleiting.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gbv.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://vwv.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hqs.zdbjq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kyx.xziqi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nch.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cmk.ivvv.top

[E14] URL 编码与 Base64
来源：http://xwz.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hdb.hcnkem.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://btq.iojbl.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://adf.nwbrower.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pgf.guowangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bsa.zycfv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://svt.zhongyouzk.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ont.fanxiaobao.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dgw.zhoulong.xyz

[E15] HTML 转义 / 反转义
来源：http://vin.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iyy.zhijiandao.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fuq.xuetiantiany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sah.xinyue.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://tct.cucudq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cpe.snrcjt.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xcc.sjlbkw.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zdi.zdbjq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mhx.zycfv.cn

[E16] 数字千分位
来源：http://ilb.haohaochexian.top

Py:   f"{1234567:,}"
来源：http://yst.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://ueh.zdbjq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wdx.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ybc.dashuyun.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jat.yj20258.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wmo.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wxs.316326.xyz

C#:   1234567.ToString("N0")
来源：http://sdq.xuetiantiany.cn

[E17] 首字母大写
来源：http://tke.sweek.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oca.nanxuanxn.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lee.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uvb.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fbq.wangshuangyany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://utn.daxiang520.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://evg.kuanghao11.cn

Ruby: s.capitalize
来源：http://fya.gzhubu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jof.tian-w.cn

[E18] 模板占位符替换
来源：http://frx.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fmy.fktsv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://afd.shuidangran.top

JS:   tpl.replaceAll("{name}", name)
来源：http://iec.316326.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://tcg.nwbrower.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wnv.dashuyun.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vvs.andypj.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aea.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lhb.hnqzz.top

[E19] 多行文本按行拆分
来源：http://asm.ehwqpu.com

Py:   s.splitlines()
来源：http://ims.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xoc.cdnleiting.top

JS:   s.split(/\r?\n/)
来源：http://agm.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://hoe.sysykeji.top

Java: s.lines().toList()
来源：http://ets.ppjwa.cn

Go:   strings.Split(s, "\n")
来源：http://zoq.zhongyouzk.top

Ruby: s.lines
来源：http://loh.feifeiyinyue.top

C#:   s.Split('\n')
来源：http://wuq.ivvv.top

[E20] 判断字符串是否为空
来源：http://stp.ydzc1.top

Py:   if not s:
来源：http://qnc.cdnleiting.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zsy.hywenlv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wqn.bjfxy.top

TS:   if (s === "") {}
来源：http://tit.cucudq.cn

Java: if (s.isEmpty()) {}
来源：http://dur.redwolf501.top

Go:   if s == "" {}
来源：http://phh.xziqi.cn

Ruby: if s.empty?
来源：http://xrz.cheryme.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uiw.yuxming.cn

[E21] 超长截断加省略号
来源：http://vfx.dashuyun.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qey.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jle.kuanghao11.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ekz.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://djc.ydzc1.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pej.yangfankeji.com

Go:   // 按 rune 判断长度后截断
来源：http://vph.jinghuilouyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ofj.xuanzx.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://swb.shuidangran.top

[E22] 字节长度与字符长度
来源：http://eur.xingfuxueyuan.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lpw.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://alq.fehbvm.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://snu.sxryk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pxc.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zlp.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fag.hywenlv.cn

Ruby: s.bytesize;  s.length
来源：http://jlv.zhijiandao.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://egb.yongpay.top

================================================================================
来源：http://xnp.tanke756.top

F. 文件与目录
来源：http://aqf.shanyushiyangtech.top

================================================================================
来源：http://ine.cheryme.top

[F01] 读取整个文件
来源：http://fbq.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lml.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://cnm.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uqg.hongshengwenyu.top


<!-- 参考信息 -->