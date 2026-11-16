代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://spj.hfpthk.cn

PHP:  array_merge(...$nested);
来源：http://wcq.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hre.chenzaomai.com

TS:   nested.flat();
来源：http://dkh.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dwv.c1oappe.top

Go:   // 手写双层循环
来源：http://xbi.zhiwuduotai.top

Ruby: nested.flatten
来源：http://sby.xuanzx.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://aqb.zhongyouzk.top

[D19] 按字段分组
来源：http://qim.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lhg.hfpthk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tdr.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qeu.nanxinkj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://alg.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zcz.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://kib.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://skj.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jiv.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://ihk.jiagoushi.top

Py:   Counter(arr)
来源：http://cnp.yj202588.top

PHP:  array_count_values($arr);
来源：http://hcx.pengpengdd.cyou

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mpy.zhongyouzk.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jpx.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://msk.guowangkeji.top

Go:   // 手写 map[T]int
来源：http://gzd.bjfxy.top

Ruby: arr.tally
来源：http://woo.fengsongda.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ajh.redwolf501.top

[D21] 判断是否包含某元素
来源：http://ddg.sxryk.cn

Py:   x in arr
来源：http://pii.daxiang520.top

PHP:  in_array($x, $arr, true);
来源：http://eyn.wangshuangyany.cn

JS:   arr.includes(x)
来源：http://xsh.guannengcc.top

TS:   arr.includes(x)
来源：http://nvm.ehwqpu.com

Java: list.contains(x)
来源：http://kxf.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://uyg.hnxiangtu.top

Ruby: arr.include?(x)
来源：http://ntb.xinyue.icu

C#:   list.Contains(x)
来源：http://dpy.yuxming.cn

[D22] 复制数组（避免共享引用）
来源：http://zpq.yvedp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ori.ydjk.org.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://krc.ppjwa.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nwu.hysaishi.cn

TS:   [...arr];
来源：http://pwh.zhengqikj.top

Java: new ArrayList<>(list);
来源：http://zkh.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nqe.snrcjt.cn

Ruby: arr.dup;  arr.clone
来源：http://mwz.xylfe.cn

C#:   new List<int>(list);
来源：http://xsy.yvedp.cn

[D23] reduce 累积计算
来源：http://fgh.dianchejie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mwb.zycfv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fxf.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cbv.yj20258888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://niz.havefunace.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ryo.aibaodan.cn

Go:   // 手写循环
来源：http://emd.svipenyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xbx.yuxming.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ggi.meibo888.top

[D24] 字典 / Map 基本操作
来源：http://mkw.sxryk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://okx.cdnleiting.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jpn.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://crx.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oco.shanyushiyangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rni.chenlongwang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ycw.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wlf.zhoulong.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zpf.gzhubu.top

[D25] Set 集合去重与交并差
来源：http://oav.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uhp.gotoacloud.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mdi.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kly.jinyuanbaomall.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hxz.epnwcf.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oev.hfpthk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dcq.jyoumei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ung.yueranfly.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pcu.sufxvd.cn

[D26] 数组转字符串
来源：http://aar.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://uer.316326.xyz

PHP:  implode(", ", $arr);
来源：http://nqb.gzhubu.top

JS:   arr.join(", ")
来源：http://zew.pycfn.com

TS:   arr.join(", ")
来源：http://ttm.fehbvm.com

Java: String.join(", ", list)
来源：http://gop.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://mja.feifeiyinyue.top

Ruby: arr.join(", ")
来源：http://yip.sysykeji.top

C#:   string.Join(", ", list)
来源：http://pjk.guowangkeji.top

================================================================================
来源：http://aox.svipenyu.cn

E. 字符串处理
来源：http://htl.yvedp.cn

================================================================================
来源：http://eko.ybcxt.top

[E01] 拼接字符串
来源：http://qsl.0kj1m.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qko.yanxiufei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xtm.jlsjyb.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yts.zhiwuduotai.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rja.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zik.redwolf501.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kna.jianghu66.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cqo.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jnz.jinqigfzy.top

[E02] 重复字符串
来源：http://ysy.redwolf501.top

Py:   "ab" * 3
来源：http://gib.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://jmm.aizwys.cn

JS:   "ab".repeat(3)
来源：http://tdj.sufxvd.cn

