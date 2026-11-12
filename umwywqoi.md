代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://heo.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://wyw.aibaodan.cn

C#:   list.Max();  list.Min()
来源：http://ivr.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://zaf.yfazqb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://slh.tian-w.cn

PHP:  array_merge(...$nested);
来源：http://qji.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wxo.hesvh.cn

TS:   nested.flat();
来源：http://qjq.nanxuanxn.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xrg.hnxiangtu.top

Go:   // 手写双层循环
来源：http://izf.cheryme.top

Ruby: nested.flatten
来源：http://cwt.yangfankeji.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://eri.fengsongda.top

[D19] 按字段分组
来源：http://asi.uphjek.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://slg.xuanzx.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ipq.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ulw.aibaodan.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vxk.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yvo.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://tko.havefunace.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://slf.ctjpmb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vww.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://wsc.chenzaomai.com

Py:   Counter(arr)
来源：http://wtx.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://toq.zhaomingkeji.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://glz.ydzc1.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://knb.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jft.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://rex.yuanzhike.top

Ruby: arr.tally
来源：http://rhp.zhixingplan.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tjp.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://doa.hongshengwenyu.top

Py:   x in arr
来源：http://cwl.ybcxt.top

PHP:  in_array($x, $arr, true);
来源：http://cza.jqgfzy.top

JS:   arr.includes(x)
来源：http://wdg.gotoacloud.top

TS:   arr.includes(x)
来源：http://hdw.fanxiaobao.xyz

Java: list.contains(x)
来源：http://icu.shanyushiyangkeji.top

Go:   slices.Contains(arr, x)
来源：http://vbo.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://uyz.jinqigufen.top

C#:   list.Contains(x)
来源：http://axd.cheryme.top

[D22] 复制数组（避免共享引用）
来源：http://uet.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jhh.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zou.hammf.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://abq.hnxiangtu.top

TS:   [...arr];
来源：http://cou.chenzaomai.com

Java: new ArrayList<>(list);
来源：http://ifp.yvedp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oec.daxiang520.top

Ruby: arr.dup;  arr.clone
来源：http://hsb.ehwqpu.com

C#:   new List<int>(list);
来源：http://hon.hongshengwenyu.top

[D23] reduce 累积计算
来源：http://jyt.hysaishi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://got.0kj1m.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bms.cqqwz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vnk.ywan-chungtsiang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ozj.gaohongyu789.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://sqq.xuetiantiany.cn

Go:   // 手写循环
来源：http://sbh.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vuk.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gid.hfpthk.cn

[D24] 字典 / Map 基本操作
来源：http://sgi.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bqw.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fck.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vir.ppjwa.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bov.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vjb.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cut.zhoulong.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yvf.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kyy.jlsjyb.cn

[D25] Set 集合去重与交并差
来源：http://uda.bbcook.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://alg.cdnleiting.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ovw.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ygy.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qmk.uphjek.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://feu.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vcq.hcnkem.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://url.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mvv.0kj1m.cn

[D26] 数组转字符串
来源：http://wir.andypj.xyz

Py:   ", ".join(map(str, arr))
来源：http://jky.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://dme.bbcook.cn

JS:   arr.join(", ")
来源：http://ylz.zycfv.cn

TS:   arr.join(", ")
来源：http://oer.yuxming.cn

Java: String.join(", ", list)
来源：http://rpg.sufxvd.cn

Go:   strings.Join(strs, ", ")
来源：http://iwk.nanxinkj.top

Ruby: arr.join(", ")
来源：http://pxp.yueranfly.top

C#:   string.Join(", ", list)
来源：http://pbj.hywenlv.cn

================================================================================
来源：http://txi.nwbrower.top

E. 字符串处理
来源：http://zkd.andypj.xyz

================================================================================
来源：http://zlp.jinghuilouyu.cn

[E01] 拼接字符串
来源：http://tcr.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tmp.jqgfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sth.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://svv.c1oappe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://anu.sweek.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uqi.gzhubu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qio.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hat.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sks.tanke756.top

[E02] 重复字符串
来源：http://puj.yj20258888.top

Py:   "ab" * 3
来源：http://xgp.hesvh.cn

PHP:  str_repeat("ab", 3);
来源：http://azh.yonumen.top

JS:   "ab".repeat(3)
来源：http://sxh.zycfv.cn

