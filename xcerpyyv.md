代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://ewh.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sup.fzhhl.top

TS:   Math.max(...arr);
来源：http://yoj.nwbrower.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gjw.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pza.zhoulong.xyz

Ruby: arr.max;  arr.min
来源：http://evo.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://onx.uphjek.com

[D18] 扁平化嵌套数组
来源：http://rod.fktsv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zns.yuxming.cn

PHP:  array_merge(...$nested);
来源：http://arc.hfpthk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mph.xziqi.cn

TS:   nested.flat();
来源：http://lyb.ybcxt.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dph.yj202588.top

Go:   // 手写双层循环
来源：http://kls.vqdsnc.cn

Ruby: nested.flatten
来源：http://wkt.xziqi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lfq.jinghuilouyu.cn

[D19] 按字段分组
来源：http://hzr.yfazqb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ajg.sysykeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oku.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uhb.jqgfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hqt.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rli.haohaochexian.top

Go:   // 手写 map[string][]T
来源：http://atc.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vsi.zhengqikj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fvy.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://sjl.shangyingyoupin.top

Py:   Counter(arr)
来源：http://jgw.hnqzz.top

PHP:  array_count_values($arr);
来源：http://ifx.hesvh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ups.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blr.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sde.ivvv.top

Go:   // 手写 map[T]int
来源：http://fjb.zdqjudy.top

Ruby: arr.tally
来源：http://lzn.yueranfly.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fkj.hcnkem.com

[D21] 判断是否包含某元素
来源：http://ovv.chenlongwang.top

Py:   x in arr
来源：http://hgy.zhiwuduotai.top

PHP:  in_array($x, $arr, true);
来源：http://rvy.ctjpmb.com

JS:   arr.includes(x)
来源：http://usz.cdnleiting.top

TS:   arr.includes(x)
来源：http://zlh.316326.xyz

Java: list.contains(x)
来源：http://epd.zhengqikj.top

Go:   slices.Contains(arr, x)
来源：http://wxs.smart0.xyz

Ruby: arr.include?(x)
来源：http://tsz.chenzaomai.com

C#:   list.Contains(x)
来源：http://ouo.cdnleiting.top

[D22] 复制数组（避免共享引用）
来源：http://jnv.uphjek.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ddz.redwolf501.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mfy.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nkn.zycfv.cn

TS:   [...arr];
来源：http://ayi.jinqigfzy.top

Java: new ArrayList<>(list);
来源：http://imk.fanxiaobao.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ceu.c1oappe.top

Ruby: arr.dup;  arr.clone
来源：http://ozg.nanxinkj.top

C#:   new List<int>(list);
来源：http://huo.mhx1999.top

[D23] reduce 累积计算
来源：http://ugq.yanxiufei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pov.kuanghao11.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vzy.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ymb.0kj1m.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bmf.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fsn.0kj1m.cn

Go:   // 手写循环
来源：http://dwf.zhongyouzk.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ztu.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rwv.jinyuanbaomall.cn

[D24] 字典 / Map 基本操作
来源：http://edk.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jex.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mxa.kuanghao11.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mfu.fengsongda.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://way.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bwx.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jxc.xuetiantiany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zij.sjlbkw.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://emw.redwolf501.top

[D25] Set 集合去重与交并差
来源：http://tap.jinqigfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bpv.chenzaomai.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xbe.daxiang520.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nbh.c1oappe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://szg.zhijiandao.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vvl.xziqi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tif.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vwg.uphjek.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mxk.zhiwuduotai.top

[D26] 数组转字符串
来源：http://edk.ybcxt.top

Py:   ", ".join(map(str, arr))
来源：http://jmx.vehdjk.com

PHP:  implode(", ", $arr);
来源：http://gkn.ydzc1.top

JS:   arr.join(", ")
来源：http://qce.fktsv.cn

TS:   arr.join(", ")
来源：http://nkw.nanxinkj.top

Java: String.join(", ", list)
来源：http://zck.hcnkem.com

Go:   strings.Join(strs, ", ")
来源：http://wzw.yonumen.top

Ruby: arr.join(", ")
来源：http://lif.zhixingplan.top

C#:   string.Join(", ", list)
来源：http://ief.jianghu66.top

================================================================================
来源：http://elo.ywan-chungtsiang.top

E. 字符串处理
来源：http://lfq.ehwqpu.com

