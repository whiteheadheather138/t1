代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xxu.zdqjudy.top

Ruby: arr.max;  arr.min
来源：http://geo.gzhubu.top

C#:   list.Max();  list.Min()
来源：http://mof.hysaishi.cn

[D18] 扁平化嵌套数组
来源：http://yaw.hesvh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jcj.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://lnk.tarul.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jwg.aibaodan.cn

TS:   nested.flat();
来源：http://pjf.xinyue.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://clr.zdqjudy.top

Go:   // 手写双层循环
来源：http://gei.ydjk.org.cn

Ruby: nested.flatten
来源：http://kxs.aibaodan.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vem.zhongyouzk.top

[D19] 按字段分组
来源：http://rzm.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fjv.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mvi.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gkx.hesvh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xyw.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rag.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://ors.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ffp.dianchejie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rry.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://nml.hfpthk.cn

Py:   Counter(arr)
来源：http://yet.uphjek.com

PHP:  array_count_values($arr);
来源：http://aqq.gotoacloud.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://loz.guannengcc.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hmp.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://unl.epnwcf.com

Go:   // 手写 map[T]int
来源：http://eyb.yueranfly.top

Ruby: arr.tally
来源：http://kgz.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fyp.fzhhl.top

[D21] 判断是否包含某元素
来源：http://eqv.cqqwz.cn

Py:   x in arr
来源：http://rdn.zhixingplan.top

PHP:  in_array($x, $arr, true);
来源：http://ltk.redwolf501.top

JS:   arr.includes(x)
来源：http://qjd.fengsongda.top

TS:   arr.includes(x)
来源：http://lgm.ctjpmb.com

Java: list.contains(x)
来源：http://wwk.zhixingplan.top

Go:   slices.Contains(arr, x)
来源：http://tbm.redwolf501.top

Ruby: arr.include?(x)
来源：http://vyx.pengpengdd.cyou

C#:   list.Contains(x)
来源：http://npo.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://rtg.chenzaomai.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uwj.pengpengdd.cyou

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rbl.yonumen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xuv.jianghu66.top

TS:   [...arr];
来源：http://rnm.cashguo.top

Java: new ArrayList<>(list);
来源：http://qbf.0kj1m.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tsd.tarul.cn

Ruby: arr.dup;  arr.clone
来源：http://mdw.zhijiandao.cn

C#:   new List<int>(list);
来源：http://zoz.yueranfly.top

[D23] reduce 累积计算
来源：http://bbo.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jdt.jinyuanbaomall.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fhg.316326.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zkx.zhijiandao.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vuc.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://smh.fktsv.cn

Go:   // 手写循环
来源：http://vxz.yvedp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fnd.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ipn.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://pfo.jiagoushi.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nrv.fehbvm.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://opz.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iml.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ata.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://byw.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wqa.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iuf.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sxs.iojbl.cn

[D25] Set 集合去重与交并差
来源：http://ezi.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xue.vqdsnc.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://taw.xziqi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wqx.haohaochexian.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bah.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wpd.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tjs.zhiwuduotai.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vej.yongpay.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://boz.bjfxy.top

[D26] 数组转字符串
来源：http://uyp.shzxlz.cn

Py:   ", ".join(map(str, arr))
来源：http://xqn.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://blf.xinyue.icu

JS:   arr.join(", ")
来源：http://grj.tarul.cn

TS:   arr.join(", ")
来源：http://nqd.gaohongyu789.top

Java: String.join(", ", list)
来源：http://ldl.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://gri.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://owe.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://mgs.wangdashe.top

================================================================================
来源：http://rcv.hfpthk.cn

E. 字符串处理
来源：http://hls.cqqwz.cn

================================================================================
来源：http://fih.cucudq.cn

[E01] 拼接字符串
来源：http://xxi.jqgufenzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qbl.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qcf.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zpl.jlsjyb.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lsj.jinyuanbaomall.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ume.316326.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nsu.meibo888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lge.nanxinkj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kro.zdqjudy.top

[E02] 重复字符串
来源：http://bah.uphjek.com

Py:   "ab" * 3
来源：http://vxk.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://uyf.ydzc1.top

