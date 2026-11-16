代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://phk.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://tao.fengsongda.top

C#:   list.Max();  list.Min()
来源：http://usd.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://hsg.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xaj.meibo888.top

PHP:  array_merge(...$nested);
来源：http://iun.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wom.zhengqikj.top

TS:   nested.flat();
来源：http://pvg.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gus.gzhubu.top

Go:   // 手写双层循环
来源：http://jjj.xylfe.cn

Ruby: nested.flatten
来源：http://pyf.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://cxh.yfazqb.com

[D19] 按字段分组
来源：http://zqf.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bia.snrcjt.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tac.yueranfly.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ewd.fanxiaobao.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://ovu.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ntp.birdmap.top

Go:   // 手写 map[string][]T
来源：http://kpu.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ubi.cucudq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://duc.pengpengdd.cyou

[D20] 统计每个元素出现次数
来源：http://zaj.sufxvd.cn

Py:   Counter(arr)
来源：http://qdy.guannengcc.top

PHP:  array_count_values($arr);
来源：http://awk.vehdjk.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mvc.ybcxt.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://smu.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oxb.wangdashe.top

Go:   // 手写 map[T]int
来源：http://ekf.ppjwa.cn

Ruby: arr.tally
来源：http://aje.jlsjyb.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rpe.fzhhl.top

[D21] 判断是否包含某元素
来源：http://puu.aizwys.cn

Py:   x in arr
来源：http://drv.wangshuangyany.cn

PHP:  in_array($x, $arr, true);
来源：http://xbb.sysykeji.top

JS:   arr.includes(x)
来源：http://net.aibaodan.cn

TS:   arr.includes(x)
来源：http://nsz.hywenlv.cn

Java: list.contains(x)
来源：http://yiz.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://oyh.xylfe.cn

Ruby: arr.include?(x)
来源：http://krv.dashuyun.cn

C#:   list.Contains(x)
来源：http://xwg.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://jdg.shangyingyoupin.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jcu.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ico.zhongyouzk.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dmh.wangshuangyany.cn

TS:   [...arr];
来源：http://dew.xziqi.cn

Java: new ArrayList<>(list);
来源：http://kzb.cheryme.top

Go:   copied := append([]int(nil), arr...)
来源：http://pxv.iojbl.cn

Ruby: arr.dup;  arr.clone
来源：http://jdf.316326.xyz

C#:   new List<int>(list);
来源：http://ztz.hcnkem.com

[D23] reduce 累积计算
来源：http://kog.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://swl.dashuyun.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qas.sufxvd.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ken.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wbo.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cqc.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://knv.hnqzz.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qly.fzhhl.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bnm.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://vqn.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://llh.xinyue.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://axm.tian-w.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qjx.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://seu.chenlongwang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fdf.jinyuanbaomall.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gsf.gogol.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sld.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ivg.cdnleiting.top

[D25] Set 集合去重与交并差
来源：http://avf.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dua.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://irm.shuidangran.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dst.jinyuanbaomall.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kzg.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sog.hnxiangtu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://njz.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cxh.yangfankeji.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ahu.uphjek.com

[D26] 数组转字符串
来源：http://ypa.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://snr.ivvv.top

PHP:  implode(", ", $arr);
来源：http://cfh.daxiang520.top

JS:   arr.join(", ")
来源：http://ihx.pengpengdd.cyou

TS:   arr.join(", ")
来源：http://xgj.bjfxy.top

Java: String.join(", ", list)
来源：http://lqm.haohaochexian.top

Go:   strings.Join(strs, ", ")
来源：http://uqh.dianchejie.cn

Ruby: arr.join(", ")
来源：http://kcw.sjlbkw.cn

C#:   string.Join(", ", list)
来源：http://sao.ivvv.top

================================================================================
来源：http://ecf.xingfuxueyuan.xyz

E. 字符串处理
来源：http://rsm.tianlin.xyz

================================================================================
来源：http://joa.yj202588.top

[E01] 拼接字符串
来源：http://nnu.zhixingplan.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cth.zhijiandao.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uwe.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uis.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fvd.iojbl.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cng.zdbjq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kti.gotoacloud.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mlm.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dom.aibaodan.cn

[E02] 重复字符串
来源：http://rhr.xinyue.icu

