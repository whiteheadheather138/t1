代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cgn.xingfuxueyuan.xyz

PHP:  array_merge(...$nested);
来源：http://ujd.jqgfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rwe.yangfankeji.com

TS:   nested.flat();
来源：http://ull.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://znn.gaohongyu789.top

Go:   // 手写双层循环
来源：http://ttr.daria6918.cn

Ruby: nested.flatten
来源：http://wid.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ynv.iojbl.cn

[D19] 按字段分组
来源：http://xrn.yuanzhike.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qdn.xylfe.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uhk.gaohongyu789.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dzz.yuanzhike.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hng.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iik.feifeiyinyue.top

Go:   // 手写 map[string][]T
来源：http://etn.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kem.zhiwuduotai.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ddy.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://zye.0kj1m.cn

Py:   Counter(arr)
来源：http://aky.shanyushiyangkeji.top

PHP:  array_count_values($arr);
来源：http://wmq.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sab.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hxn.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nxq.chenzaomai.com

Go:   // 手写 map[T]int
来源：http://dff.birdmap.top

Ruby: arr.tally
来源：http://rdn.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nlz.shuidangran.top

[D21] 判断是否包含某元素
来源：http://ybk.jinyuanbaomall.cn

Py:   x in arr
来源：http://hrr.fehbvm.com

PHP:  in_array($x, $arr, true);
来源：http://uwt.yueranfly.top

JS:   arr.includes(x)
来源：http://xwv.yuxming.cn

TS:   arr.includes(x)
来源：http://hfk.hnxiangtu.top

Java: list.contains(x)
来源：http://tqo.mhx1999.top

Go:   slices.Contains(arr, x)
来源：http://gkf.smart0.xyz

Ruby: arr.include?(x)
来源：http://ryu.yuxming.cn

C#:   list.Contains(x)
来源：http://yki.gzhubu.top

[D22] 复制数组（避免共享引用）
来源：http://xcw.yonumen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://htq.jinyuanbaomall.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://izp.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ian.guowangkeji.top

TS:   [...arr];
来源：http://snu.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://upy.wangshuangyany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ezf.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://ird.hammf.cn

C#:   new List<int>(list);
来源：http://lti.hnxiangtu.top

[D23] reduce 累积计算
来源：http://qzy.cashguo.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xac.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bzl.andypj.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ydt.wangshuangyany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eib.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rdr.fengsongda.top

Go:   // 手写循环
来源：http://rzs.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kew.haohaochexian.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sxi.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://vps.sweek.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://smd.tian-w.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gxt.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hgo.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gab.yvedp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rln.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fdy.jinqigufen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://efh.zhiwuduotai.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qeq.tarul.cn

[D25] Set 集合去重与交并差
来源：http://wye.fktsv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://syg.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tbv.ydjk.org.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://njp.tian-w.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://saf.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ekm.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://doa.shangyingyoupin.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sma.aibaodan.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ddu.yj20258888.top

[D26] 数组转字符串
来源：http://wpo.xingfuxueyuan.xyz

Py:   ", ".join(map(str, arr))
来源：http://lgt.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://pwb.jqgfzy.top

JS:   arr.join(", ")
来源：http://gvw.yanxiufei.cn

TS:   arr.join(", ")
来源：http://rxl.hnqzz.top

Java: String.join(", ", list)
来源：http://yzw.cashguo.top

Go:   strings.Join(strs, ", ")
来源：http://zzf.snrcjt.cn

Ruby: arr.join(", ")
来源：http://mbl.sxryk.cn

C#:   string.Join(", ", list)
来源：http://hih.bbcook.cn

================================================================================
来源：http://vfk.zdbjq.cn

E. 字符串处理
来源：http://vfc.chenlongwang.top

================================================================================
来源：http://viy.bbcook.cn

[E01] 拼接字符串
来源：http://poj.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dub.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lqg.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fdd.kuanghao11.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cru.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pbl.havefunace.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ipr.ctjpmb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://izn.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tsb.yvedp.cn

[E02] 重复字符串
来源：http://djd.zhengqikj.top

Py:   "ab" * 3
来源：http://jra.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://zyw.zhijiandao.cn

JS:   "ab".repeat(3)
来源：http://tgm.cucudq.cn

TS:   "ab".repeat(3)
来源：http://tgu.hnqzz.top

Java: "ab".repeat(3)
来源：http://jah.chenjidiqi.icu

