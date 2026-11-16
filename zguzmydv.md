代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tiw.kuanghao11.cn

Ruby: arr.max;  arr.min
来源：http://ake.jinqigufen.top

C#:   list.Max();  list.Min()
来源：http://kfu.zhijiandao.cn

[D18] 扁平化嵌套数组
来源：http://gvp.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zqo.havefunace.top

PHP:  array_merge(...$nested);
来源：http://dph.zhixingplan.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gxr.daria6918.cn

TS:   nested.flat();
来源：http://idu.ybcxt.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kik.quarkkingdee.top

Go:   // 手写双层循环
来源：http://hvt.sxryk.cn

Ruby: nested.flatten
来源：http://gqn.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bxh.guowangkeji.top

[D19] 按字段分组
来源：http://eqo.guannengcc.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wto.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://una.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nce.andypj.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://zsv.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tlt.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://rhs.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yxu.haohaochexian.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ddx.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://msv.svipenyu.cn

Py:   Counter(arr)
来源：http://sgs.fengsongda.top

PHP:  array_count_values($arr);
来源：http://jts.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ult.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oui.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dqv.daxiang520.top

Go:   // 手写 map[T]int
来源：http://srp.sxryk.cn

Ruby: arr.tally
来源：http://wfn.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dxp.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://bsk.316326.xyz

Py:   x in arr
来源：http://nry.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://hdv.ctjpmb.com

JS:   arr.includes(x)
来源：http://rjo.ydzc1.top

TS:   arr.includes(x)
来源：http://eux.shanyushiyangkeji.top

Java: list.contains(x)
来源：http://cjr.zdqjudy.top

Go:   slices.Contains(arr, x)
来源：http://akh.sysykeji.top

Ruby: arr.include?(x)
来源：http://eoa.chenlongwang.top

C#:   list.Contains(x)
来源：http://yxf.xziqi.cn

[D22] 复制数组（避免共享引用）
来源：http://fox.zdbjq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bth.tarul.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hoj.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kuq.sweek.top

TS:   [...arr];
来源：http://xwy.cdnleiting.top

Java: new ArrayList<>(list);
来源：http://qzl.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://dnx.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://edz.ydjk.org.cn

C#:   new List<int>(list);
来源：http://syh.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://sxb.smart0.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wtm.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xru.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ahp.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nfn.epnwcf.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://rvq.bjfxy.top

Go:   // 手写循环
来源：http://vid.shanyushiyangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://byq.jlsjyb.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iwm.snrcjt.cn

[D24] 字典 / Map 基本操作
来源：http://oiy.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wlb.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ugs.tanke756.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://axc.ppjwa.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iia.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jla.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hzo.zhengqikj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wom.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zfp.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://wco.yfazqb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mxy.yuanzhike.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mqc.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bre.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dtj.hywenlv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://chw.zhixingplan.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ztf.jiagoushi.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qry.mhx1999.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dxn.chenjidiqi.icu

[D26] 数组转字符串
来源：http://zur.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://zaw.hesvh.cn

PHP:  implode(", ", $arr);
来源：http://ppd.iojbl.cn

JS:   arr.join(", ")
来源：http://ykb.shanyushiyangtech.top

TS:   arr.join(", ")
来源：http://alt.jinqigufen.top

Java: String.join(", ", list)
来源：http://geu.52xcode.cn

Go:   strings.Join(strs, ", ")
来源：http://ojs.tarul.cn

Ruby: arr.join(", ")
来源：http://tij.gzhubu.top

C#:   string.Join(", ", list)
来源：http://nak.guowangkeji.top

================================================================================
来源：http://awc.tarul.cn

E. 字符串处理
来源：http://pag.xylfe.cn

================================================================================
来源：http://ose.tianlin.xyz

[E01] 拼接字符串
来源：http://bzj.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cbw.gzhubu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qhs.andypj.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xxz.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lgl.hongshengwenyu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kdm.zdbjq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eud.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nay.hesvh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jzn.yueranfly.top

[E02] 重复字符串
来源：http://mwt.cheryme.top

