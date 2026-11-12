代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zew.dianchejie.cn

PHP:  array_merge(...$nested);
来源：http://cuv.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://juw.hnxiangtu.top

TS:   nested.flat();
来源：http://hgb.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://twx.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://kle.gotoacloud.top

Ruby: nested.flatten
来源：http://bfs.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://ohv.daxiang520.top

[D19] 按字段分组
来源：http://cup.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lkk.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yjr.xuanzx.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://icm.fehbvm.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://dva.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kvz.shuidangran.top

Go:   // 手写 map[string][]T
来源：http://rqi.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jpt.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ppu.epnwcf.com

[D20] 统计每个元素出现次数
来源：http://cdu.fzhhl.top

Py:   Counter(arr)
来源：http://mzo.pycfn.com

PHP:  array_count_values($arr);
来源：http://zdj.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nrd.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lrj.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bxr.bjfxy.top

Go:   // 手写 map[T]int
来源：http://aev.yangfankeji.com

Ruby: arr.tally
来源：http://wgn.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://msy.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://ndd.gaohongyu789.top

Py:   x in arr
来源：http://mnd.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://qcc.c1oappe.top

JS:   arr.includes(x)
来源：http://smz.jqgfzy.top

TS:   arr.includes(x)
来源：http://vpz.daxiang520.top

Java: list.contains(x)
来源：http://zjx.wangdashe.top

Go:   slices.Contains(arr, x)
来源：http://czy.gogol.net.cn

Ruby: arr.include?(x)
来源：http://dhv.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://uic.sxryk.cn

[D22] 复制数组（避免共享引用）
来源：http://ske.jianghu66.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pgp.dashuyun.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://shb.yanxiufei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dje.yuanzhike.top

TS:   [...arr];
来源：http://rgb.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://rwf.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://bor.cucudq.cn

Ruby: arr.dup;  arr.clone
来源：http://jzg.hcnkem.com

C#:   new List<int>(list);
来源：http://fud.nwbrower.top

[D23] reduce 累积计算
来源：http://bpx.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sqp.9152youxi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://teg.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wuc.birdmap.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rnw.hcnkem.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://sws.zycfv.cn

Go:   // 手写循环
来源：http://yxb.jinghuilouyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xnv.kuanghao11.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cmy.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://xdy.yj20258888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jcq.gotoacloud.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uft.hesvh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wjk.hammf.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xht.smart0.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://piy.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lkt.ywan-chungtsiang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ulz.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iiz.xuanzx.com

[D25] Set 集合去重与交并差
来源：http://sjo.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uia.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://etp.cheryme.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gmp.aizwys.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nqt.havefunace.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://arw.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ddn.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://srh.redwolf501.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://koc.vqdsnc.cn

[D26] 数组转字符串
来源：http://ugn.smart0.xyz

Py:   ", ".join(map(str, arr))
来源：http://qpy.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://mrx.chenzaomai.com

JS:   arr.join(", ")
来源：http://rkq.redwolf501.top

TS:   arr.join(", ")
来源：http://wdv.yangfankeji.com

Java: String.join(", ", list)
来源：http://cbq.bbcook.cn

Go:   strings.Join(strs, ", ")
来源：http://hbs.zycfv.cn

Ruby: arr.join(", ")
来源：http://clr.jyoumei.cn

C#:   string.Join(", ", list)
来源：http://fee.dianchejie.cn

================================================================================
来源：http://xeq.yangfankeji.com

E. 字符串处理
来源：http://nrz.guannengcc.top

================================================================================
来源：http://lns.zhaomingkeji.xyz

[E01] 拼接字符串
来源：http://dyp.snrcjt.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fzj.jinghuilouyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sst.vqdsnc.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wyb.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cka.hnqzz.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uyk.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ods.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bgn.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://itn.zhaomingkeji.xyz

[E02] 重复字符串
来源：http://kbu.nanxinkj.top

Py:   "ab" * 3
来源：http://kuc.tian-w.cn

PHP:  str_repeat("ab", 3);
来源：http://gae.zdqjudy.top

JS:   "ab".repeat(3)
来源：http://gpi.tianlin.xyz

TS:   "ab".repeat(3)
来源：http://mte.pycfn.com

Java: "ab".repeat(3)
来源：http://ykg.chenzaomai.com

