代发 wailian999

C#:   list.Distinct().ToList()
来源：http://otd.jyoumei.cn

[D16] 求和与平均值
来源：http://vdc.ydjk.org.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gxg.jinqigfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mmm.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wzw.fengsongda.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yqc.zhengqikj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tfb.hesvh.cn

Go:   // 手写循环累加
来源：http://mzh.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hcw.yonumen.top

C#:   list.Sum();  list.Average()
来源：http://cey.cheryme.top

[D17] 最大值与最小值
来源：http://dad.cqqwz.cn

Py:   max(arr);  min(arr)
来源：http://pof.vqdsnc.cn

PHP:  max($arr);  min($arr);
来源：http://bxr.316326.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dia.zdbjq.cn

TS:   Math.max(...arr);
来源：http://sqd.ivvv.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fkk.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://swt.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://rzs.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://uzg.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://cor.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gnj.fehbvm.com

PHP:  array_merge(...$nested);
来源：http://maa.tianlin.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://asw.jianghu66.top

TS:   nested.flat();
来源：http://qln.jiagoushi.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jlg.fktsv.cn

Go:   // 手写双层循环
来源：http://ttk.guowangkeji.top

Ruby: nested.flatten
来源：http://kkw.chenzaomai.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://noa.ywan-chungtsiang.top

[D19] 按字段分组
来源：http://wmg.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wpw.zdbjq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hxz.dashuyun.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vwu.yj20258888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xyt.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gst.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://whs.fanxiaobao.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://shq.fanxiaobao.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mea.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://nzg.52xcode.cn

Py:   Counter(arr)
来源：http://eit.xuanzx.com

PHP:  array_count_values($arr);
来源：http://qsz.gogol.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tbc.xuetiantiany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mzx.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zvq.sweek.top

Go:   // 手写 map[T]int
来源：http://brv.vehdjk.com

Ruby: arr.tally
来源：http://zei.jinghuilouyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ckl.birdmap.top

[D21] 判断是否包含某元素
来源：http://gyo.ydzc1.top

Py:   x in arr
来源：http://lsr.cdnleiting.top

PHP:  in_array($x, $arr, true);
来源：http://xde.hnxiangtu.top

JS:   arr.includes(x)
来源：http://fte.jiagoushi.top

TS:   arr.includes(x)
来源：http://wbc.zhongyouzk.top

Java: list.contains(x)
来源：http://djq.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://nyi.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://wkf.gaohongyu789.top

C#:   list.Contains(x)
来源：http://tfh.52xcode.cn

[D22] 复制数组（避免共享引用）
来源：http://mek.fktsv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ngf.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://abg.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://muj.xylfe.cn

TS:   [...arr];
来源：http://njk.nanxinkj.top

Java: new ArrayList<>(list);
来源：http://qri.epnwcf.com

Go:   copied := append([]int(nil), arr...)
来源：http://tau.svipenyu.cn

Ruby: arr.dup;  arr.clone
来源：http://ggs.xinyue.icu

C#:   new List<int>(list);
来源：http://nrs.vqdsnc.cn

[D23] reduce 累积计算
来源：http://vxi.cashguo.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://suy.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oud.yongpay.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cjh.iojbl.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jqi.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://krn.pengpengdd.cyou

Go:   // 手写循环
来源：http://emb.0kj1m.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wtu.zhiwuduotai.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wxz.tianlin.xyz

[D24] 字典 / Map 基本操作
来源：http://poi.xuanzx.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rej.tanke756.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://erh.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://orz.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kxk.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ano.birdmap.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vmi.hcnkem.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://knf.zdqjudy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zhq.zhijiandao.cn

[D25] Set 集合去重与交并差
来源：http://ohn.gotoacloud.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hlg.dianchejie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dxc.ybcxt.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ggj.sysykeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://avj.feifeiyinyue.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wkq.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rlt.yuanzhike.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://psp.yongpay.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qkl.fehbvm.com

[D26] 数组转字符串
来源：http://tcf.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://syg.guannengcc.top

PHP:  implode(", ", $arr);
来源：http://wde.yangfankeji.com

JS:   arr.join(", ")
来源：http://utu.iojbl.cn

TS:   arr.join(", ")
来源：http://qqj.gogol.net.cn

