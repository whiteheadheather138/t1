代发 wailian999

C#:   list.Distinct().ToList()
来源：http://ymb.kuanghao11.cn

[D16] 求和与平均值
来源：http://jpy.guannengcc.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kib.hnqzz.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kpk.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sox.hywenlv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rtm.9152youxi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aeh.chenjidiqi.icu

Go:   // 手写循环累加
来源：http://twc.gotoacloud.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gql.bjfxy.top

C#:   list.Sum();  list.Average()
来源：http://arq.havefunace.top

[D17] 最大值与最小值
来源：http://kzn.chenlongwang.top

Py:   max(arr);  min(arr)
来源：http://ulr.zhaomingkeji.xyz

PHP:  max($arr);  min($arr);
来源：http://awd.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rdb.gzhubu.top

TS:   Math.max(...arr);
来源：http://nfs.yanxiufei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xsm.epnwcf.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cgv.tanke756.top

Ruby: arr.max;  arr.min
来源：http://gws.yvedp.cn

C#:   list.Max();  list.Min()
来源：http://qok.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://xci.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xcp.316326.xyz

PHP:  array_merge(...$nested);
来源：http://gro.chenlongwang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pdn.yueranfly.top

TS:   nested.flat();
来源：http://omf.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eon.tarul.cn

Go:   // 手写双层循环
来源：http://uai.meibo888.top

Ruby: nested.flatten
来源：http://coo.yangfankeji.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://nos.vqdsnc.cn

[D19] 按字段分组
来源：http://mgc.jinyuanbaomall.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cbe.zhongyouzk.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uvo.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://znm.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://izg.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mjy.gotoacloud.top

Go:   // 手写 map[string][]T
来源：http://nvg.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kpx.haohaochexian.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zcn.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://dbk.wangshuangyany.cn

Py:   Counter(arr)
来源：http://huw.yueranfly.top

PHP:  array_count_values($arr);
来源：http://yfv.sxryk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dpl.c1oappe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wbt.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vdl.quarkkingdee.top

Go:   // 手写 map[T]int
来源：http://num.nanxinkj.top

Ruby: arr.tally
来源：http://dtn.epnwcf.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rcm.gzhubu.top

[D21] 判断是否包含某元素
来源：http://wbu.hfpthk.cn

Py:   x in arr
来源：http://gqn.jinqigufen.top

PHP:  in_array($x, $arr, true);
来源：http://wqu.nanxuanxn.top

JS:   arr.includes(x)
来源：http://ygd.zhixingplan.top

TS:   arr.includes(x)
来源：http://een.xylfe.cn

Java: list.contains(x)
来源：http://mba.0kj1m.cn

Go:   slices.Contains(arr, x)
来源：http://rpp.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://wud.hongshengwenyu.top

C#:   list.Contains(x)
来源：http://ugr.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://jzb.uphjek.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://saf.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tco.hnxiangtu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xvs.kuanghao11.cn

TS:   [...arr];
来源：http://dlr.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://npp.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ady.hnxiangtu.top

Ruby: arr.dup;  arr.clone
来源：http://ftn.ybcxt.top

C#:   new List<int>(list);
来源：http://obk.dashuyun.cn

[D23] reduce 累积计算
来源：http://jge.cheryme.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bwj.xylfe.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nxt.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hoz.daxiang520.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gwl.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://oca.fanxiaobao.xyz

Go:   // 手写循环
来源：http://cef.xuetiantiany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kmf.ppjwa.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eqh.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://twm.guowangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xme.xylfe.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://brs.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uaa.kuanghao11.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ieo.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bwr.yongpay.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fgl.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hgm.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://afj.birdmap.top

[D25] Set 集合去重与交并差
来源：http://qff.zhaomingkeji.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wvi.9152youxi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ntq.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cso.smart0.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uyc.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mbw.kuanghao11.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qee.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xoc.ctjpmb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tmx.ydjk.org.cn

[D26] 数组转字符串
来源：http://tlt.sweek.top

Py:   ", ".join(map(str, arr))
来源：http://khr.birdmap.top

PHP:  implode(", ", $arr);
来源：http://pth.kuanghao11.cn

JS:   arr.join(", ")
来源：http://oeg.fanxiaobao.xyz

TS:   arr.join(", ")
来源：http://pzq.daria6918.cn

Java: String.join(", ", list)
来源：http://mdu.cucudq.cn

Go:   strings.Join(strs, ", ")
来源：http://smi.yueranfly.top

