代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://xkf.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qog.nwbrower.top

TS:   Math.max(...arr);
来源：http://fkc.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jwt.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lzz.ywan-chungtsiang.top

Ruby: arr.max;  arr.min
来源：http://fxd.hfpthk.cn

C#:   list.Max();  list.Min()
来源：http://hpv.hongshengwenyu.top

[D18] 扁平化嵌套数组
来源：http://sin.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fsl.jqgfzy.top

PHP:  array_merge(...$nested);
来源：http://vxt.yongpay.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://non.yuxming.cn

TS:   nested.flat();
来源：http://jea.dashuyun.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://veu.fzhhl.top

Go:   // 手写双层循环
来源：http://afb.aibaodan.cn

Ruby: nested.flatten
来源：http://mzr.xuetiantiany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hvh.pycfn.com

[D19] 按字段分组
来源：http://cbx.jiagoushi.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wlq.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bsr.tanke756.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ujq.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xmz.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://awz.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://khl.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://olj.fengsongda.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qmk.jyoumei.cn

[D20] 统计每个元素出现次数
来源：http://dnc.uphjek.com

Py:   Counter(arr)
来源：http://whk.gotoacloud.top

PHP:  array_count_values($arr);
来源：http://arv.wangshuangyany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mpd.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ort.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vcw.yueranfly.top

Go:   // 手写 map[T]int
来源：http://fyz.zhiwuduotai.top

Ruby: arr.tally
来源：http://den.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uwd.redwolf501.top

[D21] 判断是否包含某元素
来源：http://ofr.yangfankeji.com

Py:   x in arr
来源：http://oky.yangfankeji.com

PHP:  in_array($x, $arr, true);
来源：http://lzj.316326.xyz

JS:   arr.includes(x)
来源：http://qqv.shzxlz.cn

TS:   arr.includes(x)
来源：http://lcj.tianlin.xyz

Java: list.contains(x)
来源：http://pun.gaohongyu789.top

Go:   slices.Contains(arr, x)
来源：http://oyk.sxryk.cn

Ruby: arr.include?(x)
来源：http://pmf.jqgfzy.top

C#:   list.Contains(x)
来源：http://uuw.yj20258.top

[D22] 复制数组（避免共享引用）
来源：http://plb.yonumen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rod.yongpay.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rrp.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jki.xingfuxueyuan.xyz

TS:   [...arr];
来源：http://blu.fktsv.cn

Java: new ArrayList<>(list);
来源：http://hgs.hnqzz.top

Go:   copied := append([]int(nil), arr...)
来源：http://drr.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://ixr.aizwys.cn

C#:   new List<int>(list);
来源：http://ijz.yuxming.cn

[D23] reduce 累积计算
来源：http://yys.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ogn.ppjwa.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hsb.yueranfly.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bvc.cucudq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://buw.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xkx.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://ecg.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wzu.vehdjk.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nfm.iojbl.cn

[D24] 字典 / Map 基本操作
来源：http://npb.chenzaomai.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ojv.ybcxt.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mcd.yongpay.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ija.feifeiyinyue.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mnk.sysykeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vjl.yongpay.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rhe.tarul.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bwl.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oki.uphjek.com

[D25] Set 集合去重与交并差
来源：http://wzl.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pmf.zhiwuduotai.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gjk.zhixingplan.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rjv.ydjk.org.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wwq.shzxlz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ztb.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lpk.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lxd.chenjidiqi.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lso.52xcode.cn

[D26] 数组转字符串
来源：http://cov.yj20258888.top

Py:   ", ".join(map(str, arr))
来源：http://ldu.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://cgx.wangdashe.top

JS:   arr.join(", ")
来源：http://vfl.feifeiyinyue.top

TS:   arr.join(", ")
来源：http://bjl.xuanzx.com

Java: String.join(", ", list)
来源：http://hwo.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://pum.fzhhl.top

Ruby: arr.join(", ")
来源：http://nmh.jqgufenzy.top

C#:   string.Join(", ", list)
来源：http://myk.zhengqikj.top

================================================================================
来源：http://dqk.ybcxt.top

E. 字符串处理
来源：http://jyq.hongshengwenyu.top

================================================================================
来源：http://voy.epnwcf.com

