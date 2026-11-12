代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dod.xingfuxueyuan.xyz

C#:   list.Sum();  list.Average()
来源：http://dfb.smart0.xyz

[D17] 最大值与最小值
来源：http://zbm.meibo888.top

Py:   max(arr);  min(arr)
来源：http://sop.svipenyu.cn

PHP:  max($arr);  min($arr);
来源：http://gtf.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zkq.epnwcf.com

TS:   Math.max(...arr);
来源：http://ppd.cucudq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://suy.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fqa.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://rck.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://msp.jianghu66.top

[D18] 扁平化嵌套数组
来源：http://ulm.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vpo.guowangkeji.top

PHP:  array_merge(...$nested);
来源：http://tkx.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uhe.jyoumei.cn

TS:   nested.flat();
来源：http://rna.xuetiantiany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sxj.cheryme.top

Go:   // 手写双层循环
来源：http://jhx.tanke756.top

Ruby: nested.flatten
来源：http://qde.jinqigufen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fli.shanyushiyangtech.top

[D19] 按字段分组
来源：http://mam.vqdsnc.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ysm.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qvj.fengsongda.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ncp.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wem.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iwr.andypj.xyz

Go:   // 手写 map[string][]T
来源：http://ccx.birdmap.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://poy.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kcl.yonumen.top

[D20] 统计每个元素出现次数
来源：http://ubs.ydjk.org.cn

Py:   Counter(arr)
来源：http://ntz.hammf.cn

PHP:  array_count_values($arr);
来源：http://oxd.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uio.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://udw.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wir.pycfn.com

Go:   // 手写 map[T]int
来源：http://xmb.hfpthk.cn

Ruby: arr.tally
来源：http://epg.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kai.shanyushiyangkeji.top

[D21] 判断是否包含某元素
来源：http://bru.9152youxi.cn

Py:   x in arr
来源：http://ilk.pycfn.com

PHP:  in_array($x, $arr, true);
来源：http://iwy.316326.xyz

JS:   arr.includes(x)
来源：http://pwm.hongshengwenyu.top

TS:   arr.includes(x)
来源：http://yxb.feifeiyinyue.top

Java: list.contains(x)
来源：http://xmm.sxryk.cn

Go:   slices.Contains(arr, x)
来源：http://lmf.nwbrower.top

Ruby: arr.include?(x)
来源：http://yto.gzhubu.top

C#:   list.Contains(x)
来源：http://esc.xuanzx.com

[D22] 复制数组（避免共享引用）
来源：http://ymh.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aib.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nks.sufxvd.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jyn.wangdashe.top

TS:   [...arr];
来源：http://jao.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://tdt.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://mdo.daria6918.cn

Ruby: arr.dup;  arr.clone
来源：http://oza.fanxiaobao.xyz

C#:   new List<int>(list);
来源：http://spn.9152youxi.cn

[D23] reduce 累积计算
来源：http://jft.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dvi.jinyuanbaomall.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ksr.epnwcf.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qbf.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qjs.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pat.ppjwa.cn

Go:   // 手写循环
来源：http://dtr.jinqigufen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uys.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ywe.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://foy.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rwv.dianchejie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kks.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://emn.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://odb.epnwcf.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fdz.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rvo.jinghuilouyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tic.hongshengwenyu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bus.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://qkm.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bet.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ylc.fzhhl.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qqw.nanxinkj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://loi.daxiang520.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mki.yueranfly.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cxw.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ceo.tianlin.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mkq.fengsongda.top

[D26] 数组转字符串
来源：http://ztj.zhiwuduotai.top

Py:   ", ".join(map(str, arr))
来源：http://igf.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://uav.fengsongda.top

JS:   arr.join(", ")
来源：http://vtc.zhengqikj.top

TS:   arr.join(", ")
来源：http://hpt.dashuyun.cn

Java: String.join(", ", list)
来源：http://orm.52xcode.cn

Go:   strings.Join(strs, ", ")
来源：http://ozd.zhixingplan.top

Ruby: arr.join(", ")
来源：http://cbx.ivvv.top

C#:   string.Join(", ", list)
来源：http://jqu.tanke756.top

================================================================================
来源：http://vqr.kuanghao11.cn

E. 字符串处理
来源：http://ejd.cucudq.cn

================================================================================
来源：http://lde.pengpengdd.cyou