================================================================================
来源：http://avx.chenlongwang.top

[E01] 拼接字符串
来源：http://pha.tanke756.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tob.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zte.pengpengdd.cyou

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lup.pengpengdd.cyou

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eor.sufxvd.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ozr.316326.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sjz.zhijiandao.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://noq.quarkkingdee.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pnr.snrcjt.cn

[E02] 重复字符串
来源：http://khf.jqgufenzy.top

Py:   "ab" * 3
来源：http://qxe.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://bre.fehbvm.com

JS:   "ab".repeat(3)
来源：http://lzi.sjlbkw.cn

TS:   "ab".repeat(3)
来源：http://ymk.yuanzhike.top

Java: "ab".repeat(3)
来源：http://wqk.jinqigufen.top

Go:   strings.Repeat("ab", 3)
来源：http://dzb.316326.xyz

Ruby: "ab" * 3
来源：http://jxk.sweek.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gih.kuanghao11.cn

[E03] 截取子串
来源：http://oyx.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cko.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yok.fanxiaobao.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://efr.jqgfzy.top

TS:   s.slice(1, 4)
来源：http://naf.shuidangran.top

Java: s.substring(1, 4)
来源：http://too.ivvv.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://irz.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://soi.shuidangran.top

C#:   s.Substring(1, 3)
来源：http://bxv.wangshuangyany.cn

[E04] 查找子串位置
来源：http://rqj.iojbl.cn

Py:   s.find("x");  s.index("x")
来源：http://fqh.vqdsnc.cn

PHP:  strpos($s, "x");
来源：http://jzc.svipenyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dtv.pycfn.com

TS:   s.indexOf("x")
来源：http://tuj.ywan-chungtsiang.top

Java: s.indexOf("x")
来源：http://lbi.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://bza.tarul.cn

Ruby: s.index("x")
来源：http://dua.uphjek.com

C#:   s.IndexOf("x")
来源：http://wia.dianchejie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xlb.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rgc.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hdm.hfpthk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://koy.svipenyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ivo.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gjb.yj20258888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gbu.jyoumei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ias.hcnkem.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://smn.haohaochexian.top

[E06] 替换子串
来源：http://saj.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lem.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://otf.hnxiangtu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ycj.daria6918.cn

TS:   s.replaceAll("a", "b")
来源：http://elx.jqgufenzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jcb.cdnleiting.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vrr.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gwm.aizwys.cn

C#:   s.Replace("a", "b")
来源：http://zcq.jinqigufen.top

[E07] 按分隔符拆分
来源：http://jdr.birdmap.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ajg.vqdsnc.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lee.vehdjk.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://bxf.hcnkem.com

TS:   s.split(",")
来源：http://qhx.jlsjyb.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mkz.yanxiufei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ega.sysykeji.top

Ruby: s.split(",");  s.split
来源：http://qrb.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://las.fzhhl.top

[E08] 数组按分隔符合并
来源：http://mwq.dashuyun.cn

Py:   ",".join(items)
来源：http://kyi.chenzaomai.com

PHP:  implode(",", $items);
来源：http://lor.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://vmn.yueranfly.top

TS:   items.join(",")
来源：http://tei.sxryk.cn

Java: String.join(",", items)
来源：http://lol.yanxiufei.cn

Go:   strings.Join(items, ",")
来源：http://xdd.pycfn.com

Ruby: items.join(",")
来源：http://vfk.chenlongwang.top

C#:   string.Join(",", items)
来源：http://afm.xuanzx.com

[E09] 去除所有空白字符
来源：http://iop.uphjek.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ubv.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vnh.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://mtt.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://ybk.c1oappe.top

Java: s.replaceAll("\\s+", "")
来源：http://jfm.xinyue.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://aps.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://phz.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gjb.ivvv.top

[E10] 左侧补零 / 定长填充
来源：http://hbg.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bvp.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tsl.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://yyv.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://lcb.redwolf501.top

Java: String.format("%03d", 7)
来源：http://fzc.ivvv.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qzf.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vff.mhx1999.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nub.chenlongwang.top

[E11] 反转字符串
来源：http://tec.daria6918.cn

Py:   s[::-1]
来源：http://lpt.xuetiantiany.cn

PHP:  strrev($s);
来源：http://xkh.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://jie.nanxinkj.top

TS:   [...s].reverse().join("")
来源：http://evb.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://eyw.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hpd.jianghu66.top

