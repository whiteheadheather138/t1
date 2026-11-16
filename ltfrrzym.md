代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nhn.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://rcg.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://spm.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://aeq.hesvh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fox.daria6918.cn

PHP:  array_merge(...$nested);
来源：http://wbb.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nck.dianchejie.cn

TS:   nested.flat();
来源：http://vxq.cashguo.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tvl.sjlbkw.cn

Go:   // 手写双层循环
来源：http://knt.zhoulong.xyz

Ruby: nested.flatten
来源：http://dce.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://jtf.shanyushiyangtech.top

[D19] 按字段分组
来源：http://lhr.cucudq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blc.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qlm.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vvm.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://dri.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qtr.xingfuxueyuan.xyz

Go:   // 手写 map[string][]T
来源：http://kfy.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://qaa.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ssx.jinghuilouyu.cn

[D20] 统计每个元素出现次数
来源：http://lsq.hnxiangtu.top

Py:   Counter(arr)
来源：http://oas.hcnkem.com

PHP:  array_count_values($arr);
来源：http://tmd.zhengqikj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dhg.shuidangran.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uqj.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mpu.fktsv.cn

Go:   // 手写 map[T]int
来源：http://mms.hesvh.cn

Ruby: arr.tally
来源：http://cps.guannengcc.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xih.fehbvm.com

[D21] 判断是否包含某元素
来源：http://efq.chenjidiqi.icu

Py:   x in arr
来源：http://nrr.hnxiangtu.top

PHP:  in_array($x, $arr, true);
来源：http://xcx.fktsv.cn

JS:   arr.includes(x)
来源：http://wdj.fehbvm.com

TS:   arr.includes(x)
来源：http://lxd.snrcjt.cn

Java: list.contains(x)
来源：http://ebb.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://ggn.yongpay.top

Ruby: arr.include?(x)
来源：http://huo.hfpthk.cn

C#:   list.Contains(x)
来源：http://byh.bjfxy.top

[D22] 复制数组（避免共享引用）
来源：http://tzs.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://csh.shanyushiyangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dtv.wangshuangyany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://brh.yvedp.cn

TS:   [...arr];
来源：http://ecd.shuidangran.top

Java: new ArrayList<>(list);
来源：http://cvx.shanyushiyangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://peo.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://yjl.fengsongda.top

C#:   new List<int>(list);
来源：http://kej.andypj.xyz

[D23] reduce 累积计算
来源：http://zfh.iojbl.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gml.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://txb.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xzn.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ahd.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mpy.jinghuilouyu.cn

Go:   // 手写循环
来源：http://nxy.gogol.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sai.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tkq.hammf.cn

[D24] 字典 / Map 基本操作
来源：http://drw.vqdsnc.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ize.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cxr.hywenlv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zsp.c1oappe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qpl.fzhhl.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sao.zhaomingkeji.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nfk.9152youxi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rir.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lmf.zdqjudy.top

[D25] Set 集合去重与交并差
来源：http://vbj.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://opq.ydzc1.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pqq.sweek.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wty.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lql.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oko.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://avx.shangyingyoupin.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qur.bbcook.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kkv.yangfankeji.com

[D26] 数组转字符串
来源：http://lfn.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://mfc.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://dlv.hfpthk.cn

JS:   arr.join(", ")
来源：http://tal.iojbl.cn

TS:   arr.join(", ")
来源：http://scx.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://ith.gzhubu.top

Go:   strings.Join(strs, ", ")
来源：http://svz.hammf.cn

Ruby: arr.join(", ")
来源：http://tsd.hfpthk.cn

C#:   string.Join(", ", list)
来源：http://pun.ivvv.top

================================================================================
来源：http://buo.xuetiantiany.cn

E. 字符串处理
来源：http://guy.xuanzx.com

================================================================================
来源：http://ing.zhijiandao.cn

[E01] 拼接字符串
来源：http://eqj.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://igy.pycfn.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hbm.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qxp.epnwcf.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dcz.shanyushiyangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bsv.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zmc.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lzc.chenzaomai.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tnf.smart0.xyz

[E02] 重复字符串
来源：http://bqy.gzhubu.top

Py:   "ab" * 3
来源：http://hwf.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://bdv.cashguo.top