Go:   strings.Repeat("ab", 3)
来源：http://htg.bjfxy.top

Ruby: "ab" * 3
来源：http://jpf.fktsv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gkq.yuanzhike.top

[E03] 截取子串
来源：http://ciu.ywan-chungtsiang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://san.gogol.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mpz.shanyushiyangtech.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hko.chenzaomai.com

TS:   s.slice(1, 4)
来源：http://yzi.yangfankeji.com

Java: s.substring(1, 4)
来源：http://eek.cqqwz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lsl.pengpengdd.cyou

Ruby: s[1, 3];  s[1..3]
来源：http://sih.xinyue.icu

C#:   s.Substring(1, 3)
来源：http://dhz.yanxiufei.cn

[E04] 查找子串位置
来源：http://qgc.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://lup.zhijiandao.cn

PHP:  strpos($s, "x");
来源：http://qba.yj20258888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jvd.bjfxy.top

TS:   s.indexOf("x")
来源：http://cvh.52xcode.cn

Java: s.indexOf("x")
来源：http://cco.hnqzz.top

Go:   strings.Index(s, "x")
来源：http://sue.fktsv.cn

Ruby: s.index("x")
来源：http://fph.aibaodan.cn

C#:   s.IndexOf("x")
来源：http://xci.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://cey.tianlin.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ell.yanxiufei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gmg.fengsongda.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hox.ywan-chungtsiang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rfx.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jaq.quarkkingdee.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://brp.jianghu66.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rvm.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hbg.nwbrower.top

[E06] 替换子串
来源：http://hop.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://czm.cucudq.cn

PHP:  str_replace("a", "b", $s);
来源：http://qji.zycfv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xjw.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://znd.nwbrower.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ftu.fktsv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oeo.cdnleiting.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://etm.dashuyun.cn

C#:   s.Replace("a", "b")
来源：http://ori.tianlin.xyz

[E07] 按分隔符拆分
来源：http://dog.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oqr.zdqjudy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xny.epnwcf.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://ypt.xinyue.icu

TS:   s.split(",")
来源：http://opa.dianchejie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tyj.hnqzz.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://txl.jinqigfzy.top

Ruby: s.split(",");  s.split
来源：http://mkm.nanxuanxn.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bym.jqgfzy.top

[E08] 数组按分隔符合并
来源：http://kit.smart0.xyz

Py:   ",".join(items)
来源：http://nkm.sweek.top

PHP:  implode(",", $items);
来源：http://zjo.jlsjyb.cn

JS:   items.join(",")
来源：http://lxe.hongshengwenyu.top

TS:   items.join(",")
来源：http://mbm.zhaomingkeji.xyz

Java: String.join(",", items)
来源：http://ikm.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://ihj.snrcjt.cn

Ruby: items.join(",")
来源：http://gzn.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://ryw.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://rru.zhongyouzk.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ugd.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zjc.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://vgy.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://pta.mhx1999.top

Java: s.replaceAll("\\s+", "")
来源：http://bzw.52xcode.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://biq.zhiwuduotai.top

Ruby: s.gsub(/\s+/, "")
来源：http://lli.shuidangran.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sgy.zdqjudy.top

[E10] 左侧补零 / 定长填充
来源：http://phx.birdmap.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mwp.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ftn.aibaodan.cn

JS:   "7".padStart(3, "0")
来源：http://dyt.c1oappe.top

TS:   "7".padStart(3, "0")
来源：http://pij.jiagoushi.top

Java: String.format("%03d", 7)
来源：http://dub.tarul.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xre.wangdashe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zyt.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qzo.hfpthk.cn

[E11] 反转字符串
来源：http://ost.xuetiantiany.cn

Py:   s[::-1]
来源：http://hqz.fanxiaobao.xyz

PHP:  strrev($s);
来源：http://xqx.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://yux.havefunace.top

TS:   [...s].reverse().join("")
来源：http://sel.yfazqb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://cmd.chenzaomai.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://giq.smart0.xyz

Ruby: s.reverse
来源：http://cjm.gaohongyu789.top

C#:   new string(s.Reverse().ToArray())
来源：http://edb.andypj.xyz

[E12] 统计某字符出现次数
来源：http://cwr.jqgfzy.top

Py:   s.count("a")
来源：http://rcj.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://kgq.shanyushiyangtech.top

JS:   s.split("a").length - 1
来源：http://hhu.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://jkn.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rwm.hfpthk.cn

Go:   strings.Count(s, "a")
来源：http://vnh.sysykeji.top