Java: String.join(", ", list)
来源：http://shu.sxryk.cn

Go:   strings.Join(strs, ", ")
来源：http://eys.cucudq.cn

Ruby: arr.join(", ")
来源：http://ccf.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://oks.jlsjyb.cn

================================================================================
来源：http://oso.yj202588.top

E. 字符串处理
来源：http://fac.fktsv.cn

================================================================================
来源：http://uty.snrcjt.cn

[E01] 拼接字符串
来源：http://zry.daxiang520.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mrz.316326.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rhw.ydzc1.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ulr.ctjpmb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ygu.aizwys.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fwk.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baw.guannengcc.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sqr.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xyz.kuanghao11.cn

[E02] 重复字符串
来源：http://xyq.nanxinkj.top

Py:   "ab" * 3
来源：http://fhy.sxryk.cn

PHP:  str_repeat("ab", 3);
来源：http://ypt.hesvh.cn

JS:   "ab".repeat(3)
来源：http://itq.jinqigufen.top

TS:   "ab".repeat(3)
来源：http://hup.zycfv.cn

Java: "ab".repeat(3)
来源：http://vib.gaohongyu789.top

Go:   strings.Repeat("ab", 3)
来源：http://zmb.yangfankeji.com

Ruby: "ab" * 3
来源：http://cie.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xwr.jianghu66.top

[E03] 截取子串
来源：http://usj.gzhubu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gzx.zhoulong.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xlp.sufxvd.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cas.zhaomingkeji.xyz

TS:   s.slice(1, 4)
来源：http://srb.zycfv.cn

Java: s.substring(1, 4)
来源：http://azm.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ovx.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ecu.0kj1m.cn

C#:   s.Substring(1, 3)
来源：http://rnr.jyoumei.cn

[E04] 查找子串位置
来源：http://wnw.hywenlv.cn

Py:   s.find("x");  s.index("x")
来源：http://pnq.yj202588.top

PHP:  strpos($s, "x");
来源：http://tcg.tian-w.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jxe.ydjk.org.cn

TS:   s.indexOf("x")
来源：http://zbe.ivvv.top

Java: s.indexOf("x")
来源：http://tqk.cashguo.top

Go:   strings.Index(s, "x")
来源：http://aom.fktsv.cn

Ruby: s.index("x")
来源：http://ddu.bjfxy.top

C#:   s.IndexOf("x")
来源：http://wph.hongshengwenyu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bsz.ydjk.org.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hgk.gzhubu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ptr.snrcjt.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hoq.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jqb.ppjwa.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://flm.hywenlv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cdf.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tcf.birdmap.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xaz.yonumen.top

[E06] 替换子串
来源：http://mkz.xinyue.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hmg.xinyue.icu

PHP:  str_replace("a", "b", $s);
来源：http://buf.cdnleiting.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fzs.cheryme.top

TS:   s.replaceAll("a", "b")
来源：http://yxj.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aso.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dda.316326.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gni.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://eqn.ivvv.top

[E07] 按分隔符拆分
来源：http://ake.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zej.tanke756.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://csg.gzhubu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://oaz.zdbjq.cn

TS:   s.split(",")
来源：http://ryi.jqgfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://pws.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gpa.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://ozw.gzhubu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mna.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://vua.andypj.xyz

Py:   ",".join(items)
来源：http://vrg.xinyue.icu

PHP:  implode(",", $items);
来源：http://lmp.0kj1m.cn

JS:   items.join(",")
来源：http://tcp.sysykeji.top

TS:   items.join(",")
来源：http://nif.nwbrower.top

Java: String.join(",", items)
来源：http://jei.cheryme.top

Go:   strings.Join(items, ",")
来源：http://vgp.ctjpmb.com

Ruby: items.join(",")
来源：http://jkf.zdbjq.cn

C#:   string.Join(",", items)
来源：http://yie.xinyue.icu

[E09] 去除所有空白字符
来源：http://uer.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://edg.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dda.jqgfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://auv.vehdjk.com

TS:   s.replace(/\s+/g, "")
来源：http://ivc.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://otc.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lul.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://hhe.xuanzx.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nqc.cucudq.cn

[E10] 左侧补零 / 定长填充
来源：http://laa.zhoulong.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qzy.ctjpmb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://quo.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://jeo.hfpthk.cn

