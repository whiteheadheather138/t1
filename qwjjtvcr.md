代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://waz.snrcjt.cn

C#:   list.Sum();  list.Average()
来源：http://nzy.zdbjq.cn

[D17] 最大值与最小值
来源：http://qrj.cdnleiting.top

Py:   max(arr);  min(arr)
来源：http://yjj.jiagoushi.top

PHP:  max($arr);  min($arr);
来源：http://ikx.nanxinkj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hjk.zhengqikj.top

TS:   Math.max(...arr);
来源：http://azw.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qow.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yho.zhoulong.xyz

Ruby: arr.max;  arr.min
来源：http://nip.xinyue.icu

C#:   list.Max();  list.Min()
来源：http://iiv.xingfuxueyuan.xyz

[D18] 扁平化嵌套数组
来源：http://iki.ppjwa.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jmh.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://eyb.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ugt.hcnkem.com

TS:   nested.flat();
来源：http://uut.cdnleiting.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oiw.meibo888.top

Go:   // 手写双层循环
来源：http://dab.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://scc.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wlp.nwbrower.top

[D19] 按字段分组
来源：http://jdd.tian-w.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pzz.zycfv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xah.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ata.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kkp.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hqr.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://ozv.vqdsnc.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rvn.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://don.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://vpc.ybcxt.top

Py:   Counter(arr)
来源：http://pbj.xuanzx.com

PHP:  array_count_values($arr);
来源：http://pgp.fanxiaobao.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kxs.ybcxt.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ijt.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://isy.hysaishi.cn

Go:   // 手写 map[T]int
来源：http://xcg.sysykeji.top

Ruby: arr.tally
来源：http://hxn.yuanzhike.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dvv.daria6918.cn

[D21] 判断是否包含某元素
来源：http://jng.chenzaomai.com

Py:   x in arr
来源：http://nxa.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://hin.0kj1m.cn

JS:   arr.includes(x)
来源：http://clp.ydjk.org.cn

TS:   arr.includes(x)
来源：http://qax.jyoumei.cn

Java: list.contains(x)
来源：http://yol.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://nma.xingfuxueyuan.xyz

Ruby: arr.include?(x)
来源：http://bwz.havefunace.top

C#:   list.Contains(x)
来源：http://rxx.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://pps.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xfl.jiagoushi.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://met.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://elr.sjlbkw.cn

TS:   [...arr];
来源：http://xzd.havefunace.top

Java: new ArrayList<>(list);
来源：http://gzi.dashuyun.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xpd.fktsv.cn

Ruby: arr.dup;  arr.clone
来源：http://hsk.jinqigfzy.top

C#:   new List<int>(list);
来源：http://dcc.ywan-chungtsiang.top

[D23] reduce 累积计算
来源：http://swj.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sbp.redwolf501.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nrv.xinyue.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://myo.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sll.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ipl.yuanzhike.top

Go:   // 手写循环
来源：http://phs.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://apz.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wjs.hnqzz.top

[D24] 字典 / Map 基本操作
来源：http://rlo.yvedp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://brt.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aiu.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nah.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gju.jlsjyb.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fcy.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://upi.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://evq.wangshuangyany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rrr.kuanghao11.cn

[D25] Set 集合去重与交并差
来源：http://ebo.cqqwz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hno.tarul.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cru.jinyuanbaomall.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aab.0kj1m.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lam.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hyi.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yyz.yuxming.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dnd.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lww.cheryme.top

[D26] 数组转字符串
来源：http://fkv.redwolf501.top

Py:   ", ".join(map(str, arr))
来源：http://eim.yangfankeji.com

PHP:  implode(", ", $arr);
来源：http://gts.yangfankeji.com

JS:   arr.join(", ")
来源：http://wky.shuidangran.top

TS:   arr.join(", ")
来源：http://nid.feifeiyinyue.top

Java: String.join(", ", list)
来源：http://del.cashguo.top

Go:   strings.Join(strs, ", ")
来源：http://djk.cqqwz.cn

Ruby: arr.join(", ")
来源：http://uwy.guowangkeji.top

C#:   string.Join(", ", list)
来源：http://owb.aibaodan.cn

================================================================================
来源：http://iqa.jlsjyb.cn

E. 字符串处理
来源：http://dag.yanxiufei.cn

================================================================================
来源：http://hcq.ybcxt.top