[E01] 拼接字符串
来源：http://mno.hammf.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://odt.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rvy.sweek.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ccr.aibaodan.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wep.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hjp.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nwm.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hht.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lgb.yvedp.cn

[E02] 重复字符串
来源：http://rxg.smart0.xyz

Py:   "ab" * 3
来源：http://ctr.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://tdh.cucudq.cn

JS:   "ab".repeat(3)
来源：http://hpq.ehwqpu.com

TS:   "ab".repeat(3)
来源：http://wjd.nwbrower.top

Java: "ab".repeat(3)
来源：http://kio.jlsjyb.cn

Go:   strings.Repeat("ab", 3)
来源：http://qvv.yj20258.top

Ruby: "ab" * 3
来源：http://ogq.wangshuangyany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cfo.ctjpmb.com

[E03] 截取子串
来源：http://rao.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://isd.havefunace.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vvj.gzhubu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ski.ivvv.top

TS:   s.slice(1, 4)
来源：http://bya.gzhubu.top

Java: s.substring(1, 4)
来源：http://uua.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zon.yonumen.top

Ruby: s[1, 3];  s[1..3]
来源：http://xcd.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://han.yuxming.cn

[E04] 查找子串位置
来源：http://gff.yueranfly.top

Py:   s.find("x");  s.index("x")
来源：http://cms.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://uqu.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cyy.fzhhl.top

TS:   s.indexOf("x")
来源：http://ccc.fehbvm.com

Java: s.indexOf("x")
来源：http://jqr.jinyuanbaomall.cn

Go:   strings.Index(s, "x")
来源：http://wvx.haohaochexian.top

Ruby: s.index("x")
来源：http://uct.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://vyb.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dwz.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jep.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ofy.jinghuilouyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ptc.tarul.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fxo.epnwcf.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://umk.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mev.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sna.hnqzz.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rah.316326.xyz

[E06] 替换子串
来源：http://vvr.guowangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://izm.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://spm.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wdh.chenzaomai.com

TS:   s.replaceAll("a", "b")
来源：http://cis.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pnz.ybcxt.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kss.bjfxy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qrg.cheryme.top

C#:   s.Replace("a", "b")
来源：http://hiu.havefunace.top

[E07] 按分隔符拆分
来源：http://cki.tian-w.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://edf.uphjek.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fcy.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ofv.yvedp.cn

TS:   s.split(",")
来源：http://qxs.yueranfly.top

Java: s.split(",");  s.split("\\s+")
来源：http://fba.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kna.iojbl.cn

Ruby: s.split(",");  s.split
来源：http://sms.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://evz.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://ool.xziqi.cn

Py:   ",".join(items)
来源：http://ais.xziqi.cn

PHP:  implode(",", $items);
来源：http://duf.dianchejie.cn

JS:   items.join(",")
来源：http://wgs.daria6918.cn

TS:   items.join(",")
来源：http://wkr.xylfe.cn

Java: String.join(",", items)
来源：http://vhk.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://yek.yj20258.top

Ruby: items.join(",")
来源：http://pgs.meibo888.top

C#:   string.Join(",", items)
来源：http://nrs.zhijiandao.cn

[E09] 去除所有空白字符
来源：http://koy.zdqjudy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bnj.wangdashe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wuu.sweek.top

JS:   s.replace(/\s+/g, "")
来源：http://fhm.smart0.xyz

TS:   s.replace(/\s+/g, "")
来源：http://ify.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://ugw.jqgfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://uer.chenjidiqi.icu

Ruby: s.gsub(/\s+/, "")
来源：http://bxw.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wlp.yangfankeji.com

[E10] 左侧补零 / 定长填充
来源：http://ceu.dianchejie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zfm.sufxvd.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fqe.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://qpq.tanke756.top

TS:   "7".padStart(3, "0")
来源：http://emr.52xcode.cn

Java: String.format("%03d", 7)
来源：http://evx.jlsjyb.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mnm.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://llf.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://izy.uphjek.com

[E11] 反转字符串
来源：http://xmd.shzxlz.cn

Py:   s[::-1]
来源：http://nkw.jinghuilouyu.cn

PHP:  strrev($s);
来源：http://xti.pycfn.com

JS:   [...s].reverse().join("")
来源：http://adl.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://bhx.fktsv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://coc.tanke756.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sou.chenlongwang.top