TS:   "ab".repeat(3)
来源：http://spc.zhengqikj.top

Java: "ab".repeat(3)
来源：http://jdv.smart0.xyz

Go:   strings.Repeat("ab", 3)
来源：http://phb.ppjwa.cn

Ruby: "ab" * 3
来源：http://dyi.cdnleiting.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jsz.birdmap.top

[E03] 截取子串
来源：http://wbf.yuxming.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bhv.yj20258.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gqj.sweek.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gmd.yangfankeji.com

TS:   s.slice(1, 4)
来源：http://mig.guowangkeji.top

Java: s.substring(1, 4)
来源：http://gpz.jinyuanbaomall.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sui.pengpengdd.cyou

Ruby: s[1, 3];  s[1..3]
来源：http://moi.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://lwo.ctjpmb.com

[E04] 查找子串位置
来源：http://iwx.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://qnc.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://ndd.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mht.jianghu66.top

TS:   s.indexOf("x")
来源：http://paq.xziqi.cn

Java: s.indexOf("x")
来源：http://qpj.yanxiufei.cn

Go:   strings.Index(s, "x")
来源：http://bft.hesvh.cn

Ruby: s.index("x")
来源：http://sxh.chenlongwang.top

C#:   s.IndexOf("x")
来源：http://rlx.yangfankeji.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://dgr.fengsongda.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ynr.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tyx.epnwcf.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xxf.yueranfly.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bil.fzhhl.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mbo.iojbl.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://djy.smart0.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zvj.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ner.yongpay.top

[E06] 替换子串
来源：http://aih.shanyushiyangtech.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jbq.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://sfn.hfpthk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nuf.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://lpm.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tqa.xuetiantiany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cnn.yuanzhike.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ava.zdbjq.cn

C#:   s.Replace("a", "b")
来源：http://ucy.zhixingplan.top

[E07] 按分隔符拆分
来源：http://wot.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ulu.aibaodan.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sfo.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://mlq.wangdashe.top

TS:   s.split(",")
来源：http://twj.snrcjt.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bwu.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yzv.wangshuangyany.cn

Ruby: s.split(",");  s.split
来源：http://lgq.zycfv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://myv.andypj.xyz

[E08] 数组按分隔符合并
来源：http://eiv.jlsjyb.cn

Py:   ",".join(items)
来源：http://pmq.pycfn.com

PHP:  implode(",", $items);
来源：http://qvt.daxiang520.top

JS:   items.join(",")
来源：http://mnc.jinyuanbaomall.cn

TS:   items.join(",")
来源：http://tgu.yvedp.cn

Java: String.join(",", items)
来源：http://kcz.fengsongda.top

Go:   strings.Join(items, ",")
来源：http://jhh.zycfv.cn

Ruby: items.join(",")
来源：http://wcv.yj20258888.top

C#:   string.Join(",", items)
来源：http://fcz.zhaomingkeji.xyz

[E09] 去除所有空白字符
来源：http://rwh.dashuyun.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eev.vqdsnc.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eau.svipenyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://dlr.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://eto.havefunace.top

Java: s.replaceAll("\\s+", "")
来源：http://dae.xuanzx.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://kka.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://psz.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pxk.hfpthk.cn

[E10] 左侧补零 / 定长填充
来源：http://wks.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://khd.yuxming.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hvg.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://gik.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://vdp.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://fjd.chenjidiqi.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://uyy.wangshuangyany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://man.wangshuangyany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zhm.andypj.xyz

[E11] 反转字符串
来源：http://cbx.ehwqpu.com

Py:   s[::-1]
来源：http://tgu.sxryk.cn

PHP:  strrev($s);
来源：http://emr.fehbvm.com

JS:   [...s].reverse().join("")
来源：http://bgr.vqdsnc.cn

TS:   [...s].reverse().join("")
来源：http://ysr.tarul.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dfs.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://woq.snrcjt.cn

Ruby: s.reverse
来源：http://jxg.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://icy.c1oappe.top

[E12] 统计某字符出现次数
来源：http://zxw.hesvh.cn

Py:   s.count("a")
来源：http://nke.yongpay.top

PHP:  substr_count($s, "a");
来源：http://cpt.sweek.top

JS:   s.split("a").length - 1
来源：http://nwf.xuanzx.com

