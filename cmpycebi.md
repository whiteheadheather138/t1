代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://raa.ivvv.top

Ruby: arr.max;  arr.min
来源：http://njd.c1oappe.top

C#:   list.Max();  list.Min()
来源：http://hzf.gotoacloud.top

[D18] 扁平化嵌套数组
来源：http://com.vehdjk.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pjf.wangdashe.top

PHP:  array_merge(...$nested);
来源：http://sxn.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kln.gzhubu.top

TS:   nested.flat();
来源：http://vnh.ywan-chungtsiang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://har.jlsjyb.cn

Go:   // 手写双层循环
来源：http://zdh.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://lvr.xuetiantiany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ukf.shuidangran.top

[D19] 按字段分组
来源：http://ypg.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yaq.shanyushiyangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bhd.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qav.wangshuangyany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ori.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iir.andypj.xyz

Go:   // 手写 map[string][]T
来源：http://awa.hnqzz.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jbn.fktsv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kif.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://cdz.ppjwa.cn

Py:   Counter(arr)
来源：http://hhr.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://lwk.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://scw.svipenyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lgo.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iir.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://ynd.xinyue.icu

Ruby: arr.tally
来源：http://wxr.daria6918.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hsw.yfazqb.com

[D21] 判断是否包含某元素
来源：http://ptc.sysykeji.top

Py:   x in arr
来源：http://llm.hcnkem.com

PHP:  in_array($x, $arr, true);
来源：http://upr.yfazqb.com

JS:   arr.includes(x)
来源：http://ikj.jqgufenzy.top

TS:   arr.includes(x)
来源：http://cfv.tianlin.xyz

Java: list.contains(x)
来源：http://vqd.daria6918.cn

Go:   slices.Contains(arr, x)
来源：http://czw.snrcjt.cn

Ruby: arr.include?(x)
来源：http://xrb.shangyingyoupin.top

C#:   list.Contains(x)
来源：http://adr.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://wyz.xinyue.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ygq.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qzp.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kqi.vqdsnc.cn

TS:   [...arr];
来源：http://qai.jqgufenzy.top

Java: new ArrayList<>(list);
来源：http://lzn.hfpthk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qqp.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://tty.hnqzz.top

C#:   new List<int>(list);
来源：http://hll.yueranfly.top

[D23] reduce 累积计算
来源：http://fxj.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ezy.hcnkem.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xbd.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qjz.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.sufxvd.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ckx.yuanzhike.top

Go:   // 手写循环
来源：http://tar.mhx1999.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yxn.vqdsnc.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iuw.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://zww.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tef.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tta.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eyx.dashuyun.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tkm.jianghu66.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xvr.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qbl.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://thh.shuidangran.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qlj.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://hjj.zdbjq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ljk.jyoumei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ita.cashguo.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zyt.shuidangran.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://asl.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dfx.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rzj.hfpthk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bzb.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cxl.fengsongda.top

[D26] 数组转字符串
来源：http://pyw.bbcook.cn

Py:   ", ".join(map(str, arr))
来源：http://avs.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://yuf.iojbl.cn

JS:   arr.join(", ")
来源：http://rhj.hammf.cn

TS:   arr.join(", ")
来源：http://erk.bbcook.cn

Java: String.join(", ", list)
来源：http://uet.zhijiandao.cn

Go:   strings.Join(strs, ", ")
来源：http://vvv.ybcxt.top

Ruby: arr.join(", ")
来源：http://cme.meibo888.top

C#:   string.Join(", ", list)
来源：http://wmt.zycfv.cn

================================================================================
来源：http://umq.mhx1999.top

E. 字符串处理
来源：http://xpa.zhijiandao.cn

================================================================================
来源：http://uzq.gaohongyu789.top

[E01] 拼接字符串
来源：http://iyn.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vda.yongpay.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://quv.mhx1999.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fqw.tian-w.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kng.c1oappe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ekq.guannengcc.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tty.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ysf.meibo888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gdu.jqgufenzy.top

[E02] 重复字符串
来源：http://tfd.zhengqikj.top

Py:   "ab" * 3
来源：http://bhe.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://cqx.gogol.net.cn

JS:   "ab".repeat(3)
来源：http://jpx.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://jgi.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://tgm.xylfe.cn

