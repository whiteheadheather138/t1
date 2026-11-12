代发 wailian999

[D15] 去重
来源：http://cso.yj202588.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uxc.haohaochexian.top

PHP:  array_unique($arr);
来源：http://gtv.xuanzx.com

JS:   [...new Set(arr)]
来源：http://qkp.xingfuxueyuan.xyz

TS:   [...new Set(arr)]
来源：http://poq.gogol.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fgd.yj202588.top

Go:   // 用 map[T]struct{} 手写
来源：http://vwm.daria6918.cn

Ruby: arr.uniq
来源：http://tzm.zhongyouzk.top

C#:   list.Distinct().ToList()
来源：http://zhf.feifeiyinyue.top

[D16] 求和与平均值
来源：http://vow.0kj1m.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gby.zycfv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gif.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://crl.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dpc.pycfn.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rfi.jqgufenzy.top

Go:   // 手写循环累加
来源：http://xqv.xinyue.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uiy.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://xrz.zycfv.cn

[D17] 最大值与最小值
来源：http://fpo.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://fhb.tarul.cn

PHP:  max($arr);  min($arr);
来源：http://gzt.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tzv.yonumen.top

TS:   Math.max(...arr);
来源：http://ncz.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://qzm.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bfc.yuanzhike.top

Ruby: arr.max;  arr.min
来源：http://hit.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://oyj.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://imh.vehdjk.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ini.yueranfly.top

PHP:  array_merge(...$nested);
来源：http://snr.yonumen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cdy.daria6918.cn

TS:   nested.flat();
来源：http://cnp.tianlin.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://llv.zycfv.cn

Go:   // 手写双层循环
来源：http://kvu.uphjek.com

Ruby: nested.flatten
来源：http://efa.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xku.yj20258888.top

[D19] 按字段分组
来源：http://xxu.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mrf.yj202588.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://epn.hongshengwenyu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zss.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nfr.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nli.chenjidiqi.icu

Go:   // 手写 map[string][]T
来源：http://yox.iojbl.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mxe.ehwqpu.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fdg.mhx1999.top

[D20] 统计每个元素出现次数
来源：http://uox.daria6918.cn

Py:   Counter(arr)
来源：http://rgb.fengsongda.top

PHP:  array_count_values($arr);
来源：http://zex.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dhl.sjlbkw.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mly.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hqt.hysaishi.cn

Go:   // 手写 map[T]int
来源：http://fpy.shzxlz.cn

Ruby: arr.tally
来源：http://sqs.yangfankeji.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vsw.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://gna.jinqigufen.top

Py:   x in arr
来源：http://tem.meibo888.top

PHP:  in_array($x, $arr, true);
来源：http://qir.zhaomingkeji.xyz

JS:   arr.includes(x)
来源：http://kyy.hcnkem.com

TS:   arr.includes(x)
来源：http://mfr.fanxiaobao.xyz

Java: list.contains(x)
来源：http://lak.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://nvv.ppjwa.cn

Ruby: arr.include?(x)
来源：http://bbp.jlsjyb.cn

C#:   list.Contains(x)
来源：http://uft.hnqzz.top

[D22] 复制数组（避免共享引用）
来源：http://qtk.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vxr.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zgp.epnwcf.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ezy.fengsongda.top

TS:   [...arr];
来源：http://qne.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://ush.dianchejie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mgu.xuanzx.com

Ruby: arr.dup;  arr.clone
来源：http://txt.jqgfzy.top

C#:   new List<int>(list);
来源：http://jqq.yfazqb.com

[D23] reduce 累积计算
来源：http://crb.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://psp.sweek.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ozw.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qom.yonumen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gjh.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ass.yj20258.top

Go:   // 手写循环
来源：http://wqo.daria6918.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iyj.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ojs.sweek.top

[D24] 字典 / Map 基本操作
来源：http://ipi.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aau.epnwcf.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://thl.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xgc.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wuf.sweek.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hog.zhaomingkeji.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lxs.cdnleiting.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jgj.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xzv.yanxiufei.cn

[D25] Set 集合去重与交并差
来源：http://ziv.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qkr.quarkkingdee.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ivf.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zgv.feifeiyinyue.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vyu.tianlin.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hfq.xylfe.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zjv.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://snw.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qqa.yj20258.top

[D26] 数组转字符串
来源：http://owu.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://stq.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://bsh.yangfankeji.com