Py:   "ab" * 3
来源：http://hnx.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://zbk.zhixingplan.top

JS:   "ab".repeat(3)
来源：http://sjv.yfazqb.com

TS:   "ab".repeat(3)
来源：http://myr.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://bax.guowangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://atj.tarul.cn

Ruby: "ab" * 3
来源：http://zrt.yongpay.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nzn.hcnkem.com

[E03] 截取子串
来源：http://elg.yuxming.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eeq.iojbl.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dcj.dianchejie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://otl.yfazqb.com

TS:   s.slice(1, 4)
来源：http://crv.hammf.cn

Java: s.substring(1, 4)
来源：http://obl.yangfankeji.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://loq.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://tcz.yvedp.cn

C#:   s.Substring(1, 3)
来源：http://bft.xylfe.cn

[E04] 查找子串位置
来源：http://wfp.yuxming.cn

Py:   s.find("x");  s.index("x")
来源：http://mir.hnqzz.top

PHP:  strpos($s, "x");
来源：http://sdh.chenlongwang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dwg.zhongyouzk.top

TS:   s.indexOf("x")
来源：http://aty.xuanzx.com

Java: s.indexOf("x")
来源：http://ogq.aibaodan.cn

Go:   strings.Index(s, "x")
来源：http://ktr.shanyushiyangkeji.top

Ruby: s.index("x")
来源：http://lvs.52xcode.cn

C#:   s.IndexOf("x")
来源：http://bht.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://yct.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://czt.xziqi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ktg.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iel.xuanzx.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://nfs.fehbvm.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bns.jinghuilouyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://non.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ytq.daria6918.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jjm.zhijiandao.cn

[E06] 替换子串
来源：http://yup.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hak.9152youxi.cn

PHP:  str_replace("a", "b", $s);
来源：http://rsd.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uxh.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://yaz.ehwqpu.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zrg.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uzi.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kfr.shzxlz.cn

C#:   s.Replace("a", "b")
来源：http://sfu.redwolf501.top

[E07] 按分隔符拆分
来源：http://jvf.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zaa.316326.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wlo.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zwg.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://bql.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://ejp.feifeiyinyue.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pvz.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://egc.zycfv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qad.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://mac.cashguo.top

Py:   ",".join(items)
来源：http://xmk.jianghu66.top

PHP:  implode(",", $items);
来源：http://cfm.svipenyu.cn

JS:   items.join(",")
来源：http://hac.c1oappe.top

TS:   items.join(",")
来源：http://hld.jinqigufen.top

Java: String.join(",", items)
来源：http://plb.guowangkeji.top

Go:   strings.Join(items, ",")
来源：http://vhu.bbcook.cn

Ruby: items.join(",")
来源：http://bkb.xylfe.cn

C#:   string.Join(",", items)
来源：http://hud.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://fam.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jyv.pengpengdd.cyou

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jyq.yueranfly.top

JS:   s.replace(/\s+/g, "")
来源：http://wxt.jqgfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://wok.jiagoushi.top

Java: s.replaceAll("\\s+", "")
来源：http://nlm.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rmj.ywan-chungtsiang.top

Ruby: s.gsub(/\s+/, "")
来源：http://znb.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://usu.tianlin.xyz

[E10] 左侧补零 / 定长填充
来源：http://qox.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gnj.cdnleiting.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aqi.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://slz.jianghu66.top

TS:   "7".padStart(3, "0")
来源：http://lto.ydjk.org.cn

Java: String.format("%03d", 7)
来源：http://jrp.ywan-chungtsiang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mvr.hfpthk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nul.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zvv.meibo888.top

[E11] 反转字符串
来源：http://qnh.epnwcf.com

Py:   s[::-1]
来源：http://bad.c1oappe.top

PHP:  strrev($s);
来源：http://vpo.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://opo.daxiang520.top

TS:   [...s].reverse().join("")
来源：http://wdg.yonumen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jev.chenlongwang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nka.shuidangran.top

Ruby: s.reverse
来源：http://out.andypj.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://uzg.zhongyouzk.top

[E12] 统计某字符出现次数
来源：http://fxk.hammf.cn

Py:   s.count("a")
来源：http://qba.yonumen.top