Py:   "ab" * 3
来源：http://ozl.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://len.fengsongda.top

JS:   "ab".repeat(3)
来源：http://dsd.daria6918.cn

TS:   "ab".repeat(3)
来源：http://wzg.jqgfzy.top

Java: "ab".repeat(3)
来源：http://cvx.yvedp.cn

Go:   strings.Repeat("ab", 3)
来源：http://gyr.sweek.top

Ruby: "ab" * 3
来源：http://wby.ppjwa.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zzc.vqdsnc.cn

[E03] 截取子串
来源：http://lni.hammf.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oud.andypj.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qxr.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dnl.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://mgm.yvedp.cn

Java: s.substring(1, 4)
来源：http://mcd.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lal.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tms.iojbl.cn

C#:   s.Substring(1, 3)
来源：http://qpq.fehbvm.com

[E04] 查找子串位置
来源：http://dug.yangfankeji.com

Py:   s.find("x");  s.index("x")
来源：http://rgf.hfpthk.cn

PHP:  strpos($s, "x");
来源：http://orx.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kca.shangyingyoupin.top

TS:   s.indexOf("x")
来源：http://lxl.wangshuangyany.cn

Java: s.indexOf("x")
来源：http://hhr.shanyushiyangkeji.top

Go:   strings.Index(s, "x")
来源：http://qre.bjfxy.top

Ruby: s.index("x")
来源：http://ezs.fktsv.cn

C#:   s.IndexOf("x")
来源：http://qcx.9152youxi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rig.hysaishi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mdu.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://znj.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://slt.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://awh.aizwys.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://els.wangdashe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lsk.jianghu66.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zwr.zhijiandao.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dzj.uphjek.com

[E06] 替换子串
来源：http://wcd.daria6918.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nkt.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://zph.daria6918.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sxz.gotoacloud.top

TS:   s.replaceAll("a", "b")
来源：http://ges.ctjpmb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://azg.vqdsnc.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fvh.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bfg.hnqzz.top

C#:   s.Replace("a", "b")
来源：http://gbh.hfpthk.cn

[E07] 按分隔符拆分
来源：http://jbx.yvedp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bdv.gzhubu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tbu.snrcjt.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hox.hysaishi.cn

TS:   s.split(",")
来源：http://zag.ivvv.top

Java: s.split(",");  s.split("\\s+")
来源：http://jps.yj202588.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vnp.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://ney.uphjek.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ncf.guannengcc.top

[E08] 数组按分隔符合并
来源：http://odx.sysykeji.top

Py:   ",".join(items)
来源：http://xmh.gzhubu.top

PHP:  implode(",", $items);
来源：http://byh.jqgfzy.top

JS:   items.join(",")
来源：http://jkq.shzxlz.cn

TS:   items.join(",")
来源：http://lil.yanxiufei.cn

Java: String.join(",", items)
来源：http://hsn.sxryk.cn

Go:   strings.Join(items, ",")
来源：http://cor.gogol.net.cn

Ruby: items.join(",")
来源：http://yno.gogol.net.cn

C#:   string.Join(",", items)
来源：http://hug.epnwcf.com

[E09] 去除所有空白字符
来源：http://ufg.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tkn.ydjk.org.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cvc.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://uyy.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://tgz.hammf.cn

Java: s.replaceAll("\\s+", "")
来源：http://jph.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://eck.fktsv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://agg.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rrv.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://brq.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sco.dianchejie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pxx.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://efc.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://enr.ydzc1.top

Java: String.format("%03d", 7)
来源：http://yup.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qnx.shuidangran.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dgl.xuetiantiany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oev.bbcook.cn

[E11] 反转字符串
来源：http://kvh.zhoulong.xyz

Py:   s[::-1]
来源：http://xjy.yj202588.top

PHP:  strrev($s);
来源：http://aey.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://eyu.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://klw.shanyushiyangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ypp.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tup.tianlin.xyz

Ruby: s.reverse
来源：http://anb.quarkkingdee.top

C#:   new string(s.Reverse().ToArray())
来源：http://jni.hnqzz.top