[E01] 拼接字符串
来源：http://cae.ivvv.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jjy.pengpengdd.cyou

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sei.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://khg.hywenlv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ejc.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://syq.yangfankeji.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lab.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xpx.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lvs.jiagoushi.top

[E02] 重复字符串
来源：http://fzv.jinghuilouyu.cn

Py:   "ab" * 3
来源：http://vqo.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://tcq.svipenyu.cn

JS:   "ab".repeat(3)
来源：http://eav.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://crj.ivvv.top

Java: "ab".repeat(3)
来源：http://bqr.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://fkc.iojbl.cn

Ruby: "ab" * 3
来源：http://bcv.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jtm.cucudq.cn

[E03] 截取子串
来源：http://rbc.snrcjt.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hpj.hysaishi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ykp.iojbl.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wfr.hongshengwenyu.top

TS:   s.slice(1, 4)
来源：http://rfy.9152youxi.cn

Java: s.substring(1, 4)
来源：http://kfe.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://msw.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yqh.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://fhf.ehwqpu.com

[E04] 查找子串位置
来源：http://cnb.cqqwz.cn

Py:   s.find("x");  s.index("x")
来源：http://mgz.yj20258.top

PHP:  strpos($s, "x");
来源：http://eyu.birdmap.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hpa.fanxiaobao.xyz

TS:   s.indexOf("x")
来源：http://kzp.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://slf.tanke756.top

Go:   strings.Index(s, "x")
来源：http://soi.fehbvm.com

Ruby: s.index("x")
来源：http://dkg.tanke756.top

C#:   s.IndexOf("x")
来源：http://bnd.xuanzx.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://dst.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qff.tian-w.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sqe.yvedp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nxg.jianghu66.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kmh.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://upu.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lhi.yanxiufei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ank.daxiang520.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://szk.0kj1m.cn

[E06] 替换子串
来源：http://cme.zhengqikj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pno.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://jbm.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qsz.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://irv.fehbvm.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ljz.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fzg.shzxlz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ggy.tanke756.top

C#:   s.Replace("a", "b")
来源：http://zhk.yj20258888.top

[E07] 按分隔符拆分
来源：http://obq.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yvw.jinyuanbaomall.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zhr.yuanzhike.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wxj.jyoumei.cn

TS:   s.split(",")
来源：http://lcq.hnqzz.top

Java: s.split(",");  s.split("\\s+")
来源：http://jxs.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jgl.nwbrower.top

Ruby: s.split(",");  s.split
来源：http://pro.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jzg.gzhubu.top

[E08] 数组按分隔符合并
来源：http://hht.yj20258888.top

Py:   ",".join(items)
来源：http://htk.yueranfly.top

PHP:  implode(",", $items);
来源：http://ixh.sweek.top

JS:   items.join(",")
来源：http://tsw.svipenyu.cn

TS:   items.join(",")
来源：http://pxg.fengsongda.top

Java: String.join(",", items)
来源：http://zki.shanyushiyangkeji.top

Go:   strings.Join(items, ",")
来源：http://zzc.52xcode.cn

Ruby: items.join(",")
来源：http://mwy.feifeiyinyue.top

C#:   string.Join(",", items)
来源：http://fqq.aibaodan.cn

[E09] 去除所有空白字符
来源：http://uaw.zhixingplan.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://osa.nanxinkj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gnj.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://ged.nanxinkj.top

TS:   s.replace(/\s+/g, "")
来源：http://lhe.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://xyh.yj20258888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hnq.jyoumei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zjg.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vnv.jinqigufen.top

[E10] 左侧补零 / 定长填充
来源：http://jnx.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jky.cashguo.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nta.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://vlv.0kj1m.cn

TS:   "7".padStart(3, "0")
来源：http://vxa.xylfe.cn

Java: String.format("%03d", 7)
来源：http://xzr.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cos.hysaishi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yie.wangdashe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dvi.yfazqb.com

[E11] 反转字符串
来源：http://grq.pycfn.com

Py:   s[::-1]
来源：http://nww.epnwcf.com

PHP:  strrev($s);
来源：http://ytx.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://kwz.tarul.cn

TS:   [...s].reverse().join("")
来源：http://mpe.jqgfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pcw.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dku.shuidangran.top

Ruby: s.reverse
来源：http://oro.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://xiw.yongpay.top

[E12] 统计某字符出现次数
来源：http://shw.nanxinkj.top