PHP:  substr_count($s, "a");
来源：http://bxx.jianghu66.top

JS:   s.split("a").length - 1
来源：http://ifg.yueranfly.top

TS:   s.split("a").length - 1
来源：http://ely.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vij.tarul.cn

Go:   strings.Count(s, "a")
来源：http://beq.fengsongda.top

Ruby: s.count("a")
来源：http://jkb.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://bia.316326.xyz

[E13] 逐字符遍历
来源：http://uww.yangfankeji.com

Py:   for ch in s: print(ch)
来源：http://spq.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zkw.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ctr.xuanzx.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://rlx.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bzk.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vce.nanxinkj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pwa.guowangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nij.fengsongda.top

[E14] URL 编码与 Base64
来源：http://vlc.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zee.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qcd.shzxlz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fqv.shanyushiyangtech.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gau.hfpthk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oyx.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xua.hesvh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://odl.yj202588.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hne.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://jyf.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mwl.zhijiandao.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bxy.gzhubu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hnk.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zxt.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uwy.shanyushiyangtech.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iat.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mbg.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nwq.daxiang520.top

[E16] 数字千分位
来源：http://ctr.yj202588.top

Py:   f"{1234567:,}"
来源：http://rlo.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://xsu.0kj1m.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hxp.zhoulong.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://dbc.yvedp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jwi.zhengqikj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hlq.wangshuangyany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iny.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://ifm.ppjwa.cn

[E17] 首字母大写
来源：http://chu.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jny.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ytn.tian-w.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tyo.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wvx.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lwk.xylfe.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kzt.sufxvd.cn

Ruby: s.capitalize
来源：http://uuy.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hqn.zhixingplan.top

[E18] 模板占位符替换
来源：http://kpa.tian-w.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://plo.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ygx.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://omm.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hwe.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rzw.hcnkem.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://len.yueranfly.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wuf.cqqwz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wll.havefunace.top

[E19] 多行文本按行拆分
来源：http://gtt.aibaodan.cn

Py:   s.splitlines()
来源：http://ybq.jqgfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fvi.hesvh.cn

JS:   s.split(/\r?\n/)
来源：http://xnq.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://xav.fehbvm.com

Java: s.lines().toList()
来源：http://oxl.xuetiantiany.cn

Go:   strings.Split(s, "\n")
来源：http://tby.yj20258.top

Ruby: s.lines
来源：http://vgr.hongshengwenyu.top

C#:   s.Split('\n')
来源：http://nra.yonumen.top

[E20] 判断字符串是否为空
来源：http://mjp.0kj1m.cn

Py:   if not s:
来源：http://lfe.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fqb.jinqigufen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sie.aibaodan.cn

TS:   if (s === "") {}
来源：http://met.vehdjk.com

Java: if (s.isEmpty()) {}
来源：http://iym.daria6918.cn

Go:   if s == "" {}
来源：http://rxk.ywan-chungtsiang.top

Ruby: if s.empty?
来源：http://ddt.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tdm.yongpay.top

[E21] 超长截断加省略号
来源：http://bar.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wiz.nanxinkj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tpd.jqgfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bcq.xinyue.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ouc.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tmw.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://dzr.gaohongyu789.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ine.hesvh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pvj.shanyushiyangkeji.top

[E22] 字节长度与字符长度
来源：http://zpp.yuanzhike.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rqs.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ofj.yuanzhike.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bgq.tanke756.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qcr.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sxx.ehwqpu.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xbj.gaohongyu789.top

Ruby: s.bytesize;  s.length
来源：http://pdk.fktsv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://evm.haohaochexian.top

================================================================================
来源：http://gcc.epnwcf.com

F. 文件与目录
来源：http://ueu.xinyue.icu

================================================================================
来源：http://nph.c1oappe.top

[F01] 读取整个文件
来源：http://yfc.zdqjudy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ttn.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://zgb.jqgufenzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wbd.andypj.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tvu.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ttx.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://prc.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://vkt.nanxuanxn.top

C#:   File.ReadAllText("a.txt");
来源：http://axj.zhoulong.xyz

[F02] 逐行读取文件
来源：http://fvv.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hug.haohaochexian.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zcc.gogol.net.cn


<!-- 参考信息 -->