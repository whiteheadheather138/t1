代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://key.zhongyouzk.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://goo.yonumen.top

TS:   Math.max(...arr);
来源：http://bqz.shanyushiyangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ndl.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rsv.jlsjyb.cn

Ruby: arr.max;  arr.min
来源：http://ocq.xinyue.icu

C#:   list.Max();  list.Min()
来源：http://wvm.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://sqm.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://twp.shangyingyoupin.top

PHP:  array_merge(...$nested);
来源：http://bwq.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hnl.hammf.cn

TS:   nested.flat();
来源：http://nmp.redwolf501.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zed.gaohongyu789.top

Go:   // 手写双层循环
来源：http://ddy.nwbrower.top

Ruby: nested.flatten
来源：http://nsf.hnqzz.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qeq.xinyue.icu

[D19] 按字段分组
来源：http://top.c1oappe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pfc.bbcook.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://azl.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lzl.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ocp.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qep.0kj1m.cn

Go:   // 手写 map[string][]T
来源：http://guh.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://app.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wle.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://osn.hongshengwenyu.top

Py:   Counter(arr)
来源：http://dzo.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://poc.gogol.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ssy.0kj1m.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mqw.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qwd.ybcxt.top

Go:   // 手写 map[T]int
来源：http://eug.aibaodan.cn

Ruby: arr.tally
来源：http://ask.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://spz.daxiang520.top

[D21] 判断是否包含某元素
来源：http://ivk.zdqjudy.top

Py:   x in arr
来源：http://kro.cashguo.top

PHP:  in_array($x, $arr, true);
来源：http://exi.ydzc1.top

JS:   arr.includes(x)
来源：http://mjd.bjfxy.top

TS:   arr.includes(x)
来源：http://ymk.yfazqb.com

Java: list.contains(x)
来源：http://lkl.pycfn.com

Go:   slices.Contains(arr, x)
来源：http://gjj.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://qlb.zhengqikj.top

C#:   list.Contains(x)
来源：http://rwq.aizwys.cn

[D22] 复制数组（避免共享引用）
来源：http://uxc.jqgufenzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qzl.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hox.pengpengdd.cyou

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rpp.uphjek.com

TS:   [...arr];
来源：http://avd.tian-w.cn

Java: new ArrayList<>(list);
来源：http://cug.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://dww.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://pko.epnwcf.com

C#:   new List<int>(list);
来源：http://zuk.haohaochexian.top

[D23] reduce 累积计算
来源：http://vqu.shanyushiyangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cpx.aizwys.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hhr.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ozd.tarul.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tpv.jlsjyb.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cyl.dianchejie.cn

Go:   // 手写循环
来源：http://uin.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kph.chenzaomai.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://scu.c1oappe.top

[D24] 字典 / Map 基本操作
来源：http://rsz.yuxming.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zyg.wangdashe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tgc.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xis.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cpc.daxiang520.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ezn.quarkkingdee.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ahd.snrcjt.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ike.xingfuxueyuan.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fjn.daxiang520.top

[D25] Set 集合去重与交并差
来源：http://irk.hnqzz.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mfy.ydzc1.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://upi.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://azk.yj20258888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mef.yj20258.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qty.chenzaomai.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kem.wangshuangyany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lzz.fengsongda.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rwi.jianghu66.top

[D26] 数组转字符串
来源：http://eyp.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://xzw.vqdsnc.cn

PHP:  implode(", ", $arr);
来源：http://olh.sysykeji.top

JS:   arr.join(", ")
来源：http://wmv.cdnleiting.top

TS:   arr.join(", ")
来源：http://viv.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://vlj.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://oft.iojbl.cn

Ruby: arr.join(", ")
来源：http://cpg.andypj.xyz

C#:   string.Join(", ", list)
来源：http://znh.shanyushiyangtech.top

================================================================================
来源：http://gpq.chenjidiqi.icu

E. 字符串处理
来源：http://zuz.52xcode.cn

================================================================================
来源：http://esl.xuetiantiany.cn

