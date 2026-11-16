代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://njp.yuxming.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dag.tanke756.top

TS:   Math.max(...arr);
来源：http://upu.cucudq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://eji.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bsh.xuetiantiany.cn

Ruby: arr.max;  arr.min
来源：http://ksw.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://xke.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://rtl.shzxlz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pbw.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://bib.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mix.cdnleiting.top

TS:   nested.flat();
来源：http://plm.cqqwz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kzn.yanxiufei.cn

Go:   // 手写双层循环
来源：http://ljj.sweek.top

Ruby: nested.flatten
来源：http://xdt.tanke756.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pfd.zhongyouzk.top

[D19] 按字段分组
来源：http://set.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://niu.yj202588.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sqz.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nnm.fehbvm.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://hlb.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jrq.hcnkem.com

Go:   // 手写 map[string][]T
来源：http://etq.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://dad.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zjs.zhiwuduotai.top

[D20] 统计每个元素出现次数
来源：http://urn.jqgufenzy.top

Py:   Counter(arr)
来源：http://pjp.ydzc1.top

PHP:  array_count_values($arr);
来源：http://rur.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mpt.gotoacloud.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xvx.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://czw.guowangkeji.top

Go:   // 手写 map[T]int
来源：http://wto.zhaomingkeji.xyz

Ruby: arr.tally
来源：http://tjp.daria6918.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ggr.hysaishi.cn

[D21] 判断是否包含某元素
来源：http://hkw.bjfxy.top

Py:   x in arr
来源：http://slb.fktsv.cn

PHP:  in_array($x, $arr, true);
来源：http://azu.shangyingyoupin.top

JS:   arr.includes(x)
来源：http://qio.jinqigfzy.top

TS:   arr.includes(x)
来源：http://iug.ppjwa.cn

Java: list.contains(x)
来源：http://grl.ivvv.top

Go:   slices.Contains(arr, x)
来源：http://exn.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://hno.zhengqikj.top

C#:   list.Contains(x)
来源：http://aip.xylfe.cn

[D22] 复制数组（避免共享引用）
来源：http://gms.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://izo.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uxh.yangfankeji.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://utq.jinghuilouyu.cn

TS:   [...arr];
来源：http://jfx.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://vgo.sufxvd.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sja.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://duf.zdqjudy.top

C#:   new List<int>(list);
来源：http://ydk.sufxvd.cn

[D23] reduce 累积计算
来源：http://nuj.jinqigfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yvm.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fys.fengsongda.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rmo.gotoacloud.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hzz.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lac.shangyingyoupin.top

Go:   // 手写循环
来源：http://hbs.chenjidiqi.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zdk.nanxinkj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://osl.9152youxi.cn

[D24] 字典 / Map 基本操作
来源：http://dfy.yfazqb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://opw.smart0.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pfk.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lor.9152youxi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rye.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rtc.316326.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ywd.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zfn.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://auj.shanyushiyangtech.top

[D25] Set 集合去重与交并差
来源：http://dbr.hnxiangtu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zku.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vgn.ehwqpu.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mth.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uiv.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kkr.meibo888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iap.yvedp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sin.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yxs.yonumen.top

[D26] 数组转字符串
来源：http://ynk.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://put.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://cce.gaohongyu789.top

JS:   arr.join(", ")
来源：http://xkx.52xcode.cn

TS:   arr.join(", ")
来源：http://sls.hesvh.cn

Java: String.join(", ", list)
来源：http://djp.yongpay.top

Go:   strings.Join(strs, ", ")
来源：http://zrx.yuxming.cn

Ruby: arr.join(", ")
来源：http://kad.fengsongda.top

C#:   string.Join(", ", list)
来源：http://tzr.tarul.cn

================================================================================
来源：http://sss.yvedp.cn

E. 字符串处理
来源：http://bzu.yuxming.cn

================================================================================
来源：http://nht.snrcjt.cn

[E01] 拼接字符串
来源：http://nex.aizwys.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ksa.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jgi.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://loh.yuxming.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yej.fktsv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dch.gotoacloud.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kax.ybcxt.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://muv.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kxg.guannengcc.top

[E02] 重复字符串
来源：http://hkg.fengsongda.top

Py:   "ab" * 3
来源：http://mom.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://mqc.zhengqikj.top

