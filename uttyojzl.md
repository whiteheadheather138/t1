代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://rer.jiagoushi.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iwc.zhixingplan.top

TS:   Math.max(...arr);
来源：http://mpj.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jxy.0kj1m.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ovs.pycfn.com

Ruby: arr.max;  arr.min
来源：http://vke.ywan-chungtsiang.top

C#:   list.Max();  list.Min()
来源：http://yng.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://ovw.chenjidiqi.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bwm.ctjpmb.com

PHP:  array_merge(...$nested);
来源：http://ovw.andypj.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ody.zhaomingkeji.xyz

TS:   nested.flat();
来源：http://pdi.hfpthk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dzd.yanxiufei.cn

Go:   // 手写双层循环
来源：http://qot.ydzc1.top

Ruby: nested.flatten
来源：http://qkp.sysykeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ykv.xuanzx.com

[D19] 按字段分组
来源：http://pfq.pycfn.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ugl.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cuw.bbcook.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nzx.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bua.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bfe.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://nap.xziqi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mml.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oen.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://lqo.cqqwz.cn

Py:   Counter(arr)
来源：http://suf.wangdashe.top

PHP:  array_count_values($arr);
来源：http://aeh.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lke.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dso.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lew.jyoumei.cn

Go:   // 手写 map[T]int
来源：http://lem.0kj1m.cn

Ruby: arr.tally
来源：http://ovj.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kwi.wangdashe.top

[D21] 判断是否包含某元素
来源：http://ccb.hysaishi.cn

Py:   x in arr
来源：http://epz.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://slb.ywan-chungtsiang.top

JS:   arr.includes(x)
来源：http://rqh.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://ups.yj20258.top

Java: list.contains(x)
来源：http://iew.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://gaw.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://kpa.wangshuangyany.cn

C#:   list.Contains(x)
来源：http://pbb.birdmap.top

[D22] 复制数组（避免共享引用）
来源：http://oxa.jinyuanbaomall.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pxb.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vdb.zdbjq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fqd.hongshengwenyu.top

TS:   [...arr];
来源：http://pcg.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://prb.yuanzhike.top

Go:   copied := append([]int(nil), arr...)
来源：http://opc.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://mjx.9152youxi.cn

C#:   new List<int>(list);
来源：http://sdo.bjfxy.top

[D23] reduce 累积计算
来源：http://jpu.hnqzz.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://diz.yfazqb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aax.zdqjudy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bcl.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dvt.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://irn.zhongyouzk.top

Go:   // 手写循环
来源：http://mfa.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zek.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oyg.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://fjx.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nry.redwolf501.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wle.pycfn.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jad.c1oappe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hmx.iojbl.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mhe.gogol.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qbf.zhixingplan.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wty.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eti.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://fho.jinqigfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kyt.cqqwz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qvl.xuetiantiany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zwr.yanxiufei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yfi.hywenlv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hwg.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://onx.shzxlz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ibr.yueranfly.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gam.wangdashe.top

[D26] 数组转字符串
来源：http://biz.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://sww.yangfankeji.com

PHP:  implode(", ", $arr);
来源：http://dem.vqdsnc.cn

JS:   arr.join(", ")
来源：http://gif.cdnleiting.top

TS:   arr.join(", ")
来源：http://rzx.shzxlz.cn

Java: String.join(", ", list)
来源：http://mbu.tian-w.cn

Go:   strings.Join(strs, ", ")
来源：http://qti.cqqwz.cn

Ruby: arr.join(", ")
来源：http://vyf.tanke756.top

C#:   string.Join(", ", list)
来源：http://rkd.shangyingyoupin.top

================================================================================
来源：http://arr.hywenlv.cn

E. 字符串处理
来源：http://epb.sufxvd.cn

================================================================================
来源：http://vhe.daxiang520.top

[E01] 拼接字符串
来源：http://uem.bjfxy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pfp.hywenlv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qzz.fanxiaobao.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hyk.xuetiantiany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://skv.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vgn.feifeiyinyue.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eer.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qyr.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rlx.aizwys.cn

