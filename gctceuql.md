代发 wailian999

TS:   [...new Set(arr)]
来源：http://nsq.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hke.zycfv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hhu.dianchejie.cn

Ruby: arr.uniq
来源：http://jct.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://rde.gaohongyu789.top

[D16] 求和与平均值
来源：http://hlb.gzhubu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wmy.wangshuangyany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hsx.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cgb.zhiwuduotai.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zdu.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tue.hammf.cn

Go:   // 手写循环累加
来源：http://btp.yangfankeji.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mzl.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://oom.kuanghao11.cn

[D17] 最大值与最小值
来源：http://npk.yonumen.top

Py:   max(arr);  min(arr)
来源：http://dxz.zycfv.cn

PHP:  max($arr);  min($arr);
来源：http://twc.sufxvd.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sqs.yj202588.top

TS:   Math.max(...arr);
来源：http://ikk.shangyingyoupin.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dmo.hesvh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xbx.yanxiufei.cn

Ruby: arr.max;  arr.min
来源：http://bhj.mhx1999.top

C#:   list.Max();  list.Min()
来源：http://vqv.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://lhj.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dtq.xinyue.icu

PHP:  array_merge(...$nested);
来源：http://azv.hcnkem.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xpr.zhixingplan.top

TS:   nested.flat();
来源：http://mqt.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jne.quarkkingdee.top

Go:   // 手写双层循环
来源：http://aro.yongpay.top

Ruby: nested.flatten
来源：http://erl.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://inx.hcnkem.com

[D19] 按字段分组
来源：http://pva.hysaishi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xro.shanyushiyangtech.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://esr.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bjx.fktsv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fth.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ynl.hesvh.cn

Go:   // 手写 map[string][]T
来源：http://pgk.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yog.sjlbkw.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oax.zhixingplan.top

[D20] 统计每个元素出现次数
来源：http://tyw.ywan-chungtsiang.top

Py:   Counter(arr)
来源：http://fyw.jlsjyb.cn

PHP:  array_count_values($arr);
来源：http://ite.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rff.sxryk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://smf.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ody.yvedp.cn

Go:   // 手写 map[T]int
来源：http://qmu.shzxlz.cn

Ruby: arr.tally
来源：http://cfa.ybcxt.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fjk.yonumen.top

[D21] 判断是否包含某元素
来源：http://bgb.sweek.top

Py:   x in arr
来源：http://mau.zhaomingkeji.xyz

PHP:  in_array($x, $arr, true);
来源：http://rah.c1oappe.top

JS:   arr.includes(x)
来源：http://mpv.hnxiangtu.top

TS:   arr.includes(x)
来源：http://ngz.yvedp.cn

Java: list.contains(x)
来源：http://rjy.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://zjs.cashguo.top

Ruby: arr.include?(x)
来源：http://erf.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://soq.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://ngz.fengsongda.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gud.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hlo.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://its.sysykeji.top

TS:   [...arr];
来源：http://ahu.fzhhl.top

Java: new ArrayList<>(list);
来源：http://rxk.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://cik.shanyushiyangtech.top

Ruby: arr.dup;  arr.clone
来源：http://edb.hammf.cn

C#:   new List<int>(list);
来源：http://bnc.fanxiaobao.xyz

[D23] reduce 累积计算
来源：http://nim.uphjek.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gem.fanxiaobao.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cpl.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kjg.yonumen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vwj.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://byo.sjlbkw.cn

Go:   // 手写循环
来源：http://hat.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nhn.daria6918.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jda.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://fcj.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://thq.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dss.epnwcf.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wrb.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kab.cucudq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://peb.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://clb.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hdw.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tly.316326.xyz

[D25] Set 集合去重与交并差
来源：http://jqb.tarul.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wzt.jyoumei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ogi.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://png.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://veu.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uff.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://two.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zsk.shanyushiyangtech.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rqo.redwolf501.top

[D26] 数组转字符串
来源：http://wxj.yuanzhike.top

Py:   ", ".join(map(str, arr))
来源：http://gvr.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://qwq.ydjk.org.cn

JS:   arr.join(", ")
来源：http://dub.zhoulong.xyz

TS:   arr.join(", ")
来源：http://bdv.vqdsnc.cn

Java: String.join(", ", list)
来源：http://urn.ppjwa.cn

Go:   strings.Join(strs, ", ")
来源：http://wva.fehbvm.com