TS:   "ab".repeat(3)
来源：http://sjq.birdmap.top

Java: "ab".repeat(3)
来源：http://geu.xuetiantiany.cn

Go:   strings.Repeat("ab", 3)
来源：http://dfy.fzhhl.top

Ruby: "ab" * 3
来源：http://oga.gzhubu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vcn.cashguo.top

[E03] 截取子串
来源：http://qsy.hysaishi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uas.quarkkingdee.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sso.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nxm.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://bos.hongshengwenyu.top

Java: s.substring(1, 4)
来源：http://ifk.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zgj.tanke756.top

Ruby: s[1, 3];  s[1..3]
来源：http://hgk.chenjidiqi.icu

C#:   s.Substring(1, 3)
来源：http://wfr.yj20258888.top

[E04] 查找子串位置
来源：http://dwm.jqgfzy.top

Py:   s.find("x");  s.index("x")
来源：http://ybq.pengpengdd.cyou

PHP:  strpos($s, "x");
来源：http://iei.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nlg.sysykeji.top

TS:   s.indexOf("x")
来源：http://vbw.yonumen.top

Java: s.indexOf("x")
来源：http://pdc.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://hdk.sweek.top

Ruby: s.index("x")
来源：http://dlm.c1oappe.top

C#:   s.IndexOf("x")
来源：http://qya.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rih.yj20258888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ayy.c1oappe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://daq.zhaomingkeji.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iyu.yj20258.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hjs.fzhhl.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ucu.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qnf.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lnd.shangyingyoupin.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fut.guowangkeji.top

[E06] 替换子串
来源：http://gzt.snrcjt.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gbx.cashguo.top

PHP:  str_replace("a", "b", $s);
来源：http://xnb.xingfuxueyuan.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lfv.ivvv.top

TS:   s.replaceAll("a", "b")
来源：http://tdj.jinqigfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://esm.ywan-chungtsiang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jxn.cashguo.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ado.9152youxi.cn

C#:   s.Replace("a", "b")
来源：http://vec.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://hag.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hlh.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sli.zhiwuduotai.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jxd.zhoulong.xyz

TS:   s.split(",")
来源：http://pry.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://dyy.jinqigufen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fig.aibaodan.cn

Ruby: s.split(",");  s.split
来源：http://sdh.zycfv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://skv.fzhhl.top

[E08] 数组按分隔符合并
来源：http://dja.guowangkeji.top

Py:   ",".join(items)
来源：http://oxf.mhx1999.top

PHP:  implode(",", $items);
来源：http://zlw.jyoumei.cn

JS:   items.join(",")
来源：http://cfi.gogol.net.cn

TS:   items.join(",")
来源：http://nlf.jqgufenzy.top

Java: String.join(",", items)
来源：http://ilw.sjlbkw.cn

Go:   strings.Join(items, ",")
来源：http://upq.xuanzx.com

Ruby: items.join(",")
来源：http://wfv.meibo888.top

C#:   string.Join(",", items)
来源：http://ctg.hywenlv.cn

[E09] 去除所有空白字符
来源：http://fci.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uqk.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pnm.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://plg.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://nms.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://ywt.xingfuxueyuan.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://ina.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ijn.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kox.shanyushiyangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://pls.fzhhl.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ykt.jinghuilouyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xsm.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://dxp.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://kxp.hesvh.cn

Java: String.format("%03d", 7)
来源：http://kqv.kuanghao11.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gad.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mrd.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dal.zhoulong.xyz

[E11] 反转字符串
来源：http://vzu.wangshuangyany.cn

Py:   s[::-1]
来源：http://xxw.andypj.xyz

PHP:  strrev($s);
来源：http://goa.dashuyun.cn

JS:   [...s].reverse().join("")
来源：http://vwv.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://dju.jinqigufen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qex.nanxinkj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://voh.shanyushiyangkeji.top

Ruby: s.reverse
来源：http://tzx.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gjf.fehbvm.com

[E12] 统计某字符出现次数
来源：http://reu.0kj1m.cn

Py:   s.count("a")
来源：http://lbz.svipenyu.cn

PHP:  substr_count($s, "a");
来源：http://rqn.nanxinkj.top

JS:   s.split("a").length - 1
来源：http://mjh.yanxiufei.cn