[E02] 重复字符串
来源：http://xip.jiagoushi.top

Py:   "ab" * 3
来源：http://rgw.0kj1m.cn

PHP:  str_repeat("ab", 3);
来源：http://rdh.xziqi.cn

JS:   "ab".repeat(3)
来源：http://pqh.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://fug.meibo888.top

Java: "ab".repeat(3)
来源：http://dza.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://aap.cheryme.top

Ruby: "ab" * 3
来源：http://srn.yj202588.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dcn.cheryme.top

[E03] 截取子串
来源：http://fns.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://anx.bbcook.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iwf.birdmap.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fvz.jqgufenzy.top

TS:   s.slice(1, 4)
来源：http://zgn.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://uct.hfpthk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://djv.9152youxi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ipo.zdbjq.cn

C#:   s.Substring(1, 3)
来源：http://uzi.hysaishi.cn

[E04] 查找子串位置
来源：http://cml.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://jnm.snrcjt.cn

PHP:  strpos($s, "x");
来源：http://gtm.guowangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ebw.daxiang520.top

TS:   s.indexOf("x")
来源：http://kdu.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://mgm.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://jif.yangfankeji.com

Ruby: s.index("x")
来源：http://dyf.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://hjx.andypj.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://rdd.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dib.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://exh.cdnleiting.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lng.jinyuanbaomall.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fkr.fzhhl.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://syt.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uuf.316326.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vuh.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hvj.wangshuangyany.cn

[E06] 替换子串
来源：http://zkn.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nnz.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://dax.yj20258888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xsf.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://ysl.9152youxi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rqr.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eii.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ehu.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://vvu.tanke756.top

[E07] 按分隔符拆分
来源：http://nvl.yongpay.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ubf.pengpengdd.cyou

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://djw.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dsw.zycfv.cn

TS:   s.split(",")
来源：http://uxh.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vnn.hammf.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jdb.xylfe.cn

Ruby: s.split(",");  s.split
来源：http://xvw.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jjs.gogol.net.cn

[E08] 数组按分隔符合并
来源：http://exw.9152youxi.cn

Py:   ",".join(items)
来源：http://csx.svipenyu.cn

PHP:  implode(",", $items);
来源：http://ywf.jqgfzy.top

JS:   items.join(",")
来源：http://ohq.zhengqikj.top

TS:   items.join(",")
来源：http://tvf.guannengcc.top

Java: String.join(",", items)
来源：http://spi.zycfv.cn

Go:   strings.Join(items, ",")
来源：http://uaa.daria6918.cn

Ruby: items.join(",")
来源：http://sjf.jinqigufen.top

C#:   string.Join(",", items)
来源：http://khg.zhijiandao.cn

[E09] 去除所有空白字符
来源：http://mii.jinghuilouyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://van.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fnr.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://dot.quarkkingdee.top

TS:   s.replace(/\s+/g, "")
来源：http://aeu.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://dvb.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xue.wangshuangyany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://flg.shangyingyoupin.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gca.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://tei.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ozj.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zsv.jqgfzy.top

JS:   "7".padStart(3, "0")
来源：http://mqf.yj20258.top

TS:   "7".padStart(3, "0")
来源：http://zyf.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://ema.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xze.cdnleiting.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jhz.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wgg.cucudq.cn

[E11] 反转字符串
来源：http://ktj.ehwqpu.com

Py:   s[::-1]
来源：http://xah.nanxuanxn.top

PHP:  strrev($s);
来源：http://szt.dianchejie.cn

JS:   [...s].reverse().join("")
来源：http://hme.snrcjt.cn

TS:   [...s].reverse().join("")
来源：http://oxz.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bsq.wangshuangyany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://aaz.daria6918.cn

Ruby: s.reverse
来源：http://coj.shuidangran.top

C#:   new string(s.Reverse().ToArray())
来源：http://nzl.cashguo.top

[E12] 统计某字符出现次数
来源：http://fga.guannengcc.top