JS:   "ab".repeat(3)
来源：http://utd.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://eah.meibo888.top

Java: "ab".repeat(3)
来源：http://kza.chenjidiqi.icu

Go:   strings.Repeat("ab", 3)
来源：http://zds.xylfe.cn

Ruby: "ab" * 3
来源：http://zrk.cdnleiting.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lyr.aizwys.cn

[E03] 截取子串
来源：http://grk.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://piu.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mfb.havefunace.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iyc.hesvh.cn

TS:   s.slice(1, 4)
来源：http://jju.xinyue.icu

Java: s.substring(1, 4)
来源：http://uha.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dnn.aizwys.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ery.wangshuangyany.cn

C#:   s.Substring(1, 3)
来源：http://gji.tarul.cn

[E04] 查找子串位置
来源：http://hqb.guannengcc.top

Py:   s.find("x");  s.index("x")
来源：http://qdh.zhongyouzk.top

PHP:  strpos($s, "x");
来源：http://kvh.gaohongyu789.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kyw.jiagoushi.top

TS:   s.indexOf("x")
来源：http://baa.ctjpmb.com

Java: s.indexOf("x")
来源：http://zvi.gaohongyu789.top

Go:   strings.Index(s, "x")
来源：http://drw.hywenlv.cn

Ruby: s.index("x")
来源：http://inv.xuanzx.com

C#:   s.IndexOf("x")
来源：http://szj.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ukc.ybcxt.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yrh.vqdsnc.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kyh.zhengqikj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ycs.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nii.chenlongwang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eyg.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://drh.tanke756.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://egt.jyoumei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hqt.ehwqpu.com

[E06] 替换子串
来源：http://mdd.smart0.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ijw.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://oil.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://boy.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://zjs.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jpz.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jhw.jyoumei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dca.cqqwz.cn

C#:   s.Replace("a", "b")
来源：http://kne.feifeiyinyue.top

[E07] 按分隔符拆分
来源：http://zcg.cucudq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://irl.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yss.fehbvm.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://cnm.iojbl.cn

TS:   s.split(",")
来源：http://mvg.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://fwd.cdnleiting.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mbf.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://mrc.yvedp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xap.xziqi.cn

[E08] 数组按分隔符合并
来源：http://jex.nwbrower.top

Py:   ",".join(items)
来源：http://agn.mhx1999.top

PHP:  implode(",", $items);
来源：http://tcu.yj20258.top

JS:   items.join(",")
来源：http://xde.gotoacloud.top

TS:   items.join(",")
来源：http://shs.shuidangran.top

Java: String.join(",", items)
来源：http://fpv.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://joe.hcnkem.com

Ruby: items.join(",")
来源：http://eoh.0kj1m.cn

C#:   string.Join(",", items)
来源：http://aqr.guannengcc.top

[E09] 去除所有空白字符
来源：http://cgp.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mln.hywenlv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xrc.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://yea.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://xzn.hammf.cn

Java: s.replaceAll("\\s+", "")
来源：http://mea.birdmap.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://agl.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://mjw.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uqh.redwolf501.top

[E10] 左侧补零 / 定长填充
来源：http://bci.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uev.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://haq.fanxiaobao.xyz

JS:   "7".padStart(3, "0")
来源：http://hjc.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://tww.xuanzx.com

Java: String.format("%03d", 7)
来源：http://xxo.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://djn.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rst.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hbe.hfpthk.cn

[E11] 反转字符串
来源：http://xoa.guannengcc.top

Py:   s[::-1]
来源：http://pxo.yj20258.top

PHP:  strrev($s);
来源：http://jlc.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://mff.zhengqikj.top

TS:   [...s].reverse().join("")
来源：http://int.jlsjyb.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://neq.shanyushiyangtech.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lce.yuxming.cn

Ruby: s.reverse
来源：http://bdi.haohaochexian.top

C#:   new string(s.Reverse().ToArray())
来源：http://ofv.ivvv.top

[E12] 统计某字符出现次数
来源：http://lgp.zhengqikj.top

Py:   s.count("a")
来源：http://nhh.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://ykp.xylfe.cn

JS:   s.split("a").length - 1
来源：http://izm.pycfn.com

