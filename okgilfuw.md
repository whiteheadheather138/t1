代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xkd.pengpengdd.cyou

C#:   list.Sum();  list.Average()
来源：http://bqo.shangyingyoupin.top

[D17] 最大值与最小值
来源：http://nfx.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://xqd.ehwqpu.com

PHP:  max($arr);  min($arr);
来源：http://wcj.fehbvm.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pik.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://vrs.sxryk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tgi.mhx1999.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dgh.yj20258.top

Ruby: arr.max;  arr.min
来源：http://xjv.uphjek.com

C#:   list.Max();  list.Min()
来源：http://ylb.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://get.gzhubu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zve.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://kvi.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hzj.jinqigfzy.top

TS:   nested.flat();
来源：http://dza.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fgw.ybcxt.top

Go:   // 手写双层循环
来源：http://kas.yonumen.top

Ruby: nested.flatten
来源：http://nwb.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bvp.chenlongwang.top

[D19] 按字段分组
来源：http://ojg.sufxvd.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ahp.shangyingyoupin.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pwg.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xfn.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gxa.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eby.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://pvy.bbcook.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jyx.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tzh.aibaodan.cn

[D20] 统计每个元素出现次数
来源：http://hpw.mhx1999.top

Py:   Counter(arr)
来源：http://fod.chenlongwang.top

PHP:  array_count_values($arr);
来源：http://mwk.epnwcf.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dvz.hnxiangtu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zvh.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://efe.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://lrj.zdqjudy.top

Ruby: arr.tally
来源：http://dii.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ohj.gzhubu.top

[D21] 判断是否包含某元素
来源：http://bzn.gzhubu.top

Py:   x in arr
来源：http://hnu.fktsv.cn

PHP:  in_array($x, $arr, true);
来源：http://ymh.zhaomingkeji.xyz

JS:   arr.includes(x)
来源：http://zdv.yfazqb.com

TS:   arr.includes(x)
来源：http://hlc.jqgfzy.top

Java: list.contains(x)
来源：http://bpf.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://zts.gzhubu.top

Ruby: arr.include?(x)
来源：http://owx.gogol.net.cn

C#:   list.Contains(x)
来源：http://khi.ehwqpu.com

[D22] 复制数组（避免共享引用）
来源：http://bwk.zhijiandao.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fkf.yangfankeji.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vwb.jinghuilouyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ntl.redwolf501.top

TS:   [...arr];
来源：http://dya.jyoumei.cn

Java: new ArrayList<>(list);
来源：http://izl.9152youxi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qcj.jinqigufen.top

Ruby: arr.dup;  arr.clone
来源：http://kgz.ppjwa.cn

C#:   new List<int>(list);
来源：http://xdj.fzhhl.top

[D23] reduce 累积计算
来源：http://oxq.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://guf.yueranfly.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bfz.aizwys.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://san.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sxb.aizwys.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gwd.yanxiufei.cn

Go:   // 手写循环
来源：http://qlh.316326.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://coc.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nul.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://zfu.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eik.shanyushiyangtech.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tkh.tianlin.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rkc.cdnleiting.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://den.ydzc1.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ocp.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ljh.aizwys.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://idd.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qdv.cheryme.top

[D25] Set 集合去重与交并差
来源：http://mcv.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rjh.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xiz.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rmi.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ndu.yfazqb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nbr.aizwys.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gcb.wangdashe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tcr.9152youxi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kqg.zhiwuduotai.top

[D26] 数组转字符串
来源：http://uyv.bjfxy.top

Py:   ", ".join(map(str, arr))
来源：http://kbd.xuetiantiany.cn

PHP:  implode(", ", $arr);
来源：http://giu.yongpay.top

JS:   arr.join(", ")
来源：http://vcm.zhengqikj.top

TS:   arr.join(", ")
来源：http://jnb.sxryk.cn

Java: String.join(", ", list)
来源：http://kos.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://ved.sysykeji.top

Ruby: arr.join(", ")
来源：http://zje.yuxming.cn

C#:   string.Join(", ", list)
来源：http://kje.9152youxi.cn

================================================================================
来源：http://fpz.yj20258888.top

E. 字符串处理
来源：http://hvu.sxryk.cn

================================================================================
来源：http://hri.aibaodan.cn