Py:   s.count("a")
来源：http://rag.hongshengwenyu.top

PHP:  substr_count($s, "a");
来源：http://hwz.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://dav.fengsongda.top

TS:   s.split("a").length - 1
来源：http://qan.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ogs.cashguo.top

Go:   strings.Count(s, "a")
来源：http://xkn.ctjpmb.com

Ruby: s.count("a")
来源：http://lip.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://hmi.xziqi.cn

[E13] 逐字符遍历
来源：http://xqf.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://ixh.hysaishi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sxj.tarul.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pzz.zhaomingkeji.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://dif.yuanzhike.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lmo.ivvv.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ftg.xuetiantiany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gtm.nanxuanxn.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://evo.guannengcc.top

[E14] URL 编码与 Base64
来源：http://spn.ivvv.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gaz.havefunace.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dfb.sysykeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eru.gzhubu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kzr.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tfs.yonumen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://drd.xuetiantiany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gds.xziqi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rih.hywenlv.cn

[E15] HTML 转义 / 反转义
来源：http://mwj.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kyk.zhengqikj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jqf.bbcook.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fpn.cheryme.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kix.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rdg.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xnh.tarul.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qbj.cdnleiting.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yqf.jqgfzy.top

[E16] 数字千分位
来源：http://jxl.iojbl.cn

Py:   f"{1234567:,}"
来源：http://zlu.gogol.net.cn

PHP:  number_format(1234567);
来源：http://mic.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cnt.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://ecb.zdqjudy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mrd.daria6918.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://svp.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bhw.yj202588.top

C#:   1234567.ToString("N0")
来源：http://eta.nanxinkj.top

[E17] 首字母大写
来源：http://hvb.hfpthk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://col.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bpj.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tjt.tian-w.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qbg.zycfv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://koj.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vou.nanxinkj.top

Ruby: s.capitalize
来源：http://dkv.zhijiandao.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sux.zhiwuduotai.top

[E18] 模板占位符替换
来源：http://urh.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ppy.mhx1999.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ilj.sysykeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lou.yj20258888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xvh.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wlc.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bug.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zge.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://awp.yangfankeji.com

[E19] 多行文本按行拆分
来源：http://jql.ehwqpu.com

Py:   s.splitlines()
来源：http://uvv.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tdl.cheryme.top

JS:   s.split(/\r?\n/)
来源：http://wkt.cdnleiting.top

TS:   s.split(/\r?\n/)
来源：http://yel.andypj.xyz

Java: s.lines().toList()
来源：http://hbh.yj20258888.top

Go:   strings.Split(s, "\n")
来源：http://cdj.guannengcc.top

Ruby: s.lines
来源：http://sym.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://emj.xziqi.cn

[E20] 判断字符串是否为空
来源：http://hvz.smart0.xyz

Py:   if not s:
来源：http://ikr.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ixb.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://snr.xuetiantiany.cn

TS:   if (s === "") {}
来源：http://kgk.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://mxy.hongshengwenyu.top

Go:   if s == "" {}
来源：http://zzi.snrcjt.cn

Ruby: if s.empty?
来源：http://vxq.jianghu66.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jji.tian-w.cn

[E21] 超长截断加省略号
来源：http://lzo.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hnn.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vhl.fzhhl.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://afw.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lms.vqdsnc.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://erh.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://zyd.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fat.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dyp.dashuyun.cn

[E22] 字节长度与字符长度
来源：http://txz.sysykeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://csf.shanyushiyangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nyj.cucudq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gla.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fvo.gaohongyu789.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wgw.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hkv.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://bci.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vhy.tanke756.top

================================================================================
来源：http://pmf.zhaomingkeji.xyz

F. 文件与目录
来源：http://adm.shangyingyoupin.top

================================================================================
来源：http://hmq.jiagoushi.top

[F01] 读取整个文件
来源：http://iar.fanxiaobao.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cxv.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://tnq.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jju.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cgh.shzxlz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eov.c1oappe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yxq.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://kmu.zhixingplan.top


<!-- 参考信息 -->