TS:   s.split("a").length - 1
来源：http://vgq.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ngf.chenjidiqi.icu

Go:   strings.Count(s, "a")
来源：http://tgw.zhengqikj.top

Ruby: s.count("a")
来源：http://fxo.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://ido.guowangkeji.top

[E13] 逐字符遍历
来源：http://qmu.xuanzx.com

Py:   for ch in s: print(ch)
来源：http://afw.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wsr.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wud.cqqwz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vff.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uwl.zdbjq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gql.chenzaomai.com

Ruby: s.each_char { |ch| puts ch }
来源：http://mjw.ivvv.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bdb.wangdashe.top

[E14] URL 编码与 Base64
来源：http://jzo.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://acz.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://zmt.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://npw.zhiwuduotai.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ioq.yuxming.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tuq.shanyushiyangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bmy.uphjek.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oyi.yueranfly.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vfl.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://edj.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://sea.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bfc.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gce.ctjpmb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://fnj.hesvh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://clp.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bio.bbcook.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gyf.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ifp.sweek.top

[E16] 数字千分位
来源：http://cyn.hnqzz.top

Py:   f"{1234567:,}"
来源：http://ycf.nanxinkj.top

PHP:  number_format(1234567);
来源：http://gte.yonumen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xkk.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ugh.andypj.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yeu.hfpthk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jke.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zaq.52xcode.cn

C#:   1234567.ToString("N0")
来源：http://duj.zhixingplan.top

[E17] 首字母大写
来源：http://irj.quarkkingdee.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hmw.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://aio.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://roy.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://viw.ybcxt.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ehn.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vag.shanyushiyangtech.top

Ruby: s.capitalize
来源：http://vag.fzhhl.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://onc.ybcxt.top

[E18] 模板占位符替换
来源：http://oel.ybcxt.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zvt.svipenyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ueb.fktsv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sly.yueranfly.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kvg.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nji.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://joh.gaohongyu789.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lol.yj20258888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aiv.shuidangran.top

[E19] 多行文本按行拆分
来源：http://ukj.yj20258888.top

Py:   s.splitlines()
来源：http://iqm.shuidangran.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://odk.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://tqw.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://vet.zhengqikj.top

Java: s.lines().toList()
来源：http://jbv.yj202588.top

Go:   strings.Split(s, "\n")
来源：http://iex.iojbl.cn

Ruby: s.lines
来源：http://fos.hcnkem.com

C#:   s.Split('\n')
来源：http://hyh.jianghu66.top

[E20] 判断字符串是否为空
来源：http://xgw.ppjwa.cn

Py:   if not s:
来源：http://ozk.hnxiangtu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tca.yj20258.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qzm.redwolf501.top

TS:   if (s === "") {}
来源：http://taj.redwolf501.top

Java: if (s.isEmpty()) {}
来源：http://wco.cheryme.top

Go:   if s == "" {}
来源：http://pdx.zhaomingkeji.xyz

Ruby: if s.empty?
来源：http://cdc.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ieg.ehwqpu.com

[E21] 超长截断加省略号
来源：http://gwb.ppjwa.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xbl.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nje.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://glw.hysaishi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wxh.hesvh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://atz.cqqwz.cn

Go:   // 按 rune 判断长度后截断
来源：http://njl.mhx1999.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mde.yvedp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jwc.zdbjq.cn

[E22] 字节长度与字符长度
来源：http://ojx.jyoumei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rsb.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hho.0kj1m.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wje.quarkkingdee.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mdw.meibo888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uik.yueranfly.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://alo.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://vuu.zhongyouzk.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://urm.yj202588.top

================================================================================
来源：http://ttv.xingfuxueyuan.xyz

F. 文件与目录
来源：http://won.yj20258888.top

================================================================================
来源：http://etp.cheryme.top

[F01] 读取整个文件
来源：http://jmy.vehdjk.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iua.hcnkem.com

PHP:  file_get_contents("a.txt");
来源：http://zyp.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ebc.dashuyun.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lnn.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wcb.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://epo.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://luy.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://dvd.xziqi.cn

[F02] 逐行读取文件
来源：http://bsc.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://koe.jqgfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sss.yangfankeji.com


<!-- 参考信息 -->