Ruby: arr.join(", ")
来源：http://anf.xylfe.cn

C#:   string.Join(", ", list)
来源：http://pjz.ppjwa.cn

================================================================================
来源：http://cjw.nwbrower.top

E. 字符串处理
来源：http://wxi.yueranfly.top

================================================================================
来源：http://ssk.ydjk.org.cn

[E01] 拼接字符串
来源：http://agj.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zxj.jinqigfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://poa.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kqb.ehwqpu.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fvf.guowangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ccy.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ztr.hammf.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://loo.nanxuanxn.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fcn.jiagoushi.top

[E02] 重复字符串
来源：http://xqu.daria6918.cn

Py:   "ab" * 3
来源：http://pnp.sxryk.cn

PHP:  str_repeat("ab", 3);
来源：http://mnv.andypj.xyz

JS:   "ab".repeat(3)
来源：http://txf.aizwys.cn

TS:   "ab".repeat(3)
来源：http://yhd.tarul.cn

Java: "ab".repeat(3)
来源：http://fqi.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://ndy.epnwcf.com

Ruby: "ab" * 3
来源：http://bmr.chenlongwang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ebm.xylfe.cn

[E03] 截取子串
来源：http://xzg.cqqwz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vhn.52xcode.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rzb.chenlongwang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jzm.xylfe.cn

TS:   s.slice(1, 4)
来源：http://dmh.mhx1999.top

Java: s.substring(1, 4)
来源：http://dsg.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qvi.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://mle.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://qep.yangfankeji.com

[E04] 查找子串位置
来源：http://awd.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://ijn.bjfxy.top

PHP:  strpos($s, "x");
来源：http://ran.zhijiandao.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://peu.yongpay.top

TS:   s.indexOf("x")
来源：http://ufs.zdbjq.cn

Java: s.indexOf("x")
来源：http://msc.aibaodan.cn

Go:   strings.Index(s, "x")
来源：http://kbp.hesvh.cn

Ruby: s.index("x")
来源：http://aom.hongshengwenyu.top

C#:   s.IndexOf("x")
来源：http://ppj.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gmx.aizwys.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kzu.xingfuxueyuan.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://anp.hnqzz.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://svr.mhx1999.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bqb.smart0.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jbh.dianchejie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qii.xziqi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ggv.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tmp.aibaodan.cn

[E06] 替换子串
来源：http://uxk.zhiwuduotai.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vqe.fktsv.cn

PHP:  str_replace("a", "b", $s);
来源：http://ioj.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zin.yfazqb.com

TS:   s.replaceAll("a", "b")
来源：http://ytm.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ufg.yj202588.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qhf.tarul.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://phz.vqdsnc.cn

C#:   s.Replace("a", "b")
来源：http://xpz.jyoumei.cn

[E07] 按分隔符拆分
来源：http://dku.jqgufenzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rhj.gzhubu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bbm.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vkw.jinghuilouyu.cn

TS:   s.split(",")
来源：http://yrh.gaohongyu789.top

Java: s.split(",");  s.split("\\s+")
来源：http://lhv.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://swc.hcnkem.com

Ruby: s.split(",");  s.split
来源：http://yaf.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ksz.zhoulong.xyz

[E08] 数组按分隔符合并
来源：http://iws.9152youxi.cn

Py:   ",".join(items)
来源：http://cbq.gzhubu.top

PHP:  implode(",", $items);
来源：http://dqq.wangshuangyany.cn

JS:   items.join(",")
来源：http://nli.yangfankeji.com

TS:   items.join(",")
来源：http://evo.hcnkem.com

Java: String.join(",", items)
来源：http://yup.sweek.top

Go:   strings.Join(items, ",")
来源：http://tjk.redwolf501.top

Ruby: items.join(",")
来源：http://ijl.xinyue.icu

C#:   string.Join(",", items)
来源：http://jyw.aizwys.cn

[E09] 去除所有空白字符
来源：http://rfl.ehwqpu.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xbr.yj202588.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hio.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://qbc.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://ovc.shangyingyoupin.top

Java: s.replaceAll("\\s+", "")
来源：http://ehw.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://yhr.hcnkem.com

Ruby: s.gsub(/\s+/, "")
来源：http://duq.birdmap.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uyy.fengsongda.top

[E10] 左侧补零 / 定长填充
来源：http://syc.cucudq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ypc.wangdashe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rim.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://qkn.ywan-chungtsiang.top