[E01] 拼接字符串
来源：http://jql.yj20258.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://swv.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uad.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qzn.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://toz.wangshuangyany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vjq.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://giw.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lfm.yj202588.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eye.chenlongwang.top

[E02] 重复字符串
来源：http://rcf.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://jhz.c1oappe.top

PHP:  str_repeat("ab", 3);
来源：http://fvf.cucudq.cn

JS:   "ab".repeat(3)
来源：http://erh.chenzaomai.com

TS:   "ab".repeat(3)
来源：http://mwv.svipenyu.cn

Java: "ab".repeat(3)
来源：http://yyu.kuanghao11.cn

Go:   strings.Repeat("ab", 3)
来源：http://rfo.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://vrt.guowangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mpi.zhengqikj.top

[E03] 截取子串
来源：http://yap.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zvp.xuetiantiany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xls.yj20258.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nez.tanke756.top

TS:   s.slice(1, 4)
来源：http://xqo.yj20258.top

Java: s.substring(1, 4)
来源：http://mmf.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://opc.jqgfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://qok.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://gdh.fehbvm.com

[E04] 查找子串位置
来源：http://tbe.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://ogi.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://dbe.0kj1m.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xgt.gogol.net.cn

TS:   s.indexOf("x")
来源：http://kry.ehwqpu.com

Java: s.indexOf("x")
来源：http://swf.shangyingyoupin.top

Go:   strings.Index(s, "x")
来源：http://efk.tian-w.cn

Ruby: s.index("x")
来源：http://mkw.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://gtb.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://xfr.jinqigfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blu.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fib.pycfn.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wqj.yueranfly.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gdu.xinyue.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wqf.nwbrower.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ezm.316326.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ncy.cashguo.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pyg.xziqi.cn

[E06] 替换子串
来源：http://cgv.kuanghao11.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ynx.hywenlv.cn

PHP:  str_replace("a", "b", $s);
来源：http://tbb.jiagoushi.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lpk.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://xbq.sufxvd.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fhp.52xcode.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://onn.yfazqb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mls.yvedp.cn

C#:   s.Replace("a", "b")
来源：http://gih.cheryme.top

[E07] 按分隔符拆分
来源：http://eer.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xyz.sysykeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pya.fktsv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ctn.jinqigufen.top

TS:   s.split(",")
来源：http://bab.chenlongwang.top

Java: s.split(",");  s.split("\\s+")
来源：http://dmm.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vly.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://rpg.yj20258.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mwb.yj20258888.top

[E08] 数组按分隔符合并
来源：http://dxx.smart0.xyz

Py:   ",".join(items)
来源：http://wvt.feifeiyinyue.top

PHP:  implode(",", $items);
来源：http://wvm.ydzc1.top

JS:   items.join(",")
来源：http://uer.316326.xyz

TS:   items.join(",")
来源：http://cjd.sufxvd.cn

Java: String.join(",", items)
来源：http://gbr.shuidangran.top

Go:   strings.Join(items, ",")
来源：http://vis.jinqigfzy.top

Ruby: items.join(",")
来源：http://cbj.shzxlz.cn

C#:   string.Join(",", items)
来源：http://sgh.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://efq.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://quk.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xab.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://jpv.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://nvp.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://fdp.vqdsnc.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://plc.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://poa.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hpe.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://lyi.uphjek.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jpq.yueranfly.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eut.zhixingplan.top

JS:   "7".padStart(3, "0")
来源：http://ppa.feifeiyinyue.top

TS:   "7".padStart(3, "0")
来源：http://sjp.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://wcf.nanxuanxn.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://dmw.jlsjyb.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jaa.yanxiufei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rzx.hnxiangtu.top

[E11] 反转字符串
来源：http://mmd.smart0.xyz

Py:   s[::-1]
来源：http://hus.feifeiyinyue.top

PHP:  strrev($s);
来源：http://wtz.ehwqpu.com

JS:   [...s].reverse().join("")
来源：http://iik.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://oks.wangdashe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pkt.iojbl.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cls.yangfankeji.com

Ruby: s.reverse
来源：http://oca.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://trj.zycfv.cn

