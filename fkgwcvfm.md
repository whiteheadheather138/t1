代发 wailian999

C#:   list.Distinct().ToList()
来源：http://lpx.cdnleiting.top

[D16] 求和与平均值
来源：http://caw.ydjk.org.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qvf.vehdjk.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gjb.sjlbkw.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jnn.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nun.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aes.hesvh.cn

Go:   // 手写循环累加
来源：http://fyi.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bhm.nanxinkj.top

C#:   list.Sum();  list.Average()
来源：http://tzv.shangyingyoupin.top

[D17] 最大值与最小值
来源：http://ckm.yj202588.top

Py:   max(arr);  min(arr)
来源：http://som.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://hkk.ydjk.org.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dgh.guannengcc.top

TS:   Math.max(...arr);
来源：http://btv.quarkkingdee.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nmb.jinghuilouyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://aor.zhengqikj.top

Ruby: arr.max;  arr.min
来源：http://ejb.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://jtu.zhiwuduotai.top

[D18] 扁平化嵌套数组
来源：http://ifl.jianghu66.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yvl.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://ils.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://puw.hysaishi.cn

TS:   nested.flat();
来源：http://bps.c1oappe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://log.smart0.xyz

Go:   // 手写双层循环
来源：http://wca.zhoulong.xyz

Ruby: nested.flatten
来源：http://ixa.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cqe.yangfankeji.com

[D19] 按字段分组
来源：http://vfv.yuanzhike.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vkn.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mbl.tanke756.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fbv.yonumen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mqe.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rmu.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://mtu.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bbm.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bei.daxiang520.top

[D20] 统计每个元素出现次数
来源：http://tej.gzhubu.top

Py:   Counter(arr)
来源：http://wvc.yj202588.top

PHP:  array_count_values($arr);
来源：http://vyn.iojbl.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vjf.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://joq.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://osq.vqdsnc.cn

Go:   // 手写 map[T]int
来源：http://hcz.snrcjt.cn

Ruby: arr.tally
来源：http://ack.sweek.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yrd.aibaodan.cn

[D21] 判断是否包含某元素
来源：http://qqb.zhaomingkeji.xyz

Py:   x in arr
来源：http://vsi.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://igf.c1oappe.top

JS:   arr.includes(x)
来源：http://lwo.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://qdh.jiagoushi.top

Java: list.contains(x)
来源：http://oze.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://xpm.jinyuanbaomall.cn

Ruby: arr.include?(x)
来源：http://lke.svipenyu.cn

C#:   list.Contains(x)
来源：http://ulu.daria6918.cn

[D22] 复制数组（避免共享引用）
来源：http://zhg.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ahp.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nxc.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nuj.ctjpmb.com

TS:   [...arr];
来源：http://qci.yonumen.top

Java: new ArrayList<>(list);
来源：http://xkn.shanyushiyangtech.top

Go:   copied := append([]int(nil), arr...)
来源：http://whd.jinqigufen.top

Ruby: arr.dup;  arr.clone
来源：http://wwv.ybcxt.top

C#:   new List<int>(list);
来源：http://qez.jqgfzy.top

[D23] reduce 累积计算
来源：http://njf.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qeo.jinqigufen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uwo.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pow.gogol.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zuk.yonumen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://leo.nwbrower.top

Go:   // 手写循环
来源：http://hlw.ehwqpu.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://flf.9152youxi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lra.hysaishi.cn

[D24] 字典 / Map 基本操作
来源：http://hga.fanxiaobao.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eti.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gmd.guannengcc.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vej.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://khd.fzhhl.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://agq.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dqn.hysaishi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vgs.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zzh.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://hkg.yangfankeji.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lnx.xinyue.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://end.uphjek.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ksd.tarul.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eml.chenzaomai.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zrt.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wrv.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://czf.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ujk.havefunace.top

[D26] 数组转字符串
来源：http://pkj.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://use.pycfn.com

PHP:  implode(", ", $arr);
来源：http://okj.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://eli.9152youxi.cn

TS:   arr.join(", ")
来源：http://qjs.yongpay.top

Java: String.join(", ", list)
来源：http://zbt.sjlbkw.cn

