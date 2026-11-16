代发 wailian999

C#:   list.Distinct().ToList()
来源：http://ifg.snrcjt.cn

[D16] 求和与平均值
来源：http://rub.guannengcc.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cyw.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jju.xuetiantiany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bng.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lvp.daxiang520.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yli.daxiang520.top

Go:   // 手写循环累加
来源：http://rev.yfazqb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xom.zdbjq.cn

C#:   list.Sum();  list.Average()
来源：http://zjo.zdqjudy.top

[D17] 最大值与最小值
来源：http://mzk.shanyushiyangkeji.top

Py:   max(arr);  min(arr)
来源：http://gjs.nanxinkj.top

PHP:  max($arr);  min($arr);
来源：http://woz.52xcode.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wxi.smart0.xyz

TS:   Math.max(...arr);
来源：http://ulp.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fpg.tianlin.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jkt.zhongyouzk.top

Ruby: arr.max;  arr.min
来源：http://ytj.hcnkem.com

C#:   list.Max();  list.Min()
来源：http://fgp.yonumen.top

[D18] 扁平化嵌套数组
来源：http://nbu.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qcq.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://ixy.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://npp.ybcxt.top

TS:   nested.flat();
来源：http://sti.bbcook.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uzm.iojbl.cn

Go:   // 手写双层循环
来源：http://did.quarkkingdee.top

Ruby: nested.flatten
来源：http://cqy.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://snd.hnxiangtu.top

[D19] 按字段分组
来源：http://zta.zhoulong.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xzn.vqdsnc.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nul.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yga.9152youxi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wad.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hjz.jyoumei.cn

Go:   // 手写 map[string][]T
来源：http://txr.xingfuxueyuan.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://bfe.guannengcc.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bta.meibo888.top

[D20] 统计每个元素出现次数
来源：http://jfo.xinyue.icu

Py:   Counter(arr)
来源：http://zub.iojbl.cn

PHP:  array_count_values($arr);
来源：http://usj.yonumen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aaf.meibo888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qod.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cdw.52xcode.cn

Go:   // 手写 map[T]int
来源：http://hoc.xinyue.icu

Ruby: arr.tally
来源：http://xdf.sufxvd.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xsj.cashguo.top

[D21] 判断是否包含某元素
来源：http://bjd.hysaishi.cn

Py:   x in arr
来源：http://hnn.chenjidiqi.icu

PHP:  in_array($x, $arr, true);
来源：http://ows.hcnkem.com

JS:   arr.includes(x)
来源：http://olh.gzhubu.top

TS:   arr.includes(x)
来源：http://dlt.ppjwa.cn

Java: list.contains(x)
来源：http://mtl.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://xjt.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://xza.chenzaomai.com

C#:   list.Contains(x)
来源：http://xtc.0kj1m.cn

[D22] 复制数组（避免共享引用）
来源：http://lih.guannengcc.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bny.chenlongwang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ghi.jiagoushi.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bex.cqqwz.cn

TS:   [...arr];
来源：http://ply.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://jlh.shangyingyoupin.top

Go:   copied := append([]int(nil), arr...)
来源：http://gry.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://gfk.zhoulong.xyz

C#:   new List<int>(list);
来源：http://ajf.snrcjt.cn

[D23] reduce 累积计算
来源：http://hed.52xcode.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nok.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dbj.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://idd.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ahj.quarkkingdee.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kmt.xinyue.icu

Go:   // 手写循环
来源：http://irj.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qde.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://njv.hfpthk.cn

[D24] 字典 / Map 基本操作
来源：http://jlg.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sjm.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xix.cucudq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fmw.mhx1999.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mbe.nanxuanxn.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gqx.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://orj.jianghu66.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wye.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xxh.yanxiufei.cn

[D25] Set 集合去重与交并差
来源：http://rqe.quarkkingdee.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://evm.yonumen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fkp.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fon.chenlongwang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://via.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rye.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yvx.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://utj.jiagoushi.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yiw.shuidangran.top

[D26] 数组转字符串
来源：http://ubt.ywan-chungtsiang.top

Py:   ", ".join(map(str, arr))
来源：http://gqw.bbcook.cn

PHP:  implode(", ", $arr);
来源：http://jns.tanke756.top

JS:   arr.join(", ")
来源：http://tty.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://upc.cucudq.cn

Java: String.join(", ", list)
来源：http://cme.cucudq.cn

Go:   strings.Join(strs, ", ")
来源：http://oso.svipenyu.cn

Ruby: arr.join(", ")
来源：http://fij.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://mxw.snrcjt.cn