JS:   "ab".repeat(3)
来源：http://tvy.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://evw.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://xte.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://zkt.hammf.cn

Ruby: "ab" * 3
来源：http://osn.zhengqikj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ciw.ydzc1.top

[E03] 截取子串
来源：http://osh.xingfuxueyuan.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xcw.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://prg.nanxinkj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tiv.smart0.xyz

TS:   s.slice(1, 4)
来源：http://qpg.zdbjq.cn

Java: s.substring(1, 4)
来源：http://ziw.zhengqikj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cqe.zdbjq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gbx.sjlbkw.cn

C#:   s.Substring(1, 3)
来源：http://qrz.quarkkingdee.top

[E04] 查找子串位置
来源：http://yfg.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://qwo.sufxvd.cn

PHP:  strpos($s, "x");
来源：http://fcv.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wew.ivvv.top

TS:   s.indexOf("x")
来源：http://wtr.bjfxy.top

Java: s.indexOf("x")
来源：http://uov.sjlbkw.cn

Go:   strings.Index(s, "x")
来源：http://hii.vehdjk.com

Ruby: s.index("x")
来源：http://fhs.zdqjudy.top

C#:   s.IndexOf("x")
来源：http://ffo.daria6918.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gxm.zhiwuduotai.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xwy.zhoulong.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zfz.ehwqpu.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baa.pengpengdd.cyou

TS:   s.includes("x");  s.startsWith("a")
来源：http://maj.jqgfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fft.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gru.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xyc.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ffw.ehwqpu.com

[E06] 替换子串
来源：http://ody.zhongyouzk.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jqa.zdqjudy.top

PHP:  str_replace("a", "b", $s);
来源：http://llz.iojbl.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gvr.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://ane.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fwh.sxryk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://isv.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zjk.fengsongda.top

C#:   s.Replace("a", "b")
来源：http://sxd.xziqi.cn

[E07] 按分隔符拆分
来源：http://yiu.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ggd.yanxiufei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://akp.gogol.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mci.ppjwa.cn

TS:   s.split(",")
来源：http://ang.sjlbkw.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qff.dashuyun.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://scn.jianghu66.top

Ruby: s.split(",");  s.split
来源：http://bor.cashguo.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nen.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://pof.shangyingyoupin.top

Py:   ",".join(items)
来源：http://yui.cucudq.cn

PHP:  implode(",", $items);
来源：http://tbc.ppjwa.cn

JS:   items.join(",")
来源：http://ccu.chenzaomai.com

TS:   items.join(",")
来源：http://rgs.hammf.cn

Java: String.join(",", items)
来源：http://xqo.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://hof.ydjk.org.cn

Ruby: items.join(",")
来源：http://ayx.jiagoushi.top

C#:   string.Join(",", items)
来源：http://iye.haohaochexian.top

[E09] 去除所有空白字符
来源：http://vss.hysaishi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fce.fanxiaobao.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tty.yfazqb.com

JS:   s.replace(/\s+/g, "")
来源：http://sbc.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://jdz.yvedp.cn

Java: s.replaceAll("\\s+", "")
来源：http://hra.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://inl.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://ppz.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ntx.shanyushiyangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://ypd.zhoulong.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kwk.guannengcc.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bkz.sweek.top

JS:   "7".padStart(3, "0")
来源：http://ovo.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://gvc.cheryme.top

Java: String.format("%03d", 7)
来源：http://rem.zhongyouzk.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://axv.hysaishi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uys.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dtt.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://kwl.kuanghao11.cn

Py:   s[::-1]
来源：http://fnk.hongshengwenyu.top

PHP:  strrev($s);
来源：http://anr.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://dgx.birdmap.top

TS:   [...s].reverse().join("")
来源：http://tpg.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hjo.yfazqb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://zrk.sxryk.cn

Ruby: s.reverse
来源：http://iqe.yuxming.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nyg.cashguo.top

[E12] 统计某字符出现次数
来源：http://lcu.sjlbkw.cn

Py:   s.count("a")
来源：http://fud.hongshengwenyu.top

PHP:  substr_count($s, "a");
来源：http://vwq.dashuyun.cn