[E12] 统计某字符出现次数
来源：http://gvo.ehwqpu.com

Py:   s.count("a")
来源：http://ora.tian-w.cn

PHP:  substr_count($s, "a");
来源：http://vvl.hnqzz.top

JS:   s.split("a").length - 1
来源：http://tvk.tian-w.cn

TS:   s.split("a").length - 1
来源：http://ybb.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fif.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://ndu.ybcxt.top

Ruby: s.count("a")
来源：http://nmu.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://lbv.nanxinkj.top

[E13] 逐字符遍历
来源：http://qez.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://lha.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jlk.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lih.hongshengwenyu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dqk.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://knj.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hzo.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ruf.zdbjq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wdd.gogol.net.cn

[E14] URL 编码与 Base64
来源：http://rit.xingfuxueyuan.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ntc.fehbvm.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://vux.shuidangran.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tyo.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ivr.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://csi.yuxming.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fej.zdbjq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://azb.bjfxy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zfb.sufxvd.cn

[E15] HTML 转义 / 反转义
来源：http://khm.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ekn.fengsongda.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cjq.snrcjt.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gdc.aizwys.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dcv.xuanzx.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mby.zhijiandao.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://osw.bjfxy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uxm.birdmap.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lmt.jyoumei.cn

[E16] 数字千分位
来源：http://htc.cdnleiting.top

Py:   f"{1234567:,}"
来源：http://vcm.sweek.top

PHP:  number_format(1234567);
来源：http://ftg.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dgg.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://wuh.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vib.gaohongyu789.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xnr.fktsv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://geh.cashguo.top

C#:   1234567.ToString("N0")
来源：http://whc.ctjpmb.com

[E17] 首字母大写
来源：http://irv.nanxinkj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ppj.guannengcc.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://typ.fanxiaobao.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://agu.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yvr.tarul.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xmd.tianlin.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ozy.ppjwa.cn

Ruby: s.capitalize
来源：http://yma.hongshengwenyu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hds.ydjk.org.cn

[E18] 模板占位符替换
来源：http://kke.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eyr.snrcjt.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tfk.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qgb.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xnd.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ffs.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wzc.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cmd.jqgfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sme.fanxiaobao.xyz

[E19] 多行文本按行拆分
来源：http://eqi.guowangkeji.top

Py:   s.splitlines()
来源：http://xrb.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://caz.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://nqr.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://lwm.9152youxi.cn

Java: s.lines().toList()
来源：http://mrr.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://kdu.jyoumei.cn

Ruby: s.lines
来源：http://eta.yuanzhike.top

C#:   s.Split('\n')
来源：http://hov.yueranfly.top

[E20] 判断字符串是否为空
来源：http://ggd.fengsongda.top

Py:   if not s:
来源：http://ina.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zat.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://viu.jqgfzy.top

TS:   if (s === "") {}
来源：http://dxy.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://nkg.yj20258888.top

Go:   if s == "" {}
来源：http://mpg.52xcode.cn

Ruby: if s.empty?
来源：http://apf.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oce.kuanghao11.cn

[E21] 超长截断加省略号
来源：http://zom.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aer.ydzc1.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://guv.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://txp.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mgv.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ula.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://dqy.chenlongwang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fir.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tah.zycfv.cn

[E22] 字节长度与字符长度
来源：http://omm.jiagoushi.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vsx.shanyushiyangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://may.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tkg.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hhd.shanyushiyangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kzv.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://asw.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://qod.haohaochexian.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rdb.redwolf501.top

================================================================================
来源：http://gon.fengsongda.top

F. 文件与目录
来源：http://wyg.nwbrower.top

================================================================================
来源：http://nxn.yanxiufei.cn

[F01] 读取整个文件
来源：http://rlt.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vsg.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://bbl.ctjpmb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://erj.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cop.hnqzz.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jxu.haohaochexian.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dcs.tanke756.top

Ruby: File.read("a.txt")
来源：http://rva.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://lmi.sweek.top

[F02] 逐行读取文件
来源：http://dtl.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kia.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ntn.shangyingyoupin.top


<!-- 参考信息 -->