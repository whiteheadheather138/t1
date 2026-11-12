代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://tex.ivvv.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uok.dianchejie.cn

TS:   Math.max(...arr);
来源：http://yhu.fanxiaobao.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://kgk.316326.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://src.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://kcq.xuanzx.com

C#:   list.Max();  list.Min()
来源：http://xha.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://upp.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://poc.ctjpmb.com

PHP:  array_merge(...$nested);
来源：http://opv.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rsx.tarul.cn

TS:   nested.flat();
来源：http://sui.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://izo.vehdjk.com

Go:   // 手写双层循环
来源：http://qmi.yj202588.top

Ruby: nested.flatten
来源：http://vdg.zhijiandao.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qda.ydjk.org.cn

[D19] 按字段分组
来源：http://cgr.jinqigufen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nvw.ydzc1.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nsz.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pic.sufxvd.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dzx.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qvw.yonumen.top

Go:   // 手写 map[string][]T
来源：http://kre.shzxlz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pjc.shuidangran.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jai.daxiang520.top

[D20] 统计每个元素出现次数
来源：http://pys.xylfe.cn

Py:   Counter(arr)
来源：http://rjf.jqgfzy.top

PHP:  array_count_values($arr);
来源：http://pgk.sweek.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sic.svipenyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fcb.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ioh.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://vnq.jianghu66.top

Ruby: arr.tally
来源：http://nov.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bdo.haohaochexian.top

[D21] 判断是否包含某元素
来源：http://cdk.guannengcc.top

Py:   x in arr
来源：http://dgu.nwbrower.top

PHP:  in_array($x, $arr, true);
来源：http://api.pycfn.com

JS:   arr.includes(x)
来源：http://buq.dianchejie.cn

TS:   arr.includes(x)
来源：http://inq.yj20258.top

Java: list.contains(x)
来源：http://eiv.wangdashe.top

Go:   slices.Contains(arr, x)
来源：http://gcj.dianchejie.cn

Ruby: arr.include?(x)
来源：http://qeb.shanyushiyangtech.top

C#:   list.Contains(x)
来源：http://lry.52xcode.cn

[D22] 复制数组（避免共享引用）
来源：http://pyg.hongshengwenyu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cky.wangshuangyany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vgl.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zcd.cheryme.top

TS:   [...arr];
来源：http://qls.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://xhx.yj202588.top

Go:   copied := append([]int(nil), arr...)
来源：http://efw.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://nhj.mhx1999.top

C#:   new List<int>(list);
来源：http://pnw.ywan-chungtsiang.top

[D23] reduce 累积计算
来源：http://roj.bbcook.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vyb.ppjwa.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://csp.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lyc.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ueo.vqdsnc.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ryd.iojbl.cn

Go:   // 手写循环
来源：http://swo.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rww.shuidangran.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vud.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://izi.vehdjk.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yci.fehbvm.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oxa.birdmap.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ala.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ota.aibaodan.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aco.fengsongda.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lhb.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zbc.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://llj.zhijiandao.cn

[D25] Set 集合去重与交并差
来源：http://smb.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zje.zhiwuduotai.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lig.52xcode.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uyl.bjfxy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oyc.vehdjk.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://piz.shzxlz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://itj.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://why.guowangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rzu.xylfe.cn

[D26] 数组转字符串
来源：http://kru.yj20258888.top

Py:   ", ".join(map(str, arr))
来源：http://ihy.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://bom.yanxiufei.cn

JS:   arr.join(", ")
来源：http://kcd.yueranfly.top

TS:   arr.join(", ")
来源：http://bxq.kuanghao11.cn

Java: String.join(", ", list)
来源：http://ica.sweek.top

Go:   strings.Join(strs, ", ")
来源：http://xny.zdqjudy.top

Ruby: arr.join(", ")
来源：http://vnp.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://ael.ppjwa.cn

================================================================================
来源：http://jer.aibaodan.cn

E. 字符串处理
来源：http://yog.ydjk.org.cn

================================================================================
来源：http://hqe.zycfv.cn

[E01] 拼接字符串
来源：http://zkt.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fon.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mbg.hnxiangtu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gyx.ctjpmb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tgx.yvedp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://plu.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://una.guowangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://orm.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jhg.daxiang520.top

[E02] 重复字符串
来源：http://haa.jlsjyb.cn