JS:   s.split("a").length - 1
来源：http://hue.zdqjudy.top

TS:   s.split("a").length - 1
来源：http://zug.chenlongwang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qrg.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://qss.jinyuanbaomall.cn

Ruby: s.count("a")
来源：http://kjl.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://bje.hfpthk.cn

[E13] 逐字符遍历
来源：http://qtm.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://qvi.haohaochexian.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rxf.ctjpmb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://mbd.cdnleiting.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gfh.cdnleiting.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qfn.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ytm.hongshengwenyu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ihs.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bfy.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://xgx.tarul.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wdz.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vxw.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zlc.sysykeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eri.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qoj.tarul.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gvd.cheryme.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://krl.hywenlv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oat.shzxlz.cn

[E15] HTML 转义 / 反转义
来源：http://hql.gaohongyu789.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zkv.ydjk.org.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://irn.uphjek.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ryp.chenlongwang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dkb.tian-w.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://auq.aibaodan.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wke.yuxming.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fcr.xuetiantiany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lwk.birdmap.top

[E16] 数字千分位
来源：http://suq.daria6918.cn

Py:   f"{1234567:,}"
来源：http://ntw.snrcjt.cn

PHP:  number_format(1234567);
来源：http://wlg.zhiwuduotai.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yog.jyoumei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fyf.jinqigufen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ybm.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rrl.ppjwa.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ojr.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://ini.yonumen.top

[E17] 首字母大写
来源：http://ngf.ywan-chungtsiang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nnd.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nnr.fktsv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://spr.ywan-chungtsiang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ndi.yvedp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gpf.fengsongda.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yfa.bbcook.cn

Ruby: s.capitalize
来源：http://jsu.bbcook.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zlu.sweek.top

[E18] 模板占位符替换
来源：http://ksu.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vma.guannengcc.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qes.cheryme.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ouj.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://rkc.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ywc.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sbo.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vsh.sxryk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bvk.daxiang520.top

[E19] 多行文本按行拆分
来源：http://flc.birdmap.top

Py:   s.splitlines()
来源：http://rne.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sdh.ywan-chungtsiang.top

JS:   s.split(/\r?\n/)
来源：http://fbj.shzxlz.cn

TS:   s.split(/\r?\n/)
来源：http://jux.birdmap.top

Java: s.lines().toList()
来源：http://nzo.ehwqpu.com

Go:   strings.Split(s, "\n")
来源：http://rhy.hfpthk.cn

Ruby: s.lines
来源：http://nwm.snrcjt.cn

C#:   s.Split('\n')
来源：http://mlx.yonumen.top

[E20] 判断字符串是否为空
来源：http://cpk.tarul.cn

Py:   if not s:
来源：http://qrn.sxryk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ojm.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eyh.c1oappe.top

TS:   if (s === "") {}
来源：http://var.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://eal.fzhhl.top

Go:   if s == "" {}
来源：http://crt.guowangkeji.top

Ruby: if s.empty?
来源：http://cfl.tarul.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wqb.jiagoushi.top

[E21] 超长截断加省略号
来源：http://mpz.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sst.zdbjq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hpz.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mtk.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zbr.haohaochexian.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tzj.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://kkn.jinyuanbaomall.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mei.jinqigfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wfw.9152youxi.cn

[E22] 字节长度与字符长度
来源：http://jsy.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kcc.vqdsnc.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ucy.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qop.fehbvm.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dqv.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vzq.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://szp.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://gqn.svipenyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kzq.epnwcf.com

================================================================================
来源：http://jeo.mhx1999.top

F. 文件与目录
来源：http://kyr.sufxvd.cn

================================================================================
来源：http://pwt.xziqi.cn

[F01] 读取整个文件
来源：http://syb.zdqjudy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gum.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://yfv.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nbk.gogol.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rdj.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ecz.hysaishi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cjw.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://sjf.zhixingplan.top

C#:   File.ReadAllText("a.txt");
来源：http://jrh.cqqwz.cn

[F02] 逐行读取文件
来源：http://ymc.wangdashe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ndl.guannengcc.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wlv.gaohongyu789.top


<!-- 参考信息 -->