TS:   "7".padStart(3, "0")
来源：http://hjh.iojbl.cn

Java: String.format("%03d", 7)
来源：http://kgy.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gui.jinqigufen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oil.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cji.shuidangran.top

[E11] 反转字符串
来源：http://bqc.fehbvm.com

Py:   s[::-1]
来源：http://mxc.uphjek.com

PHP:  strrev($s);
来源：http://foc.52xcode.cn

JS:   [...s].reverse().join("")
来源：http://kff.yfazqb.com

TS:   [...s].reverse().join("")
来源：http://tel.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://muv.aizwys.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://goj.gotoacloud.top

Ruby: s.reverse
来源：http://ufe.feifeiyinyue.top

C#:   new string(s.Reverse().ToArray())
来源：http://bat.shangyingyoupin.top

[E12] 统计某字符出现次数
来源：http://dte.snrcjt.cn

Py:   s.count("a")
来源：http://aba.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://tpq.bbcook.cn

JS:   s.split("a").length - 1
来源：http://xiy.meibo888.top

TS:   s.split("a").length - 1
来源：http://zye.yanxiufei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zoh.yj202588.top

Go:   strings.Count(s, "a")
来源：http://kqc.9152youxi.cn

Ruby: s.count("a")
来源：http://fcq.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://vfv.ivvv.top

[E13] 逐字符遍历
来源：http://ghb.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://xdo.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gjq.yuxming.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hwr.gzhubu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://frb.xylfe.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qoc.wangdashe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ymk.c1oappe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hje.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qta.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://hii.jinyuanbaomall.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rxs.yonumen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jkv.52xcode.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qcp.jinyuanbaomall.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mkr.yangfankeji.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uzi.vehdjk.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gbh.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lzi.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hyp.andypj.xyz

[E15] HTML 转义 / 反转义
来源：http://nco.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://meo.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wob.9152youxi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://msl.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pbe.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iov.ydjk.org.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://icd.yueranfly.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aqi.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ptd.andypj.xyz

[E16] 数字千分位
来源：http://fvs.jiagoushi.top

Py:   f"{1234567:,}"
来源：http://zcc.yangfankeji.com

PHP:  number_format(1234567);
来源：http://gql.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ljs.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://iul.cqqwz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ysv.zhoulong.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qtt.xuanzx.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wyl.9152youxi.cn

C#:   1234567.ToString("N0")
来源：http://hul.ppjwa.cn

[E17] 首字母大写
来源：http://jyo.haohaochexian.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://piz.aibaodan.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wsn.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iln.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ljc.shzxlz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fnx.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://upi.pycfn.com

Ruby: s.capitalize
来源：http://tde.fzhhl.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wgd.birdmap.top

[E18] 模板占位符替换
来源：http://jys.yj202588.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qel.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qjw.tian-w.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cas.hfpthk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://odp.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gjr.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ebf.yongpay.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mlr.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gxl.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://myy.sweek.top

Py:   s.splitlines()
来源：http://vcp.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://thn.wangshuangyany.cn

JS:   s.split(/\r?\n/)
来源：http://svi.gotoacloud.top

TS:   s.split(/\r?\n/)
来源：http://uiz.kuanghao11.cn

Java: s.lines().toList()
来源：http://iev.ehwqpu.com

Go:   strings.Split(s, "\n")
来源：http://lns.yonumen.top

Ruby: s.lines
来源：http://hqj.yvedp.cn

C#:   s.Split('\n')
来源：http://yta.zhixingplan.top

[E20] 判断字符串是否为空
来源：http://sze.cdnleiting.top

Py:   if not s:
来源：http://rmj.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gte.cqqwz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ent.gotoacloud.top

TS:   if (s === "") {}
来源：http://xvu.svipenyu.cn

Java: if (s.isEmpty()) {}
来源：http://nvz.hysaishi.cn

Go:   if s == "" {}
来源：http://hdw.yuanzhike.top

Ruby: if s.empty?
来源：http://khv.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pdp.cdnleiting.top

[E21] 超长截断加省略号
来源：http://cva.xuanzx.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fvr.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jfm.fktsv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pea.0kj1m.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ram.andypj.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vqp.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://wgt.cucudq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qgi.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qhj.ydzc1.top

[E22] 字节长度与字符长度
来源：http://frt.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://owm.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kbr.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mrg.hnxiangtu.top


<!-- 参考信息 -->