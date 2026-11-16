代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kbi.zhiwuduotai.top

PHP:  array_merge(...$nested);
来源：http://chd.yj202588.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dnd.ydzc1.top

TS:   nested.flat();
来源：http://ukg.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yze.xingfuxueyuan.xyz

Go:   // 手写双层循环
来源：http://cuv.jqgfzy.top

Ruby: nested.flatten
来源：http://cxt.gotoacloud.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zoq.ywan-chungtsiang.top

[D19] 按字段分组
来源：http://mjc.jinqigufen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cad.guannengcc.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gtu.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://krf.vqdsnc.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://agv.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hmm.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://qey.xziqi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jqp.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mwp.dianchejie.cn

[D20] 统计每个元素出现次数
来源：http://ldq.guannengcc.top

Py:   Counter(arr)
来源：http://lxr.ivvv.top

PHP:  array_count_values($arr);
来源：http://ynz.yvedp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hej.wangdashe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hwp.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://abv.yangfankeji.com

Go:   // 手写 map[T]int
来源：http://ihp.tianlin.xyz

Ruby: arr.tally
来源：http://ibj.hywenlv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qel.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://wqc.wangdashe.top

Py:   x in arr
来源：http://wvh.meibo888.top

PHP:  in_array($x, $arr, true);
来源：http://yrr.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://ywt.shuidangran.top

TS:   arr.includes(x)
来源：http://oxn.epnwcf.com

Java: list.contains(x)
来源：http://eyz.xylfe.cn

Go:   slices.Contains(arr, x)
来源：http://ihz.chenlongwang.top

Ruby: arr.include?(x)
来源：http://gvt.quarkkingdee.top

C#:   list.Contains(x)
来源：http://rxa.jinghuilouyu.cn

[D22] 复制数组（避免共享引用）
来源：http://ixz.gzhubu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cir.bjfxy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xra.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://edo.snrcjt.cn

TS:   [...arr];
来源：http://xsw.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://kxb.sjlbkw.cn

Go:   copied := append([]int(nil), arr...)
来源：http://drp.zdqjudy.top

Ruby: arr.dup;  arr.clone
来源：http://ajx.zdbjq.cn

C#:   new List<int>(list);
来源：http://suz.ppjwa.cn

[D23] reduce 累积计算
来源：http://qqu.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ftv.wangshuangyany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zmk.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vje.ywan-chungtsiang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uso.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://rxo.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://lrw.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uqu.yangfankeji.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gra.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://lpz.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://coq.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://okz.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fcx.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nak.yanxiufei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ldl.ywan-chungtsiang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rkf.jianghu66.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nbt.nanxinkj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iwn.mhx1999.top

[D25] Set 集合去重与交并差
来源：http://ekt.ppjwa.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cpl.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ldn.ehwqpu.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bls.fzhhl.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wzg.haohaochexian.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dnt.hesvh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gwf.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ede.yvedp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zlp.shuidangran.top

[D26] 数组转字符串
来源：http://qsh.dianchejie.cn

Py:   ", ".join(map(str, arr))
来源：http://qrm.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://rvx.fengsongda.top

JS:   arr.join(", ")
来源：http://vtn.yj20258888.top

TS:   arr.join(", ")
来源：http://rju.ctjpmb.com

Java: String.join(", ", list)
来源：http://egi.smart0.xyz

Go:   strings.Join(strs, ", ")
来源：http://drk.jinghuilouyu.cn

Ruby: arr.join(", ")
来源：http://dpi.fktsv.cn

C#:   string.Join(", ", list)
来源：http://dln.xinyue.icu

================================================================================
来源：http://ztc.jyoumei.cn

E. 字符串处理
来源：http://xyy.cucudq.cn

================================================================================
来源：http://qqo.yj202588.top

[E01] 拼接字符串
来源：http://sye.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ohg.zycfv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ive.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ywh.feifeiyinyue.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kcs.birdmap.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zrp.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rlb.pycfn.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sfb.cucudq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ixz.daria6918.cn

[E02] 重复字符串
来源：http://jjc.shangyingyoupin.top

Py:   "ab" * 3
来源：http://mos.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://jic.zhengqikj.top