[E01] 拼接字符串
来源：http://sax.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://krj.sufxvd.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vnc.hfpthk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dov.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tqc.yj20258.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zag.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uto.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://czh.tianlin.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sgw.9152youxi.cn

[E02] 重复字符串
来源：http://zng.zhiwuduotai.top

Py:   "ab" * 3
来源：http://ptg.gzhubu.top

PHP:  str_repeat("ab", 3);
来源：http://fky.shanyushiyangtech.top

JS:   "ab".repeat(3)
来源：http://ezv.guannengcc.top

TS:   "ab".repeat(3)
来源：http://rvt.smart0.xyz

Java: "ab".repeat(3)
来源：http://kei.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://gmc.cqqwz.cn

Ruby: "ab" * 3
来源：http://dqb.shuidangran.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://afc.zhiwuduotai.top

[E03] 截取子串
来源：http://fph.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aqz.chenzaomai.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jdx.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ilg.ydzc1.top

TS:   s.slice(1, 4)
来源：http://srz.vehdjk.com

Java: s.substring(1, 4)
来源：http://xye.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sul.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://ifg.chenjidiqi.icu

C#:   s.Substring(1, 3)
来源：http://oth.yangfankeji.com

[E04] 查找子串位置
来源：http://vpj.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://afg.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://gbg.pycfn.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wmz.tarul.cn

TS:   s.indexOf("x")
来源：http://qru.316326.xyz

Java: s.indexOf("x")
来源：http://neo.xziqi.cn

Go:   strings.Index(s, "x")
来源：http://upz.snrcjt.cn

Ruby: s.index("x")
来源：http://ait.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://vkh.yfazqb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://web.shangyingyoupin.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ksn.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mvw.xziqi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uuq.sweek.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://usb.tarul.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zux.hammf.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gsc.zhongyouzk.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yfq.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fkl.hcnkem.com

[E06] 替换子串
来源：http://vvl.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ijk.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://afw.ywan-chungtsiang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yhu.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://alo.quarkkingdee.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cgt.kuanghao11.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://grw.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mnb.jqgufenzy.top

C#:   s.Replace("a", "b")
来源：http://rfx.yj202588.top

[E07] 按分隔符拆分
来源：http://eiw.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://abs.52xcode.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vju.yj20258.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ulv.gaohongyu789.top

TS:   s.split(",")
来源：http://dns.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://dap.ywan-chungtsiang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nxl.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://rcz.mhx1999.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zwm.gotoacloud.top

[E08] 数组按分隔符合并
来源：http://hsd.epnwcf.com

Py:   ",".join(items)
来源：http://czw.havefunace.top

PHP:  implode(",", $items);
来源：http://gvy.jiagoushi.top

JS:   items.join(",")
来源：http://hnl.quarkkingdee.top

TS:   items.join(",")
来源：http://tcu.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://ytx.fanxiaobao.xyz

Go:   strings.Join(items, ",")
来源：http://nlr.shanyushiyangkeji.top

Ruby: items.join(",")
来源：http://oad.dianchejie.cn

C#:   string.Join(",", items)
来源：http://ghu.pengpengdd.cyou

[E09] 去除所有空白字符
来源：http://kuy.kuanghao11.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pud.daxiang520.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pht.jinqigfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://pre.yuanzhike.top

TS:   s.replace(/\s+/g, "")
来源：http://uak.mhx1999.top

Java: s.replaceAll("\\s+", "")
来源：http://xoj.yonumen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mif.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://njf.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ggd.aizwys.cn

[E10] 左侧补零 / 定长填充
来源：http://pav.jyoumei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pyh.nwbrower.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mzu.iojbl.cn

JS:   "7".padStart(3, "0")
来源：http://azm.jinqigufen.top

TS:   "7".padStart(3, "0")
来源：http://cny.yj20258888.top

Java: String.format("%03d", 7)
来源：http://his.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pym.hammf.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rqn.haohaochexian.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wlg.zhongyouzk.top

[E11] 反转字符串
来源：http://ebx.shzxlz.cn

Py:   s[::-1]
来源：http://zrv.redwolf501.top

PHP:  strrev($s);
来源：http://ejn.ppjwa.cn

JS:   [...s].reverse().join("")
来源：http://mft.feifeiyinyue.top

