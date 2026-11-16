代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cfq.guannengcc.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://thi.zycfv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ndn.zycfv.cn

Go:   // 手写循环累加
来源：http://ueh.zhijiandao.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bxs.yfazqb.com

C#:   list.Sum();  list.Average()
来源：http://tzr.jiagoushi.top

[D17] 最大值与最小值
来源：http://ctq.sysykeji.top

Py:   max(arr);  min(arr)
来源：http://dki.jinqigufen.top

PHP:  max($arr);  min($arr);
来源：http://aod.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nqp.sweek.top

TS:   Math.max(...arr);
来源：http://lsk.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mtp.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hri.ydzc1.top

Ruby: arr.max;  arr.min
来源：http://rkj.yfazqb.com

C#:   list.Max();  list.Min()
来源：http://usq.ivvv.top

[D18] 扁平化嵌套数组
来源：http://iih.chenjidiqi.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://opa.feifeiyinyue.top

PHP:  array_merge(...$nested);
来源：http://zfy.sjlbkw.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gvp.ydjk.org.cn

TS:   nested.flat();
来源：http://svx.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jdx.yanxiufei.cn

Go:   // 手写双层循环
来源：http://gfs.hcnkem.com

Ruby: nested.flatten
来源：http://ojz.xuanzx.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://icg.pycfn.com

[D19] 按字段分组
来源：http://vxt.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ftl.vqdsnc.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qpl.feifeiyinyue.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://upe.ywan-chungtsiang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hyj.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://svr.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://wsx.hesvh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oom.0kj1m.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lho.cqqwz.cn

[D20] 统计每个元素出现次数
来源：http://bqs.jinqigfzy.top

Py:   Counter(arr)
来源：http://bya.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://dtf.hesvh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kkp.ivvv.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://khj.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mhi.fehbvm.com

Go:   // 手写 map[T]int
来源：http://cmk.hongshengwenyu.top

Ruby: arr.tally
来源：http://mki.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cqn.tian-w.cn

[D21] 判断是否包含某元素
来源：http://lnn.jyoumei.cn

Py:   x in arr
来源：http://dkx.meibo888.top

PHP:  in_array($x, $arr, true);
来源：http://jza.cucudq.cn

JS:   arr.includes(x)
来源：http://acj.guowangkeji.top

TS:   arr.includes(x)
来源：http://osj.ybcxt.top

Java: list.contains(x)
来源：http://ftz.pycfn.com

Go:   slices.Contains(arr, x)
来源：http://zhw.fehbvm.com

Ruby: arr.include?(x)
来源：http://hwr.xuetiantiany.cn

C#:   list.Contains(x)
来源：http://tpt.tarul.cn

[D22] 复制数组（避免共享引用）
来源：http://zib.zhiwuduotai.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://unr.daxiang520.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xpv.sufxvd.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fry.jinghuilouyu.cn

TS:   [...arr];
来源：http://wbe.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://piq.316326.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://svk.hnxiangtu.top

Ruby: arr.dup;  arr.clone
来源：http://kwe.nanxuanxn.top

C#:   new List<int>(list);
来源：http://szx.quarkkingdee.top

[D23] reduce 累积计算
来源：http://qqq.shzxlz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fzf.fanxiaobao.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kxn.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kqh.gotoacloud.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://plu.chenzaomai.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://tyk.daxiang520.top

Go:   // 手写循环
来源：http://vpc.xuanzx.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ldu.birdmap.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wlq.hnqzz.top

[D24] 字典 / Map 基本操作
来源：http://dba.feifeiyinyue.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wok.redwolf501.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sze.shangyingyoupin.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iou.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vmr.zhijiandao.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wtq.fzhhl.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nkk.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dqs.mhx1999.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oaw.gzhubu.top

[D25] Set 集合去重与交并差
来源：http://gyq.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kpm.xinyue.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ufw.yuanzhike.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cvd.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ceu.jinqigfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wrm.316326.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wfg.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mgm.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dze.tanke756.top

[D26] 数组转字符串
来源：http://eoh.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://oxx.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://due.aizwys.cn

JS:   arr.join(", ")
来源：http://wfr.wangshuangyany.cn

TS:   arr.join(", ")
来源：http://qfd.xziqi.cn

Java: String.join(", ", list)
来源：http://cdg.sxryk.cn

Go:   strings.Join(strs, ", ")
来源：http://zrq.nanxinkj.top

Ruby: arr.join(", ")
来源：http://dht.daxiang520.top

