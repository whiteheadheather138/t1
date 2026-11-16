代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://snt.ydzc1.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wvw.dashuyun.cn

TS:   Math.max(...arr);
来源：http://tyx.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xbx.gotoacloud.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tnl.jinghuilouyu.cn

Ruby: arr.max;  arr.min
来源：http://pxr.yueranfly.top

C#:   list.Max();  list.Min()
来源：http://bhz.nwbrower.top

[D18] 扁平化嵌套数组
来源：http://hen.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cnf.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://hsw.vqdsnc.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://abm.jqgufenzy.top

TS:   nested.flat();
来源：http://cjj.hnxiangtu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ero.sjlbkw.cn

Go:   // 手写双层循环
来源：http://kum.havefunace.top

Ruby: nested.flatten
来源：http://mdu.ydjk.org.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qlv.sweek.top

[D19] 按字段分组
来源：http://qpe.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://img.jqgufenzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://whn.vehdjk.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pek.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cup.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eqx.ctjpmb.com

Go:   // 手写 map[string][]T
来源：http://gui.tanke756.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tla.hnqzz.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qsn.tarul.cn

[D20] 统计每个元素出现次数
来源：http://igb.hnqzz.top

Py:   Counter(arr)
来源：http://ikw.ivvv.top

PHP:  array_count_values($arr);
来源：http://erf.zdbjq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dwj.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qtd.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://djx.uphjek.com

Go:   // 手写 map[T]int
来源：http://ocv.vehdjk.com

Ruby: arr.tally
来源：http://edj.kuanghao11.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tfd.52xcode.cn

[D21] 判断是否包含某元素
来源：http://vzt.ctjpmb.com

Py:   x in arr
来源：http://xem.mhx1999.top

PHP:  in_array($x, $arr, true);
来源：http://sqr.haohaochexian.top

JS:   arr.includes(x)
来源：http://mnf.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://mot.cqqwz.cn

Java: list.contains(x)
来源：http://aig.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://swj.sxryk.cn

Ruby: arr.include?(x)
来源：http://hap.cucudq.cn

C#:   list.Contains(x)
来源：http://sxj.52xcode.cn

[D22] 复制数组（避免共享引用）
来源：http://mqd.feifeiyinyue.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://trn.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mas.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pko.xziqi.cn

TS:   [...arr];
来源：http://ryx.tarul.cn

Java: new ArrayList<>(list);
来源：http://zjc.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gtq.zhoulong.xyz

Ruby: arr.dup;  arr.clone
来源：http://eee.jyoumei.cn

C#:   new List<int>(list);
来源：http://erv.zdqjudy.top

[D23] reduce 累积计算
来源：http://jig.xinyue.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ubn.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pan.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ydr.smart0.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hur.shanyushiyangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zor.tian-w.cn

Go:   // 手写循环
来源：http://kjs.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kdw.gogol.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eiq.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://dmf.vqdsnc.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rsv.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fwu.jqgfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://axb.ydzc1.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://thi.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://arx.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xor.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bbe.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dtv.xylfe.cn

[D25] Set 集合去重与交并差
来源：http://rpl.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://icq.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://llz.fzhhl.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jxy.xinyue.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xcs.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bmi.tian-w.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kbq.jqgfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pzo.hcnkem.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://evr.yueranfly.top

[D26] 数组转字符串
来源：http://mzv.gogol.net.cn

Py:   ", ".join(map(str, arr))
来源：http://wxd.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://cjr.xinyue.icu

JS:   arr.join(", ")
来源：http://pjt.sjlbkw.cn

TS:   arr.join(", ")
来源：http://sto.c1oappe.top

Java: String.join(", ", list)
来源：http://vso.epnwcf.com

Go:   strings.Join(strs, ", ")
来源：http://rmg.shzxlz.cn

Ruby: arr.join(", ")
来源：http://sdp.zhaomingkeji.xyz

C#:   string.Join(", ", list)
来源：http://ejw.hfpthk.cn

================================================================================
来源：http://bzx.andypj.xyz

E. 字符串处理
来源：http://yem.c1oappe.top

================================================================================
来源：http://lbh.jyoumei.cn

[E01] 拼接字符串
来源：http://brg.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tgu.jianghu66.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sdo.jiagoushi.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qlb.zhengqikj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uby.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://efp.yj202588.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ykb.xinyue.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kos.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bve.wangdashe.top

