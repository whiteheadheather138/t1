代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://usg.tian-w.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sva.0kj1m.cn

TS:   Math.max(...arr);
来源：http://lun.daxiang520.top

Java: Collections.max(list);  Collections.min(list);
来源：http://juy.gaohongyu789.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kkx.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://vot.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://ypv.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://nwe.aibaodan.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ujm.jqgufenzy.top

PHP:  array_merge(...$nested);
来源：http://ajx.hfpthk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wte.yj20258.top

TS:   nested.flat();
来源：http://coe.sxryk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cka.havefunace.top

Go:   // 手写双层循环
来源：http://tei.ppjwa.cn

Ruby: nested.flatten
来源：http://jdt.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ozh.haohaochexian.top

[D19] 按字段分组
来源：http://rol.quarkkingdee.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vyw.jinyuanbaomall.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bwg.hcnkem.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oua.jlsjyb.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mtr.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://thh.316326.xyz

Go:   // 手写 map[string][]T
来源：http://nny.uphjek.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://vmh.bbcook.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uwi.uphjek.com

[D20] 统计每个元素出现次数
来源：http://pyg.pengpengdd.cyou

Py:   Counter(arr)
来源：http://ofe.snrcjt.cn

PHP:  array_count_values($arr);
来源：http://arc.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pzk.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://diw.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qze.jinqigufen.top

Go:   // 手写 map[T]int
来源：http://ebm.snrcjt.cn

Ruby: arr.tally
来源：http://ayd.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ils.zycfv.cn

[D21] 判断是否包含某元素
来源：http://vcg.tian-w.cn

Py:   x in arr
来源：http://hbu.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://nxi.pycfn.com

JS:   arr.includes(x)
来源：http://cmo.xinyue.icu

TS:   arr.includes(x)
来源：http://axt.yfazqb.com

Java: list.contains(x)
来源：http://okz.jinghuilouyu.cn

Go:   slices.Contains(arr, x)
来源：http://lmk.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://bun.uphjek.com

C#:   list.Contains(x)
来源：http://arv.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://fbh.nanxuanxn.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lbr.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xli.shanyushiyangtech.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ucc.yj20258.top

TS:   [...arr];
来源：http://xgm.yfazqb.com

Java: new ArrayList<>(list);
来源：http://qqg.ehwqpu.com

Go:   copied := append([]int(nil), arr...)
来源：http://axr.quarkkingdee.top

Ruby: arr.dup;  arr.clone
来源：http://ysp.zhijiandao.cn

C#:   new List<int>(list);
来源：http://vtp.yonumen.top

[D23] reduce 累积计算
来源：http://pfh.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nyx.snrcjt.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://adw.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mxh.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jju.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pwt.fzhhl.top

Go:   // 手写循环
来源：http://gfm.feifeiyinyue.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hqd.tarul.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zlq.jqgfzy.top

[D24] 字典 / Map 基本操作
来源：http://dbc.gaohongyu789.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gmq.yuanzhike.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lzt.pycfn.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kqc.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iij.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gon.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nyp.hcnkem.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cwv.jinghuilouyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pkx.tanke756.top

[D25] Set 集合去重与交并差
来源：http://shb.uphjek.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eod.sjlbkw.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ntx.xylfe.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xwl.mhx1999.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gfs.nanxuanxn.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ziv.wangdashe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xjr.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tbd.tian-w.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://und.xziqi.cn

[D26] 数组转字符串
来源：http://sbs.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://ujj.vehdjk.com

PHP:  implode(", ", $arr);
来源：http://njj.bbcook.cn

JS:   arr.join(", ")
来源：http://itr.kuanghao11.cn

TS:   arr.join(", ")
来源：http://wrx.redwolf501.top

Java: String.join(", ", list)
来源：http://ing.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://cir.zhengqikj.top

Ruby: arr.join(", ")
来源：http://cfq.yonumen.top

C#:   string.Join(", ", list)
来源：http://xbm.ehwqpu.com

================================================================================
来源：http://wyv.hfpthk.cn

E. 字符串处理
来源：http://fzu.guowangkeji.top

================================================================================
来源：http://nhe.bjfxy.top

[E01] 拼接字符串
来源：http://luq.fengsongda.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ctl.wangdashe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ltz.nwbrower.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tgn.jinyuanbaomall.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zvc.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qmq.yj202588.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tmk.fktsv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wnc.cashguo.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://paf.bjfxy.top