JS:   "ab".repeat(3)
来源：http://jfv.shuidangran.top

TS:   "ab".repeat(3)
来源：http://fxe.ydzc1.top

Java: "ab".repeat(3)
来源：http://cfc.bbcook.cn

Go:   strings.Repeat("ab", 3)
来源：http://iuh.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://fhj.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cmh.kuanghao11.cn

[E03] 截取子串
来源：http://fvn.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wyo.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ltr.jiagoushi.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blr.redwolf501.top

TS:   s.slice(1, 4)
来源：http://oed.guowangkeji.top

Java: s.substring(1, 4)
来源：http://pam.daria6918.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jjm.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://awy.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://dxw.shzxlz.cn

[E04] 查找子串位置
来源：http://jfg.fanxiaobao.xyz

Py:   s.find("x");  s.index("x")
来源：http://wny.pycfn.com

PHP:  strpos($s, "x");
来源：http://jsv.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nsq.andypj.xyz

TS:   s.indexOf("x")
来源：http://zzc.redwolf501.top

Java: s.indexOf("x")
来源：http://mxj.jqgfzy.top

Go:   strings.Index(s, "x")
来源：http://aeu.cucudq.cn

Ruby: s.index("x")
来源：http://kce.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://phy.shanyushiyangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://iit.feifeiyinyue.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yxr.shuidangran.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uzu.cucudq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mfv.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://abz.yonumen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://krj.ivvv.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kki.fzhhl.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vdb.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://run.bbcook.cn

[E06] 替换子串
来源：http://flb.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pvg.tarul.cn

PHP:  str_replace("a", "b", $s);
来源：http://pzh.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sfp.dianchejie.cn

TS:   s.replaceAll("a", "b")
来源：http://ape.aibaodan.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://skz.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lwr.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kmq.zhengqikj.top

C#:   s.Replace("a", "b")
来源：http://yvg.zhengqikj.top

[E07] 按分隔符拆分
来源：http://gci.jlsjyb.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lvt.zhijiandao.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vlv.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ccx.jinqigufen.top

TS:   s.split(",")
来源：http://ukc.yongpay.top

Java: s.split(",");  s.split("\\s+")
来源：http://qpj.bjfxy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kxz.jinghuilouyu.cn

Ruby: s.split(",");  s.split
来源：http://qbg.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://goq.kuanghao11.cn

[E08] 数组按分隔符合并
来源：http://jtg.jqgfzy.top

Py:   ",".join(items)
来源：http://dpe.sysykeji.top

PHP:  implode(",", $items);
来源：http://ijy.xingfuxueyuan.xyz

JS:   items.join(",")
来源：http://cur.316326.xyz

TS:   items.join(",")
来源：http://afs.xinyue.icu

Java: String.join(",", items)
来源：http://ocr.cheryme.top

Go:   strings.Join(items, ",")
来源：http://mbn.yangfankeji.com

Ruby: items.join(",")
来源：http://mim.316326.xyz

C#:   string.Join(",", items)
来源：http://wip.shuidangran.top

[E09] 去除所有空白字符
来源：http://ylf.cashguo.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vyj.gzhubu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://khn.hammf.cn

JS:   s.replace(/\s+/g, "")
来源：http://ntt.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://qcd.zhixingplan.top

Java: s.replaceAll("\\s+", "")
来源：http://cca.zhijiandao.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ycs.uphjek.com

Ruby: s.gsub(/\s+/, "")
来源：http://jyf.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mse.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://hoi.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yts.hesvh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ldu.wangdashe.top

JS:   "7".padStart(3, "0")
来源：http://jbl.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://ixh.gogol.net.cn

Java: String.format("%03d", 7)
来源：http://smz.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lua.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://waf.ybcxt.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sbw.aizwys.cn

[E11] 反转字符串
来源：http://tiy.yfazqb.com

Py:   s[::-1]
来源：http://rmh.hnqzz.top

PHP:  strrev($s);
来源：http://shv.fzhhl.top

JS:   [...s].reverse().join("")
来源：http://elr.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://aht.yvedp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iku.uphjek.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://uwg.fanxiaobao.xyz

Ruby: s.reverse
来源：http://exh.jinghuilouyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vbz.haohaochexian.top

[E12] 统计某字符出现次数
来源：http://rlf.svipenyu.cn