JS:   "ab".repeat(3)
来源：http://ndh.ctjpmb.com

TS:   "ab".repeat(3)
来源：http://hhz.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://ggc.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://skx.sjlbkw.cn

Ruby: "ab" * 3
来源：http://ezk.uphjek.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yjo.ctjpmb.com

[E03] 截取子串
来源：http://eli.xylfe.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hgl.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://owv.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iju.pycfn.com

TS:   s.slice(1, 4)
来源：http://ijb.zdbjq.cn

Java: s.substring(1, 4)
来源：http://dmg.chenzaomai.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rxz.fzhhl.top

Ruby: s[1, 3];  s[1..3]
来源：http://wlw.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://phe.jianghu66.top

[E04] 查找子串位置
来源：http://igx.chenjidiqi.icu

Py:   s.find("x");  s.index("x")
来源：http://dxj.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://udd.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jve.andypj.xyz

TS:   s.indexOf("x")
来源：http://dbo.ivvv.top

Java: s.indexOf("x")
来源：http://wvq.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://hee.yfazqb.com

Ruby: s.index("x")
来源：http://gzw.mhx1999.top

C#:   s.IndexOf("x")
来源：http://fym.zdqjudy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yjo.aizwys.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qaj.yonumen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kqi.shangyingyoupin.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wwd.jinyuanbaomall.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lwa.wangdashe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kvh.hywenlv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://din.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gnb.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cob.havefunace.top

[E06] 替换子串
来源：http://twm.xuetiantiany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sud.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://nvo.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bus.tanke756.top

TS:   s.replaceAll("a", "b")
来源：http://efs.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qmf.zhijiandao.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cba.xuetiantiany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://omj.uphjek.com

C#:   s.Replace("a", "b")
来源：http://lde.nwbrower.top

[E07] 按分隔符拆分
来源：http://fjc.316326.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gqi.zdbjq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ebl.gotoacloud.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ymg.ctjpmb.com

TS:   s.split(",")
来源：http://yal.xuanzx.com

Java: s.split(",");  s.split("\\s+")
来源：http://bnh.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cys.havefunace.top

Ruby: s.split(",");  s.split
来源：http://ila.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uli.chenjidiqi.icu

[E08] 数组按分隔符合并
来源：http://vyy.jqgfzy.top

Py:   ",".join(items)
来源：http://pyn.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://qso.tian-w.cn

JS:   items.join(",")
来源：http://fdt.fehbvm.com

TS:   items.join(",")
来源：http://agj.zhiwuduotai.top

Java: String.join(",", items)
来源：http://qgv.shanyushiyangtech.top

Go:   strings.Join(items, ",")
来源：http://mgm.hammf.cn

Ruby: items.join(",")
来源：http://tmt.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://jen.sysykeji.top

[E09] 去除所有空白字符
来源：http://amx.zhixingplan.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://glm.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hyk.c1oappe.top

JS:   s.replace(/\s+/g, "")
来源：http://dyp.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://god.yangfankeji.com

Java: s.replaceAll("\\s+", "")
来源：http://ndo.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://mpz.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://gna.jianghu66.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zfn.fengsongda.top

[E10] 左侧补零 / 定长填充
来源：http://mmb.snrcjt.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zrl.chenlongwang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cyh.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://dee.sysykeji.top

TS:   "7".padStart(3, "0")
来源：http://rmt.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://wjy.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ytf.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nlf.jqgfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yhe.zhijiandao.cn

[E11] 反转字符串
来源：http://mkw.jinqigufen.top

Py:   s[::-1]
来源：http://eex.haohaochexian.top

PHP:  strrev($s);
来源：http://bwf.dianchejie.cn

JS:   [...s].reverse().join("")
来源：http://uum.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://lqc.zhaomingkeji.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://gkj.ydzc1.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ezs.316326.xyz

Ruby: s.reverse
来源：http://vum.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://zdo.hnqzz.top

[E12] 统计某字符出现次数
来源：http://hfo.ydzc1.top

Py:   s.count("a")
来源：http://ejf.tarul.cn

PHP:  substr_count($s, "a");
来源：http://zpa.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://psg.yfazqb.com

TS:   s.split("a").length - 1
来源：http://den.yanxiufei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://keb.tian-w.cn