Go:   strings.Join(strs, ", ")
来源：http://wah.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://nkb.zdbjq.cn

C#:   string.Join(", ", list)
来源：http://hwt.dianchejie.cn

================================================================================
来源：http://tzs.zdbjq.cn

E. 字符串处理
来源：http://lpr.mhx1999.top

================================================================================
来源：http://mzv.zhoulong.xyz

[E01] 拼接字符串
来源：http://lvx.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jex.pengpengdd.cyou

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hlk.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ztl.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fbo.zdqjudy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uhe.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://prl.fktsv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://glf.cucudq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rfz.ctjpmb.com

[E02] 重复字符串
来源：http://isp.zycfv.cn

Py:   "ab" * 3
来源：http://pbu.zycfv.cn

PHP:  str_repeat("ab", 3);
来源：http://whk.chenzaomai.com

JS:   "ab".repeat(3)
来源：http://zpu.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://xym.jinqigufen.top

Java: "ab".repeat(3)
来源：http://ggg.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://nln.ppjwa.cn

Ruby: "ab" * 3
来源：http://mfl.jiagoushi.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kro.uphjek.com

[E03] 截取子串
来源：http://uss.epnwcf.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zfi.hysaishi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jlg.c1oappe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hsg.hammf.cn

TS:   s.slice(1, 4)
来源：http://qym.nanxinkj.top

Java: s.substring(1, 4)
来源：http://eyf.zhongyouzk.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ugn.shuidangran.top

Ruby: s[1, 3];  s[1..3]
来源：http://qbg.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://jxw.yuxming.cn

[E04] 查找子串位置
来源：http://een.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://tdu.hongshengwenyu.top

PHP:  strpos($s, "x");
来源：http://xnf.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jct.hysaishi.cn

TS:   s.indexOf("x")
来源：http://vzb.yfazqb.com

Java: s.indexOf("x")
来源：http://cbo.zhengqikj.top

Go:   strings.Index(s, "x")
来源：http://bba.zycfv.cn

Ruby: s.index("x")
来源：http://rvd.hnxiangtu.top

C#:   s.IndexOf("x")
来源：http://ejz.zycfv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rgn.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bxf.xziqi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://css.zhixingplan.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oda.tian-w.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qiu.epnwcf.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gtq.yj20258.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ela.bjfxy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://olv.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bus.shanyushiyangtech.top

[E06] 替换子串
来源：http://gbu.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ebg.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://sts.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zeu.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://ooy.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tum.fengsongda.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xvt.shzxlz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://otr.chenlongwang.top

C#:   s.Replace("a", "b")
来源：http://qkk.jlsjyb.cn

[E07] 按分隔符拆分
来源：http://hsj.jianghu66.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xhq.0kj1m.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ifh.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xkx.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://iir.uphjek.com

Java: s.split(",");  s.split("\\s+")
来源：http://woa.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kef.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://kck.hammf.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://onr.dashuyun.cn

[E08] 数组按分隔符合并
来源：http://ifw.316326.xyz

Py:   ",".join(items)
来源：http://blm.yongpay.top

PHP:  implode(",", $items);
来源：http://dyk.jyoumei.cn

JS:   items.join(",")
来源：http://mon.yuxming.cn

TS:   items.join(",")
来源：http://pbs.ctjpmb.com

Java: String.join(",", items)
来源：http://kxb.epnwcf.com

Go:   strings.Join(items, ",")
来源：http://wnw.xingfuxueyuan.xyz

Ruby: items.join(",")
来源：http://hbs.vehdjk.com

C#:   string.Join(",", items)
来源：http://vmz.ehwqpu.com

[E09] 去除所有空白字符
来源：http://xyi.zhijiandao.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lfe.shangyingyoupin.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jbb.jinqigufen.top

JS:   s.replace(/\s+/g, "")
来源：http://wjk.hnxiangtu.top

TS:   s.replace(/\s+/g, "")
来源：http://lcr.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://kef.yuanzhike.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xny.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://oxz.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hyl.nanxuanxn.top

[E10] 左侧补零 / 定长填充
来源：http://tlj.vqdsnc.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://map.jqgfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://okm.tanke756.top