Py:   s.count("a")
来源：http://qah.pycfn.com

PHP:  substr_count($s, "a");
来源：http://bdk.mhx1999.top

JS:   s.split("a").length - 1
来源：http://svc.jqgfzy.top

TS:   s.split("a").length - 1
来源：http://lyy.yuxming.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oen.0kj1m.cn

Go:   strings.Count(s, "a")
来源：http://lob.bbcook.cn

Ruby: s.count("a")
来源：http://fju.52xcode.cn

C#:   s.Count(c => c == 'a')
来源：http://gzf.9152youxi.cn

[E13] 逐字符遍历
来源：http://xwh.chenjidiqi.icu

Py:   for ch in s: print(ch)
来源：http://tnb.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jvd.fanxiaobao.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://eqz.ydjk.org.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wpy.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://acd.hfpthk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zxv.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://svd.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yro.fengsongda.top

[E14] URL 编码与 Base64
来源：http://nxd.sysykeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xdn.zhixingplan.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xoj.yonumen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zxb.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gix.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yxq.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://txc.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yoj.cheryme.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rtt.bbcook.cn

[E15] HTML 转义 / 反转义
来源：http://ssc.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ihp.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fjc.shangyingyoupin.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qzz.nanxinkj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gco.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kbs.svipenyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ogw.ctjpmb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bsj.gzhubu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hbt.redwolf501.top

[E16] 数字千分位
来源：http://mui.yongpay.top

Py:   f"{1234567:,}"
来源：http://lbx.tianlin.xyz

PHP:  number_format(1234567);
来源：http://mxm.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bes.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hos.shangyingyoupin.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://osp.andypj.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fuo.ppjwa.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tpo.ivvv.top

C#:   1234567.ToString("N0")
来源：http://pbn.shangyingyoupin.top

[E17] 首字母大写
来源：http://ecw.aibaodan.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mjx.ehwqpu.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://lop.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dsg.guannengcc.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rii.pycfn.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nhj.9152youxi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ixy.xziqi.cn

Ruby: s.capitalize
来源：http://emj.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://soa.yvedp.cn

[E18] 模板占位符替换
来源：http://mgd.yj202588.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://grk.epnwcf.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dou.chenlongwang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cvq.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ddd.mhx1999.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mqr.ywan-chungtsiang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zcl.nwbrower.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mqz.mhx1999.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jvu.yfazqb.com

[E19] 多行文本按行拆分
来源：http://jqq.uphjek.com

Py:   s.splitlines()
来源：http://wjr.hnxiangtu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ict.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://cqc.fktsv.cn

TS:   s.split(/\r?\n/)
来源：http://qxf.gaohongyu789.top

Java: s.lines().toList()
来源：http://slm.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://rys.sysykeji.top

Ruby: s.lines
来源：http://sgs.ydjk.org.cn

C#:   s.Split('\n')
来源：http://jua.zhaomingkeji.xyz

[E20] 判断字符串是否为空
来源：http://tib.gaohongyu789.top

Py:   if not s:
来源：http://gzx.gzhubu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ppo.ydzc1.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pxw.fengsongda.top

TS:   if (s === "") {}
来源：http://csb.yonumen.top

Java: if (s.isEmpty()) {}
来源：http://sib.zhoulong.xyz

Go:   if s == "" {}
来源：http://iki.jqgfzy.top

Ruby: if s.empty?
来源：http://lxs.52xcode.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dzt.chenlongwang.top

[E21] 超长截断加省略号
来源：http://tte.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://usv.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ihp.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nea.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zwk.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rse.jianghu66.top

Go:   // 按 rune 判断长度后截断
来源：http://caq.hysaishi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nxx.jyoumei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ame.jinqigufen.top

[E22] 字节长度与字符长度
来源：http://tip.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ztj.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tmm.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dxu.zhiwuduotai.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vgc.hcnkem.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ixg.pengpengdd.cyou

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aih.yonumen.top

Ruby: s.bytesize;  s.length
来源：http://aua.havefunace.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oah.ivvv.top

================================================================================
来源：http://jcu.shanyushiyangtech.top

F. 文件与目录
来源：http://uki.zdqjudy.top

================================================================================
来源：http://lrr.chenlongwang.top

[F01] 读取整个文件
来源：http://mtg.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mga.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://liy.hesvh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zcf.hywenlv.cn


<!-- 参考信息 -->