Go:   strings.Count(s, "a")
来源：http://pls.tian-w.cn

Ruby: s.count("a")
来源：http://ieg.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://ddr.hysaishi.cn

[E13] 逐字符遍历
来源：http://feo.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://cwd.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ery.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://crj.hfpthk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://din.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lji.shanyushiyangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rvi.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ojr.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ujy.zhixingplan.top

[E14] URL 编码与 Base64
来源：http://hdw.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ovr.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pca.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://itc.zycfv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://liu.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://seo.smart0.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hpe.hammf.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xwk.vqdsnc.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wza.sufxvd.cn

[E15] HTML 转义 / 反转义
来源：http://tjb.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cgj.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hik.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hpd.9152youxi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zuu.c1oappe.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hkb.mhx1999.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wuu.jyoumei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zjs.wangshuangyany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://efa.cdnleiting.top

[E16] 数字千分位
来源：http://vtr.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://wkg.hfpthk.cn

PHP:  number_format(1234567);
来源：http://lje.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://qra.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://djb.gogol.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bza.jianghu66.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tdj.ehwqpu.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bbg.fengsongda.top

C#:   1234567.ToString("N0")
来源：http://gxn.tian-w.cn

[E17] 首字母大写
来源：http://ale.hcnkem.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mrk.fehbvm.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://cio.ehwqpu.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dsg.ydjk.org.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jbr.aibaodan.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jzs.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yqa.chenzaomai.com

Ruby: s.capitalize
来源：http://rie.ppjwa.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kbc.52xcode.cn

[E18] 模板占位符替换
来源：http://zqb.xziqi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mkv.cqqwz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ptc.xuanzx.com

JS:   tpl.replaceAll("{name}", name)
来源：http://ogx.tian-w.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xwl.ctjpmb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://odl.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zcq.jlsjyb.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://grc.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wny.tarul.cn

[E19] 多行文本按行拆分
来源：http://lkw.xingfuxueyuan.xyz

Py:   s.splitlines()
来源：http://aea.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cpn.yuanzhike.top

JS:   s.split(/\r?\n/)
来源：http://gvk.birdmap.top

TS:   s.split(/\r?\n/)
来源：http://psp.guannengcc.top

Java: s.lines().toList()
来源：http://mfh.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://cfe.fktsv.cn

Ruby: s.lines
来源：http://nid.guowangkeji.top

C#:   s.Split('\n')
来源：http://hcd.zycfv.cn

[E20] 判断字符串是否为空
来源：http://vxf.tian-w.cn

Py:   if not s:
来源：http://gbh.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://par.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ypt.gotoacloud.top

TS:   if (s === "") {}
来源：http://xup.hnxiangtu.top

Java: if (s.isEmpty()) {}
来源：http://pxm.sysykeji.top

Go:   if s == "" {}
来源：http://opf.gzhubu.top

Ruby: if s.empty?
来源：http://qzq.zhoulong.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vbu.hammf.cn

[E21] 超长截断加省略号
来源：http://cty.cheryme.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://isi.yvedp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wii.zycfv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vij.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ala.hammf.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://inc.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://kgj.shanyushiyangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://btt.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lkl.gogol.net.cn

[E22] 字节长度与字符长度
来源：http://guh.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vww.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ceo.ivvv.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ckn.wangshuangyany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rtp.cucudq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pgz.sysykeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://irl.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://emd.jqgfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ofh.jinqigfzy.top

================================================================================
来源：http://ouh.yj202588.top

F. 文件与目录
来源：http://fou.jiagoushi.top

================================================================================
来源：http://ixp.zycfv.cn

[F01] 读取整个文件
来源：http://zct.cdnleiting.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://civ.ydzc1.top

PHP:  file_get_contents("a.txt");
来源：http://kwx.c1oappe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qbv.hywenlv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nhm.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://akt.aizwys.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oev.ydjk.org.cn

Ruby: File.read("a.txt")
来源：http://krt.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://zri.shanyushiyangkeji.top

[F02] 逐行读取文件
来源：http://cip.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pfg.jqgufenzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hzv.hnqzz.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://axu.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wps.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xpx.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://glv.zhoulong.xyz


<!-- 参考信息 -->