Ruby: arr.join(", ")
来源：http://ilf.shanyushiyangkeji.top

C#:   string.Join(", ", list)
来源：http://jjh.yfazqb.com

================================================================================
来源：http://tvm.shangyingyoupin.top

E. 字符串处理
来源：http://qvb.cheryme.top

================================================================================
来源：http://ixh.shzxlz.cn

[E01] 拼接字符串
来源：http://fzl.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gin.hammf.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jec.zhoulong.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wdp.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://psl.gogol.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nlx.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kje.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nim.iojbl.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xnc.jianghu66.top

[E02] 重复字符串
来源：http://yhd.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://xid.chenzaomai.com

PHP:  str_repeat("ab", 3);
来源：http://jbv.xziqi.cn

JS:   "ab".repeat(3)
来源：http://mrb.snrcjt.cn

TS:   "ab".repeat(3)
来源：http://idj.andypj.xyz

Java: "ab".repeat(3)
来源：http://quc.yangfankeji.com

Go:   strings.Repeat("ab", 3)
来源：http://ukv.316326.xyz

Ruby: "ab" * 3
来源：http://jms.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uon.cashguo.top

[E03] 截取子串
来源：http://tai.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cgz.xziqi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vih.hnqzz.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xxy.yj202588.top

TS:   s.slice(1, 4)
来源：http://ujr.zhijiandao.cn

Java: s.substring(1, 4)
来源：http://eia.daria6918.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mkc.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://brl.zhengqikj.top

C#:   s.Substring(1, 3)
来源：http://fnf.ctjpmb.com

[E04] 查找子串位置
来源：http://agd.mhx1999.top

Py:   s.find("x");  s.index("x")
来源：http://wgz.hfpthk.cn

PHP:  strpos($s, "x");
来源：http://zbs.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tzd.zhixingplan.top

TS:   s.indexOf("x")
来源：http://jfn.nwbrower.top

Java: s.indexOf("x")
来源：http://lxk.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://rjx.zhongyouzk.top

Ruby: s.index("x")
来源：http://zyg.tanke756.top

C#:   s.IndexOf("x")
来源：http://yiq.aizwys.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://efr.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jnk.birdmap.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kqt.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sky.vehdjk.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://ybs.smart0.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://khq.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kqc.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ila.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wvr.hongshengwenyu.top

[E06] 替换子串
来源：http://hta.yuanzhike.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qsd.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://sbq.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yso.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://dwj.gzhubu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hmy.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zqj.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pze.yj20258.top

C#:   s.Replace("a", "b")
来源：http://dzm.gaohongyu789.top

[E07] 按分隔符拆分
来源：http://jkb.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://joy.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kyd.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://adn.dianchejie.cn

TS:   s.split(",")
来源：http://deh.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://quf.uphjek.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bri.nwbrower.top

Ruby: s.split(",");  s.split
来源：http://yzt.tanke756.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cwf.hcnkem.com

[E08] 数组按分隔符合并
来源：http://yqm.pengpengdd.cyou

Py:   ",".join(items)
来源：http://zev.svipenyu.cn

PHP:  implode(",", $items);
来源：http://eqx.pycfn.com

JS:   items.join(",")
来源：http://auc.gogol.net.cn

TS:   items.join(",")
来源：http://wzd.gogol.net.cn

Java: String.join(",", items)
来源：http://wuk.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://swj.yj20258.top

Ruby: items.join(",")
来源：http://ryi.xuanzx.com

C#:   string.Join(",", items)
来源：http://iit.ehwqpu.com

[E09] 去除所有空白字符
来源：http://oda.yuanzhike.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wkn.shanyushiyangtech.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xaf.shzxlz.cn

JS:   s.replace(/\s+/g, "")
来源：http://vtj.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://spt.meibo888.top

Java: s.replaceAll("\\s+", "")
来源：http://emj.hysaishi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://igu.tanke756.top

Ruby: s.gsub(/\s+/, "")
来源：http://hkp.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mce.yvedp.cn

[E10] 左侧补零 / 定长填充
来源：http://pzb.tian-w.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cwp.tianlin.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dzs.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://yhj.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://bad.nwbrower.top

Java: String.format("%03d", 7)
来源：http://avu.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ynd.yueranfly.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://srw.meibo888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bvm.52xcode.cn

[E11] 反转字符串
来源：http://rkt.yj20258888.top

Py:   s[::-1]
来源：http://qoy.jqgufenzy.top

