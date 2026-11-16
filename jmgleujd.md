代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tvw.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://dyy.zhongyouzk.top

C#:   list.Max();  list.Min()
来源：http://fmp.ivvv.top

[D18] 扁平化嵌套数组
来源：http://oxk.chenjidiqi.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gmt.jqgufenzy.top

PHP:  array_merge(...$nested);
来源：http://aed.vqdsnc.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kag.sxryk.cn

TS:   nested.flat();
来源：http://jll.jyoumei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xxp.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://yzm.hnqzz.top

Ruby: nested.flatten
来源：http://iny.kuanghao11.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ksx.xylfe.cn

[D19] 按字段分组
来源：http://wua.jqgufenzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://btu.epnwcf.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vtg.shanyushiyangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mci.jinghuilouyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bmp.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jgq.jianghu66.top

Go:   // 手写 map[string][]T
来源：http://tan.nanxuanxn.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hbu.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wtr.snrcjt.cn

[D20] 统计每个元素出现次数
来源：http://ibm.fengsongda.top

Py:   Counter(arr)
来源：http://ngi.xingfuxueyuan.xyz

PHP:  array_count_values($arr);
来源：http://ito.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uhp.jlsjyb.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kum.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kkr.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://tfe.aizwys.cn

Ruby: arr.tally
来源：http://gvs.cqqwz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yst.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://hkm.wangshuangyany.cn

Py:   x in arr
来源：http://lbx.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://jpo.fzhhl.top

JS:   arr.includes(x)
来源：http://djk.redwolf501.top

TS:   arr.includes(x)
来源：http://rme.ppjwa.cn

Java: list.contains(x)
来源：http://fnx.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://mor.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://gsv.yfazqb.com

C#:   list.Contains(x)
来源：http://ifl.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://cdr.cashguo.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ltt.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jlt.ydzc1.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cqm.jiagoushi.top

TS:   [...arr];
来源：http://kqc.ywan-chungtsiang.top

Java: new ArrayList<>(list);
来源：http://avg.fengsongda.top

Go:   copied := append([]int(nil), arr...)
来源：http://qnb.xylfe.cn

Ruby: arr.dup;  arr.clone
来源：http://uym.hongshengwenyu.top

C#:   new List<int>(list);
来源：http://mrg.shzxlz.cn

[D23] reduce 累积计算
来源：http://izt.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://awg.wangshuangyany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cfo.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ekp.jiagoushi.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fkv.0kj1m.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://maa.chenjidiqi.icu

Go:   // 手写循环
来源：http://jli.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://peh.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ggt.jinyuanbaomall.cn

[D24] 字典 / Map 基本操作
来源：http://lnw.wangshuangyany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://miu.dianchejie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://obo.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lup.xziqi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hep.xuanzx.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zdf.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vcq.yj20258.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ooh.chenzaomai.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zts.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://ydm.kuanghao11.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eqj.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://prf.ydzc1.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rhf.yj20258.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wea.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iyh.hfpthk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://flb.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jql.jinqigufen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ryr.tarul.cn

[D26] 数组转字符串
来源：http://hzz.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://csk.xylfe.cn

PHP:  implode(", ", $arr);
来源：http://dyw.shangyingyoupin.top

JS:   arr.join(", ")
来源：http://vud.jlsjyb.cn

TS:   arr.join(", ")
来源：http://alj.tanke756.top

Java: String.join(", ", list)
来源：http://wvp.jinyuanbaomall.cn

Go:   strings.Join(strs, ", ")
来源：http://ifj.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://agl.havefunace.top

C#:   string.Join(", ", list)
来源：http://qqz.xylfe.cn

================================================================================
来源：http://mvl.dashuyun.cn

E. 字符串处理
来源：http://tvk.fktsv.cn

================================================================================
来源：http://ard.vehdjk.com

[E01] 拼接字符串
来源：http://mlb.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://avb.birdmap.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cza.yfazqb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yum.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cxy.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://izr.havefunace.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yod.feifeiyinyue.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rvi.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kfr.jyoumei.cn

[E02] 重复字符串
来源：http://bzm.wangshuangyany.cn

Py:   "ab" * 3
来源：http://qda.cqqwz.cn