[E01] 拼接字符串
来源：http://xsy.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zws.gzhubu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xyw.fengsongda.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://luv.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yha.52xcode.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cdx.nanxinkj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://udl.tarul.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ooq.uphjek.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xzn.daria6918.cn

[E02] 重复字符串
来源：http://tzg.hysaishi.cn

Py:   "ab" * 3
来源：http://teb.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://ozf.jinqigfzy.top

JS:   "ab".repeat(3)
来源：http://ava.yonumen.top

TS:   "ab".repeat(3)
来源：http://gnm.jqgfzy.top

Java: "ab".repeat(3)
来源：http://krl.shangyingyoupin.top

Go:   strings.Repeat("ab", 3)
来源：http://vih.jinqigufen.top

Ruby: "ab" * 3
来源：http://pgh.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vcr.nwbrower.top

[E03] 截取子串
来源：http://xtg.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://asx.jqgfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yqn.yj202588.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gir.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://amf.ydjk.org.cn

Java: s.substring(1, 4)
来源：http://ffk.wangshuangyany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yvm.yuanzhike.top

Ruby: s[1, 3];  s[1..3]
来源：http://bnq.52xcode.cn

C#:   s.Substring(1, 3)
来源：http://kja.havefunace.top

[E04] 查找子串位置
来源：http://ldt.shuidangran.top

Py:   s.find("x");  s.index("x")
来源：http://qgc.52xcode.cn

PHP:  strpos($s, "x");
来源：http://lqg.ydjk.org.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://orr.shuidangran.top

TS:   s.indexOf("x")
来源：http://cdw.ppjwa.cn

Java: s.indexOf("x")
来源：http://rox.svipenyu.cn

Go:   strings.Index(s, "x")
来源：http://jwn.0kj1m.cn

Ruby: s.index("x")
来源：http://wph.tian-w.cn

C#:   s.IndexOf("x")
来源：http://wwx.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://xqt.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qzr.zhengqikj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uym.dashuyun.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vvu.snrcjt.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mbj.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mwg.ydjk.org.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://poo.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jfg.chenlongwang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jwx.xinyue.icu

[E06] 替换子串
来源：http://hor.birdmap.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sss.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://amh.tarul.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tgh.chenjidiqi.icu

TS:   s.replaceAll("a", "b")
来源：http://hfm.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ibw.ppjwa.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bah.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://umk.uphjek.com

C#:   s.Replace("a", "b")
来源：http://hfz.mhx1999.top

[E07] 按分隔符拆分
来源：http://kvw.xuanzx.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fld.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://shn.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://jbr.gaohongyu789.top

TS:   s.split(",")
来源：http://ewn.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://vyt.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://akl.dashuyun.cn

Ruby: s.split(",");  s.split
来源：http://sux.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ctg.zhiwuduotai.top

[E08] 数组按分隔符合并
来源：http://fnv.cqqwz.cn

Py:   ",".join(items)
来源：http://qaj.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://tcm.zhiwuduotai.top

JS:   items.join(",")
来源：http://xrr.kuanghao11.cn

TS:   items.join(",")
来源：http://ewj.hfpthk.cn

Java: String.join(",", items)
来源：http://ygm.shzxlz.cn

Go:   strings.Join(items, ",")
来源：http://fgm.xziqi.cn

Ruby: items.join(",")
来源：http://kts.pengpengdd.cyou

C#:   string.Join(",", items)
来源：http://mne.zhengqikj.top

[E09] 去除所有空白字符
来源：http://mdv.haohaochexian.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://okj.jqgfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bsk.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://rmt.yfazqb.com

TS:   s.replace(/\s+/g, "")
来源：http://jqh.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://jah.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qlm.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://lxm.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vcv.fanxiaobao.xyz

[E10] 左侧补零 / 定长填充
来源：http://xls.jinyuanbaomall.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vvw.aizwys.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ewy.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://vpz.guannengcc.top

TS:   "7".padStart(3, "0")
来源：http://pos.zhoulong.xyz

Java: String.format("%03d", 7)
来源：http://ncv.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://btj.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pcw.yvedp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iwb.dianchejie.cn

[E11] 反转字符串
来源：http://ktj.nanxinkj.top

Py:   s[::-1]
来源：http://rlj.yangfankeji.com

PHP:  strrev($s);
来源：http://ypv.shzxlz.cn