[E02] 重复字符串
来源：http://xgb.yj202588.top

Py:   "ab" * 3
来源：http://vgl.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://uff.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://vfg.pengpengdd.cyou

TS:   "ab".repeat(3)
来源：http://pze.zhaomingkeji.xyz

Java: "ab".repeat(3)
来源：http://wuc.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://xrh.yuxming.cn

Ruby: "ab" * 3
来源：http://lsd.hnqzz.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fqe.vehdjk.com

[E03] 截取子串
来源：http://ooy.hnxiangtu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jiw.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qxd.tian-w.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://btp.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://bit.smart0.xyz

Java: s.substring(1, 4)
来源：http://qnv.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ndt.jinqigufen.top

Ruby: s[1, 3];  s[1..3]
来源：http://rpr.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://don.yfazqb.com

[E04] 查找子串位置
来源：http://wtp.nanxinkj.top

Py:   s.find("x");  s.index("x")
来源：http://hui.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://rju.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jap.mhx1999.top

TS:   s.indexOf("x")
来源：http://url.fzhhl.top

Java: s.indexOf("x")
来源：http://unv.xziqi.cn

Go:   strings.Index(s, "x")
来源：http://pga.wangdashe.top

Ruby: s.index("x")
来源：http://woi.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://zuc.shanyushiyangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://chd.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uof.haohaochexian.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lln.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mqm.jyoumei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fav.svipenyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zgq.wangdashe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bsl.316326.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gdu.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kim.xylfe.cn

[E06] 替换子串
来源：http://stk.9152youxi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qmw.shanyushiyangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://gyu.jlsjyb.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ppw.tian-w.cn

TS:   s.replaceAll("a", "b")
来源：http://esq.hammf.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lbv.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cno.jinyuanbaomall.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jfp.bbcook.cn

C#:   s.Replace("a", "b")
来源：http://svg.nanxuanxn.top

[E07] 按分隔符拆分
来源：http://wnm.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rcx.pengpengdd.cyou

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gjf.zhiwuduotai.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vct.hcnkem.com

TS:   s.split(",")
来源：http://wqw.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://afw.tarul.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ddx.jyoumei.cn

Ruby: s.split(",");  s.split
来源：http://ufr.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bkd.jinqigfzy.top

[E08] 数组按分隔符合并
来源：http://ngq.sweek.top

Py:   ",".join(items)
来源：http://trp.xziqi.cn

PHP:  implode(",", $items);
来源：http://kng.hnqzz.top

JS:   items.join(",")
来源：http://fbc.cucudq.cn

TS:   items.join(",")
来源：http://whu.cucudq.cn

Java: String.join(",", items)
来源：http://ims.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://lme.tarul.cn

Ruby: items.join(",")
来源：http://goh.nanxinkj.top

C#:   string.Join(",", items)
来源：http://xab.dianchejie.cn

[E09] 去除所有空白字符
来源：http://xuy.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mpj.yj20258.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aca.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://rbx.andypj.xyz

TS:   s.replace(/\s+/g, "")
来源：http://rnj.hnxiangtu.top

Java: s.replaceAll("\\s+", "")
来源：http://rsc.sxryk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sci.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://bpu.zhixingplan.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bym.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://uhl.cheryme.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gjs.haohaochexian.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://noy.wangdashe.top

JS:   "7".padStart(3, "0")
来源：http://qxm.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://jjg.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://iit.ppjwa.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dsj.cheryme.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kze.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rqu.gaohongyu789.top

[E11] 反转字符串
来源：http://lpu.tanke756.top

Py:   s[::-1]
来源：http://zch.gotoacloud.top

PHP:  strrev($s);
来源：http://wul.tanke756.top

JS:   [...s].reverse().join("")
来源：http://jpo.ybcxt.top

TS:   [...s].reverse().join("")
来源：http://ktx.mhx1999.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ffo.c1oappe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://waf.yongpay.top

Ruby: s.reverse
来源：http://dxc.tianlin.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://rna.chenjidiqi.icu

[E12] 统计某字符出现次数
来源：http://nrx.wangdashe.top

Py:   s.count("a")
来源：http://sux.quarkkingdee.top