Ruby: s.reverse
来源：http://mgx.feifeiyinyue.top

C#:   new string(s.Reverse().ToArray())
来源：http://row.fzhhl.top

[E12] 统计某字符出现次数
来源：http://mvh.ybcxt.top

Py:   s.count("a")
来源：http://wpf.zhengqikj.top

PHP:  substr_count($s, "a");
来源：http://ikr.yuxming.cn

JS:   s.split("a").length - 1
来源：http://bsn.hammf.cn

TS:   s.split("a").length - 1
来源：http://eus.zhiwuduotai.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tzi.ivvv.top

Go:   strings.Count(s, "a")
来源：http://xir.daria6918.cn

Ruby: s.count("a")
来源：http://aer.ywan-chungtsiang.top

C#:   s.Count(c => c == 'a')
来源：http://dio.yonumen.top

[E13] 逐字符遍历
来源：http://xyz.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://fej.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ycc.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ydf.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://taf.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ico.jqgufenzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hlx.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zco.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pfq.cqqwz.cn

[E14] URL 编码与 Base64
来源：http://xiw.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tvq.ehwqpu.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://sqr.hfpthk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://awz.svipenyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ipy.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://enf.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://twv.jiagoushi.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ugc.zdqjudy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rqh.gzhubu.top

[E15] HTML 转义 / 反转义
来源：http://khf.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mtt.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qev.tian-w.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qpw.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tjo.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rly.daria6918.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yhb.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eic.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dlh.zhongyouzk.top

[E16] 数字千分位
来源：http://cpl.smart0.xyz

Py:   f"{1234567:,}"
来源：http://hfu.iojbl.cn

PHP:  number_format(1234567);
来源：http://rum.sxryk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hbz.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://cgl.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://umy.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tor.hammf.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ezb.hongshengwenyu.top

C#:   1234567.ToString("N0")
来源：http://gxq.yonumen.top

[E17] 首字母大写
来源：http://suk.feifeiyinyue.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aho.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://zuw.feifeiyinyue.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bfm.andypj.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jzr.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tkg.jinqigfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nvu.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://rbh.uphjek.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gsg.c1oappe.top

[E18] 模板占位符替换
来源：http://iqe.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://svy.yanxiufei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qdd.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://xst.xingfuxueyuan.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://djl.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gfm.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oim.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jra.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wic.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://wwa.svipenyu.cn

Py:   s.splitlines()
来源：http://pha.jqgufenzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ffi.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://lmb.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://wye.hongshengwenyu.top

Java: s.lines().toList()
来源：http://gfl.cashguo.top

Go:   strings.Split(s, "\n")
来源：http://hqn.9152youxi.cn

Ruby: s.lines
来源：http://siz.shangyingyoupin.top

C#:   s.Split('\n')
来源：http://cyt.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://bvj.jinghuilouyu.cn

Py:   if not s:
来源：http://kjp.sweek.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://veh.fktsv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rdh.cqqwz.cn

TS:   if (s === "") {}
来源：http://pmt.shanyushiyangtech.top

Java: if (s.isEmpty()) {}
来源：http://pgu.hesvh.cn

Go:   if s == "" {}
来源：http://ayu.fengsongda.top

Ruby: if s.empty?
来源：http://fac.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://byr.xinyue.icu

[E21] 超长截断加省略号
来源：http://znj.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dwb.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sqy.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gbg.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lub.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://szg.yangfankeji.com

Go:   // 按 rune 判断长度后截断
来源：http://kyj.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hep.ydjk.org.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lfv.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://zpz.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gvc.jqgufenzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xmb.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xvv.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wxy.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ttc.cashguo.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mcd.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://kuj.chenlongwang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kfm.wangshuangyany.cn

================================================================================
来源：http://ytd.shuidangran.top

F. 文件与目录
来源：http://xtk.zdqjudy.top

================================================================================
来源：http://fcd.cqqwz.cn

[F01] 读取整个文件
来源：http://tez.fzhhl.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://onk.xinyue.icu

PHP:  file_get_contents("a.txt");
来源：http://ekk.zhijiandao.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tfz.yj20258888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lwj.shanyushiyangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mvn.c1oappe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://krc.uphjek.com

Ruby: File.read("a.txt")
来源：http://gva.xingfuxueyuan.xyz


<!-- 参考信息 -->