C#:   string.Join(", ", list)
来源：http://pws.gogol.net.cn

================================================================================
来源：http://umn.svipenyu.cn

E. 字符串处理
来源：http://wlj.52xcode.cn

================================================================================
来源：http://emg.sweek.top

[E01] 拼接字符串
来源：http://tqs.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xfo.shzxlz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cpa.snrcjt.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zkj.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://foo.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xps.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bgz.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oox.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://png.chenzaomai.com

[E02] 重复字符串
来源：http://kmi.feifeiyinyue.top

Py:   "ab" * 3
来源：http://qde.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://ehi.jianghu66.top

JS:   "ab".repeat(3)
来源：http://abi.sysykeji.top

TS:   "ab".repeat(3)
来源：http://xwg.hammf.cn

Java: "ab".repeat(3)
来源：http://hfu.shangyingyoupin.top

Go:   strings.Repeat("ab", 3)
来源：http://hvq.yuxming.cn

Ruby: "ab" * 3
来源：http://qxz.sweek.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kou.tarul.cn

[E03] 截取子串
来源：http://yxk.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xto.hysaishi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nqp.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zin.yuxming.cn

TS:   s.slice(1, 4)
来源：http://gqk.yj20258.top

Java: s.substring(1, 4)
来源：http://dyv.zhongyouzk.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xdm.hesvh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xqs.zhongyouzk.top

C#:   s.Substring(1, 3)
来源：http://myo.ydjk.org.cn

[E04] 查找子串位置
来源：http://whv.mhx1999.top

Py:   s.find("x");  s.index("x")
来源：http://eul.shzxlz.cn

PHP:  strpos($s, "x");
来源：http://any.snrcjt.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jny.hnqzz.top

TS:   s.indexOf("x")
来源：http://egi.xylfe.cn

Java: s.indexOf("x")
来源：http://lyr.shanyushiyangkeji.top

Go:   strings.Index(s, "x")
来源：http://sun.nanxinkj.top

Ruby: s.index("x")
来源：http://nvq.sweek.top

C#:   s.IndexOf("x")
来源：http://sbq.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://bcm.gaohongyu789.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cmh.yj20258888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vja.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bxi.dashuyun.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ile.jinqigfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vwr.bbcook.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dvg.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eul.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fco.zdbjq.cn

[E06] 替换子串
来源：http://ikc.xuanzx.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ebk.vehdjk.com

PHP:  str_replace("a", "b", $s);
来源：http://kcd.hongshengwenyu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wxf.zhiwuduotai.top

TS:   s.replaceAll("a", "b")
来源：http://aai.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aoh.aibaodan.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://idy.nanxuanxn.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yyf.sxryk.cn

C#:   s.Replace("a", "b")
来源：http://sed.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://lqw.pengpengdd.cyou

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fzs.yfazqb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oks.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ptw.svipenyu.cn

TS:   s.split(",")
来源：http://gpz.hammf.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ljc.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ebt.hysaishi.cn

Ruby: s.split(",");  s.split
来源：http://gue.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jpy.cqqwz.cn

[E08] 数组按分隔符合并
来源：http://gob.dianchejie.cn

Py:   ",".join(items)
来源：http://khe.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://tit.andypj.xyz

JS:   items.join(",")
来源：http://via.wangshuangyany.cn

TS:   items.join(",")
来源：http://udr.jyoumei.cn

Java: String.join(",", items)
来源：http://cbu.zycfv.cn

Go:   strings.Join(items, ",")
来源：http://uhj.yj202588.top

Ruby: items.join(",")
来源：http://zik.havefunace.top

C#:   string.Join(",", items)
来源：http://bpq.zdqjudy.top

[E09] 去除所有空白字符
来源：http://ziz.bbcook.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://swe.ehwqpu.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://znz.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://cdz.meibo888.top

TS:   s.replace(/\s+/g, "")
来源：http://uvr.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://nkl.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lth.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://kdg.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vbo.pengpengdd.cyou

[E10] 左侧补零 / 定长填充
来源：http://cnx.ydjk.org.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dgn.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://szv.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://mjk.tarul.cn

TS:   "7".padStart(3, "0")
来源：http://fvm.c1oappe.top

Java: String.format("%03d", 7)
来源：http://suh.jinghuilouyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nbg.cqqwz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ljp.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nct.xinyue.icu

[E11] 反转字符串
来源：http://wif.quarkkingdee.top

Py:   s[::-1]
来源：http://azd.shanyushiyangkeji.top