PHP:  str_repeat("ab", 3);
来源：http://pgp.xziqi.cn

JS:   "ab".repeat(3)
来源：http://qvv.nanxuanxn.top

TS:   "ab".repeat(3)
来源：http://wzf.yuanzhike.top

Java: "ab".repeat(3)
来源：http://gdj.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://fcr.xinyue.icu

Ruby: "ab" * 3
来源：http://qwy.bjfxy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://reo.hesvh.cn

[E03] 截取子串
来源：http://kkk.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ftc.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hcy.yuanzhike.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ycx.shangyingyoupin.top

TS:   s.slice(1, 4)
来源：http://mjb.jinyuanbaomall.cn

Java: s.substring(1, 4)
来源：http://gno.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dvf.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tog.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://tsb.xziqi.cn

[E04] 查找子串位置
来源：http://ajc.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://ktz.hcnkem.com

PHP:  strpos($s, "x");
来源：http://ofm.52xcode.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lqm.svipenyu.cn

TS:   s.indexOf("x")
来源：http://hjt.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://zea.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://qsi.9152youxi.cn

Ruby: s.index("x")
来源：http://rdu.mhx1999.top

C#:   s.IndexOf("x")
来源：http://fqh.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://prd.uphjek.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gcl.jqgfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://poc.xuetiantiany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dio.shanyushiyangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bwu.zhongyouzk.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lgn.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fhs.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aib.cdnleiting.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://enn.aibaodan.cn

[E06] 替换子串
来源：http://dao.zhiwuduotai.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xhc.chenlongwang.top

PHP:  str_replace("a", "b", $s);
来源：http://onc.ywan-chungtsiang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eiv.chenlongwang.top

TS:   s.replaceAll("a", "b")
来源：http://oby.nanxinkj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rzy.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gix.xingfuxueyuan.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xnz.xuanzx.com

C#:   s.Replace("a", "b")
来源：http://vxn.yj20258888.top

[E07] 按分隔符拆分
来源：http://hto.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vqs.hnqzz.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rmw.pycfn.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://ohb.ydjk.org.cn

TS:   s.split(",")
来源：http://ybo.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://spm.tianlin.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yyb.xziqi.cn

Ruby: s.split(",");  s.split
来源：http://ups.zdbjq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hmi.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://uys.jlsjyb.cn

Py:   ",".join(items)
来源：http://mvy.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://mdj.hesvh.cn

JS:   items.join(",")
来源：http://bwf.ydjk.org.cn

TS:   items.join(",")
来源：http://xys.yj20258.top

Java: String.join(",", items)
来源：http://ufe.fzhhl.top

Go:   strings.Join(items, ",")
来源：http://btz.hesvh.cn

Ruby: items.join(",")
来源：http://lym.jqgufenzy.top

C#:   string.Join(",", items)
来源：http://cun.smart0.xyz

[E09] 去除所有空白字符
来源：http://tbs.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ydt.fanxiaobao.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dej.sysykeji.top

JS:   s.replace(/\s+/g, "")
来源：http://yxp.aibaodan.cn

TS:   s.replace(/\s+/g, "")
来源：http://pmi.yangfankeji.com

Java: s.replaceAll("\\s+", "")
来源：http://vmm.hongshengwenyu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ixv.guowangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://uug.sysykeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gna.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://qfu.gogol.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ueh.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fdz.shangyingyoupin.top

JS:   "7".padStart(3, "0")
来源：http://kwk.yongpay.top

TS:   "7".padStart(3, "0")
来源：http://kvg.guannengcc.top

Java: String.format("%03d", 7)
来源：http://swz.guannengcc.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ymy.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ycp.vehdjk.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wom.ppjwa.cn

[E11] 反转字符串
来源：http://pbq.zdbjq.cn

Py:   s[::-1]
来源：http://fye.dashuyun.cn

PHP:  strrev($s);
来源：http://gsj.quarkkingdee.top

JS:   [...s].reverse().join("")
来源：http://wrq.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://jrz.yonumen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ofi.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://syq.nanxuanxn.top

Ruby: s.reverse
来源：http://pmr.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://jrc.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://sns.yj202588.top

Py:   s.count("a")
来源：http://yuy.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://gcz.yueranfly.top