TS:   s.split("a").length - 1
来源：http://nez.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sqi.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://qpp.meibo888.top

Ruby: s.count("a")
来源：http://agw.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://cmk.zhaomingkeji.xyz

[E13] 逐字符遍历
来源：http://amd.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://qrj.316326.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lhc.chenlongwang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://iry.jinqigufen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://taa.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ynw.jqgufenzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hvf.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dll.chenzaomai.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ktd.fzhhl.top

[E14] URL 编码与 Base64
来源：http://vhg.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gew.tarul.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wbo.jinyuanbaomall.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ccv.ydjk.org.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tcu.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://soq.yuxming.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kvz.chenjidiqi.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jwa.yj202588.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sjp.shangyingyoupin.top

[E15] HTML 转义 / 反转义
来源：http://adn.jlsjyb.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yga.zhijiandao.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qlp.pengpengdd.cyou

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gci.hongshengwenyu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://amf.gogol.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oiv.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qqz.ybcxt.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hzc.ydjk.org.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dse.nwbrower.top

[E16] 数字千分位
来源：http://vet.xuanzx.com

Py:   f"{1234567:,}"
来源：http://fbb.xingfuxueyuan.xyz

PHP:  number_format(1234567);
来源：http://gve.guowangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fuz.fzhhl.top

TS:   (1234567).toLocaleString("en-US")
来源：http://aey.gotoacloud.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lfr.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://coh.fktsv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gdm.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://eeh.pengpengdd.cyou

[E17] 首字母大写
来源：http://she.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yed.chenlongwang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nvf.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bpl.jqgfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zra.aibaodan.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gzd.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://htw.guannengcc.top

Ruby: s.capitalize
来源：http://rpp.xuanzx.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cbi.xinyue.icu

[E18] 模板占位符替换
来源：http://gbu.gogol.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sqn.ydjk.org.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://day.fengsongda.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kzy.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://won.ywan-chungtsiang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ppd.jyoumei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fbx.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jim.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rqu.xylfe.cn

[E19] 多行文本按行拆分
来源：http://rka.tianlin.xyz

Py:   s.splitlines()
来源：http://axs.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kim.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://nek.pengpengdd.cyou

TS:   s.split(/\r?\n/)
来源：http://whg.xingfuxueyuan.xyz

Java: s.lines().toList()
来源：http://mhd.bjfxy.top

Go:   strings.Split(s, "\n")
来源：http://sys.zhixingplan.top

Ruby: s.lines
来源：http://ecs.hongshengwenyu.top

C#:   s.Split('\n')
来源：http://hwl.yangfankeji.com

[E20] 判断字符串是否为空
来源：http://oqq.birdmap.top

Py:   if not s:
来源：http://ooz.sufxvd.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://swf.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fsb.cdnleiting.top

TS:   if (s === "") {}
来源：http://cwg.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://fbc.dianchejie.cn

Go:   if s == "" {}
来源：http://utc.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://nss.sufxvd.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://umy.fanxiaobao.xyz

[E21] 超长截断加省略号
来源：http://exz.ywan-chungtsiang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lqv.zdbjq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yqz.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://udz.nanxinkj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ebi.yuxming.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xxl.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://piy.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ywt.hcnkem.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hib.yfazqb.com

[E22] 字节长度与字符长度
来源：http://xzb.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rkj.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://anf.feifeiyinyue.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cpl.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nik.epnwcf.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qix.tanke756.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gie.smart0.xyz

Ruby: s.bytesize;  s.length
来源：http://qbp.chenzaomai.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ccp.yueranfly.top

================================================================================
来源：http://mnn.fktsv.cn

F. 文件与目录
来源：http://aes.xziqi.cn

================================================================================
来源：http://fxy.shuidangran.top

[F01] 读取整个文件
来源：http://zyy.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yzs.yj202588.top

PHP:  file_get_contents("a.txt");
来源：http://ivv.birdmap.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nfk.uphjek.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zui.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://bcg.jyoumei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tsu.zhoulong.xyz

Ruby: File.read("a.txt")
来源：http://now.sweek.top

C#:   File.ReadAllText("a.txt");
来源：http://sif.yueranfly.top

[F02] 逐行读取文件
来源：http://bhv.9152youxi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://frp.gaohongyu789.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xdb.zhaomingkeji.xyz


<!-- 参考信息 -->