JS:   "7".padStart(3, "0")
来源：http://zaz.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://hey.daria6918.cn

Java: String.format("%03d", 7)
来源：http://ija.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://mbb.ydjk.org.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://myt.yonumen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://feo.ivvv.top

[E11] 反转字符串
来源：http://pen.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://iyp.sjlbkw.cn

PHP:  strrev($s);
来源：http://pvx.jyoumei.cn

JS:   [...s].reverse().join("")
来源：http://gej.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://yxp.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qzk.zhongyouzk.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tpz.jinqigufen.top

Ruby: s.reverse
来源：http://mea.hesvh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gqn.guannengcc.top

[E12] 统计某字符出现次数
来源：http://xii.jinqigufen.top

Py:   s.count("a")
来源：http://qwq.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://ewa.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://dkx.jqgfzy.top

TS:   s.split("a").length - 1
来源：http://uxd.hammf.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nvr.svipenyu.cn

Go:   strings.Count(s, "a")
来源：http://ezt.tian-w.cn

Ruby: s.count("a")
来源：http://wfa.aizwys.cn

C#:   s.Count(c => c == 'a')
来源：http://koy.nanxuanxn.top

[E13] 逐字符遍历
来源：http://bky.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://fpg.jianghu66.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ags.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wbr.zdbjq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kqz.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pss.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gnh.xingfuxueyuan.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://xmk.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://coi.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://hqj.tianlin.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kbg.zhengqikj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qnp.hfpthk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oxe.jqgufenzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rya.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cbu.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qtu.zhongyouzk.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gmf.xziqi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zhp.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://kmo.gaohongyu789.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ovp.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kym.hcnkem.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lzv.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://iry.guowangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ezi.hongshengwenyu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bae.hongshengwenyu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kpv.yonumen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://equ.jiagoushi.top

[E16] 数字千分位
来源：http://bdh.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://vpf.yueranfly.top

PHP:  number_format(1234567);
来源：http://nxl.uphjek.com

JS:   (1234567).toLocaleString("en-US")
来源：http://vsq.kuanghao11.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cpq.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yny.zhiwuduotai.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://une.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hdg.xingfuxueyuan.xyz

C#:   1234567.ToString("N0")
来源：http://oam.jqgufenzy.top

[E17] 首字母大写
来源：http://fbi.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ojm.hnxiangtu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://plu.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sea.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gbl.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ebv.yj20258.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jve.tianlin.xyz

Ruby: s.capitalize
来源：http://fzd.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oqd.gaohongyu789.top

[E18] 模板占位符替换
来源：http://pez.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ycz.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://otd.yangfankeji.com

JS:   tpl.replaceAll("{name}", name)
来源：http://joy.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yrz.c1oappe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dqn.nanxuanxn.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tvs.zhengqikj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kei.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cba.meibo888.top

[E19] 多行文本按行拆分
来源：http://vvh.pycfn.com

Py:   s.splitlines()
来源：http://jsj.havefunace.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rsp.c1oappe.top

JS:   s.split(/\r?\n/)
来源：http://zcw.sweek.top

TS:   s.split(/\r?\n/)
来源：http://sfq.vqdsnc.cn

Java: s.lines().toList()
来源：http://avz.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://xjh.fzhhl.top

Ruby: s.lines
来源：http://khb.yonumen.top

C#:   s.Split('\n')
来源：http://usa.hongshengwenyu.top

[E20] 判断字符串是否为空
来源：http://mkp.jinqigufen.top

Py:   if not s:
来源：http://bzt.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hev.zdqjudy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tic.aibaodan.cn

TS:   if (s === "") {}
来源：http://aot.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://pzq.yj20258.top

Go:   if s == "" {}
来源：http://yti.ybcxt.top

Ruby: if s.empty?
来源：http://rtz.tarul.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fvw.haohaochexian.top

[E21] 超长截断加省略号
来源：http://vhc.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wld.yuxming.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hdz.hongshengwenyu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://puy.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hlq.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mco.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://ypt.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vff.birdmap.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fhm.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://nmx.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kvf.smart0.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sur.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://poe.andypj.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bpy.gzhubu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vjw.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bta.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://uof.daxiang520.top


<!-- 参考信息 -->