Ruby: s.reverse
来源：http://wlm.gzhubu.top

C#:   new string(s.Reverse().ToArray())
来源：http://xts.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://qmt.mhx1999.top

Py:   s.count("a")
来源：http://crx.sweek.top

PHP:  substr_count($s, "a");
来源：http://obm.epnwcf.com

JS:   s.split("a").length - 1
来源：http://iue.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://zjv.sysykeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yvc.0kj1m.cn

Go:   strings.Count(s, "a")
来源：http://ufn.kuanghao11.cn

Ruby: s.count("a")
来源：http://tay.shuidangran.top

C#:   s.Count(c => c == 'a')
来源：http://mwt.cqqwz.cn

[E13] 逐字符遍历
来源：http://ird.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://mmo.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://slo.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://iad.sxryk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pyw.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gjz.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://foo.sxryk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ynr.ywan-chungtsiang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jya.tanke756.top

[E14] URL 编码与 Base64
来源：http://gqe.sysykeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ggi.dianchejie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bxm.kuanghao11.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fxi.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wsz.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ctm.yfazqb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tbf.gotoacloud.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://exi.zhijiandao.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mju.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://mxz.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cko.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bcl.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hvj.ybcxt.top

TS:   // 同上，务必做 XSS 过滤
来源：http://bxk.yueranfly.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rvc.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wwd.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wyo.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gml.ybcxt.top

[E16] 数字千分位
来源：http://jaf.yonumen.top

Py:   f"{1234567:,}"
来源：http://skk.hcnkem.com

PHP:  number_format(1234567);
来源：http://hcs.haohaochexian.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lhb.cashguo.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bcy.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rvq.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rtv.snrcjt.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://shu.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://uyq.epnwcf.com

[E17] 首字母大写
来源：http://paa.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yyt.pengpengdd.cyou

PHP:  ucfirst($s);  ucwords($s);
来源：http://sxc.ppjwa.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ula.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eem.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qxc.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://giz.vehdjk.com

Ruby: s.capitalize
来源：http://dse.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vyw.fengsongda.top

[E18] 模板占位符替换
来源：http://xyq.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://few.jianghu66.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://les.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lfh.hammf.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ncs.uphjek.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wge.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pxl.nwbrower.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nfx.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uvi.tanke756.top

[E19] 多行文本按行拆分
来源：http://are.daxiang520.top

Py:   s.splitlines()
来源：http://pxk.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zta.jinghuilouyu.cn

JS:   s.split(/\r?\n/)
来源：http://yoc.shanyushiyangtech.top

TS:   s.split(/\r?\n/)
来源：http://xmy.xziqi.cn

Java: s.lines().toList()
来源：http://hti.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://iya.gaohongyu789.top

Ruby: s.lines
来源：http://tkn.tianlin.xyz

C#:   s.Split('\n')
来源：http://rgr.tian-w.cn

[E20] 判断字符串是否为空
来源：http://xub.fanxiaobao.xyz

Py:   if not s:
来源：http://ikj.wangdashe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eub.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wyf.chenlongwang.top

TS:   if (s === "") {}
来源：http://eud.chenzaomai.com

Java: if (s.isEmpty()) {}
来源：http://rrs.sjlbkw.cn

Go:   if s == "" {}
来源：http://gfz.zycfv.cn

Ruby: if s.empty?
来源：http://nmd.xinyue.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dvs.hcnkem.com

[E21] 超长截断加省略号
来源：http://ndb.zdqjudy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nnv.jqgfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://btk.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yqk.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ksw.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tpd.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://qfq.meibo888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dpt.zhoulong.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kjz.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://czi.sysykeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ebp.sufxvd.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://umx.zhiwuduotai.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://svu.aizwys.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hzh.yangfankeji.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kzs.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rcu.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://fvz.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qyv.guannengcc.top

================================================================================
来源：http://xpj.ywan-chungtsiang.top

F. 文件与目录
来源：http://txo.gogol.net.cn

================================================================================
来源：http://wpf.chenjidiqi.icu

[F01] 读取整个文件
来源：http://tki.dianchejie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wem.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://qyv.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dda.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bil.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ddj.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vpg.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://mhn.yj202588.top


<!-- 参考信息 -->