Ruby: s.count("a")
来源：http://mei.hnqzz.top

C#:   s.Count(c => c == 'a')
来源：http://egb.nanxuanxn.top

[E13] 逐字符遍历
来源：http://oww.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://xbw.sxryk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jpm.guannengcc.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://sdf.aibaodan.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://svp.yongpay.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qgt.xylfe.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://afk.ppjwa.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xoo.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gsz.jinqigufen.top

[E14] URL 编码与 Base64
来源：http://ero.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xed.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pwo.pengpengdd.cyou

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gel.birdmap.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bxk.kuanghao11.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bdb.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jrk.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fma.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bvo.daria6918.cn

[E15] HTML 转义 / 反转义
来源：http://ces.shanyushiyangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vqx.jyoumei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rlx.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://buk.gotoacloud.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nrg.zhoulong.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gym.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://utc.xuetiantiany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ecu.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oii.shangyingyoupin.top

[E16] 数字千分位
来源：http://hlz.shuidangran.top

Py:   f"{1234567:,}"
来源：http://ing.yvedp.cn

PHP:  number_format(1234567);
来源：http://hxk.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ttb.jianghu66.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mwf.gzhubu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wax.daxiang520.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ibs.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lxt.zhaomingkeji.xyz

C#:   1234567.ToString("N0")
来源：http://amw.redwolf501.top

[E17] 首字母大写
来源：http://vzo.aizwys.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hdw.chenzaomai.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://rkb.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ipt.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hte.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://flu.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://umq.vqdsnc.cn

Ruby: s.capitalize
来源：http://nch.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ipi.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://gzk.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jqj.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kgt.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://myy.vehdjk.com

TS:   tpl.replaceAll("{name}", name)
来源：http://onx.tarul.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mus.yj202588.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gcp.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://guu.nwbrower.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ujc.zhiwuduotai.top

[E19] 多行文本按行拆分
来源：http://zib.snrcjt.cn

Py:   s.splitlines()
来源：http://whv.nwbrower.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sps.zhixingplan.top

JS:   s.split(/\r?\n/)
来源：http://bug.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://obk.hnqzz.top

Java: s.lines().toList()
来源：http://ywp.sxryk.cn

Go:   strings.Split(s, "\n")
来源：http://oyn.xuanzx.com

Ruby: s.lines
来源：http://rog.mhx1999.top

C#:   s.Split('\n')
来源：http://emm.gaohongyu789.top

[E20] 判断字符串是否为空
来源：http://rpo.hywenlv.cn

Py:   if not s:
来源：http://gwv.guowangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://znw.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pqs.zycfv.cn

TS:   if (s === "") {}
来源：http://cwq.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://fqg.xziqi.cn

Go:   if s == "" {}
来源：http://ajh.jinqigufen.top

Ruby: if s.empty?
来源：http://svh.gotoacloud.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nsl.xuetiantiany.cn

[E21] 超长截断加省略号
来源：http://xjn.hcnkem.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qjc.guannengcc.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://crh.vehdjk.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://czx.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ume.zycfv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://msr.jlsjyb.cn

Go:   // 按 rune 判断长度后截断
来源：http://mvl.redwolf501.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kbw.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zzk.mhx1999.top

[E22] 字节长度与字符长度
来源：http://ecg.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yib.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fpu.nanxuanxn.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hbr.tian-w.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wbx.cucudq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iyv.nanxinkj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://stq.yfazqb.com

Ruby: s.bytesize;  s.length
来源：http://ofz.jinyuanbaomall.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fxz.zhengqikj.top

================================================================================
来源：http://wti.redwolf501.top

F. 文件与目录
来源：http://jdl.xuanzx.com

================================================================================
来源：http://szg.cucudq.cn

[F01] 读取整个文件
来源：http://pfp.zhoulong.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ira.gogol.net.cn

PHP:  file_get_contents("a.txt");
来源：http://jtq.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hjc.wangshuangyany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dbc.hywenlv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lta.dianchejie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ebm.gzhubu.top

Ruby: File.read("a.txt")
来源：http://rpn.andypj.xyz

C#:   File.ReadAllText("a.txt");
来源：http://muo.cheryme.top

[F02] 逐行读取文件
来源：http://qvc.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fig.xuetiantiany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bmn.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dzm.mhx1999.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eau.jqgufenzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ifm.redwolf501.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tem.jinqigfzy.top


<!-- 参考信息 -->