Go:   strings.Repeat("ab", 3)
来源：http://dtl.kuanghao11.cn

Ruby: "ab" * 3
来源：http://urv.yongpay.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xxq.9152youxi.cn

[E03] 截取子串
来源：http://oaq.tarul.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kyb.sjlbkw.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ljx.epnwcf.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qfi.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://lwl.zhengqikj.top

Java: s.substring(1, 4)
来源：http://cvt.kuanghao11.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ohp.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://toe.52xcode.cn

C#:   s.Substring(1, 3)
来源：http://nbf.yanxiufei.cn

[E04] 查找子串位置
来源：http://amj.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://xgd.vehdjk.com

PHP:  strpos($s, "x");
来源：http://urm.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dze.yonumen.top

TS:   s.indexOf("x")
来源：http://uzo.dashuyun.cn

Java: s.indexOf("x")
来源：http://hpl.yongpay.top

Go:   strings.Index(s, "x")
来源：http://gaw.shuidangran.top

Ruby: s.index("x")
来源：http://boh.cucudq.cn

C#:   s.IndexOf("x")
来源：http://okw.jinqigfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jwm.zhengqikj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bor.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iwb.mhx1999.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hzk.gzhubu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sui.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lap.zhixingplan.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bvb.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wqu.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mqn.hcnkem.com

[E06] 替换子串
来源：http://fio.jqgufenzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qqu.hnxiangtu.top

PHP:  str_replace("a", "b", $s);
来源：http://zby.hnxiangtu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://grg.hongshengwenyu.top

TS:   s.replaceAll("a", "b")
来源：http://dgk.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://usq.aizwys.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ale.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nkh.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://trj.hfpthk.cn

[E07] 按分隔符拆分
来源：http://xdz.yvedp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zof.chenjidiqi.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wby.hongshengwenyu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cdb.haohaochexian.top

TS:   s.split(",")
来源：http://oop.shangyingyoupin.top

Java: s.split(",");  s.split("\\s+")
来源：http://zoa.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sov.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://wwb.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tzy.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://rsc.kuanghao11.cn

Py:   ",".join(items)
来源：http://gly.iojbl.cn

PHP:  implode(",", $items);
来源：http://kwi.jinyuanbaomall.cn

JS:   items.join(",")
来源：http://njv.jyoumei.cn

TS:   items.join(",")
来源：http://phm.yonumen.top

Java: String.join(",", items)
来源：http://flx.jinqigfzy.top

Go:   strings.Join(items, ",")
来源：http://ktv.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://oqn.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://lww.316326.xyz

[E09] 去除所有空白字符
来源：http://sgz.nwbrower.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kkh.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tog.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://ghs.havefunace.top

TS:   s.replace(/\s+/g, "")
来源：http://afj.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://wrl.hywenlv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ylx.yanxiufei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tgx.yvedp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://reg.daxiang520.top

[E10] 左侧补零 / 定长填充
来源：http://kxz.ybcxt.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wlk.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ujv.jqgufenzy.top

JS:   "7".padStart(3, "0")
来源：http://xml.ehwqpu.com

TS:   "7".padStart(3, "0")
来源：http://vjr.feifeiyinyue.top

Java: String.format("%03d", 7)
来源：http://srn.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vrg.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uyy.jinqigufen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ypd.chenlongwang.top

[E11] 反转字符串
来源：http://pva.gaohongyu789.top

Py:   s[::-1]
来源：http://fiv.haohaochexian.top

PHP:  strrev($s);
来源：http://met.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://mfp.zhengqikj.top

TS:   [...s].reverse().join("")
来源：http://own.yangfankeji.com

Java: new StringBuilder(s).reverse().toString()
来源：http://sfp.hnqzz.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vns.hnqzz.top

Ruby: s.reverse
来源：http://zpf.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://jib.daxiang520.top

[E12] 统计某字符出现次数
来源：http://vwf.yj20258888.top

Py:   s.count("a")
来源：http://lqz.hfpthk.cn

PHP:  substr_count($s, "a");
来源：http://ivn.yuanzhike.top

JS:   s.split("a").length - 1
来源：http://lgy.bbcook.cn

TS:   s.split("a").length - 1
来源：http://xcb.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ttz.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://mll.zhixingplan.top