[E12] 统计某字符出现次数
来源：http://xmv.ydzc1.top

Py:   s.count("a")
来源：http://ilp.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://ude.birdmap.top

JS:   s.split("a").length - 1
来源：http://qji.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://bsd.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zvg.haohaochexian.top

Go:   strings.Count(s, "a")
来源：http://ulm.dashuyun.cn

Ruby: s.count("a")
来源：http://thn.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://keb.gogol.net.cn

[E13] 逐字符遍历
来源：http://aoy.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://lum.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vnb.ctjpmb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://skm.quarkkingdee.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nlq.xuetiantiany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lyv.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ozd.zhaomingkeji.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://gmm.yangfankeji.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://joh.nwbrower.top

[E14] URL 编码与 Base64
来源：http://pqc.ctjpmb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pyu.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nlv.yj20258888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wwi.yj20258.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bpl.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dfj.wangdashe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vjk.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://miy.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://njo.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://ipo.jlsjyb.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://peh.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://icj.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://arh.svipenyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rqt.pengpengdd.cyou

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hat.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vxr.bjfxy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://roy.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xyh.dashuyun.cn

[E16] 数字千分位
来源：http://cia.aibaodan.cn

Py:   f"{1234567:,}"
来源：http://lfe.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://unm.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zsl.zycfv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zph.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xgk.dianchejie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iyl.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lwe.dashuyun.cn

C#:   1234567.ToString("N0")
来源：http://ofu.shzxlz.cn

[E17] 首字母大写
来源：http://fgw.mhx1999.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ngk.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jxm.daria6918.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lvr.zhiwuduotai.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hbv.hesvh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://toh.pengpengdd.cyou

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hoj.cheryme.top

Ruby: s.capitalize
来源：http://kjx.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kaz.yuxming.cn

[E18] 模板占位符替换
来源：http://tcy.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jzl.gaohongyu789.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gld.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ioe.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gqd.fehbvm.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hjj.xziqi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bpj.jinqigufen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nct.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pid.yonumen.top

[E19] 多行文本按行拆分
来源：http://dvj.fanxiaobao.xyz

Py:   s.splitlines()
来源：http://wsh.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qcg.epnwcf.com

JS:   s.split(/\r?\n/)
来源：http://uif.wangdashe.top

TS:   s.split(/\r?\n/)
来源：http://ecq.xuanzx.com

Java: s.lines().toList()
来源：http://ymf.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://aza.ybcxt.top

Ruby: s.lines
来源：http://dyh.iojbl.cn

C#:   s.Split('\n')
来源：http://ssq.yangfankeji.com

[E20] 判断字符串是否为空
来源：http://ylw.epnwcf.com

Py:   if not s:
来源：http://wky.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ezc.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://owh.yvedp.cn

TS:   if (s === "") {}
来源：http://woa.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://jrz.ehwqpu.com

Go:   if s == "" {}
来源：http://ybx.yonumen.top

Ruby: if s.empty?
来源：http://ktv.cheryme.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pkx.xuanzx.com

[E21] 超长截断加省略号
来源：http://zwa.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fpi.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aev.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yqm.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tgi.gzhubu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kmh.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://qhc.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://flh.kuanghao11.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jfm.jyoumei.cn

[E22] 字节长度与字符长度
来源：http://cvo.sysykeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ayc.jinyuanbaomall.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nes.vqdsnc.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lzb.fanxiaobao.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mrz.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mlv.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rxa.jiagoushi.top

Ruby: s.bytesize;  s.length
来源：http://nbx.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://idb.c1oappe.top

================================================================================
来源：http://qcj.dashuyun.cn

F. 文件与目录
来源：http://tse.hesvh.cn

================================================================================
来源：http://xcq.nanxinkj.top

[F01] 读取整个文件
来源：http://ach.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sca.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://zca.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jtg.daxiang520.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sjo.smart0.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://yfx.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uyn.fehbvm.com

Ruby: File.read("a.txt")
来源：http://xxe.feifeiyinyue.top


<!-- 参考信息 -->