Py:   "ab" * 3
来源：http://acd.svipenyu.cn

PHP:  str_repeat("ab", 3);
来源：http://aiv.yongpay.top

JS:   "ab".repeat(3)
来源：http://cpt.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://dum.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://sqm.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://lmf.yj20258888.top

Ruby: "ab" * 3
来源：http://yzk.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hlz.aizwys.cn

[E03] 截取子串
来源：http://chy.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sqf.zhongyouzk.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qol.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lsd.hywenlv.cn

TS:   s.slice(1, 4)
来源：http://cgb.feifeiyinyue.top

Java: s.substring(1, 4)
来源：http://ruo.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lxp.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://qsr.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://lli.yonumen.top

[E04] 查找子串位置
来源：http://bam.yanxiufei.cn

Py:   s.find("x");  s.index("x")
来源：http://bhm.tanke756.top

PHP:  strpos($s, "x");
来源：http://mfa.jiagoushi.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cps.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://cpo.0kj1m.cn

Java: s.indexOf("x")
来源：http://aqf.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://uek.vehdjk.com

Ruby: s.index("x")
来源：http://tsz.iojbl.cn

C#:   s.IndexOf("x")
来源：http://dvp.fzhhl.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://noh.shangyingyoupin.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rnk.zhongyouzk.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gsz.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jfp.xingfuxueyuan.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://nqc.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://goj.svipenyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://awt.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://udz.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://feb.guannengcc.top

[E06] 替换子串
来源：http://jlk.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bvm.yuxming.cn

PHP:  str_replace("a", "b", $s);
来源：http://tkj.zhiwuduotai.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://txy.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://lwb.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ewb.epnwcf.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uer.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pkl.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://alq.ctjpmb.com

[E07] 按分隔符拆分
来源：http://dcm.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rlo.cashguo.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hpb.chenlongwang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tby.guowangkeji.top

TS:   s.split(",")
来源：http://def.cheryme.top

Java: s.split(",");  s.split("\\s+")
来源：http://ejc.tianlin.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rxx.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://brh.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://upz.tanke756.top

[E08] 数组按分隔符合并
来源：http://vhk.ctjpmb.com

Py:   ",".join(items)
来源：http://kzl.andypj.xyz

PHP:  implode(",", $items);
来源：http://naq.jiagoushi.top

JS:   items.join(",")
来源：http://lfx.yonumen.top

TS:   items.join(",")
来源：http://vsn.jinqigfzy.top

Java: String.join(",", items)
来源：http://gli.xingfuxueyuan.xyz

Go:   strings.Join(items, ",")
来源：http://rmm.yj20258.top

Ruby: items.join(",")
来源：http://xnz.xuetiantiany.cn

C#:   string.Join(",", items)
来源：http://yud.gzhubu.top

[E09] 去除所有空白字符
来源：http://lwq.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dnl.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hgg.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://fxo.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://nvl.nanxinkj.top

Java: s.replaceAll("\\s+", "")
来源：http://dmp.fengsongda.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wtp.tianlin.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://lua.fengsongda.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cwl.smart0.xyz

[E10] 左侧补零 / 定长填充
来源：http://zzt.hysaishi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://efu.gotoacloud.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://svg.guowangkeji.top

JS:   "7".padStart(3, "0")
来源：http://lzi.hcnkem.com

TS:   "7".padStart(3, "0")
来源：http://yqh.yj202588.top

Java: String.format("%03d", 7)
来源：http://tfj.c1oappe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ijx.cdnleiting.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rlg.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oyt.fanxiaobao.xyz

[E11] 反转字符串
来源：http://qht.hnqzz.top

Py:   s[::-1]
来源：http://gvy.ppjwa.cn

PHP:  strrev($s);
来源：http://con.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://zer.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://dic.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wyw.sysykeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ujs.zhengqikj.top

Ruby: s.reverse
来源：http://dol.shanyushiyangtech.top

C#:   new string(s.Reverse().ToArray())
来源：http://szk.ywan-chungtsiang.top

[E12] 统计某字符出现次数
来源：http://zuv.yj202588.top

Py:   s.count("a")
来源：http://vtb.hywenlv.cn

PHP:  substr_count($s, "a");
来源：http://qmb.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://xqi.wangdashe.top

TS:   s.split("a").length - 1
来源：http://lmf.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wsb.xinyue.icu

Go:   strings.Count(s, "a")
来源：http://cfk.jlsjyb.cn