Go:   strings.Repeat("ab", 3)
来源：http://jtr.gaohongyu789.top

Ruby: "ab" * 3
来源：http://smk.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tmk.sweek.top

[E03] 截取子串
来源：http://twe.fktsv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://idm.gotoacloud.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xzw.jinyuanbaomall.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vwq.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://tfe.sufxvd.cn

Java: s.substring(1, 4)
来源：http://vle.vehdjk.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bqr.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://fje.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://jyd.yanxiufei.cn

[E04] 查找子串位置
来源：http://ecz.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://nbv.chenzaomai.com

PHP:  strpos($s, "x");
来源：http://rtp.jiagoushi.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://obn.yonumen.top

TS:   s.indexOf("x")
来源：http://qof.9152youxi.cn

Java: s.indexOf("x")
来源：http://bng.zhijiandao.cn

Go:   strings.Index(s, "x")
来源：http://cus.sufxvd.cn

Ruby: s.index("x")
来源：http://nyw.bbcook.cn

C#:   s.IndexOf("x")
来源：http://wmq.guowangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zal.feifeiyinyue.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xqb.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lzx.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dse.jlsjyb.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hbi.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qnr.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ycd.gzhubu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ejm.jlsjyb.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ayb.jinghuilouyu.cn

[E06] 替换子串
来源：http://coq.zycfv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://meu.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://auq.gotoacloud.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fsf.xingfuxueyuan.xyz

TS:   s.replaceAll("a", "b")
来源：http://mld.zhiwuduotai.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mes.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cgx.cqqwz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://osi.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://kwl.hnqzz.top

[E07] 按分隔符拆分
来源：http://kbb.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vga.jqgufenzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tcl.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oef.yuanzhike.top

TS:   s.split(",")
来源：http://hrx.yj20258.top

Java: s.split(",");  s.split("\\s+")
来源：http://bbf.jqgufenzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dgj.feifeiyinyue.top

Ruby: s.split(",");  s.split
来源：http://wdr.gzhubu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aen.yueranfly.top

[E08] 数组按分隔符合并
来源：http://ooi.meibo888.top

Py:   ",".join(items)
来源：http://qeb.wangdashe.top

PHP:  implode(",", $items);
来源：http://tov.pycfn.com

JS:   items.join(",")
来源：http://peu.fanxiaobao.xyz

TS:   items.join(",")
来源：http://mcp.aizwys.cn

Java: String.join(",", items)
来源：http://rtm.chenlongwang.top

Go:   strings.Join(items, ",")
来源：http://hji.jianghu66.top

Ruby: items.join(",")
来源：http://zdc.yj202588.top

C#:   string.Join(",", items)
来源：http://ais.fengsongda.top

[E09] 去除所有空白字符
来源：http://jyo.chenjidiqi.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zpq.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jfk.xingfuxueyuan.xyz

JS:   s.replace(/\s+/g, "")
来源：http://snk.zdqjudy.top

TS:   s.replace(/\s+/g, "")
来源：http://wfe.hnxiangtu.top

Java: s.replaceAll("\\s+", "")
来源：http://tis.aizwys.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fbh.fanxiaobao.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://zos.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jcf.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://wdf.zhongyouzk.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jzv.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bmu.zhengqikj.top

JS:   "7".padStart(3, "0")
来源：http://nqa.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://tpv.jlsjyb.cn

Java: String.format("%03d", 7)
来源：http://ygc.tarul.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sfl.fzhhl.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://haa.wangshuangyany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ghe.feifeiyinyue.top

[E11] 反转字符串
来源：http://who.yfazqb.com

Py:   s[::-1]
来源：http://reb.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://ihn.dianchejie.cn

JS:   [...s].reverse().join("")
来源：http://szo.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://pdl.sweek.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rfn.haohaochexian.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jaj.guowangkeji.top

Ruby: s.reverse
来源：http://gna.vehdjk.com

C#:   new string(s.Reverse().ToArray())
来源：http://mzw.cdnleiting.top

[E12] 统计某字符出现次数
来源：http://zdy.jqgufenzy.top

Py:   s.count("a")
来源：http://cys.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://aqv.epnwcf.com

JS:   s.split("a").length - 1
来源：http://kqq.hysaishi.cn