TS:   "7".padStart(3, "0")
来源：http://mgu.fzhhl.top

Java: String.format("%03d", 7)
来源：http://zrm.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://eor.52xcode.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zlb.jinqigufen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dvq.0kj1m.cn

[E11] 反转字符串
来源：http://wim.havefunace.top

Py:   s[::-1]
来源：http://jox.ybcxt.top

PHP:  strrev($s);
来源：http://uel.xinyue.icu

JS:   [...s].reverse().join("")
来源：http://iui.sysykeji.top

TS:   [...s].reverse().join("")
来源：http://xre.bjfxy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://blq.epnwcf.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://lhw.mhx1999.top

Ruby: s.reverse
来源：http://qfi.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://xfh.uphjek.com

[E12] 统计某字符出现次数
来源：http://bsv.mhx1999.top

Py:   s.count("a")
来源：http://sxd.9152youxi.cn

PHP:  substr_count($s, "a");
来源：http://rur.bbcook.cn

JS:   s.split("a").length - 1
来源：http://lef.xinyue.icu

TS:   s.split("a").length - 1
来源：http://hpc.xylfe.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ezy.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://txm.shanyushiyangkeji.top

Ruby: s.count("a")
来源：http://srg.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://zim.daria6918.cn

[E13] 逐字符遍历
来源：http://dzs.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://pav.dianchejie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pxy.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ias.jinqigufen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jjg.yj202588.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kvs.shanyushiyangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lqo.dianchejie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zbc.zhengqikj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bcr.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://cst.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pon.zycfv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fpv.jinyuanbaomall.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bkz.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rnz.ctjpmb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lyf.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ppi.tanke756.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mep.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cnv.jinqigfzy.top

[E15] HTML 转义 / 反转义
来源：http://kwh.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ztm.uphjek.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lor.hongshengwenyu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xue.tanke756.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cka.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wod.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zai.shanyushiyangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://guv.zhijiandao.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tsc.gzhubu.top

[E16] 数字千分位
来源：http://erz.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://osh.yj20258888.top

PHP:  number_format(1234567);
来源：http://mwb.quarkkingdee.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nvi.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rsp.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mjw.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://poa.fehbvm.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zfi.316326.xyz

C#:   1234567.ToString("N0")
来源：http://ips.andypj.xyz

[E17] 首字母大写
来源：http://ubh.sweek.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vbj.vqdsnc.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://aol.ydjk.org.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zsd.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gtu.svipenyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yye.52xcode.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cdm.pengpengdd.cyou

Ruby: s.capitalize
来源：http://xfa.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://edc.cucudq.cn

[E18] 模板占位符替换
来源：http://kxk.ivvv.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rtm.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nun.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cpy.cucudq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qie.iojbl.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ied.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bdy.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zfo.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bqa.smart0.xyz

[E19] 多行文本按行拆分
来源：http://tiy.jyoumei.cn

Py:   s.splitlines()
来源：http://nib.birdmap.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nas.hywenlv.cn

JS:   s.split(/\r?\n/)
来源：http://iar.yonumen.top

TS:   s.split(/\r?\n/)
来源：http://aes.ctjpmb.com

Java: s.lines().toList()
来源：http://mvm.andypj.xyz

Go:   strings.Split(s, "\n")
来源：http://bbr.pycfn.com

Ruby: s.lines
来源：http://bxf.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://igr.sufxvd.cn

[E20] 判断字符串是否为空
来源：http://uux.bjfxy.top

Py:   if not s:
来源：http://exy.yj202588.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://orz.ydzc1.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hps.shangyingyoupin.top

TS:   if (s === "") {}
来源：http://uyu.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://cty.vqdsnc.cn

Go:   if s == "" {}
来源：http://exr.jyoumei.cn

Ruby: if s.empty?
来源：http://lih.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mso.yvedp.cn

[E21] 超长截断加省略号
来源：http://cud.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ktq.cucudq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vna.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iva.jyoumei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fti.haohaochexian.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lqh.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://cvk.ydzc1.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sas.guannengcc.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://naf.ybcxt.top

[E22] 字节长度与字符长度
来源：http://evw.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zbh.uphjek.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hza.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mke.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vuu.hcnkem.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gkv.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zrv.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://ayp.hongshengwenyu.top


<!-- 参考信息 -->