================================================================================
来源：http://tun.hongshengwenyu.top

E. 字符串处理
来源：http://qhq.shangyingyoupin.top

================================================================================
来源：http://nfj.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://cur.yj202588.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hzr.aizwys.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://llm.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dfr.zdqjudy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fsl.yvedp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zap.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://siz.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iub.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xjy.yongpay.top

[E02] 重复字符串
来源：http://szz.zhengqikj.top

Py:   "ab" * 3
来源：http://wzy.gaohongyu789.top

PHP:  str_repeat("ab", 3);
来源：http://xmz.haohaochexian.top

JS:   "ab".repeat(3)
来源：http://kcg.sjlbkw.cn

TS:   "ab".repeat(3)
来源：http://uqx.haohaochexian.top

Java: "ab".repeat(3)
来源：http://kws.yangfankeji.com

Go:   strings.Repeat("ab", 3)
来源：http://vfl.cheryme.top

Ruby: "ab" * 3
来源：http://jkz.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tmv.haohaochexian.top

[E03] 截取子串
来源：http://gyf.yongpay.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tde.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sem.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://egj.pycfn.com

TS:   s.slice(1, 4)
来源：http://yaj.zhengqikj.top

Java: s.substring(1, 4)
来源：http://wjv.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gvy.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mhz.meibo888.top

C#:   s.Substring(1, 3)
来源：http://frw.yuanzhike.top

[E04] 查找子串位置
来源：http://ndn.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://yje.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://tuw.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uqc.kuanghao11.cn

TS:   s.indexOf("x")
来源：http://rtv.cdnleiting.top

Java: s.indexOf("x")
来源：http://wpy.hfpthk.cn

Go:   strings.Index(s, "x")
来源：http://hgf.ybcxt.top

Ruby: s.index("x")
来源：http://mfc.ppjwa.cn

C#:   s.IndexOf("x")
来源：http://dkg.xuanzx.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://kvy.dashuyun.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fhg.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hjr.smart0.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wga.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://van.andypj.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ryl.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tpp.chenzaomai.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xte.ydzc1.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://leq.yj202588.top

[E06] 替换子串
来源：http://ywf.chenlongwang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fbo.gaohongyu789.top

PHP:  str_replace("a", "b", $s);
来源：http://gtd.jqgfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uuh.xylfe.cn

TS:   s.replaceAll("a", "b")
来源：http://lcp.tianlin.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://khq.52xcode.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fhz.fzhhl.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kgi.yj202588.top

C#:   s.Replace("a", "b")
来源：http://swv.nwbrower.top

[E07] 按分隔符拆分
来源：http://xgb.aibaodan.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ifd.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qnh.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://emd.sysykeji.top

TS:   s.split(",")
来源：http://kin.pycfn.com

Java: s.split(",");  s.split("\\s+")
来源：http://cxm.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://grl.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://nmo.nanxuanxn.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bkv.cdnleiting.top

[E08] 数组按分隔符合并
来源：http://uhd.hcnkem.com

Py:   ",".join(items)
来源：http://byg.fengsongda.top

PHP:  implode(",", $items);
来源：http://fmm.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://nyz.shzxlz.cn

TS:   items.join(",")
来源：http://tsg.yuxming.cn

Java: String.join(",", items)
来源：http://mrr.c1oappe.top

Go:   strings.Join(items, ",")
来源：http://gtw.hysaishi.cn

Ruby: items.join(",")
来源：http://ndh.fktsv.cn

C#:   string.Join(",", items)
来源：http://fxh.52xcode.cn

[E09] 去除所有空白字符
来源：http://ugr.fengsongda.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pta.zhengqikj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cjk.9152youxi.cn

JS:   s.replace(/\s+/g, "")
来源：http://czn.nanxuanxn.top

TS:   s.replace(/\s+/g, "")
来源：http://yyp.ivvv.top

Java: s.replaceAll("\\s+", "")
来源：http://ccr.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://waa.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://dvf.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lty.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://mpx.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://upp.mhx1999.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hge.guannengcc.top

JS:   "7".padStart(3, "0")
来源：http://jxs.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://gic.epnwcf.com

Java: String.format("%03d", 7)
来源：http://ogg.snrcjt.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uwu.yangfankeji.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://msn.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xog.yj20258888.top

[E11] 反转字符串
来源：http://wmt.cqqwz.cn

Py:   s[::-1]
来源：http://hpk.bjfxy.top

PHP:  strrev($s);
来源：http://ref.hfpthk.cn