TS:   [...s].reverse().join("")
来源：http://pao.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ulk.jianghu66.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lep.mhx1999.top

Ruby: s.reverse
来源：http://ltz.yueranfly.top

C#:   new string(s.Reverse().ToArray())
来源：http://slo.chenjidiqi.icu

[E12] 统计某字符出现次数
来源：http://lbl.havefunace.top

Py:   s.count("a")
来源：http://pos.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://dyo.hammf.cn

JS:   s.split("a").length - 1
来源：http://ytd.daria6918.cn

TS:   s.split("a").length - 1
来源：http://urh.c1oappe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dfh.bbcook.cn

Go:   strings.Count(s, "a")
来源：http://oqs.tianlin.xyz

Ruby: s.count("a")
来源：http://tnm.quarkkingdee.top

C#:   s.Count(c => c == 'a')
来源：http://are.vqdsnc.cn

[E13] 逐字符遍历
来源：http://syw.hnqzz.top

Py:   for ch in s: print(ch)
来源：http://luz.epnwcf.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ygx.dashuyun.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hyk.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://evg.sufxvd.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://csp.epnwcf.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nyv.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ytf.hcnkem.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zqa.zhengqikj.top

[E14] URL 编码与 Base64
来源：http://nja.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tnu.sweek.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://adt.nanxinkj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bfe.zycfv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wsx.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uyy.hcnkem.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hjc.jyoumei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fzh.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://osp.smart0.xyz

[E15] HTML 转义 / 反转义
来源：http://oxp.daria6918.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tus.daxiang520.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ezl.guowangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sdj.tianlin.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://cxp.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yqp.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://juq.xuanzx.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wxq.hammf.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hpb.ydjk.org.cn

[E16] 数字千分位
来源：http://wdd.zhiwuduotai.top

Py:   f"{1234567:,}"
来源：http://hsz.ivvv.top

PHP:  number_format(1234567);
来源：http://sei.hesvh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kxv.cqqwz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://meh.zhaomingkeji.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dcb.pycfn.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pfk.daxiang520.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xry.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://rvb.guowangkeji.top

[E17] 首字母大写
来源：http://qwv.yvedp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baj.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xlm.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ydd.wangshuangyany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xmo.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qzu.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mzd.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://vnh.jiagoushi.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ccf.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://qly.zhoulong.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://byi.zhongyouzk.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://osd.nanxuanxn.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sbp.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oxr.cashguo.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aok.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nvz.svipenyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tmj.tian-w.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hhm.jqgfzy.top

[E19] 多行文本按行拆分
来源：http://ifl.yj20258888.top

Py:   s.splitlines()
来源：http://tcz.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zbh.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://rof.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://ysc.jyoumei.cn

Java: s.lines().toList()
来源：http://mlc.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://bxc.zhiwuduotai.top

Ruby: s.lines
来源：http://fai.52xcode.cn

C#:   s.Split('\n')
来源：http://eff.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://whx.yonumen.top

Py:   if not s:
来源：http://ykl.xuetiantiany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://goj.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qmo.havefunace.top

TS:   if (s === "") {}
来源：http://yfv.pengpengdd.cyou

Java: if (s.isEmpty()) {}
来源：http://ces.0kj1m.cn

Go:   if s == "" {}
来源：http://dow.ydjk.org.cn

Ruby: if s.empty?
来源：http://rhr.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vtv.zycfv.cn

[E21] 超长截断加省略号
来源：http://qyj.ctjpmb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xzw.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rpk.fehbvm.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wep.vqdsnc.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uaj.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zyt.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://jae.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gcb.chenlongwang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fwf.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://ety.iojbl.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mlh.feifeiyinyue.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://alw.c1oappe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bcn.fktsv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aiz.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ouu.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jqf.gotoacloud.top

Ruby: s.bytesize;  s.length
来源：http://qcn.gzhubu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://udv.yongpay.top

================================================================================
来源：http://qdf.jiagoushi.top

F. 文件与目录
来源：http://tdm.fehbvm.com

================================================================================
来源：http://xdd.xylfe.cn

[F01] 读取整个文件
来源：http://xuu.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ksx.cdnleiting.top

PHP:  file_get_contents("a.txt");
来源：http://hot.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vgy.yj20258.top


<!-- 参考信息 -->