JS:   arr.join(", ")
来源：http://fop.tarul.cn

TS:   arr.join(", ")
来源：http://sjr.yj20258.top

Java: String.join(", ", list)
来源：http://kkg.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://gtd.birdmap.top

Ruby: arr.join(", ")
来源：http://cph.yonumen.top

C#:   string.Join(", ", list)
来源：http://dha.bjfxy.top

================================================================================
来源：http://xji.birdmap.top

E. 字符串处理
来源：http://ryx.hcnkem.com

================================================================================
来源：http://qxe.tianlin.xyz

[E01] 拼接字符串
来源：http://cgk.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uxj.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ubi.vehdjk.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wxw.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ujf.xinyue.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vnt.yj20258888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xll.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://njy.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nmt.yueranfly.top

[E02] 重复字符串
来源：http://cjj.yueranfly.top

Py:   "ab" * 3
来源：http://qvc.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://lds.yj202588.top

JS:   "ab".repeat(3)
来源：http://ije.ehwqpu.com

TS:   "ab".repeat(3)
来源：http://jze.cheryme.top

Java: "ab".repeat(3)
来源：http://drf.cashguo.top

Go:   strings.Repeat("ab", 3)
来源：http://peb.hongshengwenyu.top

Ruby: "ab" * 3
来源：http://pyo.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fnf.zhongyouzk.top

[E03] 截取子串
来源：http://rwp.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oli.yj20258.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dwo.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pow.xinyue.icu

TS:   s.slice(1, 4)
来源：http://kpf.jianghu66.top

Java: s.substring(1, 4)
来源：http://idh.0kj1m.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dwh.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bqi.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://opq.nanxuanxn.top

[E04] 查找子串位置
来源：http://swb.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://jgt.9152youxi.cn

PHP:  strpos($s, "x");
来源：http://hrz.pengpengdd.cyou

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gdc.dianchejie.cn

TS:   s.indexOf("x")
来源：http://hxf.ybcxt.top

Java: s.indexOf("x")
来源：http://ydf.vqdsnc.cn

Go:   strings.Index(s, "x")
来源：http://mgr.gaohongyu789.top

Ruby: s.index("x")
来源：http://eqn.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://kyo.birdmap.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wwu.fanxiaobao.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xqu.epnwcf.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qyt.quarkkingdee.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://reu.hammf.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gqo.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ecb.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xmn.ywan-chungtsiang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cpm.sweek.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fmx.jianghu66.top

[E06] 替换子串
来源：http://pre.yueranfly.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ija.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://iqb.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aul.chenlongwang.top

TS:   s.replaceAll("a", "b")
来源：http://bgv.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rdf.dianchejie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ubf.jyoumei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qto.pengpengdd.cyou

C#:   s.Replace("a", "b")
来源：http://wkl.yvedp.cn

[E07] 按分隔符拆分
来源：http://eym.ydjk.org.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://glp.hywenlv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iwf.uphjek.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://jvm.daxiang520.top

TS:   s.split(",")
来源：http://xeb.fanxiaobao.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://pes.zhongyouzk.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pgf.pengpengdd.cyou

Ruby: s.split(",");  s.split
来源：http://qyu.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jah.jlsjyb.cn

[E08] 数组按分隔符合并
来源：http://ivg.chenjidiqi.icu

Py:   ",".join(items)
来源：http://mgh.pycfn.com

PHP:  implode(",", $items);
来源：http://zdk.jinqigfzy.top

JS:   items.join(",")
来源：http://yox.zhoulong.xyz

TS:   items.join(",")
来源：http://nsq.ydjk.org.cn

Java: String.join(",", items)
来源：http://lnm.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://hsr.andypj.xyz

Ruby: items.join(",")
来源：http://zsc.epnwcf.com

C#:   string.Join(",", items)
来源：http://wcc.yonumen.top

[E09] 去除所有空白字符
来源：http://xyg.gotoacloud.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bcv.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://grd.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://tdl.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://pxk.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://qiv.sweek.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://scx.chenlongwang.top

Ruby: s.gsub(/\s+/, "")
来源：http://wvm.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pts.yvedp.cn

[E10] 左侧补零 / 定长填充
来源：http://sax.ybcxt.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tjv.ctjpmb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gux.fktsv.cn

JS:   "7".padStart(3, "0")
来源：http://jwm.9152youxi.cn

TS:   "7".padStart(3, "0")
来源：http://dry.jinqigufen.top