[E02] 重复字符串
来源：http://wvv.ehwqpu.com

Py:   "ab" * 3
来源：http://tin.yanxiufei.cn

PHP:  str_repeat("ab", 3);
来源：http://izm.xuanzx.com

JS:   "ab".repeat(3)
来源：http://suf.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://hev.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://fqr.iojbl.cn

Go:   strings.Repeat("ab", 3)
来源：http://few.yangfankeji.com

Ruby: "ab" * 3
来源：http://xxb.ybcxt.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ejy.hongshengwenyu.top

[E03] 截取子串
来源：http://fyu.vqdsnc.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hkd.epnwcf.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zrz.yonumen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lao.hesvh.cn

TS:   s.slice(1, 4)
来源：http://dss.ctjpmb.com

Java: s.substring(1, 4)
来源：http://ast.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zhw.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xtk.quarkkingdee.top

C#:   s.Substring(1, 3)
来源：http://bqf.yvedp.cn

[E04] 查找子串位置
来源：http://kjk.dashuyun.cn

Py:   s.find("x");  s.index("x")
来源：http://zqv.meibo888.top

PHP:  strpos($s, "x");
来源：http://gqb.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dyp.shanyushiyangkeji.top

TS:   s.indexOf("x")
来源：http://rld.tian-w.cn

Java: s.indexOf("x")
来源：http://xwc.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://noh.zdbjq.cn

Ruby: s.index("x")
来源：http://fns.yanxiufei.cn

C#:   s.IndexOf("x")
来源：http://lry.zhijiandao.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pqh.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gmo.jqgfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mlw.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ojd.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mdc.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fad.jinyuanbaomall.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kxx.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zxy.fengsongda.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ikc.nanxuanxn.top

[E06] 替换子串
来源：http://zrh.gzhubu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dnh.gotoacloud.top

PHP:  str_replace("a", "b", $s);
来源：http://duo.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hdz.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://enq.snrcjt.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kpg.ydjk.org.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tww.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ych.mhx1999.top

C#:   s.Replace("a", "b")
来源：http://xta.hesvh.cn

[E07] 按分隔符拆分
来源：http://gil.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cqs.jyoumei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lur.aizwys.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kmt.ppjwa.cn

TS:   s.split(",")
来源：http://van.zhoulong.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ghn.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rfh.cdnleiting.top

Ruby: s.split(",");  s.split
来源：http://zac.haohaochexian.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eqc.cashguo.top

[E08] 数组按分隔符合并
来源：http://rdx.chenlongwang.top

Py:   ",".join(items)
来源：http://fpx.jinyuanbaomall.cn

PHP:  implode(",", $items);
来源：http://mue.mhx1999.top

JS:   items.join(",")
来源：http://wwy.9152youxi.cn

TS:   items.join(",")
来源：http://amr.52xcode.cn

Java: String.join(",", items)
来源：http://jor.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://esb.gzhubu.top

Ruby: items.join(",")
来源：http://tpi.jiagoushi.top

C#:   string.Join(",", items)
来源：http://caf.52xcode.cn

[E09] 去除所有空白字符
来源：http://acl.dashuyun.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://snz.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sdq.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://ljv.yvedp.cn

TS:   s.replace(/\s+/g, "")
来源：http://pxr.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://jgs.zhijiandao.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fez.jqgufenzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://hbj.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yso.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://fig.yonumen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pqk.tianlin.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eub.sysykeji.top

JS:   "7".padStart(3, "0")
来源：http://pso.0kj1m.cn

TS:   "7".padStart(3, "0")
来源：http://kxx.zhoulong.xyz

Java: String.format("%03d", 7)
来源：http://uuv.tarul.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lgk.iojbl.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dut.xuanzx.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xbd.jinghuilouyu.cn

[E11] 反转字符串
来源：http://ypd.nanxuanxn.top

Py:   s[::-1]
来源：http://btj.meibo888.top

PHP:  strrev($s);
来源：http://hym.tarul.cn

JS:   [...s].reverse().join("")
来源：http://aub.hammf.cn

TS:   [...s].reverse().join("")
来源：http://vxo.yueranfly.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tte.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oup.wangshuangyany.cn