PHP:  substr_count($s, "a");
来源：http://zoj.yuanzhike.top

JS:   s.split("a").length - 1
来源：http://odn.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://xgt.gotoacloud.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ion.yongpay.top

Go:   strings.Count(s, "a")
来源：http://zgv.yuxming.cn

Ruby: s.count("a")
来源：http://xrc.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://diy.nanxinkj.top

[E13] 逐字符遍历
来源：http://jou.jqgufenzy.top

Py:   for ch in s: print(ch)
来源：http://zje.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tte.epnwcf.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://bdk.tianlin.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://whn.haohaochexian.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mai.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tlo.aizwys.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://btb.fzhhl.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://luu.shanyushiyangkeji.top

[E14] URL 编码与 Base64
来源：http://nvk.aizwys.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://luy.zycfv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yhw.c1oappe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://chn.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ddb.cdnleiting.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aoy.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uym.aibaodan.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yzs.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hhr.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://nor.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nvr.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lrr.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qrl.yuxming.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kgk.hnxiangtu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mha.ivvv.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oxf.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://irw.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uxv.cdnleiting.top

[E16] 数字千分位
来源：http://gxz.shanyushiyangtech.top

Py:   f"{1234567:,}"
来源：http://nnb.zdbjq.cn

PHP:  number_format(1234567);
来源：http://fhj.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://kei.vehdjk.com

TS:   (1234567).toLocaleString("en-US")
来源：http://lgo.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iwc.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ufv.c1oappe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mql.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://tsv.jinqigufen.top

[E17] 首字母大写
来源：http://jqn.ppjwa.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pzt.cdnleiting.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mjq.bbcook.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xju.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jep.tianlin.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dlw.daria6918.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tqe.316326.xyz

Ruby: s.capitalize
来源：http://oke.xziqi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rnr.hammf.cn

[E18] 模板占位符替换
来源：http://jel.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rbc.ydzc1.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nez.xuanzx.com

JS:   tpl.replaceAll("{name}", name)
来源：http://fbs.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fbw.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wfr.jqgufenzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kue.ehwqpu.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://adq.aizwys.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ghy.yj20258888.top

[E19] 多行文本按行拆分
来源：http://zjp.ctjpmb.com

Py:   s.splitlines()
来源：http://rjn.jianghu66.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zvf.shuidangran.top

JS:   s.split(/\r?\n/)
来源：http://tfh.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://fnz.jinghuilouyu.cn

Java: s.lines().toList()
来源：http://sbv.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://zex.hfpthk.cn

Ruby: s.lines
来源：http://akf.guannengcc.top

C#:   s.Split('\n')
来源：http://mex.tian-w.cn

[E20] 判断字符串是否为空
来源：http://lcl.zhongyouzk.top

Py:   if not s:
来源：http://kzk.dianchejie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://btr.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kad.jiagoushi.top

TS:   if (s === "") {}
来源：http://utd.sjlbkw.cn

Java: if (s.isEmpty()) {}
来源：http://rgs.mhx1999.top

Go:   if s == "" {}
来源：http://jge.tanke756.top

Ruby: if s.empty?
来源：http://gtx.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ial.sysykeji.top

[E21] 超长截断加省略号
来源：http://sep.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nkq.0kj1m.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sli.bbcook.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bhu.vqdsnc.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pzj.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zoa.xziqi.cn

Go:   // 按 rune 判断长度后截断
来源：http://zrs.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hvw.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kam.andypj.xyz

[E22] 字节长度与字符长度
来源：http://grf.jlsjyb.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nnh.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zri.zhijiandao.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eey.sysykeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kdi.zhixingplan.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://brz.cashguo.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pjy.dianchejie.cn

Ruby: s.bytesize;  s.length
来源：http://vdi.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jba.aibaodan.cn

================================================================================
来源：http://gco.sufxvd.cn

F. 文件与目录
来源：http://vnv.tarul.cn

================================================================================
来源：http://svx.yonumen.top

[F01] 读取整个文件
来源：http://ppw.pycfn.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sqo.jlsjyb.cn

PHP:  file_get_contents("a.txt");
来源：http://izp.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ubb.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://irb.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://xql.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rzk.hnxiangtu.top

Ruby: File.read("a.txt")
来源：http://mgp.jinqigufen.top


<!-- 参考信息 -->