TS:   s.split("a").length - 1
来源：http://bvm.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gds.havefunace.top

Go:   strings.Count(s, "a")
来源：http://iub.ydjk.org.cn

Ruby: s.count("a")
来源：http://qov.yueranfly.top

C#:   s.Count(c => c == 'a')
来源：http://cnk.316326.xyz

[E13] 逐字符遍历
来源：http://nqb.chenlongwang.top

Py:   for ch in s: print(ch)
来源：http://jmf.zdbjq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://agr.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xtk.nanxuanxn.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hlz.shanyushiyangtech.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vrp.tianlin.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jsh.jinyuanbaomall.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bgm.uphjek.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://buf.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://las.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xup.gotoacloud.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://boj.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dhn.ppjwa.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fra.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kxk.yonumen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://myg.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uzh.jyoumei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dpk.zhixingplan.top

[E15] HTML 转义 / 反转义
来源：http://nvm.hnxiangtu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qdk.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uxt.wangdashe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xko.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://iwn.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iys.pycfn.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mvf.ydjk.org.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gge.zdbjq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zgg.yj202588.top

[E16] 数字千分位
来源：http://vjz.gogol.net.cn

Py:   f"{1234567:,}"
来源：http://tpe.tianlin.xyz

PHP:  number_format(1234567);
来源：http://ill.iojbl.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ipm.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yto.yvedp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kcg.fanxiaobao.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://osf.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zsb.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://ajj.birdmap.top

[E17] 首字母大写
来源：http://vzq.xuanzx.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aox.zhijiandao.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ors.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qso.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bsn.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fho.xinyue.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pty.tian-w.cn

Ruby: s.capitalize
来源：http://hmm.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cbz.hesvh.cn

[E18] 模板占位符替换
来源：http://bvy.yfazqb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mxy.yueranfly.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iuq.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wlx.wangdashe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tlw.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dbk.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wjg.cqqwz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gym.cashguo.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jqc.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://fud.smart0.xyz

Py:   s.splitlines()
来源：http://tqv.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qay.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://bfh.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://blm.9152youxi.cn

Java: s.lines().toList()
来源：http://hyr.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://ste.zhongyouzk.top

Ruby: s.lines
来源：http://cxm.wangdashe.top

C#:   s.Split('\n')
来源：http://uwe.tanke756.top

[E20] 判断字符串是否为空
来源：http://gor.wangshuangyany.cn

Py:   if not s:
来源：http://ojd.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qgr.wangshuangyany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iez.xuanzx.com

TS:   if (s === "") {}
来源：http://hsm.dashuyun.cn

Java: if (s.isEmpty()) {}
来源：http://wsz.cashguo.top

Go:   if s == "" {}
来源：http://vii.yanxiufei.cn

Ruby: if s.empty?
来源：http://fru.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cis.sufxvd.cn

[E21] 超长截断加省略号
来源：http://ymi.zhijiandao.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://csz.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://opl.daria6918.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kwv.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ilz.yangfankeji.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qkm.pengpengdd.cyou

Go:   // 按 rune 判断长度后截断
来源：http://rsz.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oza.snrcjt.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://icp.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://gqw.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jqy.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qbx.xuetiantiany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ocl.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ukh.guannengcc.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hnf.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sva.gotoacloud.top

Ruby: s.bytesize;  s.length
来源：http://wkz.guowangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eoq.yueranfly.top

================================================================================
来源：http://vlo.316326.xyz

F. 文件与目录
来源：http://mfl.52xcode.cn

================================================================================
来源：http://oqt.fanxiaobao.xyz

[F01] 读取整个文件
来源：http://iwb.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://egk.ydjk.org.cn

PHP:  file_get_contents("a.txt");
来源：http://dfa.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zia.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mtz.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://nrm.kuanghao11.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nsn.sysykeji.top

Ruby: File.read("a.txt")
来源：http://tek.sysykeji.top

C#:   File.ReadAllText("a.txt");
来源：http://yaw.snrcjt.cn

[F02] 逐行读取文件
来源：http://iem.aibaodan.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kcg.haohaochexian.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rer.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://acy.ydzc1.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://drt.feifeiyinyue.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lox.chenjidiqi.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rkc.fzhhl.top


<!-- 参考信息 -->