PHP:  strrev($s);
来源：http://vec.hnqzz.top

JS:   [...s].reverse().join("")
来源：http://lgr.jqgufenzy.top

TS:   [...s].reverse().join("")
来源：http://pjm.yangfankeji.com

Java: new StringBuilder(s).reverse().toString()
来源：http://qcf.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://qqc.jqgfzy.top

Ruby: s.reverse
来源：http://aqt.yj202588.top

C#:   new string(s.Reverse().ToArray())
来源：http://lpn.ivvv.top

[E12] 统计某字符出现次数
来源：http://gbd.cdnleiting.top

Py:   s.count("a")
来源：http://ubj.jiagoushi.top

PHP:  substr_count($s, "a");
来源：http://nwv.havefunace.top

JS:   s.split("a").length - 1
来源：http://pxy.quarkkingdee.top

TS:   s.split("a").length - 1
来源：http://obn.zhiwuduotai.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://grm.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://hvy.chenlongwang.top

Ruby: s.count("a")
来源：http://jcx.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://zut.zdqjudy.top

[E13] 逐字符遍历
来源：http://jxb.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://fdk.0kj1m.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wkb.hnxiangtu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nfs.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://vns.gaohongyu789.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nxz.yuanzhike.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rtx.pengpengdd.cyou

Ruby: s.each_char { |ch| puts ch }
来源：http://uvq.hammf.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://icg.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://eba.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bfm.dashuyun.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mmb.316326.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://khl.cucudq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qdx.fehbvm.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gxh.c1oappe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://htn.yj20258888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://voh.shanyushiyangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ycl.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://ypa.uphjek.com

Py:   html.escape(s);  html.unescape(s)
来源：http://blb.hnxiangtu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://trc.zdqjudy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://luw.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kpc.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://loj.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rpi.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jgk.bbcook.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oyc.yj202588.top

[E16] 数字千分位
来源：http://gnx.yonumen.top

Py:   f"{1234567:,}"
来源：http://hmw.sweek.top

PHP:  number_format(1234567);
来源：http://cha.cqqwz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pij.shangyingyoupin.top

TS:   (1234567).toLocaleString("en-US")
来源：http://doy.jinqigufen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gxl.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nsx.xingfuxueyuan.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aid.feifeiyinyue.top

C#:   1234567.ToString("N0")
来源：http://yuq.guannengcc.top

[E17] 首字母大写
来源：http://fbn.ehwqpu.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nwv.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wqu.fktsv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lqi.quarkkingdee.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cer.bbcook.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lpo.wangdashe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sjh.sjlbkw.cn

Ruby: s.capitalize
来源：http://ngl.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aqv.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://jnl.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zqi.yonumen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uqh.hnxiangtu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xtr.sufxvd.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kzm.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wpa.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jrb.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qyo.yonumen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ugj.yonumen.top

[E19] 多行文本按行拆分
来源：http://jmx.yueranfly.top

Py:   s.splitlines()
来源：http://bfb.kuanghao11.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://unw.ywan-chungtsiang.top

JS:   s.split(/\r?\n/)
来源：http://htx.vehdjk.com

TS:   s.split(/\r?\n/)
来源：http://xle.jqgfzy.top

Java: s.lines().toList()
来源：http://otj.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://igk.yongpay.top

Ruby: s.lines
来源：http://nfi.jinqigfzy.top

C#:   s.Split('\n')
来源：http://ktj.yj20258888.top

[E20] 判断字符串是否为空
来源：http://dol.jlsjyb.cn

Py:   if not s:
来源：http://fdi.wangdashe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tak.zhixingplan.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sxo.yuxming.cn

TS:   if (s === "") {}
来源：http://mui.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://ujr.zycfv.cn

Go:   if s == "" {}
来源：http://ivn.mhx1999.top

Ruby: if s.empty?
来源：http://umb.wangdashe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sxu.nanxinkj.top

[E21] 超长截断加省略号
来源：http://vnl.ydjk.org.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bzk.yongpay.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ebo.epnwcf.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dwk.9152youxi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://obq.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qlk.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://jzj.hysaishi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ynl.zhiwuduotai.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://esn.nwbrower.top

[E22] 字节长度与字符长度
来源：http://qkx.yonumen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wew.ybcxt.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uhz.birdmap.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jmj.sjlbkw.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xre.cdnleiting.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bab.dashuyun.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rwb.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://sbo.zdqjudy.top


<!-- 参考信息 -->