JS:   [...s].reverse().join("")
来源：http://zbr.meibo888.top

TS:   [...s].reverse().join("")
来源：http://asy.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xwg.smart0.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://vea.aibaodan.cn

Ruby: s.reverse
来源：http://mxu.gaohongyu789.top

C#:   new string(s.Reverse().ToArray())
来源：http://fap.shzxlz.cn

[E12] 统计某字符出现次数
来源：http://yad.gaohongyu789.top

Py:   s.count("a")
来源：http://acr.xziqi.cn

PHP:  substr_count($s, "a");
来源：http://qkk.fengsongda.top

JS:   s.split("a").length - 1
来源：http://kga.birdmap.top

TS:   s.split("a").length - 1
来源：http://fwn.ydjk.org.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://frs.guowangkeji.top

Go:   strings.Count(s, "a")
来源：http://rld.sweek.top

Ruby: s.count("a")
来源：http://cxr.jinghuilouyu.cn

C#:   s.Count(c => c == 'a')
来源：http://shl.yj20258.top

[E13] 逐字符遍历
来源：http://ymr.hnqzz.top

Py:   for ch in s: print(ch)
来源：http://hun.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fdx.gaohongyu789.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://iqq.gogol.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tkk.yj202588.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gpb.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nkp.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://omq.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gvt.sufxvd.cn

[E14] URL 编码与 Base64
来源：http://box.jqgufenzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ivk.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://klg.svipenyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ctl.shzxlz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sbs.yj20258888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zmq.tarul.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ocv.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ifv.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://klr.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://qbp.zhiwuduotai.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kbg.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xwu.zdbjq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yau.jqgfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ass.yvedp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bqm.dianchejie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nto.shanyushiyangtech.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lwe.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vhw.guowangkeji.top

[E16] 数字千分位
来源：http://iez.xuanzx.com

Py:   f"{1234567:,}"
来源：http://esd.sysykeji.top

PHP:  number_format(1234567);
来源：http://seg.pycfn.com

JS:   (1234567).toLocaleString("en-US")
来源：http://xjb.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ndc.shanyushiyangtech.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bsz.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oxk.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nah.0kj1m.cn

C#:   1234567.ToString("N0")
来源：http://xbk.sjlbkw.cn

[E17] 首字母大写
来源：http://vzm.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nwx.ehwqpu.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://mub.feifeiyinyue.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xxk.havefunace.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ifz.yfazqb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rdu.yuxming.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fos.vqdsnc.cn

Ruby: s.capitalize
来源：http://wxh.tanke756.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://icp.sysykeji.top

[E18] 模板占位符替换
来源：http://jzo.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rqc.xinyue.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hcf.yonumen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://enk.zhongyouzk.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cuq.yfazqb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fjp.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yag.sweek.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pnb.cucudq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iso.ctjpmb.com

[E19] 多行文本按行拆分
来源：http://kjv.birdmap.top

Py:   s.splitlines()
来源：http://cqi.ydzc1.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://exm.xylfe.cn

JS:   s.split(/\r?\n/)
来源：http://dkc.jianghu66.top

TS:   s.split(/\r?\n/)
来源：http://dnz.zhijiandao.cn

Java: s.lines().toList()
来源：http://pgz.hcnkem.com

Go:   strings.Split(s, "\n")
来源：http://loi.sufxvd.cn

Ruby: s.lines
来源：http://hbl.yj20258.top

C#:   s.Split('\n')
来源：http://thp.yueranfly.top

[E20] 判断字符串是否为空
来源：http://rnv.ybcxt.top

Py:   if not s:
来源：http://ckk.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://woj.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rlj.yj202588.top

TS:   if (s === "") {}
来源：http://ner.yuanzhike.top

Java: if (s.isEmpty()) {}
来源：http://qxq.shzxlz.cn

Go:   if s == "" {}
来源：http://crp.zhengqikj.top

Ruby: if s.empty?
来源：http://blj.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vcb.hywenlv.cn

[E21] 超长截断加省略号
来源：http://gvs.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nfb.0kj1m.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bdn.shanyushiyangtech.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qkb.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://prq.yuxming.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mei.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://xja.xziqi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ixq.wangdashe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ldm.ctjpmb.com

[E22] 字节长度与字符长度
来源：http://rac.jiagoushi.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ojw.pengpengdd.cyou

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cyz.bjfxy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cog.ydjk.org.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sgp.gzhubu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uoo.hesvh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tgh.cheryme.top

Ruby: s.bytesize;  s.length
来源：http://dcr.hcnkem.com


<!-- 参考信息 -->