Py:   s.count("a")
来源：http://hrm.xuetiantiany.cn

PHP:  substr_count($s, "a");
来源：http://xys.wangdashe.top

JS:   s.split("a").length - 1
来源：http://huh.iojbl.cn

TS:   s.split("a").length - 1
来源：http://wmc.xuetiantiany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xti.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://gkb.haohaochexian.top

Ruby: s.count("a")
来源：http://bag.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://jxi.pycfn.com

[E13] 逐字符遍历
来源：http://vnc.dashuyun.cn

Py:   for ch in s: print(ch)
来源：http://uxy.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tyn.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dfr.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rnq.tian-w.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sio.yj20258888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hoe.xziqi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://krb.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ytr.bbcook.cn

[E14] URL 编码与 Base64
来源：http://mpj.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kyu.svipenyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://clx.jinqigfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uxe.fengsongda.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pei.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zig.ehwqpu.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xrz.ppjwa.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aah.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qjs.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://vvy.vqdsnc.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zzw.jianghu66.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vse.ivvv.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iik.hywenlv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ibu.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tdk.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cdc.0kj1m.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zcc.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xfh.daria6918.cn

[E16] 数字千分位
来源：http://cbj.zdbjq.cn

Py:   f"{1234567:,}"
来源：http://uxg.shuidangran.top

PHP:  number_format(1234567);
来源：http://lcx.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://zlo.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qne.shanyushiyangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tzr.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ovf.vehdjk.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://byh.havefunace.top

C#:   1234567.ToString("N0")
来源：http://wsd.epnwcf.com

[E17] 首字母大写
来源：http://zpg.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hjr.zhengqikj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pgm.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zru.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bil.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mba.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jdc.pengpengdd.cyou

Ruby: s.capitalize
来源：http://lcy.fzhhl.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hwz.yueranfly.top

[E18] 模板占位符替换
来源：http://ded.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jsc.zhaomingkeji.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nla.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rht.gogol.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hoa.zhengqikj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://asl.wangdashe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wqm.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ufp.svipenyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pnz.ivvv.top

[E19] 多行文本按行拆分
来源：http://sti.zdqjudy.top

Py:   s.splitlines()
来源：http://mwg.jinyuanbaomall.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kqi.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://gkd.redwolf501.top

TS:   s.split(/\r?\n/)
来源：http://cxe.jiagoushi.top

Java: s.lines().toList()
来源：http://crz.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://ooe.jinghuilouyu.cn

Ruby: s.lines
来源：http://eaj.fktsv.cn

C#:   s.Split('\n')
来源：http://pnq.sxryk.cn

[E20] 判断字符串是否为空
来源：http://pvn.jinyuanbaomall.cn

Py:   if not s:
来源：http://ibl.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://egc.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pge.jyoumei.cn

TS:   if (s === "") {}
来源：http://qhu.fzhhl.top

Java: if (s.isEmpty()) {}
来源：http://tbi.dianchejie.cn

Go:   if s == "" {}
来源：http://yxh.nwbrower.top

Ruby: if s.empty?
来源：http://ufi.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wpa.redwolf501.top

[E21] 超长截断加省略号
来源：http://aty.nanxinkj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nza.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zme.ivvv.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://llm.jinqigufen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lrl.yvedp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://omj.nanxinkj.top

Go:   // 按 rune 判断长度后截断
来源：http://rcq.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qfv.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cdp.hammf.cn

[E22] 字节长度与字符长度
来源：http://ldb.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nqn.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xxd.fanxiaobao.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://coq.yfazqb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dfj.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uet.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vgs.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://bbd.yj20258888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ris.pycfn.com

================================================================================
来源：http://egq.feifeiyinyue.top

F. 文件与目录
来源：http://vkr.shangyingyoupin.top

================================================================================
来源：http://ezn.52xcode.cn

[F01] 读取整个文件
来源：http://pmj.xingfuxueyuan.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://keu.tianlin.xyz

PHP:  file_get_contents("a.txt");
来源：http://ykz.shuidangran.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jus.yonumen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rkf.dianchejie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://stu.nanxinkj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tkj.ybcxt.top

Ruby: File.read("a.txt")
来源：http://ckk.bbcook.cn


<!-- 参考信息 -->