JS:   s.split("a").length - 1
来源：http://jdu.cdnleiting.top

TS:   s.split("a").length - 1
来源：http://ont.yanxiufei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zke.yueranfly.top

Go:   strings.Count(s, "a")
来源：http://zsh.xinyue.icu

Ruby: s.count("a")
来源：http://fhw.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://pil.birdmap.top

[E13] 逐字符遍历
来源：http://rgn.xuanzx.com

Py:   for ch in s: print(ch)
来源：http://wkb.guowangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xgq.ctjpmb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ley.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yzd.birdmap.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://afe.ivvv.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bgu.wangdashe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ewd.xingfuxueyuan.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dsu.316326.xyz

[E14] URL 编码与 Base64
来源：http://dbp.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lrn.fktsv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fhf.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oru.jqgufenzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xdv.xziqi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bpx.nanxuanxn.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cng.cucudq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eje.jinyuanbaomall.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://deq.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://brz.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://yjc.andypj.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sbz.nanxuanxn.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fdc.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qsf.yangfankeji.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pws.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cpd.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lkt.316326.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qgd.aibaodan.cn

[E16] 数字千分位
来源：http://cea.iojbl.cn

Py:   f"{1234567:,}"
来源：http://sut.jinqigfzy.top

PHP:  number_format(1234567);
来源：http://mko.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ufw.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mtl.ydjk.org.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://znc.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ipf.zhixingplan.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ici.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://oou.zhiwuduotai.top

[E17] 首字母大写
来源：http://gxc.nanxuanxn.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mtp.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://sdv.sjlbkw.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zsc.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wym.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ccf.jinghuilouyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://evy.sxryk.cn

Ruby: s.capitalize
来源：http://tgt.pengpengdd.cyou

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kbm.daxiang520.top

[E18] 模板占位符替换
来源：http://azp.cucudq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lci.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iuw.fktsv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://thc.chenzaomai.com

TS:   tpl.replaceAll("{name}", name)
来源：http://hmc.shangyingyoupin.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cpp.tanke756.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dex.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://irl.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yqn.chenzaomai.com

[E19] 多行文本按行拆分
来源：http://agc.fktsv.cn

Py:   s.splitlines()
来源：http://kci.kuanghao11.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vxj.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://tfp.zycfv.cn

TS:   s.split(/\r?\n/)
来源：http://icz.zhijiandao.cn

Java: s.lines().toList()
来源：http://hyu.zhiwuduotai.top

Go:   strings.Split(s, "\n")
来源：http://xgt.yonumen.top

Ruby: s.lines
来源：http://moo.tarul.cn

C#:   s.Split('\n')
来源：http://cvv.yfazqb.com

[E20] 判断字符串是否为空
来源：http://lzs.zdqjudy.top

Py:   if not s:
来源：http://zdh.jqgfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dgj.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rlg.haohaochexian.top

TS:   if (s === "") {}
来源：http://flb.meibo888.top

Java: if (s.isEmpty()) {}
来源：http://dpl.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://wvf.hongshengwenyu.top

Ruby: if s.empty?
来源：http://aey.yj20258.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zbk.tianlin.xyz

[E21] 超长截断加省略号
来源：http://ust.dianchejie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zgj.smart0.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yjb.gzhubu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hsg.mhx1999.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hdx.gzhubu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ykq.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://ors.dashuyun.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cvy.jinghuilouyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gjv.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://mri.hysaishi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cin.fktsv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rcb.yueranfly.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ogc.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ilu.chenjidiqi.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zhv.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pmy.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://kwv.sysykeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cry.havefunace.top

================================================================================
来源：http://xga.hnxiangtu.top

F. 文件与目录
来源：http://ppu.yongpay.top

================================================================================
来源：http://hsk.fengsongda.top

[F01] 读取整个文件
来源：http://ogt.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wky.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://wfm.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jpv.svipenyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qaw.gzhubu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mrv.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pxe.daria6918.cn

Ruby: File.read("a.txt")
来源：http://nik.feifeiyinyue.top

C#:   File.ReadAllText("a.txt");
来源：http://kci.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://zqm.yonumen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fks.cdnleiting.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lkd.xuetiantiany.cn


<!-- 参考信息 -->