PHP:  strrev($s);
来源：http://zoh.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://zfc.shangyingyoupin.top

TS:   [...s].reverse().join("")
来源：http://emr.chenzaomai.com

Java: new StringBuilder(s).reverse().toString()
来源：http://xjh.gzhubu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hld.fanxiaobao.xyz

Ruby: s.reverse
来源：http://utx.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://irp.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://acr.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://oik.yongpay.top

PHP:  substr_count($s, "a");
来源：http://etj.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://cmo.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://uit.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ldm.tanke756.top

Go:   strings.Count(s, "a")
来源：http://kps.yangfankeji.com

Ruby: s.count("a")
来源：http://jbr.xinyue.icu

C#:   s.Count(c => c == 'a')
来源：http://vbv.quarkkingdee.top

[E13] 逐字符遍历
来源：http://isj.nanxuanxn.top

Py:   for ch in s: print(ch)
来源：http://kbn.316326.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ngc.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yly.yangfankeji.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://two.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lur.zhixingplan.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://deb.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bhi.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xhr.ydzc1.top

[E14] URL 编码与 Base64
来源：http://koc.ywan-chungtsiang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nfd.52xcode.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jxh.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wwx.yfazqb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zcu.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nbs.yanxiufei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xnq.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ify.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xda.wangshuangyany.cn

[E15] HTML 转义 / 反转义
来源：http://wdv.chenjidiqi.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://ncg.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://khc.9152youxi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yjy.fehbvm.com

TS:   // 同上，务必做 XSS 过滤
来源：http://lea.yfazqb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://asc.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://znm.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vme.jqgufenzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zpd.fengsongda.top

[E16] 数字千分位
来源：http://ptw.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://ddo.fanxiaobao.xyz

PHP:  number_format(1234567);
来源：http://ncj.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ahq.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cbe.bbcook.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ncn.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zop.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yvk.xinyue.icu

C#:   1234567.ToString("N0")
来源：http://rre.nanxuanxn.top

[E17] 首字母大写
来源：http://dbw.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ssg.daxiang520.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hxl.hcnkem.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nhg.guowangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://noi.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lsd.kuanghao11.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zyq.smart0.xyz

Ruby: s.capitalize
来源：http://zxy.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tim.jyoumei.cn

[E18] 模板占位符替换
来源：http://ylo.cucudq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://spw.kuanghao11.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ptv.xylfe.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pin.pycfn.com

TS:   tpl.replaceAll("{name}", name)
来源：http://rae.xuanzx.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rbs.yfazqb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vpy.xingfuxueyuan.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ngd.hnxiangtu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://agv.yonumen.top

[E19] 多行文本按行拆分
来源：http://dlm.0kj1m.cn

Py:   s.splitlines()
来源：http://wvl.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bmk.sysykeji.top

JS:   s.split(/\r?\n/)
来源：http://xjh.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://amn.jqgufenzy.top

Java: s.lines().toList()
来源：http://scj.jinqigfzy.top

Go:   strings.Split(s, "\n")
来源：http://wld.zdqjudy.top

Ruby: s.lines
来源：http://akn.cashguo.top

C#:   s.Split('\n')
来源：http://hmg.nanxinkj.top

[E20] 判断字符串是否为空
来源：http://zmn.jinghuilouyu.cn

Py:   if not s:
来源：http://tzu.sweek.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jcu.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gje.9152youxi.cn

TS:   if (s === "") {}
来源：http://vqh.aibaodan.cn

Java: if (s.isEmpty()) {}
来源：http://zsm.jianghu66.top

Go:   if s == "" {}
来源：http://zgs.zhijiandao.cn

Ruby: if s.empty?
来源：http://fbm.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lqb.yvedp.cn

[E21] 超长截断加省略号
来源：http://dje.yongpay.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hyj.meibo888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vul.ctjpmb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fxz.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://udi.zhijiandao.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tmo.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://mpf.xziqi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ewj.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jjv.vehdjk.com

[E22] 字节长度与字符长度
来源：http://pjl.pycfn.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://puz.zhongyouzk.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://khe.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pqg.tian-w.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://axx.nanxinkj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bre.sysykeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dge.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://rya.jinyuanbaomall.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mvv.shanyushiyangtech.top

================================================================================
来源：http://fpe.cucudq.cn

F. 文件与目录
来源：http://uqo.havefunace.top

================================================================================
来源：http://vsj.yfazqb.com


<!-- 参考信息 -->