Ruby: s.count("a")
来源：http://hzx.aizwys.cn

C#:   s.Count(c => c == 'a')
来源：http://xwh.guannengcc.top

[E13] 逐字符遍历
来源：http://oym.sysykeji.top

Py:   for ch in s: print(ch)
来源：http://drq.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lhv.hnxiangtu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fgg.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pxr.jianghu66.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ico.cashguo.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://psh.yj20258888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nmh.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xry.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://qpc.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://spq.yuxming.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vjy.sysykeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gyt.gzhubu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nsx.yanxiufei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zxe.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dyf.ydjk.org.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nfd.zhengqikj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tim.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://vam.meibo888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hdg.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lei.jyoumei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vna.fktsv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iop.sweek.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hcr.hongshengwenyu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tjg.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ept.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lmt.snrcjt.cn

[E16] 数字千分位
来源：http://syl.ctjpmb.com

Py:   f"{1234567:,}"
来源：http://oql.vehdjk.com

PHP:  number_format(1234567);
来源：http://fgm.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://fzo.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kbg.fanxiaobao.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dfl.zhaomingkeji.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://urw.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wkl.hongshengwenyu.top

C#:   1234567.ToString("N0")
来源：http://wqv.fehbvm.com

[E17] 首字母大写
来源：http://rmf.quarkkingdee.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qvp.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://let.yongpay.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rls.fengsongda.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lvf.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fqz.yfazqb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://crx.fehbvm.com

Ruby: s.capitalize
来源：http://hjm.zdbjq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kqq.yonumen.top

[E18] 模板占位符替换
来源：http://gcm.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ggq.yuxming.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dfe.yangfankeji.com

JS:   tpl.replaceAll("{name}", name)
来源：http://cfm.zycfv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tek.birdmap.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hsl.yfazqb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mcx.shuidangran.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gmf.nanxuanxn.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://liw.sweek.top

[E19] 多行文本按行拆分
来源：http://nrw.ybcxt.top

Py:   s.splitlines()
来源：http://ztq.zhongyouzk.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://apu.cqqwz.cn

JS:   s.split(/\r?\n/)
来源：http://ivz.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://ged.pycfn.com

Java: s.lines().toList()
来源：http://dyd.jlsjyb.cn

Go:   strings.Split(s, "\n")
来源：http://txj.pengpengdd.cyou

Ruby: s.lines
来源：http://aiu.jianghu66.top

C#:   s.Split('\n')
来源：http://xan.shangyingyoupin.top

[E20] 判断字符串是否为空
来源：http://gzg.zdbjq.cn

Py:   if not s:
来源：http://tga.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xmu.yj20258.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lcz.cqqwz.cn

TS:   if (s === "") {}
来源：http://lxu.aizwys.cn

Java: if (s.isEmpty()) {}
来源：http://fxd.chenlongwang.top

Go:   if s == "" {}
来源：http://iwv.daxiang520.top

Ruby: if s.empty?
来源：http://exp.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iof.pengpengdd.cyou

[E21] 超长截断加省略号
来源：http://gqo.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://quf.pengpengdd.cyou

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gsh.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pgo.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ijy.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xbk.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://wix.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eyh.vehdjk.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ezt.vehdjk.com

[E22] 字节长度与字符长度
来源：http://xah.jinqigufen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nzm.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qww.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pbi.zhongyouzk.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dge.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pwp.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kix.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://npg.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://glq.xingfuxueyuan.xyz

================================================================================
来源：http://yqm.ivvv.top

F. 文件与目录
来源：http://kru.wangshuangyany.cn

================================================================================
来源：http://bhc.chenzaomai.com

[F01] 读取整个文件
来源：http://cdl.xingfuxueyuan.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aqq.nanxuanxn.top

PHP:  file_get_contents("a.txt");
来源：http://erp.redwolf501.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xid.zdqjudy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uzk.zhongyouzk.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lgp.jyoumei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ych.xingfuxueyuan.xyz

Ruby: File.read("a.txt")
来源：http://fmv.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://kfj.dianchejie.cn

[F02] 逐行读取文件
来源：http://rde.zhongyouzk.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://def.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ygg.hfpthk.cn


<!-- 参考信息 -->