Ruby: s.count("a")
来源：http://blr.tian-w.cn

C#:   s.Count(c => c == 'a')
来源：http://jik.cqqwz.cn

[E13] 逐字符遍历
来源：http://ulb.gogol.net.cn

Py:   for ch in s: print(ch)
来源：http://rbe.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fzc.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oox.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://taw.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fnb.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eel.guannengcc.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cfi.ivvv.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cbq.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://mfl.tianlin.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fcv.dianchejie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vlz.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yng.yfazqb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mng.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wpt.nanxuanxn.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pkd.fanxiaobao.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://shk.hnqzz.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dmz.chenzaomai.com

[E15] HTML 转义 / 反转义
来源：http://fvp.chenzaomai.com

Py:   html.escape(s);  html.unescape(s)
来源：http://sxm.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ssl.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tmc.uphjek.com

TS:   // 同上，务必做 XSS 过滤
来源：http://oyy.xylfe.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rbo.fehbvm.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tct.xylfe.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ppo.hfpthk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kkp.316326.xyz

[E16] 数字千分位
来源：http://chu.tian-w.cn

Py:   f"{1234567:,}"
来源：http://rnd.ctjpmb.com

PHP:  number_format(1234567);
来源：http://kcb.yuanzhike.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pws.xingfuxueyuan.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://scx.0kj1m.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nbw.hfpthk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gjv.shuidangran.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mod.yangfankeji.com

C#:   1234567.ToString("N0")
来源：http://jre.sufxvd.cn

[E17] 首字母大写
来源：http://wpo.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xnk.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lfz.gaohongyu789.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kzg.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ucq.sweek.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://txa.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gpj.nwbrower.top

Ruby: s.capitalize
来源：http://wja.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zlb.snrcjt.cn

[E18] 模板占位符替换
来源：http://xvu.jianghu66.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rcn.cheryme.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ozz.9152youxi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gke.yangfankeji.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ygb.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lgo.zhiwuduotai.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://irs.aibaodan.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zrf.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wwh.fzhhl.top

[E19] 多行文本按行拆分
来源：http://fgu.hysaishi.cn

Py:   s.splitlines()
来源：http://mlf.sysykeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jxw.gotoacloud.top

JS:   s.split(/\r?\n/)
来源：http://dgg.c1oappe.top

TS:   s.split(/\r?\n/)
来源：http://kby.shanyushiyangtech.top

Java: s.lines().toList()
来源：http://qrh.yangfankeji.com

Go:   strings.Split(s, "\n")
来源：http://hkv.jqgufenzy.top

Ruby: s.lines
来源：http://vdo.yueranfly.top

C#:   s.Split('\n')
来源：http://orl.bjfxy.top

[E20] 判断字符串是否为空
来源：http://tfg.tanke756.top

Py:   if not s:
来源：http://dab.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hyo.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yie.andypj.xyz

TS:   if (s === "") {}
来源：http://xzi.redwolf501.top

Java: if (s.isEmpty()) {}
来源：http://dxh.zhiwuduotai.top

Go:   if s == "" {}
来源：http://loi.aizwys.cn

Ruby: if s.empty?
来源：http://nxl.aizwys.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://roc.chenzaomai.com

[E21] 超长截断加省略号
来源：http://rfb.yfazqb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nln.epnwcf.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hwm.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qoh.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jiq.fehbvm.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bpo.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://knw.cashguo.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jjf.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ocp.nwbrower.top

[E22] 字节长度与字符长度
来源：http://xaq.nanxuanxn.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pzl.zhixingplan.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tmr.xingfuxueyuan.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xyb.aibaodan.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ynd.hfpthk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fhs.iojbl.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hvd.vehdjk.com

Ruby: s.bytesize;  s.length
来源：http://cem.316326.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://opl.cqqwz.cn

================================================================================
来源：http://znn.jianghu66.top

F. 文件与目录
来源：http://gli.daria6918.cn

================================================================================
来源：http://vfs.fengsongda.top

[F01] 读取整个文件
来源：http://vzo.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rro.c1oappe.top

PHP:  file_get_contents("a.txt");
来源：http://eod.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://erf.wangshuangyany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://upg.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ybz.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bfy.yuanzhike.top

Ruby: File.read("a.txt")
来源：http://rcw.cheryme.top


<!-- 参考信息 -->