JS:   [...s].reverse().join("")
来源：http://mxs.aibaodan.cn

TS:   [...s].reverse().join("")
来源：http://ioi.hnxiangtu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ptj.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://cam.fanxiaobao.xyz

Ruby: s.reverse
来源：http://nnv.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://jsg.aizwys.cn

[E12] 统计某字符出现次数
来源：http://egu.yfazqb.com

Py:   s.count("a")
来源：http://iso.guowangkeji.top

PHP:  substr_count($s, "a");
来源：http://nle.zycfv.cn

JS:   s.split("a").length - 1
来源：http://aok.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://zzo.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://teu.aizwys.cn

Go:   strings.Count(s, "a")
来源：http://wxw.gogol.net.cn

Ruby: s.count("a")
来源：http://vvx.tarul.cn

C#:   s.Count(c => c == 'a')
来源：http://hhf.tarul.cn

[E13] 逐字符遍历
来源：http://src.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://wzk.shanyushiyangtech.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vog.sweek.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://icg.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ecq.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dmw.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lfl.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bkc.nanxuanxn.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://izg.yongpay.top

[E14] URL 编码与 Base64
来源：http://ytn.tanke756.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nke.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nxr.zycfv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ulf.sxryk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lml.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://txj.yuanzhike.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ybk.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xbi.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uep.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://fof.smart0.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://ohb.nanxuanxn.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pdc.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yqv.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://azd.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eph.daria6918.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://epv.zdqjudy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vmq.yangfankeji.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://smz.yvedp.cn

[E16] 数字千分位
来源：http://mxt.cheryme.top

Py:   f"{1234567:,}"
来源：http://rmf.jinyuanbaomall.cn

PHP:  number_format(1234567);
来源：http://htx.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xek.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fcd.ywan-chungtsiang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iga.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mzn.zhengqikj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wcz.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://wxx.wangshuangyany.cn

[E17] 首字母大写
来源：http://mwm.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dwh.xziqi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hcy.jinqigfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kqz.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pqc.9152youxi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oyc.snrcjt.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aph.dianchejie.cn

Ruby: s.capitalize
来源：http://sku.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ddo.hesvh.cn

[E18] 模板占位符替换
来源：http://fge.cucudq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cif.cucudq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://izz.shuidangran.top

JS:   tpl.replaceAll("{name}", name)
来源：http://obu.yonumen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zoo.zhiwuduotai.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ufd.zdqjudy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://taf.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hlv.shanyushiyangtech.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aaj.yongpay.top

[E19] 多行文本按行拆分
来源：http://cch.cqqwz.cn

Py:   s.splitlines()
来源：http://ggk.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cbg.fengsongda.top

JS:   s.split(/\r?\n/)
来源：http://gbu.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://bhg.wangdashe.top

Java: s.lines().toList()
来源：http://wom.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://pua.shzxlz.cn

Ruby: s.lines
来源：http://qfx.xingfuxueyuan.xyz

C#:   s.Split('\n')
来源：http://nxh.yueranfly.top

[E20] 判断字符串是否为空
来源：http://xuq.tanke756.top

Py:   if not s:
来源：http://mfb.quarkkingdee.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ffb.gotoacloud.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hfu.fengsongda.top

TS:   if (s === "") {}
来源：http://csj.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://ydf.snrcjt.cn

Go:   if s == "" {}
来源：http://wfl.hesvh.cn

Ruby: if s.empty?
来源：http://zqe.yuanzhike.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://idc.cdnleiting.top

[E21] 超长截断加省略号
来源：http://mza.pengpengdd.cyou

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tod.xinyue.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xhq.ywan-chungtsiang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nmj.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://glw.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nbc.hnqzz.top

Go:   // 按 rune 判断长度后截断
来源：http://wxc.dashuyun.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://raa.zycfv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ntu.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://xtu.jiagoushi.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lcn.cheryme.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://anf.yanxiufei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sfe.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://phi.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xvc.jqgfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bik.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://fol.redwolf501.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mpm.cashguo.top

================================================================================
来源：http://fhd.ydjk.org.cn

F. 文件与目录
来源：http://kjv.ywan-chungtsiang.top

================================================================================
来源：http://wzl.aibaodan.cn

[F01] 读取整个文件
来源：http://sfx.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://emo.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://bvb.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ncf.cucudq.cn


<!-- 参考信息 -->