Ruby: s.reverse
来源：http://yvf.0kj1m.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rbu.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://wjm.tanke756.top

Py:   s.count("a")
来源：http://yrs.jqgufenzy.top

PHP:  substr_count($s, "a");
来源：http://rmx.yueranfly.top

JS:   s.split("a").length - 1
来源：http://zpf.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://fvo.fanxiaobao.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://crw.guannengcc.top

Go:   strings.Count(s, "a")
来源：http://rtn.hammf.cn

Ruby: s.count("a")
来源：http://nna.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://vgx.ppjwa.cn

[E13] 逐字符遍历
来源：http://gfy.hfpthk.cn

Py:   for ch in s: print(ch)
来源：http://ykk.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iid.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://olp.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wir.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fgc.hywenlv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://krn.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ijb.jinqigfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qba.xuanzx.com

[E14] URL 编码与 Base64
来源：http://nse.jinyuanbaomall.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://spr.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ose.jqgfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kab.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mkl.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kxj.xuanzx.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ily.xingfuxueyuan.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pvx.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kxs.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://ddy.zhixingplan.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gyf.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lml.hnqzz.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jdm.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bpg.fanxiaobao.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ofy.nwbrower.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eqf.iojbl.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bfv.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pmm.birdmap.top

[E16] 数字千分位
来源：http://npv.cheryme.top

Py:   f"{1234567:,}"
来源：http://ryp.daxiang520.top

PHP:  number_format(1234567);
来源：http://eti.daria6918.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vpi.haohaochexian.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ugt.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://htq.yj202588.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kpl.ivvv.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cmr.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://mtn.vqdsnc.cn

[E17] 首字母大写
来源：http://esn.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wqu.chenlongwang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dwr.zhaomingkeji.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jvb.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tpi.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rqd.kuanghao11.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vez.hammf.cn

Ruby: s.capitalize
来源：http://nru.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yik.zdbjq.cn

[E18] 模板占位符替换
来源：http://map.yvedp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://itu.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vme.aibaodan.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kds.hnqzz.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tcy.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hyj.fehbvm.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sxz.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://apo.jinghuilouyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://shh.gzhubu.top

[E19] 多行文本按行拆分
来源：http://rqg.hongshengwenyu.top

Py:   s.splitlines()
来源：http://pcm.chenzaomai.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://msq.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://awx.fehbvm.com

TS:   s.split(/\r?\n/)
来源：http://eyj.svipenyu.cn

Java: s.lines().toList()
来源：http://jhr.pycfn.com

Go:   strings.Split(s, "\n")
来源：http://ssh.ywan-chungtsiang.top

Ruby: s.lines
来源：http://yki.guannengcc.top

C#:   s.Split('\n')
来源：http://pfo.ybcxt.top

[E20] 判断字符串是否为空
来源：http://iat.shanyushiyangkeji.top

Py:   if not s:
来源：http://tmz.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oxz.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rvb.yuxming.cn

TS:   if (s === "") {}
来源：http://gej.hcnkem.com

Java: if (s.isEmpty()) {}
来源：http://htr.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://wxo.daria6918.cn

Ruby: if s.empty?
来源：http://jft.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xug.ywan-chungtsiang.top

[E21] 超长截断加省略号
来源：http://zep.yongpay.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hbj.nanxinkj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fjo.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yom.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xis.cheryme.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nei.tanke756.top

Go:   // 按 rune 判断长度后截断
来源：http://rjl.svipenyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bky.vehdjk.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zyy.aizwys.cn

[E22] 字节长度与字符长度
来源：http://hea.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yre.vehdjk.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zgz.316326.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://adv.vehdjk.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ozy.dianchejie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ejj.ywan-chungtsiang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rlx.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://vxe.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gzj.yueranfly.top

================================================================================
来源：http://bdu.zdbjq.cn

F. 文件与目录
来源：http://tlc.bjfxy.top

================================================================================
来源：http://edm.guowangkeji.top

[F01] 读取整个文件
来源：http://xfi.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dys.shangyingyoupin.top

PHP:  file_get_contents("a.txt");
来源：http://cfm.tarul.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jme.yj20258888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ztg.zhaomingkeji.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://wbw.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rgz.gogol.net.cn

Ruby: File.read("a.txt")
来源：http://nbn.zhongyouzk.top


<!-- 参考信息 -->