TS:   s.split("a").length - 1
来源：http://bod.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rkp.pengpengdd.cyou

Go:   strings.Count(s, "a")
来源：http://nnm.sweek.top

Ruby: s.count("a")
来源：http://tcw.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://rem.ybcxt.top

[E13] 逐字符遍历
来源：http://pre.jqgufenzy.top

Py:   for ch in s: print(ch)
来源：http://hef.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dkt.ydzc1.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://deq.gogol.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uas.0kj1m.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sgd.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wba.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://awr.wangdashe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://trw.bjfxy.top

[E14] URL 编码与 Base64
来源：http://ljz.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iqv.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://twy.jinqigfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://quh.bbcook.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dvv.mhx1999.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fep.ywan-chungtsiang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xdm.ppjwa.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gcn.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pzo.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://owv.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tze.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xpm.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kth.zhiwuduotai.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tcw.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://swu.nanxuanxn.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://otl.zdbjq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xlg.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jgx.gogol.net.cn

[E16] 数字千分位
来源：http://dcn.fehbvm.com

Py:   f"{1234567:,}"
来源：http://dzb.shanyushiyangtech.top

PHP:  number_format(1234567);
来源：http://ibu.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sxb.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wvq.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ajz.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pso.xinyue.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vdf.havefunace.top

C#:   1234567.ToString("N0")
来源：http://wgm.vehdjk.com

[E17] 首字母大写
来源：http://qft.vehdjk.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ker.ybcxt.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yit.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tca.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tum.hammf.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://irj.yvedp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fzw.shzxlz.cn

Ruby: s.capitalize
来源：http://xzv.zhengqikj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jbl.gogol.net.cn

[E18] 模板占位符替换
来源：http://sce.tarul.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://azb.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mpc.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hpd.yangfankeji.com

TS:   tpl.replaceAll("{name}", name)
来源：http://dxp.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://add.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ycv.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vyt.zhiwuduotai.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kjg.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://knl.aibaodan.cn

Py:   s.splitlines()
来源：http://jjq.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qyk.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://lzk.nwbrower.top

TS:   s.split(/\r?\n/)
来源：http://drf.smart0.xyz

Java: s.lines().toList()
来源：http://yfk.shzxlz.cn

Go:   strings.Split(s, "\n")
来源：http://mjv.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://ikb.chenlongwang.top

C#:   s.Split('\n')
来源：http://neq.hnqzz.top

[E20] 判断字符串是否为空
来源：http://rwj.yuxming.cn

Py:   if not s:
来源：http://oho.hnxiangtu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mnd.hesvh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bpb.xylfe.cn

TS:   if (s === "") {}
来源：http://gox.sysykeji.top

Java: if (s.isEmpty()) {}
来源：http://hwm.xylfe.cn

Go:   if s == "" {}
来源：http://irk.xingfuxueyuan.xyz

Ruby: if s.empty?
来源：http://exu.tianlin.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xep.yangfankeji.com

[E21] 超长截断加省略号
来源：http://ssl.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xop.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jzh.hnqzz.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rbm.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aqz.hfpthk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ltf.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://gtv.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hxs.tarul.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ejp.hammf.cn

[E22] 字节长度与字符长度
来源：http://svi.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ljo.52xcode.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rgk.zhongyouzk.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://heb.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rig.xuanzx.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://efs.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pvh.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://cqt.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yty.sweek.top

================================================================================
来源：http://ygq.havefunace.top

F. 文件与目录
来源：http://uzd.mhx1999.top

================================================================================
来源：http://fdz.sufxvd.cn

[F01] 读取整个文件
来源：http://tps.hfpthk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wzx.tianlin.xyz

PHP:  file_get_contents("a.txt");
来源：http://qlm.yongpay.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oep.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oyj.sjlbkw.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://icp.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hco.fehbvm.com

Ruby: File.read("a.txt")
来源：http://tvo.tian-w.cn

C#:   File.ReadAllText("a.txt");
来源：http://evs.zhoulong.xyz

[F02] 逐行读取文件
来源：http://nwi.shzxlz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://plj.ydjk.org.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dtm.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://usa.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tng.gotoacloud.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ztx.hnqzz.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sap.jyoumei.cn


<!-- 参考信息 -->