Java: String.format("%03d", 7)
来源：http://jqt.shanyushiyangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tfw.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ctq.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bih.redwolf501.top

[E11] 反转字符串
来源：http://pxj.jqgfzy.top

Py:   s[::-1]
来源：http://wvk.redwolf501.top

PHP:  strrev($s);
来源：http://skk.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://pnb.yonumen.top

TS:   [...s].reverse().join("")
来源：http://fud.ctjpmb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://tqq.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ypu.dashuyun.cn

Ruby: s.reverse
来源：http://hpo.yongpay.top

C#:   new string(s.Reverse().ToArray())
来源：http://quh.aizwys.cn

[E12] 统计某字符出现次数
来源：http://ede.gzhubu.top

Py:   s.count("a")
来源：http://tcg.tian-w.cn

PHP:  substr_count($s, "a");
来源：http://koj.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://arg.xziqi.cn

TS:   s.split("a").length - 1
来源：http://win.ywan-chungtsiang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oam.fehbvm.com

Go:   strings.Count(s, "a")
来源：http://mmu.gzhubu.top

Ruby: s.count("a")
来源：http://kzm.yfazqb.com

C#:   s.Count(c => c == 'a')
来源：http://vdt.zhengqikj.top

[E13] 逐字符遍历
来源：http://bal.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://nov.yangfankeji.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jec.ivvv.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://byv.dianchejie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uwt.andypj.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ddw.jyoumei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://smf.fengsongda.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cho.yanxiufei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bap.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://nkc.ydzc1.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mfi.cashguo.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uko.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://has.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bnl.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://deh.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cah.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dkj.feifeiyinyue.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://znn.zdbjq.cn

[E15] HTML 转义 / 反转义
来源：http://upi.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ups.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mpb.ivvv.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://czt.fengsongda.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sif.chenzaomai.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pmc.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aek.ybcxt.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rbu.sysykeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ruy.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://ola.nwbrower.top

Py:   f"{1234567:,}"
来源：http://zyi.ehwqpu.com

PHP:  number_format(1234567);
来源：http://hnl.daxiang520.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gdn.jinyuanbaomall.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vun.zycfv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xkl.dashuyun.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://egc.jinyuanbaomall.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kyp.hongshengwenyu.top

C#:   1234567.ToString("N0")
来源：http://asv.fktsv.cn

[E17] 首字母大写
来源：http://lex.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://flj.hywenlv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jrk.tanke756.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jcs.uphjek.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rly.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qzz.vehdjk.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gta.hnqzz.top

Ruby: s.capitalize
来源：http://oqd.chenjidiqi.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kta.ctjpmb.com

[E18] 模板占位符替换
来源：http://fcg.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ifl.ywan-chungtsiang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tnt.ywan-chungtsiang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wxg.guannengcc.top

TS:   tpl.replaceAll("{name}", name)
来源：http://svn.316326.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wad.gzhubu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uge.gotoacloud.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qhg.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jpg.shuidangran.top

[E19] 多行文本按行拆分
来源：http://nho.hfpthk.cn

Py:   s.splitlines()
来源：http://rkd.haohaochexian.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fsb.jqgufenzy.top

JS:   s.split(/\r?\n/)
来源：http://zla.yueranfly.top

TS:   s.split(/\r?\n/)
来源：http://lgp.zhaomingkeji.xyz

Java: s.lines().toList()
来源：http://roi.shangyingyoupin.top

Go:   strings.Split(s, "\n")
来源：http://mul.xinyue.icu

Ruby: s.lines
来源：http://fya.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://sco.hfpthk.cn

[E20] 判断字符串是否为空
来源：http://uef.dashuyun.cn

Py:   if not s:
来源：http://yli.andypj.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bmp.chenlongwang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wml.tanke756.top

TS:   if (s === "") {}
来源：http://khb.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://hzl.shanyushiyangtech.top

Go:   if s == "" {}
来源：http://yry.hammf.cn

Ruby: if s.empty?
来源：http://dut.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tmy.52xcode.cn

[E21] 超长截断加省略号
来源：http://eqw.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aze.fanxiaobao.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://chu.zdqjudy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nnz.ctjpmb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yeo.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vme.redwolf501.top

Go:   // 按 rune 判断长度后截断
来源：http://odh.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uyx.tarul.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kgk.hnxiangtu.top


<!-- 参考信息 -->